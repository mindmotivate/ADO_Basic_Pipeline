# Snyk Overview

Snyk is a security platform designed to help developers and organizations identify and fix vulnerabilities in their open-source dependencies and container images. It plays a crucial role in enhancing the security of software development by seamlessly integrating into the development lifecycle.

## Standalone Testing Application

As a standalone testing application, Snyk allows developers to:

- Scan their codebase for known vulnerabilities in third-party libraries and dependencies.
- Receive actionable insights and remediation guidance to address identified security issues.

This functionality enables teams to proactively manage and mitigate potential risks in their codebase.

## Azure DevOps (ADO) CI/CD Integration

In Azure DevOps CI/CD environments, Snyk is commonly used as an extension to:

- Integrate security checks into the continuous integration and continuous deployment (CI/CD) pipelines.
- Automatically scan code changes and dependencies during the build and deployment processes.

By seamlessly incorporating Snyk into the CI/CD workflow, development teams can achieve:

- Early detection of vulnerabilities.
- Integration of security considerations as an integral part of the development and deployment pipeline.

In summary, Snyk serves as a versatile tool for developers and organizations, offering both standalone testing capabilities and smooth integration into CI/CD environments to foster a secure and efficient development lifecycle.


install extension from marketplace

# Installing Snyk Extension in Azure DevOps (ADO)

1. **Go to Azure DevOps:**
   - Visit the [Azure DevOps website](https://dev.azure.com/).

2. **Navigate to Extensions:**
   - Once logged in, find the "Extensions" tab on the left-hand sidebar.

3. **Search for Snyk:**
   - In the Extensions marketplace, search for "Snyk" in the search bar.

4. **Select Snyk Extension:**
   - Find the Snyk extension in the search results and click on it.

5. **Install the Extension:**
   - On the extension page, look for 

![image](https://github.com/mindmotivate/ADO_Basic_Pipeline/assets/130941970/5c1b592e-ff45-4e70-b307-a6b7de1fae44)

![image](https://github.com/mindmotivate/ADO_Basic_Pipeline/assets/130941970/7524cf96-1cd5-4aad-97e6-4a5e9eee75c7)



https://support.snyk.io/hc/en-us

![image](https://github.com/mindmotivate/ADO_Basic_Pipeline/assets/130941970/ac3c2d33-9bd1-4101-aa99-da339083fb69)


# Creating a Service Account in Azure DevOps for Snyk

1. **Navigate to Project Settings:**
   - In Azure DevOps, go to the settings of your project.

2. **Select Service Connections:**
   - Look for a section called "Service connections" and select it.

3. **Add a New Service Connection:**
   - Find an option to add a new service connection and choose "Snyk" as the service type.

4. **Enter Snyk Token:**
   - Go back to the Snyk website, log in, and generate a token (usually under account settings). Copy the token.

5. **Copy and Paste Token:**
   - Paste the token into the Azure DevOps service connection form.

6. **Save and Verify:**
   - Save the service connection, and there might be an option to verify if the connection is successful.

# Overview for Non-Technical Audience

- **Why Snyk Extension:**
  - The Snyk extension helps keep our code secure by checking for any potential vulnerabilities in the software we build.

- **Signing Up on Snyk's Website:**
  - We sign up on Snyk's website to create an account, allowing us to use their tools to make sure our code is safe.

- **Creating a Service Account in Azure DevOps:**
  - By connecting Snyk to our Azure DevOps project, we ensure that every time we build or deploy our software, it automatically checks for any security issues.

- **Importance:**
  - This process is crucial because it helps us catch and fix any security problems in our code early on, making sure our software is safe and trustworthy for everyone who uses it.
