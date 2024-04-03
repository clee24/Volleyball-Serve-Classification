This project utilizes integration with google collab and drive. Here you can find the serve clips, pre and post processing: https://drive.google.com/drive/folders/1ScFt0AOFuzxsFSDifwvLVahLI6p4xtHA?usp=sharing. 
<br />
<br />
**Project flow**

We gather a set of two different types of volleyball serves: topspin and float as video clips

We format them for editing, standardizing the timing to ~1 second and isolating the player's serve from the penultimate jump

We use AlphaPose to extract keypoints (e.g. shoulders, hips, elbows, wrists)

We use these keypoints to calculate a backswing angle in each frame for a player's serve. 

We process the serves into two empty lists "backswing_angles" and "labels" that contain the sequence of backswing angles and a label if that serve is a topspin or float serve. 

We then train a Random Forest Algorithm to classify serves, which it correctly does for a serve not included in the dataset (float5)

***Currently working on expanding the dataset for a more robust algorithm. 
