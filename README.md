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


### 1. Exercise 1: Setting Up GitHub Copilot for Azure

####  **Objective**: 

  Configure GitHub Copilot for Azure (Preview) with Visual Code Insider

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
      

### 3. Exercise 2: Deploying a Web Application with @azure

**Objective**:

Use GitHub Copilot @azure to deploy a web application to Azure.
 
**Steps**:
  1. **Create a New Project**: Initialize a new web application project (e.g., using Node.js or Python).
 
**Outcome**: Participants will deploy a web application to Azure using GitHub Copilot.

### 4. Exercise 3: Implementing CI/CD with GitHub Actions 

**Objective**:
Set up a CI/CD pipeline using GitHub Actions and GitHub Copilot.

**Steps**:

**Outcome**: Participants will have a CI/CD pipeline set up for their web application.

---

This hackathon will help participants get hands-on experience with GitHub Copilot for Azure, enhancing their development workflows and productivity. Enjoy the hackathon! 🚀

