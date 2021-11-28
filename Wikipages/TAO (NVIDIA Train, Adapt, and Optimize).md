All instructions stem from this <a href="https://docs.nvidia.com/tao/tao-toolkit/text/tao_toolkit_quick_start_guide.html">Nvidia Doc</a>.

# Requirements

### Hardware Requirements (Recommended)

    32 GB system RAM

    32 GB of GPU RAM

    8 core CPU

    1 NVIDIA GPU

    100 GB of SSD space

### Hardware Requirements (REQUIRED)

     - TAO Toolkit is supported on **A100**, **V100** and **RTX 30x0 GPUs**.

# Login to the NGC docker registry.

Login to the NGC docker registry:
Use the command 

       docker login nvcr.io 
and enter the following credentials:

       a. Username: "$oauthtoken"
       b. Password: "YOUR_NGC_API_KEY"

 - Where YOUR_NGC_API_KEY corresponds to the key you generated from step 3.

![image](https://user-images.githubusercontent.com/589439/143663405-5323b62f-74a8-409f-80a8-c2c6ad961497.png)

# Installing TAO Toolkit

 - TAO Toolkit is a Python pip package that is hosted on the NVIDIA PyIndex. The package uses the docker restAPI under the hood to interact with the NGC Docker registry to pull and instantiate the underlying docker containers. You must have an NGC account and an API key associated with your account. See the Installation Prerequisites section for details on creating an NGC account and obtaining an API key.

## 1. Create a new virtualenv using virtualenvwrapper

 - Click this <a href="https://python-guide-cn.readthedocs.io/en/latest/dev/virtualenvs.html"> link</a> to understand how virtual enviroments in python work.

 - Make sure you have virtualenv installed by checking it's version. (Instructions are in this <a href="https://github.com/pantelis-classes/omniverse-ai/wiki/NVIDIA-Transfer-Learning-Toolkit-(TLT)-Installation#1-create-new-python-virtual-environment">page</a> of the)

        virtualenv --version

![image](https://user-images.githubusercontent.com/589439/143723668-73111ae8-0ac5-4729-b89b-481d29b25d16.png)

 ## 2. Define the environment variable called VIRTUALENVWRAPPER_PYTHON.

  - Run this command to see where your python is located.

        which python3

![image](https://user-images.githubusercontent.com/589439/143723824-968874c9-5f8e-44cc-a535-d0d336a72b78.png)

  - Define the environment variable of your Python location.

        export VIRTUALENVWRAPPER_PYTHON=/usr/bin/python3

![image](https://user-images.githubusercontent.com/589439/143723906-baf552bc-e9d1-435b-8d43-553f6f0a6707.png)

 - Run this command to make sure the enviroment variable was created. (There should be red output with the variable name.)

        env | grep 'VIRTUALENVWRAPPER_PYTHON'

![image](https://user-images.githubusercontent.com/589439/143723930-c9c8658f-339d-4693-894a-daf70dea28ae.png)

 - Run this command to create a virtualenv named "launcher".

        mkvirtualenv launcher -p $VIRTUALENVWRAPPER_PYTHON

![image](https://user-images.githubusercontent.com/589439/143724110-61196b6e-7d6e-4fc5-86a4-c7234cd4d379.png)

 - You should now see a (launcher) prepending your username in the CLI.

![image](https://user-images.githubusercontent.com/589439/143724128-692a9f83-0365-4f0f-9068-e8e6af9cac15.png)

## Intructions on how to activate/deactive the vitualenv.

 - When you are done with you session, you may deactivate your virtualenv using the deactivate command:

        deactivate

![image](https://user-images.githubusercontent.com/589439/143724159-ae6c0578-14e4-463b-8287-ef4147ff0f34.png)

 - You may re-instantiate this created virtualenv env using the workon command.

        workon launcher

![image](https://user-images.githubusercontent.com/589439/143724167-70721d41-12f2-4322-b611-3f07df92d344.png)

## 3. Once you have logged into the virtualenv, the command prompt should show the name of your virtual environment.










 Set the Python version in the virtualenv.