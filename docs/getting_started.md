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