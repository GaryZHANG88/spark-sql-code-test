# spark-sql-code-test

> Thie notebook is for analyzing profile data which can be found here (https://coding-challenge-public.s3.ap-southeast-2.amazonaws.com/test-data.zip). Dataset includes 20 Json files. Apache Spark (Spark SQL) is used to load data into PySpark DataFrame and complete a set of analysis and satistics.  

## What is this?

This is a Jupyter notebook for operating a set of analysis on the profile dataset. Users need to set up a working Jupyter environment using docker to use this notebook. There are no other prerequisites and assumptions about the environment. You can find the steps of setting up your local environment to use this notebook.

## How to set up environment?

 * Install Git Bash in your laptop. For windows, you can find download link from https://gitforwindows.org/
 * Create a folder for storing thie repository. For example, a folder is created as "jupyterProject".
 * Open Git Bash, navigate to folder "jupyterProject" and clone this repository using command "git clone git@github.com:GaryZHANG88/spark-sql-code-test.git"  
 * Install Docker Desktop in your laptop. For windows, you can find download link from https://docs.docker.com/desktop/install/windows-install/
 * Open windows powershell to download and install pyspark jupyter notebook environment. Replace "created folder path" with the path of your created folder. The first    time will download the images to your laptop. Once it is downloaded, it won't have downloading process again when you run the docker container the second time.
   docker run -p 8888:8888 -v {created folder path}:/home/jovyan/work jupyter/pyspark-notebook
 * Open a browser with http://localhost:8888 to start the Jupyter notebook. You will see the project files inside Jupyter Notebook as shown below.

![image](https://user-images.githubusercontent.com/131972943/235287302-33e3fedf-1306-4d08-bb44-91f4f0ebd6a5.png)
