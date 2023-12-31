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
   
![image](https://github.com/mindmotivate/ADO_Basic_Pipeline/assets/130941970/69726016-98ae-4207-a391-d52ea46b4617)

5. **Create Your Pipeline:**
   Now that we have the code, let's create the pipeline. Head to "Pipelines" and select "New Pipeline" or "Create Pipeline" if it's your first.
   ![image](https://github.com/mindmotivate/ADO_Basic_Pipeline/assets/130941970/a6bb2a11-f8a2-4c28-9ef8-46f1cad65c28)

   ![image](https://github.com/mindmotivate/ADO_Basic_Pipeline/assets/130941970/8b75b264-706f-4149-b0f4-6e231a875d94)


   - Repository: Select the repository you just imported.
   - ![image](https://github.com/mindmotivate/ADO_Basic_Pipeline/assets/130941970/c2663912-9081-4561-a0f5-855a404956dc)

![image](https://github.com/mindmotivate/ADO_Basic_Pipeline/assets/130941970/a0ad87da-dcc5-4ed4-a7b7-e4e9dec0f1af)


You're all set! in the following step we will choose a template for our Pipeline project.

![image](https://github.com/mindmotivate/ADO_Basic_Pipeline/assets/130941970/dc6b3c8b-7b61-4a62-8cf6-a1252563c563)
