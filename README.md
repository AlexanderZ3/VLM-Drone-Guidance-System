# VLM-Drone-Guidance-System
This is an integrated VLM-Drone Guidance System, and we developed a way-finding signs dataset.

The system is designed to assist people with visual impairements in locating specified targets within environments rich in signage information. During navigation, the drone instructs users to stop, turn left, right, or move forward as appropriate when encountering obstacles or detecting way-finding signs. Upon reaching the target, the system alerts the user to stop.

![sample_dataset](https://github.com/user-attachments/assets/da2a18e6-fb05-4a91-967f-d8067909673a)

Above showcases scenarios randomly sampled from our collected dataset to demonstrate its complexity. It is important to recognize that way-finding signs may contain implicit semantic information. For instance, if the target is room "310" and the sign in the upper middle sub-image of the figure shows "302 to 315" with a left arrow, the guidance drone must interpret that the target room is within this range and provide navigational guidance as "turn left."

To the best of our knowledge, no existing datasets are designed to address the above task. We develop a dataset consisting of 320 way-finding sign images and 1,184 image-text Visual Question Answering (VQA) pairs for VLM fine-tuning and testing. The way-finding signs images are paired with a directional guidance label. The dataset can be augmented, as each image contains multiple signs, enabling the generation of diverse VQA input pairs by varying the target destination in the questions. Although the focus is on indoor navigation assistance, the dataset also includes outdoor way-finding signs to enhance training and evaluation, emphasizing the semantic content. The dataset has been open-sourced and will be continuously expanded to support future research.

This dataset can be used to train and evaluate the VQA and VLM models for way-finding signs understanding and reasoning tasks.
Please contact zezhong002@e.ntu.edu.sg  for downloading dataset.
