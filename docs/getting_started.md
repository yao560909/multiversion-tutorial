### Create a project
kubebuilder init --domain tutorial.kubebuilder.io --repo tutorial.kubebuilder.io --project-name multiversion-tutorial

INFO Writing kustomize manifests for you to edit...
INFO Writing scaffold for you to edit...
INFO Get controller runtime:
$ go get sigs.k8s.io/controller-runtime@v0.20.2
INFO Update dependencies:
$ go mod tidy
Next: define a resource with:
$ kubebuilder create api
### Adding a new API
kubebuilder create api --group batch --version v1 --kind CronJob

INFO Create Resource [y/n]                        
y
INFO Create Controller [y/n]                      
y
INFO Writing kustomize manifests for you to edit...
INFO Writing scaffold for you to edit...          
INFO api/v1/cronjob_types.go                      
INFO api/v1/groupversion_info.go                  
INFO internal/controller/suite_test.go            
INFO internal/controller/cronjob_controller.go    
INFO internal/controller/cronjob_controller_test.go
INFO Update dependencies:
$ go mod tidy           
INFO Running make:
$ make generate                
mkdir -p /Users/yaolong/Documents/gitProject/github/yao560909/multiversion-tutorial/bin
Downloading sigs.k8s.io/controller-tools/cmd/controller-gen@v0.17.2
/Users/yaolong/Documents/gitProject/github/yao560909/multiversion-tutorial/bin/controller-gen object:headerFile="hack/boilerplate.go.txt" paths="./..."
Next: implement your new API and generate the manifests (e.g. CRDs,CRs) with:
$ make manifests