# Setting Up Your Azure DevOps Project

Embark on your Azure Pipelines journey by following these steps:

1. **Login to Azure DevOps:**
   Open your browser, go to [Azure DevOps](https://dev.azure.com/), and log in. Ensure that you're an administrator of the Azure DevOps organization you want to use.

2. **Create a New Project:**
   After logging in, create a fresh project within your organization. Give it the name "Basic-Pipeline." This project will serve as our canvas for CI/CD artistry.

3. **Import the Example Repository:**
   Before creating the pipeline, let's import the example repository into our Azure DevOps project. Navigate to "Repos" in your new project, click on "Import," and use the following Git repository URL:
   - Repository URL: `https://github.com/MicrosoftDocs/pipelines-java`

   Follow the prompts to complete the import. Now, you have the necessary codebase in your Azure DevOps repository.

4. **Create Your Pipeline:**
   Now that we have the code, let's create the pipeline. Head to "Pipelines" and select "New Pipeline" or "Create Pipeline" if it's your first. Choose GitHub as your source location, and you might need to sign in to GitHub if prompted.

   - Repository: Select the repository you just imported.

   - Azure Pipelines will guide you through the setup process, suggesting a Maven pipeline template tailored for Java.

You're all set! The stage is yours to craft your Basic Pipeline project.
