# Hackathon: Improve Platform Engineering experience with GitHub Copilot for Azure 
Simple Mini-Hack to show some aspect of Platform Engineering to surface it as a service through GitHub copilot extensions like GHCP for azure

## Objective
To leverage GitHub Copilot for Azure to streamline development and deployment processes and improve productivity.

## Duration
1-2 hours

## Prerequisites
- GitHub account and access to GitHub Copilot.
- [Latest Visual Studio Code Insiders](https://code.visualstudio.com/insiders/)
- MCAP Azure subscription.

## Agenda


### Exercise 1: Setting Up GitHub Copilot for Azure

####  **Objective**: 

  - Configure GitHub Copilot for Azure (Preview) with Visual Code Insider

    ![image](/images/azure_extension.png)

**Steps**:
  1. [Install Visual Studio Code's GitHub Copilot extension](https://docs.github.com/en/copilot/quickstart)
  2. [Install GitHub Copilot For Azure](https://github.com/microsoft/GitHub-Copilot-for-Azure?tab=readme-ov-file#installation)
  3. Invoke the @azure copilot extension by putting @azure before your query with a few simple prompts:
      - Learning about Azure and its resources        
        ```
        @azure do static web apps support static ip addresses?        
        ```   
      - Getting information about your Azure resources
        ```
        @azure what is the URL for my webapp named [name]?
        @azure how many storage accounts do I have in uksouth?
        ```

      More sample questions [here](https://github.com/microsoft/GitHub-Copilot-for-Azure?tab=readme-ov-file#sample-questions)

  4. You can find a shortcut to chat with @azure in the context menu for resources in the Azure Extensions: 
    
      - In Visual Studio Code Insiders, open the command pallete via <kbd>F1</kbd> or <kbd>Ctrl/Cmd</kbd> + <kbd>Shift</kbd> + <kbd>P</kbd>, and run the command "Extensions: Install Extensions..."
        
      - Search for [Azure Resources](https://marketplace.visualstudio.com/tems?itemName=ms-azuretools.vscode-azureresourcegroups) and install it
     
    
      - Navigate to your resource and right click to use it in the context menu

        ![image](/images/contextualMenu.png)
      

### Exercise 2: Deploying a Web Application with @azure ([GitHub Copilot For Azure](https://techcommunity.microsoft.com/t5/microsoft-developer-community/introducing-github-copilot-for-azure-your-cloud-coding-companion/ba-p/4127644))

**Objective**:

- Use GitHub Copilot @azure to deploy a web application to Azure.
 
**Steps**:
  1. **Cloning and Running a Simple Web App:**     
  
      - [Install Node.js and npm locally](https://www.geeksforgeeks.org/how-to-install-node-run-npm-in-vs-code/)                 
      - open a new Terminal with <kbd>Ctrl/Cmd</kbd> + <kbd>Shift</kbd> + <kbd>'</kbd>
      - Clone the repository    
        ```bash
        git clone https://github.com/heroku/node-js-getting-started.git
        cd node-js-getting-started
        ```

      - Install Dependencies:
        ```bash
        npm install
        ```
      - Run the Application Locally:
        ```bash
        npm start
        ```
      - Open your browser and go to `http://localhost:5000` to see the app running.
      - When you're ready close the application from the terminal with <kbd>Ctrl/Cmd</kbd> + <kbd>C</kbd> 
  
  2. **Setting up a CI/CD pipeline using GitHub Actions and GitHub Copilot for Azure to deploy NodeJs web aoo to Azure**  
    
     -  Use GitHub Copilot Chat to generate deployment scripts. Here is an example prompts to get your started:
        **Prompt 1**:
        ```plaintext
        How do I create a GitHub Action to deploy my Node.js app using azd?
        ```
        **Prompt 2**:
         ```plaintext
        @azure Generate a GitHub Actions workflow to deploy my app to Azure App Service.
        ```
        **Prompt 3**:
        ```plaintext
        @azure What are the steps to configure continuous deployment for my web app using GitHub Actions?

        ```








