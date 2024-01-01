# Enhancing Security in Your Pipeline

To fortify the security measures in your pipeline, you can include tasks for Snyk. Following the steps below will help you seamlessly integrate these security tasks into your pipeline:

## **Snyk:**
   - **Purpose:** Snyk scans your Java project for known security vulnerabilities and offers actionable recommendations.
   - **Importance:** Preventing exploitation of known vulnerabilities ensures a more secure Java project.

## Adding SnkykSecurity Tasks to Your Pipeline:
   - In order to add security testing to our build we can adjust the orginal .yml file that was created in the initial project phases

````
   - # Maven
# Build your Java project and run tests with Apache Maven.
# Add steps that analyze code, save build artifacts, deploy, and more:
# https://docs.microsoft.com/azure/devops/pipelines/languages/java

trigger:
- main

pool:
  vmImage: ubuntu-latest

stages:
- stage: Build
  jobs:
  - job: MavenBuild
    steps:
    - task: Maven@3
      inputs:
        mavenPomFile: 'pom.xml'
        mavenOptions: '-Xmx3072m'
        javaHomeOption: 'JDKVersion'
        jdkVersionOption: '1.8'
        jdkArchitectureOption: 'x64'
        publishJUnitResults: true
        testResultsFiles: '**/surefire-reports/TEST-*.xml'
        goals: 'package'

- stage: SnykScan  # New Security Stage
  jobs:
  - job: SnykScanJob
    steps:
    - task: SnykSecurityScan@1.3.3
      inputs:
        serviceConnectionEndpoint: 'Snyk-ADO'

````

## Here's the breakdown of what we added here:

This input specifies a connection endpoint named 'Snyk-ADO.' An endpoint is like a secret handshake or key that allows the pipeline to securely communicate with external services. In this case, it's used to connect to Snyk for the security scan.  This piece of code sets up a new part of the pipeline specifically for a security check using Snyk. It tells the pipeline to run a task that performs the security scan, and it provides the necessary connection details to securely communicate with Snyk. This ensures that the security scan is seamlessly integrated into the development process without manual setup in the Azure DevOps portal.

- This code snippet integrates a Snyk security scan into the pipeline.
- It creates a dedicated stage and job for the scan.
- It executes the SnykSecurityScan task with the necessary connection details.
- This ensures the scan runs automatically within the pipeline, streamlining the security process.

````
stage: SnykScan  # New Security Stage
  jobs:
  - job: SnykScanJob
    steps:
    - task: SnykSecurityScan@1.3.3
      inputs:
        serviceConnectionEndpoint: 'Snyk-ADO'
````

### **Breaking it down:**

- **`stage: SnykScan:`**
 - This line defines a new stage in the pipeline named "SnykScan," specifically dedicated to security scanning.

- **`jobs: - job: SnykScanJob:`**
 - This section creates a job within the SnykScan stage, named "SnykScanJob." A job groups related tasks together.

- **`steps: - task: SnykSecurityScan@1.3.3:`**
 - This line specifies a single step within the SnykScanJob, which involves executing the SnykSecurityScan task (version 1.3.3).

- **`inputs: serviceConnectionEndpoint: 'Snyk-ADO'`**
 - This section provides input to the SnykSecurityScan task, specifically a connection endpoint named "Snyk-ADO." This endpoint facilitates secure communication with Snyk for the scan.


## This code yields the following run:
![image](https://github.com/mindmotivate/ADO_Basic_Pipeline/assets/130941970/c2945cd8-db6a-49e9-b839-6cd78a0be5ea)
![image](https://github.com/mindmotivate/ADO_Basic_Pipeline/assets/130941970/4e185edd-2d47-4287-aef9-e3639c204a7c)
![image](https://github.com/mindmotivate/ADO_Basic_Pipeline/assets/130941970/03bbaacc-6e8b-467b-87a1-4fd7172b65bf)

![image](https://github.com/mindmotivate/ADO_Basic_Pipeline/assets/130941970/a9978e2f-5cae-4eff-a106-54d864330b7e)
![image](https://github.com/mindmotivate/ADO_Basic_Pipeline/assets/130941970/a8283fc3-4498-41d6-b23f-fca2c0140150)

![image](https://github.com/mindmotivate/ADO_Basic_Pipeline/assets/130941970/30654613-dd71-4e0a-82bb-e0f92b4ed14d)

