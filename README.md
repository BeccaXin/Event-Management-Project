
# Rockets

## Introduction & Architecture

### Front-end technology stack
Basic framework [React](https://react.dev/) 

UI framework [bootstrap (responsive)](https://www.bootcss.com/),[Element Plus (Vue)](https://element-plus.org/),[Ant Design (React)]( https://ant.design/),[Vant (mobile terminal)](https://vant-contrib.gitee.io/),[tailwindcss (a well-designed CSS library)](https://tailwindcss .com/)

Dependent libraries: [axios](https://axios-http.com/docs/intro) (interact with backend data), [ckeditor](https://ckeditor.com/ckeditor-5/demo/headless/) (rich text editing, comments/replies available)


# You can see the function in /rockets-frontend/src/setupProxy.js 

## In the Cloud API database
Swagger UI: [http://54.206.38.19:8080/swagger-ui/index.html]

##Server Locally (Optional)
### Local database API
[http://127.0.0.1:8080]

### You can see the function in /rockets-frontend/src/setupProxy.js 
### Requirements: JDK 17+, Maven

## Step 1. Configure rockets-frontend/src/setupProxy.js file, change target to
http://127.0.0.1:8080


## Step 2. Cd to backend folder
cd capstone-project-9900f18arockets/rockets-backend

## Step 3: Package backend server into JAR file using Maven. (Make sure Maven is installed)
mvn clean package -DskipTests=true

## Step 4: Run JAR file to start backend terminal 
java -jar rockets-backend-0.0.1-SNAPSHOT.jar

## Step 5: Now the back-end server is running, you can start your front-end server as described in Section 5.1


# User Decument in CSE vlab

## CSE Vlab use yarn open front-end folder

Installation via script (for Unix-based systems like Linux or macOS)

###1. Code under the front-end document:

curl -o- -L https://yarnpkg.com/install.sh | bash

### 2.Open your .bash_profile file (or create it if it doesn't exist):

nano ~/.bash_profile

### 3.Add the following line at the end of the file:

export PATH="$HOME/.yarn/bin:$HOME/.config/yarn/global/node_modules/.bin:$PATH"

### 4. Press CTRL + X to close the editor. Press Y to save the changes and Enter to confirm the file name.

### 5.You will need to upgrade Node.js to a version that's compatible with create-react-app. Here's how you can do that using a tool called nvm (Node Version Manager), which allows you to install and manage multiple versions of Node.js:
install nvm by downloading and running the install script with curl:

curl -o- https://raw.githubusercontent.com/nvm-sh/nvm/v0.39.1/install.sh | bash

### 6.Check your .bash_profile

nano ~/.bash_profile

Make sure you have export nvm in your file and if don’t have add it below

export NVM_DIR="$HOME/.nvm"
[ -s "$NVM_DIR/nvm.sh" ] && \. "$NVM_DIR/nvm.sh"
[ -s "$NVM_DIR/bash_completion" ] && \. "$NVM_DIR/bash_completion"

### 7.load the .bash_profile into the current shell session:

source ~/.bash_profile

### 8. You can use nvm to install the latest version of Node.js

nvm install node

### 9.You can check version about yarn , nvm and node version to make sure it can compatible

yarn --version
nvm –version
node --version

### 10. You can yarn install under the front-end document
yarn install

### 10. You can yarn start under the front-end document
yarn start





## Backend technology stack

Technical framework SpringBoot
Data Persistence Mysql
Involves dependencies on spring-security, spring-data-jpa

### Development/Deployment Guide

Interface debugging/reference swagger address [http://54.206.38.19:8080/swagger-ui/index.html](http://54.206.38.19:8080/swagger-ui/index.html).

The deployed interface proxy prefix is `/api`, which means accessing 54.206.38.19/api/demo will be proxied to 54.206.38.19:8080/demo

Front-end proxy configuration reference [proxying-api-requests-in-development](https://create-react-app.dev/docs/proxying-api-requests-in-development/)
