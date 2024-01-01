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
