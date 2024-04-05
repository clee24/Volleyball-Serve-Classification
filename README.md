This project utilizes integration with google collab and drive. Here you can find the serve clips, pre and post processing: https://drive.google.com/drive/folders/1_UTDNu_3ikEUtE5SoVbYhcdkLD2lSOK3?usp=drive_link. 
<br />
<br />
<br />
**Project flow**
<br />
<br />
1. We gather a set of two different types of volleyball serves: topspin and float as video clips
  
2. We format them for editing, standardizing the timing to ~1 second and isolating the player’s serve from the penultimate jump

3. We use AlphaPose to extract keypoints (e.g. shoulders, hips, elbows, wrists)

4. We use these keypoints to calculate a backswing angle in each frame for a player’s serve.

5. We process the serves into two empty lists “backswing_angles” and “labels” that contain sequences of backswing angles and labels for serve type, respectively.

6. We then train a Random Forest Algorithm to classify serves, which it correctly does for a test serve not included in the dataset (float1)
<br />
<br />
**Update 4/5 Made a quick WordPress website for the program: https://wp.nyu.edu/volleyball_serve_classification/
