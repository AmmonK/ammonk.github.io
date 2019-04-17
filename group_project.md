# Creating project boilerplate Step 1

## Option 1: Express + Angular

Dependencies

- express-generator: `npm install -g express-generator`
- @angular/cli: `npm install -g @angular/cli`

Create a project folder, inside that folder run these commands:

```
express --no-view
ng new client --skipTests=true --skipInstall=true --skipGit=true
```

## Option 2: Express + React

Dependencies:

- express-geneator: `npm install -g express-generator`
- create-react-app: `npm install -g create-react-app`

Create a project folder, inside that folder run these commands:

```
express --no-view
create-react-app client
```

Delete the .git folder under client

## Option 3: Spring + Angular

Dependencies:

- @angular/cli `npm install -g @angular/cli`
- [Spring Initializr](https://start.spring.io/)

Use Spring Initializr to generate a spring project

- Project: Maven Project
- Language: Java
- Spring Boot: 2.1.4
- Project Metadata
  - Group: com.group
  - Artifact: YOUR_GROUP_NAME
- Dependencies: Web

Extract folder from the download, inside folder run command:

```
ng new client --skipTests=true --skipInstall=true --skipGit=true
```

## Option 3: Spring + React

Dependencies:

- express-generator: `npm install -g express-generator`
- [Spring Initializr](https://start.spring.io/)

Use Spring Initializr to generate a spring project

- Project: Maven Project
- Language: Java
- Spring Boot: 2.1.4
- Project Metadata
  - Group: com.group
  - Artifact: YOUR_GROUP_NAME
- Dependencies: Web

Extract folder from the download, inside folder run command:

```
create-react-app client
```

# Create project boilerplate Step 2

Push to repository

```
git init
git add .
git commit -m "initial commit";
git remote add origin URL_OF_GITHUB_REPO.git
git push -u origin master
```
