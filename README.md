# ArgoCD App of Apps with Kustomize and Helm

## Kustomize Example

eamples-kustomize Directory

├───apps
├───argocdapps
├───base
│   ├───app1
│   └───app2
└───overlays
    ├───production
    └───staging

The top apps folder will have Kustomize based ArgoCD Apps; that is 
templated by Kustomize. These deploy the microserviecs, app1 and app2.
You need to appy via kubectl argocdapps/appofapps.yaml


## Helm Example

examples-helm Directory

├───apps
│   ├───charts
│   └───templates
├───argocdapps
└───microservices
    ├───charts
    └───templates
        └───app3

Here the microservics folder has the helm based apps app1, app2,app3
The apps folder has the Argocd spps




