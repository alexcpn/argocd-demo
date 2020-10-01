# ArgoCD App of Apps with Kustomize and Helm

## Kustomize Example

eamples-kustomize Directory

```
├───appofapps
├───argocdapps
├───base
│   ├───app1
│   └───app2
└───overlays
    ├───production
    └───staging
```

The top appofapps folder has the main ArgoCD app that points to 
argocdapps folder, which contains the Kustomize based ArgocdApps
produciton and staging which deploy to production and staging cluster the microservices (here app1 and app2)


## Helm Example

```
├───appofapps
├───argocdapps
│   ├───charts
│   └───templates
└───microservices
    ├───charts
    └───templates
        ├───app1
        ├───app2
        └───app3
```

Here the microservics folder has the helm based apps app1, app2,app3
The appofapps folder has the Argocd main app that point to other Helmbase argocdapps folder. This has produciton and staging ArgoCD apps that deploy the MS to production and staging clusters with different images and replicas

Here is the main app and sub Apps

![appofapps](https://i.imgur.com/lzgiRBV.png)


