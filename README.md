# spring-cloud-serverless repo

This repo provides a simple serverless Hello web app based on Spring Boot and Spring Cloud Function.

It can be deployed as a standalone web app, as a Tanzu Application Platform workload resource or, as a Kubernetes Deployment and Service.

## The code

> **NOTE**: The project uses Spring Boot 3.0 and is configured for Java 17.

The project contains the following Function bean definition:

```text
	@Bean
	public Function<String, String> hello() {
		return (in) -> {
			return "Hello " + in;
		};
	}
```

This simple serverless app returns the input value, prefixed with "Hello ". This is just a simple example what a Spring Cloud Function app can do. 
It is defined in `src/main/java/com/example/helloapp/HelloAppApplication.java`

## Deployment

This app can be deployed as a stand-alone web app, as a Tanzu Application Platform (TAP) workload resource or, as a Kubernetes Deployment and Service.

### Standalone app with embedded Tomcat server

You can build the project using Maven:

```bash
mvn clean package
```

To run the app using the embedded Tomcat server you can run this command:

```bash
mvn spring-boot:run
```

You can access the app using `curl`:

```bash
curl -w'\n' -H 'Content-Type: text/plain' localhost:8080 -d "Fun"
```
### Deploying to Kubernetes using VMware Tanzu Developer Tools for Visual Studio Code

You can open this project using Visual Studio Code. Make sure you have [VMware Tanzu Developer Tools for Visual Studio Code](https://docs.vmware.com/en/Tanzu-Application-Platform/1.0/tap/GUID-vscode-extension-about.html) installed.

For best results use Tilt version v0.23.2 or later. You can install Tilt by following these instructions: https://docs.tilt.dev/install.html

Follow [instructions in the documentation](https://docs.vmware.com/en/Tanzu-Application-Platform/1.0/tap/GUID-vscode-extension-usage-iterating-on-app.html) for deploying your app for live update and debugging.

These are the basic steps to use live update:

1. In Visual Studio Code, navigate to `Preferences > Settings > Extensions > Tanzu`.
    - In the `Source Image` field, provide the destination image repository to publish an image containing your workload source code. This should match what is specified for `SOURCE_IMAGE` default in the Tiltfile.
1. From the Command Palette (⇧⌘P), type "Tanzu", and select `Tanzu: Live Update Start`. You can view output from Tanzu Application Platform and from Tilt indicating that the container is being built and deployed.
    - You see "Live Update starting..." in the status bar at the bottom right.
    - Live update can take 1-3 minutes while the workload deploys and the Knative service becomes available.
        > Note: Depending on the type of cluster you use, you might see an error similar to the following:
        ```
        ERROR: Stop! cluster-name might be production.
        If you're sure you want to deploy there, add:
                allow_k8s_contexts('cluster-name')
        to your Tiltfile. Otherwise, switch k8s contexts and restart Tilt.
        ```
        Follow the instructions and add the line "allow_k8s_contexts('cluster-name')" to your Tiltfile.
1. When the Live Update status in the status bar is visible, resolve to "Live Update Started", navigate to http://localhost:8080 in your browser, and view your running application.
1. Make changes to the source code. When the codes is saved the running application will get updated.
1. Either continue making changes, or stop the live update when finished. Open the command palette (⇧⌘P), type "Tanzu", and select `Tanzu: Live Update Stop`.

### Deploying to Kubernetes as a TAP workload with Tanzu CLI

If you make modifications to the source and push to your own Git repository, then you can update the `spec.source.git` information in the `config/workload.yaml` file.

When you are done developing your serverless app, you can simply deploy it using:

```
tanzu apps workload apply -f config/workload.yaml
```

If you would like deploy the code from your local working directory you can use the following command:

```
tanzu apps workload create spring-cloud-serverless -f config/workload.yaml \
  --local-path . \
  --source-image <REPOSITORY-PREFIX>/spring-cloud-serverless-source \
  --type web
```

### Deploying to Kubernetes as a TAP workload using GraalVM native compile

If you would like to build the serverless app using the GraalVM native compile feature, then all you need to do is set the build env `BP_NATIVE_IMAGE` to true in the `workload.yaml` before applying it.

This can also be accomplished using the Tanzu CLI with the following command:

```
tanzu apps workload create spring-cloud-serverless -f config/workload.yaml \
  --build-env "BP_NATIVE_IMAGE=true"
```

### Accessing the app deployed to your cluster

If you don't have `curl` installed it can be installed using downloads here: https://curl.se/download.html

Determine the URL to use for the accessing the app by running:

```
tanzu apps workload get spring-cloud-serverless
```

You can assign the URL to a variable to make it easier to reference it:

```
URL=$(kubectl get services.serving.knative.dev/spring-cloud-serverless -o=jsonpath='{.status.url}')
 ```

To invoke the deployed app run the following `curl` command in another terminal window:

```
curl ${URL} -w'\n' -H 'Content-Type: text/plain' -d Fun
```

This depends on the TAP installation having DNS configured for the Knative ingress.
