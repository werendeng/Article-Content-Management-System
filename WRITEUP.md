# Write-up Template

### Analyze, choose, and justify the appropriate resource option for deploying the app.

*For **both** a VM or App Service solution for the CMS app:*
- *Analyze costs, scalability, availability, and workflow*
- *Choose the appropriate solution (VM or App Service) for deploying the app*
- *Justify your choice*

Virtual Machine Vs App Service:
- Cost: 
    Even though a virtual machine provides a lower up-front cost compared to purchasing or maintainig the needed hardware, it is much more expensive when compared to an App service.

- Scalability:
     For the case of Virtual machines, a Developer handles scalability issues by means of load balancers or virtual machine scale sets, whereas an App service being a platform as a service, comes with auto-scaling.

- Availability:
    Multiple virtual machines are grouped together to address availability issues, whereas by default, App services comes with high availability.

- Workflow:
    Virtual machines requires more on-going maintenance which can be time consuming for the Developer, on the other hand, App service has support for continuous deployment models such as Azure DevOps, GitHub.

In regards to this project, the appropriate deployment option would be an App Service. Reasons being that:  
  -  It is a lightweight Python Web app which actually does not require high perfomance, and there is not the need for a dedicated operating system to run the app, and also because App service supports Python language. 
  - App service reqires less time and effort to deploy and maintain, which gives the Developer more time to concentrate on maintaining and developing new features for his app whlie caring less about the infrastructure that runs the app.

### Assess app changes that would change your decision.

*Detail how the app and any other needs would have to change for you to change your decision in the last section.* 
- Should the app grow beyond the maximum supported hardware capacities of and App service and also if there arise the need to have control over the operating system with which to run the app, then a virtual machine would best serve this case. Another reason is if performance becomes of greater concern and or the app needs to be re-written using another language which is not supported by an App service, a virtual machine will be utilize.