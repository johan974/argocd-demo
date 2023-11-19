# Example Git repo config file
- To be used by an ArgoCD server

# Make helm chart for ArgoCD
- Create a helm chart
  - $ helm create helmconfig
  - Edit the templates files
  - Check the syntax: 
    - $ helm template helmconfig
  - Check the syntax AND validate against the Kubernetes resources fules
    - $ helm install anyname helmconfig --dry-run
- Create ArgoCD application using the Helm chart
  - Copy the application of the source folder to a Helm chart version
  - Edit it to refer to the helmconfig folder
  - $ kubectl apply -f argocd-demo-helm-public.yaml
- Browse to: http://localhost:8080/random-quote
