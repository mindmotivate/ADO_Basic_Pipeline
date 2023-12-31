# Setting Up Your Azure DevOps Project

Embark on your Azure Pipelines journey by following these steps:

1. **Login to Azure DevOps:**
   Open your browser, go to [Azure DevOps](https://dev.azure.com/), and log in. Ensure that you're an administrator of the Azure DevOps organization you want to use.

2. **Create a New Project:**
   After logging in, create a fresh project within your organization. Give it the name "Basic-Pipeline." This project will serve as our canvas for CI/CD artistry.

   <img src="https://github.com/mindmotivate/ADO_Basic_Pipeline/assets/130941970/4461b584-9bf0-4cc4-85fb-df7596ca9bed" alt="image" width="50%"/>

3. **Import the Example Repository:**
   Before creating the pipeline, let's import the example repository into our Azure DevOps project. Navigate to "Repos" in your new project, click on "Import," and use the following Git repository URL:

   <img src="https://github.com/mindmotivate/ADO_Basic_Pipeline/assets/130941970/b00cc041-ec5a-4a9d-8b57-73e2db3aa429" alt="image" width="50%"/>

   - Repository URL: `https://github.com/MicrosoftDocs/pipelines-java`

     Enter this repo URL in the "Clone URL *" field
<img src="https://github.com/mindmotivate/ADO_Basic_Pipeline/assets/130941970/88004761-9b26-4fda-8717-2e5b8fc348e7" alt="image" width="50%"/>

*We will need to wait a moment while the repo loads...*
   <img src="https://github.com/mindmotivate/ADO_Basic_Pipeline/assets/130941970/75e063ef-91b9-4219-ba80-b01518fafa67" alt="image" width="45%"/>

   Follow the prompts to complete the import. Now, you have the necessary codebase in your Azure DevOps repository.

5. **Create Your Pipeline:**
   Now that we have the code, let's create the pipeline. Head to "Pipelines" and select "New Pipeline" or "Create Pipeline" if it's your first. Choose GitHub as your source location, and you might need to sign in to GitHub if prompted.

   - Repository: Select the repository you just imported.

   - Azure Pipelines will guide you through the setup process, suggesting a Maven pipeline template tailored for Java.

You're all set! The stage is yours to craft your Basic Pipeline project.

