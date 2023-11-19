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

