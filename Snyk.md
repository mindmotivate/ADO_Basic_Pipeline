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






# Creating a Snyk Account on the Offical Website:

## Step 1: Visit Snyk's Website

- Go to [Snyk's official website](https://snyk.io/).

## Step 2: Sign Up for an Account

- Find the "Sign Up" or "Register" button on the website.
- Provide your email address and create a password.
- Follow any additional instructions to complete the registration.

## Step 3: Verify Your Email

- Check your email inbox for a verification message from Snyk.
- Click on the provided link to verify your email address.

## Step 4: Connect to Repositories

- After verifying your email, log in to your Snyk account.

## Option 1: Connect to Git Repositories

- If your code is stored in Git repositories (like GitHub, GitLab, or Bitbucket):
  - Look for an option to "Connect to Git" or "Add a Git Provider."
  - Follow the on-screen instructions to authorize Snyk to access your Git repositories.
  - Select the repositories you want to connect to.

## Option 2: Connect to Azure Repositories

- If you are using Azure DevOps Repositories:
  - Look for an option to "Connect to Azure Repos" or a similar option.
  - Follow the on-screen instructions to authorize Snyk to access your Azure Repositories.
  - Select the repositories you want to connect to.

## Option 3: Connect to Other Services

- Snyk supports various other repositories and services:
  - Explore the Snyk interface for options like "Connect to Other Repositories" or similar.
  - Follow the provided instructions to connect to your specific repository or service.





# Creating a Service Account in Azure DevOps for Snyk


A **service connection** in Azure DevOps is like a secret handshake between Azure DevOps and another service, such as Snyk. It's a way for them to securely talk to each other.
Imagine you have a super-secret club (Azure DevOps) and a special agent (Snyk) who needs to access the club without giving away the secret password every time. Instead of sharing the password openly, they use a service connection. It's a safe and private way for the club and the agent to work together.

- **Club:** Azure DevOps
- **Special Agent:** Snyk
- **Service Connection:** The secret agreement between Azure DevOps and Snyk.

When Azure DevOps needs Snyk to check for security issues in the code (like a security guard), they use the service connection to communicate. It ensures a smooth and secure collaboration without revealing any secret details to the outside world.
In simpler terms, a service connection is like a VIP pass that allows different tools (like Azure DevOps and Snyk) to work together behind the scenes, making sure everything runs smoothly without compromising any secrets.


1. **Navigate to Project Settings:**
   - In Azure DevOps, go to the settings of your project.

2. **Select Service Connections:**
   - Look for a section called "Service connections" underneath the "Pipelines" category and select it.
   - 
![image](https://github.com/mindmotivate/ADO_Basic_Pipeline/assets/130941970/1f920233-7ed4-462b-84b0-94dd4fd37be9)

3. **Add a New Service Connection:**
   - Find an option to add a new service connection and choose "Snyk" as the service type.
![image](https://github.com/mindmotivate/ADO_Basic_Pipeline/assets/130941970/5fc8f5f0-c118-46c5-9fc8-bed535f9a75c)

![image](https://github.com/mindmotivate/ADO_Basic_Pipeline/assets/130941970/0738ae62-6d52-41a9-a207-e5ed528f65db)


4. **Enter Snyk Token:**
   - Go back to the Snyk website, log in, and generate a token (usually under account settings). Copy the token.

![image](https://github.com/mindmotivate/ADO_Basic_Pipeline/assets/130941970/5d5e73c4-cc33-4367-bcab-ea1872f9ad35)


5. **Copy and Paste Token:**
   - Paste the token into the Azure DevOps service connection form.

![image](https://github.com/mindmotivate/ADO_Basic_Pipeline/assets/130941970/71ad0aaa-29c0-4650-8c2d-d7bfc967244b)

6. **Save and Verify:**
   - Save the service connection, and there might be an option to verify if the connection is successful.


- **Snyk Extension:**
  - The Snyk extension helps keep our code secure by checking for any potential vulnerabilities in the software we build.
  - We sign up on Snyk's website to create an account, allowing us to use their tools to make sure our code is safe.
  - By connecting Snyk to our Azure DevOps project, we ensure that every time we build or deploy our software, it automatically checks for any security issues.
  - This process is crucial because it helps us catch and fix any security problems in our code early on, making sure our software is safe and trustworthy for everyone who uses it.
 



  
