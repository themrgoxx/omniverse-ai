

 - Run these commands to remove pre-made files.

        cd ~/cv_samples_v1.2.0/ 
        
        rm -r detectnet_v2/ 

        mkdir detectnet_v2/

![image](https://user-images.githubusercontent.com/589439/143729065-f90e8ed0-07ac-4c77-8e4b-8d4c7fcffdef.png)

 - Navigate to Home -> cv_samples_v1.2.0 -> detectnet_v2

 ![image](https://user-images.githubusercontent.com/589439/143727464-598963b9-73c6-4b65-a617-5eecf454f4e9.png)

 - Download the detectnet_v2.zip from this <a href="https://github.com/pantelis-classes/omniverse-ai/raw/main/detectnet_v2.zip">link</a>.

![image](https://user-images.githubusercontent.com/589439/143727479-6828fc05-4672-4c60-8a21-f1fe6e97d0ea.png)

 - Run this command to move the .zip from your downloads folder to your detectnet_v2 folder.

        mv ~/Downloads/detectnet_v2.zip ~/cv_samples_v1.2.0/detectnet_v2

![image](https://user-images.githubusercontent.com/589439/143727509-2313c55c-bc6d-4451-91f1-f4424fac580a.png)

 - Run this command to unzip the folder.

        unzip ~/cv_samples_v1.2.0/detectnet_v2/detectnet_v2

![image](https://user-images.githubusercontent.com/589439/143729162-ad6f82c6-643e-4ec0-a082-75842c237053.png)

![image](https://user-images.githubusercontent.com/589439/143729154-00111bfe-534d-4403-bcab-92e3adf032ee.png)

 - Run this command to copy your dataset to the TAO folder. (You generate this dataset in this <a href="https://github.com/pantelis-classes/omniverse-ai/wiki/Synthetic-Data-Generation-(Python-API)#offline-training-with-tlt">wiki page</a>.)

        cp -r ~/.local/share/ov/pkg/isaac_sim-2021.2.0/output/testing/ ~/cv_samples_v1.2.0/detectnet_v2/workspace/tao-experiment/data/

        cp -r ~/.local/share/ov/pkg/isaac_sim-2021.2.0/output/training/ ~/cv_samples_v1.2.0/detectnet_v2/workspace/tao-experiment/data/

![image](https://user-images.githubusercontent.com/589439/143730111-33db8027-2c8e-41e8-98a6-9e5e45984fc5.png)

![image](https://user-images.githubusercontent.com/589439/143730115-59cf1d93-b27b-4902-a39b-522551733281.png)

 - Navigate to Home -> cv_samples_v1.2.0 -> detectnet_v2

 - Open the detectnet_v2.ipynb file.

![image](https://user-images.githubusercontent.com/589439/143729232-16e479b2-527e-4b0f-94b0-e43bd08cfba8.png)

![image](https://user-images.githubusercontent.com/589439/143729376-8e7db409-6651-4a55-90a7-8750d77d5838x.png)

 - Scroll down to section "0. Set up env variables and map drives" (Ctrl + F)

 ![image](https://user-images.githubusercontent.com/589439/143729413-dffdd2dc-d0cb-40aa-8b0f-fd567b2a527c.png)

 - Replace "diego" with your username. (TIP: whoami in BASH)

 ![image](https://user-images.githubusercontent.com/589439/143729441-e43fde75-76ed-489d-acef-56fea5ddf539.png)

 ![image](https://user-images.githubusercontent.com/589439/143729521-c7b0fc38-baf0-4701-9032-dba324497f5e.png)

 - Please watch this video to gain an understanding of the notebook.

 # VIDEO