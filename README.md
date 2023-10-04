# IDS_706-Data_Engineering_Systems
## Mini-Project 5 : Python Script interacting with SQL Database



***

#### Purpose

This project is for a data engineering course (Mini-Project 5). It involves the use of a Python script to interact with an SQL database. The project also implements continuous integration through GitHub Actions to automate the setup of the environment, perform testing, code formatting, and code linting.

***

#### ETL-Query Operations

Extract (E): Retrieves a dataset in CSV format from a specified URL.
Transform (T): Cleans, filters, and enriches the extracted data, preparing it for analysis.
Load (L): Loads the transformed data into a SQLite Database table using Python's sqlite3 module.
Query (Q): Writes and executes SQL queries on the SQLite database to analyze and extract insights from the data.

****

#### Process

The template given by Professor Noah was used in this project. It was modified by replacing the original dataset (food market) with a dataset related to ice-cream flavours sold by Baskin Robbins. This dataset was extracted into a local CSV file. It was cleaned and transformed, and then loaded into a .db file. SQL queries were then executed to analyze the data. This repo also includes functions for data extraction, transformation and data loading. It also includes a a function which Implements an SQL log to record all actions performed during queries.

Dataset: [Baskin Robbins Ice-Cream](https://raw.githubusercontent.com/prasertcbs/basic-dataset/master/baskin_icecream.csv)

***

#### This template includes:
1. **.devcontainer**: configuration folder which contains a **Dockerfile** and **devcontainer.json**.
   - **Dockerfile**: specifies the instructions for building a Docker container image that will be used as the development environment.
   - **devcontainer.json**: defines the settings for the development container, such as which Dockerfile to use and environment variables.
3. **Makefile**: contains a set of rules that define how to compile source code, run tests, and perform other development tasks. 
4. **requirements.txt**: lists all the external libraries and dependencies required for the project to run correctly. It helps ensure that everyone working on the project uses the same versions of libraries, which is important for reproducibility and compatibility.
5. **workflows**: contains configuration file **(cicd.yml)** for matrix build that tests more than one version of Python.
6. **main.py**: contains a basic function which displays system info.
7. **test_main.py**: python file to test the function in main.
8. **README**: gives developers a detailed description of the GitHub project.
9. **.gitignore**: specifies files and directories that should be ignored by Git, the version control system used by GitHub. Changes in files or directories in the .gitignore file will not be tracked by Git, and they will not be included in the version history.

***

### Commands to Run the Repo

To run the project, you can use the Makefile and follow these commands:
1. ```
   # To install the required the python packages
   make install
   ```
2. ```
   # To check code style
   make lint
   ```
3. ```
   # To run tests
   make test
   ```
4. ```
   # To format the code
   make format
   ```
5. ```
   # To perform all the above tasks (install, test, format, lint)
   make all
   ```

***
