# dotnet-github-cicd-azure-appservice-proj-11

#objective: 
A simple hello-word dotnet website, to test the azure cicd and also delete the artifact after deploy to azure app service 

# steps plan:
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
  - Basic
    ![image](https://github.com/user-attachments/assets/c345e41f-feb7-477d-886a-f55049c6b2d3)


