# Creating project boilerplate Step 1, Back End

## Option 1: Express

Dependencies

- express-generator: `npm install -g express-generator`

Create a project folder, inside that folder run this command:

```
express --no-view
```

## Option 2: Spring

Dependencies:

- [Spring Initializr](https://start.spring.io/)

Use Spring Initializr to generate a spring project

- Project: Maven Project
- Language: Java
- Spring Boot: 2.1.4
- Project Metadata
  - Group: com.group
  - Artifact: YOUR_GROUP_NAME
- Dependencies: Web

## Option 3: .NET Core

Dependencies:

- .NET Core SDK

Create a project folder, inside that folder run this command:

```
dotnet new webapi
```

# Creating project boilerplate Step 1, Front End

## Option 1: Angular

Dependencies

- @angular/cli: `npm install -g @angular/cli`

Inside the back end folder, run this command:

```
ng new client --skipTests=true --skipInstall=true --skipGit=true
```

## Option 2: React

Dependencies

- create-react-app: `npm install -g create-react-app`

Inside the back end folder, run this command:

```
create-react-app client
```

# Create project boilerplate Step 3, Git

Cleanup: remove any .git folders found

- check back end folder
- check client folder
- make sure that "view hidden" is selected

Push to repository

```
git init
git add .
git commit -m "initial commit";
git remote add origin URL_OF_GITHUB_REPO.git
git push -u origin master
```
