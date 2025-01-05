# winterknotweed

## Introduction
  - So, umm this dataset was annotated on roboflow, leveraging their Label Assist tool to rapidly draw bounding boxes, then I reviewed all images manually and made corrections/deletions/additions as needed to all the annotations.  Then I downloaded the dataset as shown in the datasets folder here.
  - Today, I am leveraging my existing AWS account to train on an AWS GPU because although I could train at the nano level on my PC, training on the medium level gives many NMS time limit warnings and will result in a poor model.
  - Later I will add my Raspbery PI 5 robot code (scroll down for picture).  Right now, this is just to train the model and tie the computer vision to the steering.
  - The next generation robot will need to map the target area, probably with lidar and require more advanced autonomous or assisted steering and driving as well as remediation attachments.
  - In August I will photograph living knotweed and retrain. August/September is the optimal time to terminate knotweed.
  - I have until then to develop the robot.
## Training steps
  - Purchase an AWS EC2 P3 Instance
     - Deep Learning OSS Nvidia Driver AMI GPU TensorFlow 2.18 (Ubuntu 22.04)
     - g4dn 12XLarge $6.12 and hour
     - created a pem key for access (computervision.pem)
     - Allowing ssh access from my IP
  - Logged in via ssh
  - ssh -i C:\Users\User\source\python\winter_knotweed\computervision.pem ubuntu@ec2-52-206-140-136.compute-1.amazonaws.com

The Dave 209 robot test bed
 ![20250104_192800 (Small)](https://github.com/user-attachments/assets/59fe39b7-ece7-4dbe-a2ac-2eb8297dff12)
  -  


