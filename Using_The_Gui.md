# Using the ADO GUI

In Azure DevOps GUI builds without YAML, the configuration process revolves around a graphical interface, allowing users to set up the build pipeline by visually selecting options and defining tasks. While it provides a user-friendly experience, offering a quick setup particularly suitable for projects with straightforward build requirements, it comes with limitations in version control. Although Azure DevOps offers versioning for GUI builds, it may not achieve the same level of granularity as YAML-based configurations

#### New Release Pipeline:
We will attempt to create the same functionality with a "New Release Pipeline".  Here are some of the main differences with this approach:

- **Modularity:**
  - **Definition:** The new release pipeline focuses on modular components, allowing you to break down your deployment process into stages, each with its set of tasks.

- **Artifact-Based:**
  - **Artifact Dependency:** The release pipeline depends on artifacts, which are specific versions of your software or application. These artifacts are built and stored, ensuring a clear versioning mechanism.

- **Environment Control:**
  - **Deployment Environments:** Environments are central to the new release pipeline, providing controlled spaces for deploying and testing your application. Each environment can have its specific configurations and approvals.

- **Flexibility:**
  - **Customizable Stages:** You have flexibility in defining multiple stages, such as development, testing, and production, tailoring the deployment process to fit your application's lifecycle.


## Select "New Release Pipeline" 
![image](https://github.com/mindmotivate/ADO_Basic_Pipeline/assets/130941970/010e467e-68fd-4690-8dc0-da273fd3e2c6)
### Select empty job
![image](https://github.com/mindmotivate/ADO_Basic_Pipeline/assets/130941970/ba8426c9-92fa-4943-b738-383c05b48f09)
### Add the artifact which is the repo containing your project repo
![image](https://github.com/mindmotivate/ADO_Basic_Pipeline/assets/130941970/827e5760-daab-4d3c-bef7-74dfecc7c995)
### Add a task
![image](https://github.com/mindmotivate/ADO_Basic_Pipeline/assets/130941970/899f12db-819e-4cb0-9f90-e9a03b90e3b7)
### Add Agent Job
![image](https://github.com/mindmotivate/ADO_Basic_Pipeline/assets/130941970/28fdb883-499a-497f-b576-ab480a175a0a)
### Add Maven
![image](https://github.com/mindmotivate/ADO_Basic_Pipeline/assets/130941970/6d209a25-7b6d-4432-8c17-9add0a18c689)
![image](https://github.com/mindmotivate/ADO_Basic_Pipeline/assets/130941970/f9cd5cd1-5745-4d48-880f-8680be61bd7d)
![image](https://github.com/mindmotivate/ADO_Basic_Pipeline/assets/130941970/8ef2c680-2256-419e-958a-6370f35da5da)




