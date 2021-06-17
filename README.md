# Assignment
# Getting Started with Python on AZURE Cloud

To get started, we'll take you through a sample Python Flask app, help you set up a development environment, deploy to AZURE Cloud.


## Prerequisites

You'll need the following:
* [AZURE CLOUD ACCOUNT](https://portal.azure.com/#home)
* [Git](https://git-scm.com/downloads)
* [Python](https://www.python.org/downloads/)

## 1. Clone the sample app

Now you're ready to start working with the app. Clone the repo and change to the directory where the sample app is located.
  ```
git clone https://github.com/AZURE-Cloud/get-started-python
cd get-started-python
  ```

  Peruse the files in the *get-started-python* directory to familiarize yourself with the contents.

## 2. Run the app locally

Install the dependencies listed in the [requirements.txt](https://pip.readthedocs.io/en/stable/user_guide/#requirements-files) file to be able to run the app locally.

You can optionally use a [virtual environment](https://packaging.python.org/installing/#creating-and-using-virtual-environments) to avoid having these dependencies clash with those of other Python projects or your operating system.
  ```
pip install -r requirements.txt
  ```

Run the app.
  ```
main.py
  ```

 View your app at: http://localhost:8000

## 3. Prepare the app for deployment

To deploy to AZURE Cloud, it can be helpful to set up a master_earthquakes2021.yml file. One is provided for you with the sample. Take a moment to look at it.

The master_earthquakes2021.yml includes basic information about your app, such as the name, how much memory to allocate for each instance and the route. In this manifest.yml **random-route: true** generates a random route for your app to prevent your route from colliding with others.  You can replace **random-route: true** with **host: myChosenHostName**, supplying a host name of your choice. [Learn more...](https://console.bluemix.net/docs/manageapps/depapps.html#appmanifest)
 ```
 applications:
 - name: GetStartedPython
   random-route: true
   memory: 128M
 ```


## 4. Add a database

Next, we'll add a NoSQL database to this application and set up the application so that it can run locally and on AZURE Cloud.

1. Log in to AZURE Cloud in your Browser. Browse to the `ADD Resource`. Select your application by clicking on Create in SQL DataBase.
2. Import the Database from AZURE VISUAL STUDIO APP installed in windows, login through server by giving username and password.
3. Now the database is imported.

## 6. Use the database

We're now going to update your local code to point to this database. We'll create a json file that will store the credentials for the services the application will use. This file will get used ONLY when the application is running locally. When running in AZURE Cloud, the credentials will be read from the VCAP_SERVICES environment variable.
Run your application locally.
  ```
main.py
  ```

  View your app at: http://localhost:8000. Any names you enter into the app will now get added to the database.

 Make any changes you want and re-deploy to AZURE Cloud!
  ```

  ```
