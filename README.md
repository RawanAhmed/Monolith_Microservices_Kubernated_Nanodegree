# Refactor Monolith to Microservices Kubernates

The project is split into there parts:

1- first part is backend display user 
2- second part is backend display feed 
3- third part is frontend

## ScreenShots: 


(ScreenShots/1.jpg)


## Getting Started

### Prerequisite
1. The depends on the Node Package Manager (NPM). You will need to download and install Node from [https://nodejs.com/en/download](https://nodejs.org/en/download/). This will allow you to be able to run `npm` commands.

### Database & Filestore
For this project, a Postgres database and S3 bucket were previously set up from AWS that are no longer running. If you wish to use your own database, filestore, update the config parameters on src/config/config.ts file

### Backend API
* To download all the package dependencies, run the command from the directories `udagram-api-user/` and `udagram-api-feed/`:
    ```bash
    npm install .
    ```
* To run the application locally, run:
    ```bash
    npm run dev
    ```
* You can visit `http://localhost:8100/api/v0/feed` in your web browser to verify that the application is running. You should see a JSON payload. 

### Frontend App
* To download all the package dependencies, run the command from the directory `udagram-frontend/`:
    ```bash
    npm install .
    ```
* Install Ionic Framework's Command Line tools for us to build and run the application:
    ```bash
    npm install -g ionic
    ```
* Prepare your application by compiling them into static files.
    ```bash
    ionic build
    ```
* Run the application locally using files created from the `ionic build` command.
    ```bash
    ionic serve
    ```
* You can visit `http://localhost:8100` in your web browser to verify that the application is running. You should see a web interface.

