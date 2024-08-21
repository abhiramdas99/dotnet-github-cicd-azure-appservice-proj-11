
# objective: 
Demonstrating how to build and deploy a simple .NET-based application to Azure App Service using GitHub Actions

# Agenda:
-   create a free azure app service
-   create new repo in git clone to your local pc
-   write a simple application and test it locally
-   Integrate cicd pipline with azure app service

# lets start : 
## I create free azure app service
1) create new repo in git
2) create an azure app serivice and follow this url for create resource group & app-service plan -  https://github.com/abhiramdas99/manage-azure-infra

## create new repo in git clone to your local pc
- navigate to your workspace folder and paste the following  command
```
git clone https://github.com/abhiramdas99/dotnet-github-cicd-azure-appservice-proj-11.git
cd dotnet-github-cicd-azure-appservice-proj-11
```
## write a simple application and test it locally
```
dotnet new webapp --force
```
- Open the Pages/Index.cshtml file in your code editor.
```
@page
@model IndexModel
@{
    ViewData["Title"] = "Home Page";
}

<h1>Hello World</h1>

```
- make sure the folder structure should be like this.
![image](https://github.com/user-attachments/assets/f8601f52-db50-42fd-83b6-0118cebbdc17)

- build and  run
```
dotnet build
dotnet run
```
![image](https://github.com/user-attachments/assets/e2a4e61e-0bd0-423e-912b-f4d14a91eb63)

# Integrate cicd pipline with azure app service
- push the code to git
```
git add .
git commit -m "1st commit"
git push 
```
- now create azure app resource in free plan
  ### Basic
  ![image](https://github.com/user-attachments/assets/c345e41f-feb7-477d-886a-f55049c6b2d3)
  ![image](https://github.com/user-attachments/assets/dbecaf05-14ad-4e59-b7d5-caa55f8883b7)
  ![image](https://github.com/user-attachments/assets/f755fedf-27cc-455c-8f46-9cbe78a1642e)
  ![image](https://github.com/user-attachments/assets/53a57425-9a05-480a-9bd8-c4777a5de95c)
  ![image](https://github.com/user-attachments/assets/145c5e61-3068-4491-8a3a-b4513e9434d9)
### Deployment
  ![image](https://github.com/user-attachments/assets/de3c8191-6c26-433e-a6e4-8de21660cdf3)
  ![image](https://github.com/user-attachments/assets/89f6475a-f51c-40c3-b1a6-b45383726f4a)
  ![image](https://github.com/user-attachments/assets/4fcc21bd-f6b6-4695-ba71-79727e741e2a)
- now you can see the changes in github also
  ![image](https://github.com/user-attachments/assets/12e77c64-7fc9-4395-aeee-f7e610b9bfe9)
- lets push the code from your local pc to build and deploy the application
- 



