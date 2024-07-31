# Trusted Application Pipeline Software Template

This application, **aqf5pk4fa-python**, was created from a Trusted Application Pipeline Software Template.

The software templates create a new source and gitops deployment repositories with a sample source application. 

## Repositories

The source code for your application can be found in [https://github.com/rhtap-test-organization-jk/aqf5pk4fa-python ](https://github.com/rhtap-test-organization-jk/aqf5pk4fa-python ).
 
The gitops repository, which contains the kubernetes manifests for the application can be found in 
[https://github.com/rhtap-test-organization-jk/aqf5pk4fa-python-gitops ](https://github.com/rhtap-test-organization-jk/aqf5pk4fa-python-gitops ) 

## Application namespaces 

The default application will be found in the following namespaces. Applications can be deployed into unique namespaces or multiple software templates can also bet generated into the same group namespaces.  

|  Namespace   |  Description   |  
| -------- | -------- |   
| **rhtap-app-development** | The default application during development. Every build will be deployed to this namespace for testing. | 
| **rhtap-app-stage** | The staging namespace for this application. Promotion from development to stage is manual via an update to the [gitops repository](https://github.com/rhtap-test-organization-jk/aqf5pk4fa-python-gitops ) in the components/aqf5pk4fa-python/overlays/prod directory |  
| **rhtap-app-prod** | The production namespace for this application. Promotion from stage to production is manual via an update to the [gitops repository](https://github.com/rhtap-test-organization-jk/aqf5pk4fa-python-gitops ) in the components/aqf5pk4fa-python/overlays/prod directory | 