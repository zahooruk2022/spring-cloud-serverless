# Accelerator Log

## Options
```json
{
  "bsGitBranch" : "main",
  "bsGitRepository" : "github.com?owner=zahooruk2022&repo=spring-cloud-serverless",
  "deploymentType" : "workload",
  "includeBuildToolWrapper" : true,
  "projectName" : "spring-cloud-serverless",
  "sourceRepositoryPrefix" : "dev.local"
}
```
## Log
```
┏ engine (Chain)
┃  Info Running Chain(GeneratorValidationTransform, UniquePath)
┃ ┏ ┏ engine.transformations[0].validated (Combo)
┃ ┃ ┃  Info Combo running as Chain
┃ ┃ ┃ engine.transformations[0].validated.delegate (Chain)
┃ ┃ ┃  Info Running Chain(Merge, UniquePath)
┃ ┃ ┃ ┏ engine.transformations[0].validated.delegate.transformations[0] (Merge)
┃ ┃ ┃ ┃  Info Running Merge(Combo, Combo, Combo, Combo, Combo, Combo, Combo, Combo, Combo, InvokeFragment, Provenance)
┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.delegate.transformations[0].sources[0] (Combo)
┃ ┃ ┃ ┃ ┃  Info Combo running as Chain
┃ ┃ ┃ ┃ ┃ engine.transformations[0].validated.delegate.transformations[0].sources[0].delegate (Chain)
┃ ┃ ┃ ┃ ┃  Info Running Chain(Include, Exclude)
┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.delegate.transformations[0].sources[0].delegate.transformations[0] (Include)
┃ ┃ ┃ ┃ ┃ ┃  Info Will include [**]
┃ ┃ ┃ ┃ ┃ ┃ Debug .gitignore matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug .tanzuignore matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug LICENSE matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug README.md matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug catalog/catalog-info.yaml matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug kubernetes/k8s/DEPLOYING.md matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug kubernetes/k8s/Tiltfile matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug kubernetes/k8s/deployment.yaml matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug kubernetes/k8s/service.yaml matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug kubernetes/tap/.tanzuignore matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug kubernetes/tap/DEPLOYING.md matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug kubernetes/tap/Tiltfile matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug kubernetes/tap/workload.yaml matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug pom.xml matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/example/helloapp/HelloAppApplication.java matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/application.properties matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┗ Debug src/test/java/com/example/helloapp/HelloAppApplicationTests.java matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.delegate.transformations[0].sources[0].delegate.transformations[1] (Exclude)
┃ ┃ ┃ ┃ ┃ ┃  Info Will exclude [pom.xml, README.md, grype.yaml, kubernetes/**, catalog/*.yaml, .github/workflows/**]
┃ ┃ ┃ ┃ ┃ ┃ Debug .gitignore didn't match [pom.xml, README.md, grype.yaml, kubernetes/**, catalog/*.yaml, .github/workflows/**] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug .tanzuignore didn't match [pom.xml, README.md, grype.yaml, kubernetes/**, catalog/*.yaml, .github/workflows/**] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug LICENSE didn't match [pom.xml, README.md, grype.yaml, kubernetes/**, catalog/*.yaml, .github/workflows/**] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug README.md matched [pom.xml, README.md, grype.yaml, kubernetes/**, catalog/*.yaml, .github/workflows/**] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug catalog/catalog-info.yaml matched [pom.xml, README.md, grype.yaml, kubernetes/**, catalog/*.yaml, .github/workflows/**] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug kubernetes/k8s/DEPLOYING.md matched [pom.xml, README.md, grype.yaml, kubernetes/**, catalog/*.yaml, .github/workflows/**] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug kubernetes/k8s/Tiltfile matched [pom.xml, README.md, grype.yaml, kubernetes/**, catalog/*.yaml, .github/workflows/**] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug kubernetes/k8s/deployment.yaml matched [pom.xml, README.md, grype.yaml, kubernetes/**, catalog/*.yaml, .github/workflows/**] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug kubernetes/k8s/service.yaml matched [pom.xml, README.md, grype.yaml, kubernetes/**, catalog/*.yaml, .github/workflows/**] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug kubernetes/tap/.tanzuignore matched [pom.xml, README.md, grype.yaml, kubernetes/**, catalog/*.yaml, .github/workflows/**] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug kubernetes/tap/DEPLOYING.md matched [pom.xml, README.md, grype.yaml, kubernetes/**, catalog/*.yaml, .github/workflows/**] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug kubernetes/tap/Tiltfile matched [pom.xml, README.md, grype.yaml, kubernetes/**, catalog/*.yaml, .github/workflows/**] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug kubernetes/tap/workload.yaml matched [pom.xml, README.md, grype.yaml, kubernetes/**, catalog/*.yaml, .github/workflows/**] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug pom.xml matched [pom.xml, README.md, grype.yaml, kubernetes/**, catalog/*.yaml, .github/workflows/**] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/example/helloapp/HelloAppApplication.java didn't match [pom.xml, README.md, grype.yaml, kubernetes/**, catalog/*.yaml, .github/workflows/**] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/application.properties didn't match [pom.xml, README.md, grype.yaml, kubernetes/**, catalog/*.yaml, .github/workflows/**] -> included
┃ ┃ ┃ ┃ ┗ ┗ Debug src/test/java/com/example/helloapp/HelloAppApplicationTests.java didn't match [pom.xml, README.md, grype.yaml, kubernetes/**, catalog/*.yaml, .github/workflows/**] -> included
┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.delegate.transformations[0].sources[1] (Combo)
┃ ┃ ┃ ┃ ┃  Info Combo running as Chain
┃ ┃ ┃ ┃ ┃ engine.transformations[0].validated.delegate.transformations[0].sources[1].delegate (Chain)
┃ ┃ ┃ ┃ ┃  Info Running Chain(Include, ReplaceText)
┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.delegate.transformations[0].sources[1].delegate.transformations[0] (Include)
┃ ┃ ┃ ┃ ┃ ┃  Info Will include [pom.xml]
┃ ┃ ┃ ┃ ┃ ┃ Debug .gitignore didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug .tanzuignore didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug LICENSE didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug README.md didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug catalog/catalog-info.yaml didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug kubernetes/k8s/DEPLOYING.md didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug kubernetes/k8s/Tiltfile didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug kubernetes/k8s/deployment.yaml didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug kubernetes/k8s/service.yaml didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug kubernetes/tap/.tanzuignore didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug kubernetes/tap/DEPLOYING.md didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug kubernetes/tap/Tiltfile didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug kubernetes/tap/workload.yaml didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug pom.xml matched [pom.xml] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/example/helloapp/HelloAppApplication.java didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/application.properties didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┗ Debug src/test/java/com/example/helloapp/HelloAppApplicationTests.java didn't match [pom.xml] -> excluded
┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.delegate.transformations[0].sources[1].delegate.transformations[1] (ReplaceText)
┃ ┃ ┃ ┃ ┗ ┗  Info Will replace [hello-fun->spring-cloud-serverl...(truncated)]
┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.delegate.transformations[0].sources[2] (Combo)
┃ ┃ ┃ ┃ ┃  Info Condition (#deploymentType == 'k8s-simple') evaluated to false
┃ ┃ ┃ ┃ ┗ null ()
┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.delegate.transformations[0].sources[3] (Combo)
┃ ┃ ┃ ┃ ┃  Info Condition (#deploymentType == 'k8s-simple') evaluated to false
┃ ┃ ┃ ┃ ┗ null ()
┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.delegate.transformations[0].sources[4] (Combo)
┃ ┃ ┃ ┃ ┃  Info Condition (#deploymentType == 'workload') evaluated to true
┃ ┃ ┃ ┃ ┃  Info Combo running as Chain
┃ ┃ ┃ ┃ ┃ engine.transformations[0].validated.delegate.transformations[0].sources[4].delegate (Chain)
┃ ┃ ┃ ┃ ┃  Info Running Chain(Include, ReplaceText, RewritePath, Combo)
┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.delegate.transformations[0].sources[4].delegate.transformations[0] (Include)
┃ ┃ ┃ ┃ ┃ ┃  Info Will include [kubernetes/tap/workload.yaml]
┃ ┃ ┃ ┃ ┃ ┃ Debug .gitignore didn't match [kubernetes/tap/workload.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug .tanzuignore didn't match [kubernetes/tap/workload.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug LICENSE didn't match [kubernetes/tap/workload.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug README.md didn't match [kubernetes/tap/workload.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug catalog/catalog-info.yaml didn't match [kubernetes/tap/workload.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug kubernetes/k8s/DEPLOYING.md didn't match [kubernetes/tap/workload.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug kubernetes/k8s/Tiltfile didn't match [kubernetes/tap/workload.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug kubernetes/k8s/deployment.yaml didn't match [kubernetes/tap/workload.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug kubernetes/k8s/service.yaml didn't match [kubernetes/tap/workload.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug kubernetes/tap/.tanzuignore didn't match [kubernetes/tap/workload.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug kubernetes/tap/DEPLOYING.md didn't match [kubernetes/tap/workload.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug kubernetes/tap/Tiltfile didn't match [kubernetes/tap/workload.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug kubernetes/tap/workload.yaml matched [kubernetes/tap/workload.yaml] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug pom.xml didn't match [kubernetes/tap/workload.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/example/helloapp/HelloAppApplication.java didn't match [kubernetes/tap/workload.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/application.properties didn't match [kubernetes/tap/workload.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┗ Debug src/test/java/com/example/helloapp/HelloAppApplicationTests.java didn't match [kubernetes/tap/workload.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.delegate.transformations[0].sources[4].delegate.transformations[1] (ReplaceText)
┃ ┃ ┃ ┃ ┃ ┗  Info Will replace [: hello-fun->: spring-cloud-serve...(truncated)]
┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.delegate.transformations[0].sources[4].delegate.transformations[2] (RewritePath)
┃ ┃ ┃ ┃ ┃ ┗ Debug Path 'kubernetes/tap/workload.yaml' matched '^(?<folder>.*/)?(?<filename>([^/]+?|)(?=(?<ext>\.[^/.]*)?)$)' with groups {ext=.yaml, folder=kubernetes/tap/, filename=workload.yaml, g0=kubernetes/tap/workload.yaml, g1=kubernetes/tap/, g2=workload.yaml, g3=workload.yaml, g4=.yaml} and was rewritten to 'config/workload.yaml'
┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.delegate.transformations[0].sources[4].delegate.transformations[3] (Combo)
┃ ┃ ┃ ┃ ┃ ┃  Info Combo running as Chain
┃ ┃ ┃ ┃ ┃ ┃ engine.transformations[0].validated.delegate.transformations[0].sources[4].delegate.transformations[3].delegate (Chain)
┃ ┃ ┃ ┃ ┃ ┃  Info Running Chain(Merge, UniquePath)
┃ ┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.delegate.transformations[0].sources[4].delegate.transformations[3].delegate.transformations[0] (Merge)
┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Running Merge(InvokeFragment, Combo)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.delegate.transformations[0].sources[4].delegate.transformations[3].delegate.transformations[0].sources[0] (InvokeFragment)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.delegate.transformations[0].sources[4].delegate.transformations[3].delegate.transformations[0].sources[0].validated (Combo)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Condition (#bsGitRepository != null) evaluated to true
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Combo running as Let
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ engine.transformations[0].validated.delegate.transformations[0].sources[4].delegate.transformations[3].delegate.transformations[0].sources[0].validated.delegate (Let)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug Adding symbol repoUrl with value 'https://github.com?owner=zahooruk2022&repo=spring-cloud-serverless'
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.delegate.transformations[0].sources[4].delegate.transformations[3].delegate.transformations[0].sources[0].validated.delegate.in (Chain)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Running Chain(OpenRewriteRecipe, ReplaceText)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ╺ engine.transformations[0].validated.delegate.transformations[0].sources[4].delegate.transformations[3].delegate.transformations[0].sources[0].validated.delegate.in.transformations[0] (OpenRewriteRecipe)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.delegate.transformations[0].sources[4].delegate.transformations[3].delegate.transformations[0].sources[0].validated.delegate.in.transformations[1] (ReplaceText)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┗ ┗ ┗ ┗  Info Will replace regex '(?<beforeBranch>[\s\S]+)(?<branch>branch: [\S]+)(?<rest>[\S\s]*)' with '${beforeBranch}branc...(truncated)'
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.delegate.transformations[0].sources[4].delegate.transformations[3].delegate.transformations[0].sources[1] (Combo)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Combo running as Include
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ engine.transformations[0].validated.delegate.transformations[0].sources[4].delegate.transformations[3].delegate.transformations[0].sources[1].delegate (Include)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Will include [**]
┃ ┃ ┃ ┃ ┃ ┃ ┗ ┗ Debug config/workload.yaml matched [**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.delegate.transformations[0].sources[4].delegate.transformations[3].delegate.transformations[1] (UniquePath)
┃ ┃ ┃ ┃ ┗ ┗ ┗ Debug Multiple representations for path 'config/workload.yaml', will use the one appearing first 
┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.delegate.transformations[0].sources[5] (Combo)
┃ ┃ ┃ ┃ ┃  Info Condition (#deploymentType == 'workload') evaluated to true
┃ ┃ ┃ ┃ ┃  Info Combo running as Chain
┃ ┃ ┃ ┃ ┃ engine.transformations[0].validated.delegate.transformations[0].sources[5].delegate (Chain)
┃ ┃ ┃ ┃ ┃  Info Running Chain(Include, ReplaceText, ReplaceText, RewritePath)
┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.delegate.transformations[0].sources[5].delegate.transformations[0] (Include)
┃ ┃ ┃ ┃ ┃ ┃  Info Will include [kubernetes/tap/Tiltfile]
┃ ┃ ┃ ┃ ┃ ┃ Debug .gitignore didn't match [kubernetes/tap/Tiltfile] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug .tanzuignore didn't match [kubernetes/tap/Tiltfile] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug LICENSE didn't match [kubernetes/tap/Tiltfile] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug README.md didn't match [kubernetes/tap/Tiltfile] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug catalog/catalog-info.yaml didn't match [kubernetes/tap/Tiltfile] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug kubernetes/k8s/DEPLOYING.md didn't match [kubernetes/tap/Tiltfile] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug kubernetes/k8s/Tiltfile didn't match [kubernetes/tap/Tiltfile] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug kubernetes/k8s/deployment.yaml didn't match [kubernetes/tap/Tiltfile] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug kubernetes/k8s/service.yaml didn't match [kubernetes/tap/Tiltfile] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug kubernetes/tap/.tanzuignore didn't match [kubernetes/tap/Tiltfile] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug kubernetes/tap/DEPLOYING.md didn't match [kubernetes/tap/Tiltfile] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug kubernetes/tap/Tiltfile matched [kubernetes/tap/Tiltfile] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug kubernetes/tap/workload.yaml didn't match [kubernetes/tap/Tiltfile] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug pom.xml didn't match [kubernetes/tap/Tiltfile] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/example/helloapp/HelloAppApplication.java didn't match [kubernetes/tap/Tiltfile] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/application.properties didn't match [kubernetes/tap/Tiltfile] -> excluded
┃ ┃ ┃ ┃ ┃ ┗ Debug src/test/java/com/example/helloapp/HelloAppApplicationTests.java didn't match [kubernetes/tap/Tiltfile] -> excluded
┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.delegate.transformations[0].sources[5].delegate.transformations[1] (ReplaceText)
┃ ┃ ┃ ┃ ┃ ┗  Info Will replace [hello-fun->spring-cloud-serverl...(truncated)]
┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.delegate.transformations[0].sources[5].delegate.transformations[2] (ReplaceText)
┃ ┃ ┃ ┃ ┃ ┗  Info Will replace [dev.local->dev.local]
┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.delegate.transformations[0].sources[5].delegate.transformations[3] (RewritePath)
┃ ┃ ┃ ┃ ┗ ┗ Debug Path 'kubernetes/tap/Tiltfile' matched '^(?<folder>.*/)?(?<filename>([^/]+?|)(?=(?<ext>\.[^/.]*)?)$)' with groups {ext=null, folder=kubernetes/tap/, filename=Tiltfile, g0=kubernetes/tap/Tiltfile, g1=kubernetes/tap/, g2=Tiltfile, g3=Tiltfile, g4=null} and was rewritten to 'Tiltfile'
┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.delegate.transformations[0].sources[6] (Combo)
┃ ┃ ┃ ┃ ┃  Info Condition (#deploymentType == 'workload') evaluated to true
┃ ┃ ┃ ┃ ┃  Info Combo running as Chain
┃ ┃ ┃ ┃ ┃ engine.transformations[0].validated.delegate.transformations[0].sources[6].delegate (Chain)
┃ ┃ ┃ ┃ ┃  Info Running Chain(Include, RewritePath)
┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.delegate.transformations[0].sources[6].delegate.transformations[0] (Include)
┃ ┃ ┃ ┃ ┃ ┃  Info Will include [kubernetes/tap/.tanzuignore]
┃ ┃ ┃ ┃ ┃ ┃ Debug .gitignore didn't match [kubernetes/tap/.tanzuignore] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug .tanzuignore didn't match [kubernetes/tap/.tanzuignore] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug LICENSE didn't match [kubernetes/tap/.tanzuignore] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug README.md didn't match [kubernetes/tap/.tanzuignore] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug catalog/catalog-info.yaml didn't match [kubernetes/tap/.tanzuignore] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug kubernetes/k8s/DEPLOYING.md didn't match [kubernetes/tap/.tanzuignore] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug kubernetes/k8s/Tiltfile didn't match [kubernetes/tap/.tanzuignore] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug kubernetes/k8s/deployment.yaml didn't match [kubernetes/tap/.tanzuignore] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug kubernetes/k8s/service.yaml didn't match [kubernetes/tap/.tanzuignore] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug kubernetes/tap/.tanzuignore matched [kubernetes/tap/.tanzuignore] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug kubernetes/tap/DEPLOYING.md didn't match [kubernetes/tap/.tanzuignore] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug kubernetes/tap/Tiltfile didn't match [kubernetes/tap/.tanzuignore] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug kubernetes/tap/workload.yaml didn't match [kubernetes/tap/.tanzuignore] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug pom.xml didn't match [kubernetes/tap/.tanzuignore] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/example/helloapp/HelloAppApplication.java didn't match [kubernetes/tap/.tanzuignore] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/application.properties didn't match [kubernetes/tap/.tanzuignore] -> excluded
┃ ┃ ┃ ┃ ┃ ┗ Debug src/test/java/com/example/helloapp/HelloAppApplicationTests.java didn't match [kubernetes/tap/.tanzuignore] -> excluded
┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.delegate.transformations[0].sources[6].delegate.transformations[1] (RewritePath)
┃ ┃ ┃ ┃ ┗ ┗ Debug Path 'kubernetes/tap/.tanzuignore' matched '^(?<folder>.*/)?(?<filename>([^/]+?|)(?=(?<ext>\.[^/.]*)?)$)' with groups {ext=null, folder=kubernetes/tap/, filename=.tanzuignore, g0=kubernetes/tap/.tanzuignore, g1=kubernetes/tap/, g2=.tanzuignore, g3=.tanzuignore, g4=null} and was rewritten to '.tanzuignore'
┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.delegate.transformations[0].sources[7] (Combo)
┃ ┃ ┃ ┃ ┃  Info Condition (#deploymentType != 'none') evaluated to true
┃ ┃ ┃ ┃ ┃  Info Combo running as Chain
┃ ┃ ┃ ┃ ┃ engine.transformations[0].validated.delegate.transformations[0].sources[7].delegate (Chain)
┃ ┃ ┃ ┃ ┃  Info Running Chain(Include, ReplaceText)
┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.delegate.transformations[0].sources[7].delegate.transformations[0] (Include)
┃ ┃ ┃ ┃ ┃ ┃  Info Will include [catalog/*.yaml]
┃ ┃ ┃ ┃ ┃ ┃ Debug .gitignore didn't match [catalog/*.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug .tanzuignore didn't match [catalog/*.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug LICENSE didn't match [catalog/*.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug README.md didn't match [catalog/*.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug catalog/catalog-info.yaml matched [catalog/*.yaml] -> included
┃ ┃ ┃ ┃ ┃ ┃ Debug kubernetes/k8s/DEPLOYING.md didn't match [catalog/*.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug kubernetes/k8s/Tiltfile didn't match [catalog/*.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug kubernetes/k8s/deployment.yaml didn't match [catalog/*.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug kubernetes/k8s/service.yaml didn't match [catalog/*.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug kubernetes/tap/.tanzuignore didn't match [catalog/*.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug kubernetes/tap/DEPLOYING.md didn't match [catalog/*.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug kubernetes/tap/Tiltfile didn't match [catalog/*.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug kubernetes/tap/workload.yaml didn't match [catalog/*.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug pom.xml didn't match [catalog/*.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/example/helloapp/HelloAppApplication.java didn't match [catalog/*.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/application.properties didn't match [catalog/*.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┗ Debug src/test/java/com/example/helloapp/HelloAppApplicationTests.java didn't match [catalog/*.yaml] -> excluded
┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.delegate.transformations[0].sources[7].delegate.transformations[1] (ReplaceText)
┃ ┃ ┃ ┃ ┗ ┗  Info Will replace [hello-fun->spring-cloud-serverl...(truncated)]
┃ ┃ ┃ ┃ ┏ README (Combo)
┃ ┃ ┃ ┃ ┃  Info Combo running as Chain
┃ ┃ ┃ ┃ ┃ README.delegate (Chain)
┃ ┃ ┃ ┃ ┃  Info Running Chain(Merge, UniquePath)
┃ ┃ ┃ ┃ ┃ ┏ README.delegate.transformations[0] (Merge)
┃ ┃ ┃ ┃ ┃ ┃  Info Running Merge(Combo, Combo, Combo)
┃ ┃ ┃ ┃ ┃ ┃ ┏ README.delegate.transformations[0].sources[0] (Combo)
┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Combo running as Chain
┃ ┃ ┃ ┃ ┃ ┃ ┃ README.delegate.transformations[0].sources[0].delegate (Chain)
┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Running Chain(Include, ReplaceText)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┏ README.delegate.transformations[0].sources[0].delegate.transformations[0] (Include)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Will include [README.md]
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gitignore didn't match [README.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .tanzuignore didn't match [README.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug LICENSE didn't match [README.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug README.md matched [README.md] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug catalog/catalog-info.yaml didn't match [README.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug kubernetes/k8s/DEPLOYING.md didn't match [README.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug kubernetes/k8s/Tiltfile didn't match [README.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug kubernetes/k8s/deployment.yaml didn't match [README.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug kubernetes/k8s/service.yaml didn't match [README.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug kubernetes/tap/.tanzuignore didn't match [README.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug kubernetes/tap/DEPLOYING.md didn't match [README.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug kubernetes/tap/Tiltfile didn't match [README.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug kubernetes/tap/workload.yaml didn't match [README.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug pom.xml didn't match [README.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/example/helloapp/HelloAppApplication.java didn't match [README.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/application.properties didn't match [README.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┗ Debug src/test/java/com/example/helloapp/HelloAppApplicationTests.java didn't match [README.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┏ README.delegate.transformations[0].sources[0].delegate.transformations[1] (ReplaceText)
┃ ┃ ┃ ┃ ┃ ┃ ┗ ┗  Info Will replace [hello-fun template repo->spring-cloud-serverl...(truncated)]
┃ ┃ ┃ ┃ ┃ ┃ ┏ README.delegate.transformations[0].sources[1] (Combo)
┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Condition (#deploymentType == 'k8s-simple') evaluated to false
┃ ┃ ┃ ┃ ┃ ┃ ┗ null ()
┃ ┃ ┃ ┃ ┃ ┃ ┏ README.delegate.transformations[0].sources[2] (Combo)
┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Condition (#deploymentType == 'workload') evaluated to true
┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Combo running as Chain
┃ ┃ ┃ ┃ ┃ ┃ ┃ README.delegate.transformations[0].sources[2].delegate (Chain)
┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Running Chain(Include, ReplaceText, RewritePath)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┏ README.delegate.transformations[0].sources[2].delegate.transformations[0] (Include)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Will include [kubernetes/tap/DEPLOYING.md]
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gitignore didn't match [kubernetes/tap/DEPLOYING.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .tanzuignore didn't match [kubernetes/tap/DEPLOYING.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug LICENSE didn't match [kubernetes/tap/DEPLOYING.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug README.md didn't match [kubernetes/tap/DEPLOYING.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug catalog/catalog-info.yaml didn't match [kubernetes/tap/DEPLOYING.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug kubernetes/k8s/DEPLOYING.md didn't match [kubernetes/tap/DEPLOYING.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug kubernetes/k8s/Tiltfile didn't match [kubernetes/tap/DEPLOYING.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug kubernetes/k8s/deployment.yaml didn't match [kubernetes/tap/DEPLOYING.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug kubernetes/k8s/service.yaml didn't match [kubernetes/tap/DEPLOYING.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug kubernetes/tap/.tanzuignore didn't match [kubernetes/tap/DEPLOYING.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug kubernetes/tap/DEPLOYING.md matched [kubernetes/tap/DEPLOYING.md] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug kubernetes/tap/Tiltfile didn't match [kubernetes/tap/DEPLOYING.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug kubernetes/tap/workload.yaml didn't match [kubernetes/tap/DEPLOYING.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug pom.xml didn't match [kubernetes/tap/DEPLOYING.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/example/helloapp/HelloAppApplication.java didn't match [kubernetes/tap/DEPLOYING.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/application.properties didn't match [kubernetes/tap/DEPLOYING.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┗ Debug src/test/java/com/example/helloapp/HelloAppApplicationTests.java didn't match [kubernetes/tap/DEPLOYING.md] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┏ README.delegate.transformations[0].sources[2].delegate.transformations[1] (ReplaceText)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┗  Info Will replace [hello-fun->spring-cloud-serverl...(truncated)]
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┏ README.delegate.transformations[0].sources[2].delegate.transformations[2] (RewritePath)
┃ ┃ ┃ ┃ ┃ ┗ ┗ ┗ Debug Path 'kubernetes/tap/DEPLOYING.md' matched '^(?<folder>.*/)?(?<filename>([^/]+?|)(?=(?<ext>\.[^/.]*)?)$)' with groups {ext=.md, folder=kubernetes/tap/, filename=DEPLOYING.md, g0=kubernetes/tap/DEPLOYING.md, g1=kubernetes/tap/, g2=DEPLOYING.md, g3=DEPLOYING.md, g4=.md} and was rewritten to 'README.md'
┃ ┃ ┃ ┃ ┃ ┏ README.delegate.transformations[1] (UniquePath)
┃ ┃ ┃ ┃ ┗ ┗ Debug Multiple representations for path 'README.md', will concatenate them together
┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.delegate.transformations[0].sources[9] (InvokeFragment)
┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.delegate.transformations[0].sources[9].validated (Combo)
┃ ┃ ┃ ┃ ┃ ┃  Info Combo running as Chain
┃ ┃ ┃ ┃ ┃ ┃ engine.transformations[0].validated.delegate.transformations[0].sources[9].validated.delegate (Chain)
┃ ┃ ┃ ┃ ┃ ┃  Info Running Chain(Merge, UniquePath)
┃ ┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.delegate.transformations[0].sources[9].validated.delegate.transformations[0] (Merge)
┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Running Merge(Combo)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┏ engine.transformations[0].validated.delegate.transformations[0].sources[9].validated.delegate.transformations[0].sources[0] (Combo)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Condition (#includeBuildToolWrapper) evaluated to true
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Combo running as Include
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ engine.transformations[0].validated.delegate.transformations[0].sources[9].validated.delegate.transformations[0].sources[0].delegate (Include)
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃  Info Will include [mvnw, mvnw.cmd, .mvn/**]
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .gitignore didn't match [mvnw, mvnw.cmd, .mvn/**] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .tanzuignore didn't match [mvnw, mvnw.cmd, .mvn/**] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug LICENSE didn't match [mvnw, mvnw.cmd, .mvn/**] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug README.md didn't match [mvnw, mvnw.cmd, .mvn/**] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug catalog/catalog-info.yaml didn't match [mvnw, mvnw.cmd, .mvn/**] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug kubernetes/k8s/DEPLOYING.md didn't match [mvnw, mvnw.cmd, .mvn/**] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug kubernetes/k8s/Tiltfile didn't match [mvnw, mvnw.cmd, .mvn/**] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug kubernetes/k8s/deployment.yaml didn't match [mvnw, mvnw.cmd, .mvn/**] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug kubernetes/k8s/service.yaml didn't match [mvnw, mvnw.cmd, .mvn/**] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug kubernetes/tap/.tanzuignore didn't match [mvnw, mvnw.cmd, .mvn/**] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug kubernetes/tap/DEPLOYING.md didn't match [mvnw, mvnw.cmd, .mvn/**] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug kubernetes/tap/Tiltfile didn't match [mvnw, mvnw.cmd, .mvn/**] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug kubernetes/tap/workload.yaml didn't match [mvnw, mvnw.cmd, .mvn/**] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug pom.xml didn't match [mvnw, mvnw.cmd, .mvn/**] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/java/com/example/helloapp/HelloAppApplication.java didn't match [mvnw, mvnw.cmd, .mvn/**] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/main/resources/application.properties didn't match [mvnw, mvnw.cmd, .mvn/**] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug src/test/java/com/example/helloapp/HelloAppApplicationTests.java didn't match [mvnw, mvnw.cmd, .mvn/**] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug .mvn/wrapper/maven-wrapper.properties matched [mvnw, mvnw.cmd, .mvn/**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug README.md didn't match [mvnw, mvnw.cmd, .mvn/**] -> excluded
┃ ┃ ┃ ┃ ┃ ┃ ┃ ┃ Debug mvnw matched [mvnw, mvnw.cmd, .mvn/**] -> included
┃ ┃ ┃ ┃ ┃ ┃ ┗ ┗ Debug mvnw.cmd matched [mvnw, mvnw.cmd, .mvn/**] -> included
┃ ┃ ┃ ┃ ┗ ┗ ╺ engine.transformations[0].validated.delegate.transformations[0].sources[9].validated.delegate.transformations[1] (UniquePath)
┃ ┃ ┃ ┗ ╺ engine.transformations[0].validated.delegate.transformations[0].sources[10] (Provenance)
┃ ┃ ┃ ┏ engine.transformations[0].validated.delegate.transformations[1] (UniquePath)
┃ ┃ ┃ ┃ Debug Multiple representations for path 'README.md', will use the one appearing last 
┃ ┗ ┗ ┗ Debug Multiple representations for path '.tanzuignore', will use the one appearing last 
┗ ╺ engine.transformations[1] (UniquePath)
```
