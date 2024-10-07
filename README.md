# Azure Practical Task

## Simple Personal Website for Azure Static Web App 

This project is a simple personal website created to develop and test the Azure Static Web App using GitHub Actions or to utilize Create Azure Web App with Azure App Services. It is part of the task assigned for the EPAM [Fundamentals] Cloud & DevOps Assessment Mexico, as part of the Cloud Assessment program.

### Purpose

The goal of this project is to demonstrate the ability to:

- Deploy a personal website using Azure Static Web Apps.
- Utilize GitHub Actions for Continuous Integration/Continuous Deployment (CI/CD).
- Explore the usage of Azure App Services for web hosting and deployment.

### Project Contents
- A basic HTML file that includes:
  - A black background.
  - A title with the developer's name.
  - A link to the developer's LinkedIn profile.
  - A link to the developer's GitHub profile.
  - A centered image.
- A GitHub Actions workflow to automate deployment to Azure.
- Step-by-step instructions and screenshots (found in the README.md file) that detail the setup and deployment process. Additionally, there is a [link to the Azure Fundamentals Task Instructions](documents/Azure_Fundamentals_Task_Gustavo_Adolfo_Carrillo_Camacho.pdf) to the same instructions and screenshots in PDF format located in the section of the README.md named 'Additional Resources.'

### Deployment
The project is deployed on Azure Static Web Apps, with the DNS record provided by Microsoft under the .azurewebsites.net domain.

### Additional Resources
For detailed instructions on how to deploy the simple web app on the Cloud Azure, please refer to the PDF document located in the documents folder: [Azure Fundamentals Task Instructions](documents/Azure_Fundamentals_Task_Gustavo_Adolfo_Carrillo_Camacho.pdf)

### Setup and Deployment Process

1.	#### Create Azure Web App with Azure App Services. 
Go to Azure portal. Azure Static Web Apps is very simple and easy to work with. There are 3 ways to create the Azure Static Web Apps, i.e., VS Code, Azure portal, and Azure CLI. 
Select an option from the 3 given, in this example was selected Access student benefits.

<p align="center">
  <img src="images/create_static_web_app_0.png" width="596" height="338" alt="Create Azure Portal Account">
</p>
<p align="center">

<p align="center">
  <em>Fig 1: Create Azure Portal Account</em>
</p>

2.	#### Create GitHub repo with simple personal website. 
**Create GitHub repo**

GitHub repositories store a variety of projects. In this guide, you'll create a repository and commit your first change.

  - In the upper-right corner of any page, select, then click New repository.

<p align="center">
  <img src="images/github_1.png" width="223" height="158" alt="Create GitHub repository">
</p>
<p align="center">

<p align="center">
  <em>Fig 2: Create GitHub repository</em>
</p>

  - Type a short, memorable name for your repository. For example, "hello-world".

<p align="center">
  <img src="images/github_2.png" width="514" height="135" alt="Create GitHub repository">
</p>
<p align="center">

<p align="center">
  <em>Fig 3: Create GitHub repository</em>
</p>

  - Optionally, add a description of your repository. For example, "My first repository on GitHub."
  - Choose a repository visibility. 
  - Select Initialize this repository with a README.
  - Click Create repository.

Congratulations! You've successfully created your first repository and initialized it with a README file.

**Commit your first change**

A commit is like a snapshot of all the files in your project at a particular point in time.
When you created your new repository, you initialized it with a README file. README files are a great place to describe your project in more detail or add some documentation such as how to install or use your project. The contents of your README file are automatically shown on the front page of your repository.

Let's commit a change to the README file.

  - In your repository's list of files, select README.md.

<p align="center">
  <img src="images/github_3.png" width="481" height="143" alt="Commit your first change">
</p>
<p align="center">

<p align="center">
  <em>Fig 4: Commit your first change</em>
</p>

  - In the upper right corner of the file view, click to open the file editor.

<p align="center">
  <img src="images/github_4.png" width="512" height="165" alt="Commit your first change">
</p>
<p align="center">

<p align="center">
  <em>Fig 5: Commit your first change</em>
</p>

  - In the text box, type some information about yourself.
  - Above the new content, click `Preview`.

<p align="center">
  <img src="images/github_5.png" width="554" height="113" alt="Commit your first change">
</p>
<p align="center">

<p align="center">
  <em>Fig 6: Commit your first change</em>
</p>

  - Review the changes you made to the file. If you select Show diff, you will see the new content in green.

<p align="center">
  <img src="images/github_6.png" width="1015" height="238" alt="Commit your first change">
</p>
<p align="center">

<p align="center">
  <em>Fig 7: Commit your first change</em>
</p>

  - Click Commit changes...
  - In the "Commit message" field, type a short, meaningful commit message that describes the change you made to the file. You can attribute the commit to more than one author in the commit message.  
  - Below the commit message fields, decide whether to add your commit to the current branch or to a new branch. If your current branch is the default branch, you should choose to create a new branch for your commit and then create a pull request. 

  <p align="center">
  <img src="images/github_7.png" width="517" height="130" alt="Commit your first change">
</p>
<p align="center">

<p align="center">
  <em>Fig 8: Commit your first change</em>
</p>


  - Click Commit changes or Propose changes.

**Next steps**

You have now created a repository, including a README file, and created your first commit on GitHub.
  - You can now clone a GitHub repository to create a local copy on your computer. From your local repository you can commit and create a pull request to update the changes in the upstream repository. 
  - You can find interesting projects and repositories on GitHub and make changes to them by creating a fork of the repository. Forking a repository will allow you to make changes to another repository without affecting the original.
  - Each repository on GitHub is owned by a person or an organization. You can interact with the people, repositories, and organizations by connecting and following them on GitHub.
  - GitHub has a great support community where you can ask for help and talk to people from around the world. Join the conversation on GitHub Community.

>Create the files to generate the simple web site inside your cloned GitHub repository.


3.	#### Deploy an application with GitHub Actions and Azure Static Web Apps. 

Give a resource Group name at the `Static Web App details`.

<p align="center">
  <img src="images/create_static_web_app_1.png" width="596" height="338" alt="Deploy of the Static Web App on the Azure Portal">
</p>
<p align="center">

<p align="center">
  <em>Fig 9: Deploy of the Static Web App on the Azure Portal</em>
</p>

Select the `Plan type`, `Deployment details` and then select the `Organization`.

<p align="center">
  <img src="images/create_static_web_app_2.png" width="596" height="338" alt="Deploy of the Static Web App on the Azure Portal">
</p>
<p align="center">

<p align="center">
  <em>Fig 10: Deploy of the Static Web App on the Azure Portal</em>
</p>

Select the desired `Repository` to deploy on Azure Cloud services and choose the appropriate branch from which you will deploy the project. Additionally, select the type of `Build Presets` for your project. Complete the remaining required information, and then click the `Next: Advanced` button.

<p align="center">
  <img src="images/create_static_web_app_3.png" width="596" height="338" alt="Deploy of the Static Web App on the Azure Portal">
</p>
<p align="center">

<p align="center">
  <em>Fig 11: Deploy of the Static Web App on the Azure Portal</em>
</p>

Select `Azure Functions and staging details` API and continue.

<p align="center">
  <img src="images/create_static_web_app_4.png" width="596" height="338" alt="Deploy of the Static Web App on the Azure Portal">
</p>
<p align="center">

<p align="center">
  <em>Fig 12: Deploy of the Static Web App on the Azure Portal</em>
</p>

Set `Tags` if needed, read the hint for more information about it, then continue.

<p align="center">
  <img src="images/create_static_web_app_5.png" width="596" height="338" alt="Deploy of the Static Web App on the Azure Portal">
</p>
<p align="center">

<p align="center">
  <em>Fig 13: Deploy of the Static Web App on the Azure Portal</em>
</p>

Check the details of the instance to be generated and then click on the button `Create`.

<p align="center">
  <img src="images/create_static_web_app_6.png" width="596" height="338" alt="Deploy of the Static Web App on the Azure Portal">
</p>
<p align="center">

<p align="center">
  <em>Fig 14: Deploy of the Static Web App on the Azure Portal</em>
</p>

Now your site web is completely deployed on the Cloud Azure. Click on `Go to resource`.

<p align="center">
  <img src="images/create_static_web_app_7.png" width="596" height="338" alt="Deploy of the Static Web App on the Azure Portal">
</p>
<p align="center">

<p align="center">
  <em>Fig 15: Deploy of the Static Web App on the Azure Portal</em>
</p>

<p align="center">
  <img src="images/create_static_web_app_8.png" width="596" height="338" alt="Deploy of the Static Web App on the Azure Portal">
</p>
<p align="center">

<p align="center">
  <em>Fig 16: Deploy of the Static Web App on the Azure Portal</em>
</p>

Here pressing on the `Visit your site` button, you can see **`the static app deployed on Cloud Azure under the DNS provided by Microsoft`**.

Here is the Azure Static Web App developed for this task.

<p align="center">
  <img src="images/create_static_web_app_9.png" width="596" height="338" alt="Deployed of the Static Web App on the Azure Portal">
</p>
<p align="center">

<p align="center">
  <em>Fig 17: Deployed of the Static Web App on the Azure Portal</em>
</p>

This is the web site address provided by Microsoft with the DNS azurestaticapps.net: 

https://witty-wave-096ae4210.5.azurestaticapps.net/

Direct link to the deployed web site:  [Adolfo Carrillo](https://witty-wave-096ae4210.5.azurestaticapps.net/)

The repository was set with an access modifier of type ‘Public’ because a non-individual reviewer was assigned. Here next is the address to the repository used on this deployment.

GitHub repository used on this deployment: [Simple-personal-website](https://github.com/AdolfCarr/Simple-personal-website)

**Important**

Please note that the CI/CD jobs and actions are configured and managed by Azure Cloud. This configuration can be found in the root directory of the project's GitHub repository, specifically in the .github/workflows folder. Inside this folder, you will find the .yml file that automates the entire deployment workflow on Azure Cloud.

<p align="center">
  <img src="images/create_static_web_app_10.png" width="596" height="338" alt="GitHub repository of the Static Web App">
</p>
<p align="center">

<p align="center">
  <em>Fig 18: GitHub repository of the Static Web App</em>
</p>

**References**

- GitHub, Inc. (2024). creating-and-managing-repositories/quickstart-for-repositories . Retrieved from docs.github.com: https://docs.github.com/en/repositories/creating-and-managing-repositories/quickstart-for-repositories?tool=webui
- Microsoft. (2024). Azure Static Web Apps . Retrieved from learn.microsoft.com: https://learn.microsoft.com/en-us/training/paths/azure-static-web-apps/
- Planet, D. (2023, Octuber 03). Create Azure Static Web App service with GitHub | Azure Static web app. Retrieved from www.youtube.com: https://www.youtube.com/watch?v=XM6h2l3ln0E








