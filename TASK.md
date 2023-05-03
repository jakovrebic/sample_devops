#DevOps task

First order of business is taking the task apart and defining bigger logical parts of work that need to be done:

 - Make Dockerfile for building sample Node app
    - Create sample app
 - Make Helm template which packages the app 
 - Make ArgoCD template which deploys the app

While doing the above tasks, we have to keep in mind the requirements:
 - running Nginx on custom port
 - staging and production env
 - CI pipeline
 - potentially adding DB

Notes and questions:
 - Depending on the importance and future reusability of the application, creating custom Helm Chart for it would be smart option. This would also mean easy adding of database to the service as a dependency to the umbrella Helm Chart.
 -  
