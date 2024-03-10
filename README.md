# Flask Application in Azure Web Apps.

This repository contains the code and instructions for deploying a Flask application in Azure Web Apps.

You can view the application at https://triluxo-app.azurewebsites.net/


# Deploy to Azure Web Apps using Azure Portal

### 1. Sign in to Azure Portal
 - Sign in to your Azure account at Azure Portal.

###  2. Create a New Web App
  - Click on Create a resource.
  - Search for *Web App* and click **Create**.
   - Fill in the required details such as  **App name**, **Subscription** (Free tier or Pay as you go), **Resource group**(create new), and **App Service plan** (Based on user load).
   - Click **Review + create** and then **Create**.
###  3. Create Repository
  - Create a GitHub account and create a new repository(copy this repository as it is into the new repository, or create your own flask application).
  - This repository contains the application in this structure.
	  - app.py  (contains the flask application)
	  - requirements.txt  (contains the requirements for the flask application)
	  - .gitignore
###  4. Deploy Your Flask Application
  - Navigate to your newly created Web App in the Azure Portal.
  - Under **Deployments** , select **Deployment Center**.
  - Choose your preferred deployment method (e.g., Local Git, GitHub, Azure DevOps, FTP).
  - In this project, GitHub has been chosen.
  - First, the GitHub account is authorized in which the application is created.
  - The **Repository**(triluxo-app), **Organization**(*default*) and **Branch**(main) are chosen.
  - The default Workload *yaml* file is used.
  - The changes are **saved**.

Then, the build process will start every time there is a new change in the repository.

### 3. Access Your Flask Application
  - Once deployment is complete, you can access your Flask application using the URL provided by Azure Web Apps (https://triluxo-app.azurewebsites.net/).
