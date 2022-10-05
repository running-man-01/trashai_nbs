## STEP 0. Boot up machine

Start a local or remote linux machine with one or more GPU's, preferably with `Ubuntu 20.04 LTS`.

Go to: https://www.nvidia.com/Download/index.aspx and find the appropriate GPU driver for your machine. 

You **MUST** have Nvidia GPU and Nvidia Driver>=455.23 installed to enable GPU training. Yolo needs GPU and Detectron 2 **MUST** have GPU.


## STEP 1. install necessary dependencies

`sudo apt update`

`sudo apt install git wget curl python3-pip -y`



## STEP 2. get necessary files

`sudo wget https://raw.githubusercontent.com/running-man-01/trashai_nbs/main/starter.sh`



## STEP 3. deploy docker container

`bash starter.sh`

`sudo docker run --ipc=host -it -v "$(pwd)"/workdir:/usr/src/ -p 8888:8888 ultralytics/yolov5:latest`

`git clone https://github.com/running-man-01/trashai_nbs && cd trashai_nbs && jupyter-lab --ip=0.0.0.0 --port=8888 --no-browser --allow-root`

So far, the environment has been set up. You can go to the Jupyter Lab link pops up in the terminal.

Open Jupyter Notebooks you want to review in Jupyter Lab.
![lab](https://raw.githubusercontent.com/running-man-01/trashai_nbs/main/jlab.png)
