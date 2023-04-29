# spark-sql-code-test

> Thie notebook is for analyzing profile data which can be found here (https://coding-challenge-public.s3.ap-southeast-2.amazonaws.com/test-data.zip). Dataset includes 20 Json files. Apache Spark (Spark SQL) is used to load data into PySpark DataFrame and complete a set of analysis and satistics.  

## What is this?

This is a Jupyter notebook for operating a set of analysis on the profile dataset. Users need to set up a working Jupyter environment using docker to use this notebook. There are no other prerequisites and assumptions about the environment. You can find the steps of setting up your local environment to use this notebook.

## How to set up environment and use this repository?

 * Install Git Bash in your laptop. For windows, you can find download link from https://gitforwindows.org/
 * Generating SSH key and adding it to ssh-agent. Reference https://docs.github.com/en/authentication/connecting-to-github-with-ssh/generating-a-new-ssh-key-and-adding-it-to-the-ssh-agent.
 * Add SSH Key to your github account. Reference https://docs.github.com/en/authentication/connecting-to-github-with-ssh/adding-a-new-ssh-key-to-your-github-account.
 * Find a location in your local laptop to clone this repository. For example, we create a folder named as "jupyterProject".
 * In git bash terminal, navigate to the created folder "jupyterProject" and clone this repository: git clone git@github.com:GaryZHANG88/spark-sql-code-test.git.
 * Create a folder named as "test_data" to store json files and a folder named as "output" to store output parquet files. The repository folder structure will be shown below. Note: we are not uploading the test files into the remote repository because of the file size. We are also not adding the output parquet files into the remote repository.
 ![image](https://user-images.githubusercontent.com/131972943/235296684-f90932d4-19ed-40cc-a6eb-671c1f0f7c55.png)
 * Download test data files from https://coding-challenge-public.s3.ap-southeast-2.amazonaws.com/test-data.zip. Unzip the file and copy the 20 json files into the test_data folder in the repository.
 ![image](https://user-images.githubusercontent.com/131972943/235296780-7da432c0-97cc-43ed-811d-29a0a55f0f4a.png)
 * Install Docker Desktop in your laptop. For windows, you can find download link from https://docs.docker.com/desktop/install/windows-install/
 * Start Docker Desktop. In windows PowerShell, run command:  docker run -p 8888:8888 -v repository_folder_path:/home/jovyan/work jupyter/pyspark-notebook. repository_folder_path is the folder path that you created for clone the repository. In our example, the repository_folder_path is C:\Users\61450\jupyterProject. When we run this command the first time, docker cannot find the Jupyter image. It will downloand jupyter/pyspark-notebook image and create a docker container for jupyter notebook. The second time when we run this command to start docker container, it will skip to download step to start the container. After container is started, you can find a token in the powershell which will be used in next step.
 ![image](https://user-images.githubusercontent.com/131972943/235297413-a6171d26-e47a-460c-9cae-4ba6946d9a46.png)
 * Open a browser with http://localhost:8888 to start the Jupyter notebook. You will be directed to this page. Copy the token from last step and log in to Jupyter Notebook.
 ![image](https://user-images.githubusercontent.com/131972943/235297550-9c6ceafc-0796-4c7a-8dee-bda9e4211e4f.png)
* You will see the repository in Jupyter Notebook as shown below.
![image](https://user-images.githubusercontent.com/131972943/235287302-33e3fedf-1306-4d08-bb44-91f4f0ebd6a5.png)
