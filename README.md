This project implements a novel solution for classifying volleyball serves using computer
vision and machine learning techniques. Python, AlphaPose, and a scikit-learn Random
Forest Algorithm are utilized to process and categorize short clips of volleyball serves as
either float or topspin serves. This project was written in a Google Colab and Drive environment.
Clips of serves are gathered, standardized, and cleaned. They are then processed through
AlphaPose to extract keypoints (e.g. shoulders, hips, elbows, wrists), which we use to
calculate a backswing angle in each frame for each a player’s serve. We process the serves
into two empty lists that contain sequences of backswing angles and labels for the serve type,
then train a Random Forest Algorithm to classify serves based on this input. Our program
successfully processes and classifies the test serve given (float1) which is not included in the
training dataset.
