# Assignment3
# Python on AZURE Cloud



## Prerequisites

You'll need the following:
* [AZURE CLOUD ACCOUNT](https://portal.azure.com/#home)
* [Visual Studio Code](https://code.visualstudio.com/download)


## 1. Run the app locally

Install the dependencies listed in the [requirements.txt](https://pip.readthedocs.io/en/stable/user_guide/#requirements-files) file to be able to run the app locally.

You can optionally use a [virtual environment](https://packaging.python.org/installing/#creating-and-using-virtual-environments) to avoid having these dependencies clash with those of other Python projects or your operating system.
  ```
pip install -r requirements.txt
  ```

Run the app.
  ```
Python app.py
  ```

 View your app at: http://localhost:8000

## 2. Create HTML files under Templates folder required for the Assignment
1. index.html
2. search.html


## 3. Add a database

Next, we'll add a Ms SQL database to this application and set up the application so that it can run locally and on AZURE Cloud.

1. Log in to AZURE Cloud in your Browser. Browse to the `ADD Resource`. Select your application by clicking on Create in SQL DataBase.
2. Import the Database from AZURE VISUAL STUDIO APP installed in windows, login through server by giving username and password.
3. Now the database is imported.

## 4. Use the database

We're now going to update your local code to point to this database. We'll create a json file that will store the credentials for the services the application will use. This file will get used ONLY when the application is running locally. When running in AZURE Cloud, the credentials will be read from the VCAP_SERVICES environment variable.
Run your application locally.
  ```
Python app.py
  ```

  View your app at: http://localhost:8000. Any names you enter into the app will now get added to the database.

## 5. Prepare the app for deployment

1. We're going to add Azure extensions in Visual Studio Code 
2. Select the file to be deployed.
3. Select the web app into which the app has to be deployed.
4. After the deployment, we can browse the web app created.

[ASSIGNMENT3](https://code.visualstudio.com/download)

  ```

  ```
