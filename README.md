# eCommerce Application using OPENAPI Generator

- The repository contains a spring boot application that has been built from an open api generator and containerized using docker.
- The yaml file from which the code is generated is located at `./openapi/api.yaml`.
- The application generates [Swagger API](http://localhost:8080/swagger-ui/index.html) endpoints for easy testing.

## About the Application

- This application mimics the world of eCommerce. It allows users to create user accounts, add products to the database, attach a product category to each product and write reviews for products available in the database.
- The endpoints also allow for users to retrieve information about the reviews for each product that is available.

- **Authentication**
  - This application uses basic authentication.
  - All endpoints outside `/register` must be authenticated. 
  - Only users with an "ADMIN ROLE" may access `HTTP DELETE`
  - Ensure your basic authentication details are provided in postman prior to  sending any requests.

- **Endpoints**
  - All endpoints are available at `./postman collection` in the application directory.

## REQUIRED SOFTWARE
- An IDE ( [Visual Studio Code](https://code.visualstudio.com/download) or [Intellij IDEA](https://www.jetbrains.com/idea/download/?source=google&medium=cpc&campaign=APAC_en_AU_IDEA_Branded&term=intellij+idea&content=602143185772&gclid=EAIaIQobChMI-f3uuYnegwMVwqRmAh0_ewXKEAAYASABEgImY_D_BwE&section=windows) )
- [Docker](https://www.docker.com/products/docker-desktop/)
- [Postman API](https://www.postman.com/downloads/)
- A Web Browser ( [Google Chrome](https://www.google.com/chrome/) or [FireFox](https://www.mozilla.org/en-US/firefox/new/))
- [Java](https://www.oracle.com/java/technologies/downloads/) 17 at minimum installed on your local machine.
- [Git](https://www.git-scm.com/downloads)
- [GitHub Desktop](https://desktop.github.com/) (OPTIONAL)

  
## Setting Up - CLONE THE PROJECT
- Open a terminal or command prompt (Powershell on Windows, Terminal on linux or macOs)
- Navigate to the project directory. e.g. `cd path/to/your/directory`
- Run `git clone git@github.com:msackey-IW/springboot-docker-openapi-generator.git`
- Alternatively, in the [ project repository](https://github.com/msackey-IW/springboot-docker-openapi-generator) navigate to `code -> Open with GitHub Desktop`. Clone and open the product in GitHub Desktop
- Run `cd openapi`
- Run `docker-compose up` - This will create and run the springboot application by running the api.yaml file.
- All endpoints are available on [swagger](http://localhost:8080/swagger-ui/index.html).

## Setting Up - DOWNLOAD THE PROJECT
- Open and run Docker on your machine.
- Download the application [here](https://github.com/IntegrationWorks/springboot-docker-applications) by navigating to `code -> download ZIP`.
- Unzip the folder and open the extracted files in your downloaded IDE(Intellij or VSCode).
- Run `cd openapi` in the IDE terminal.
- Run `docker-compose up` - This will create and run the springboot application by running the api.yaml file.
- All endpoints are available on [swagger](http://localhost:8080/swagger-ui/index.html).

## Testing the Endpoints
- Open and run POSTMAN API
- In the main repository directory, navigate to `postman`
- The folder contains 4 JSON files. Each file must be uploaded to POSTMAN API via `settings -> data -> import Data -> Import Data file`.
- The collection now give you access to all the endpoints available in the application. 
- Requests may now be sent and received.

