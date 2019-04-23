# Group project will create a Project Stack

A project stack is the set of frameworks that are used to run the project, consisting of

- Database
- Back End
- Front End

The Database can be either MySQL, SQLite, or MongoDb.

The Back End can be either Express, Spring, or .NET core.

The Front End can be either React, or Angular.

---

# Step 1: Pick a Back-End

## Option 1: Express

Dependencies

- express-generator: `npm install -g express-generator`

Create a project folder, inside that folder run this command:

```
express --no-view --git
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

---

# Step 2: Pick a Front-End

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

If you are using React with Express, change the Express port to 3001

> Edit bin/www line 15

Output listening port

> Copy `debug("Listening on " + bind);` and paste onto a new line below. Modify to `console.log("Listening on " + bind);`

---

# Step 3: Add project to Github

Cleanup: remove any .git folders found

- check back end folder
- check client folder
- make sure that "view hidden" is selected

Make a `.gitignore` file in the root of the project with the below text. This excludes the node_modules folder from the repository.

```
/node_modules
```

_DO NOT CHECK IN NODE_MODULES TO YOUR GITHUB REPOSITORY_

How to push to repository

```
git init
git add .
git commit -m "initial commit";
git remote add origin URL_OF_GITHUB_REPO.git
git push -u origin master
```

---

# Step 4: Pick a Database

It is recommended to use the database that was outlined in your Back End Foundations course. If you would like to use a database not listed, seek instructor approval. Any of the databases can be used with any of the back end frameworks.
