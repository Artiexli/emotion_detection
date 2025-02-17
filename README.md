# Textual Emotion Detection

RoBERTa Large powered Natural Language Processing project. Given a line of text, predict the emotion category under which that text falls under. Based upon the Paul Ekman Discrete Emotion Model (DEM) of human emotion with 6 categories, alongside an additional "neutral" category. 

Implemented as part of KotakeeOS Speech Server with a companion Emotion Representation class that is tied into the server's ability to output speech. That is to say, whenever the program says anything, an accompanying emotion will be predicted and presented to the user with a visual representation. 

Project background and concept informed by [1], which provided a wonderful overview of the subject.

Models may be trained on a combination of datasets obtained from online resources, as well as homegrown personally labelled datasets. All possible combinations include subsets from the following datasets:

1 ISEAR
  https://www.kaggle.com/shrivastava/isears-dataset

2 WASSA-2017 Emotion Intensities(EmoInt)
  http://alt.qcri.org/semeval2017/task4/index.php?id=download-the-full-training-data-for-semeval-2017-task-4 

3 Cecilia Ovesdotter Alm's Affect data
  http://people.rc.rit.edu/∼coagla/affectdata/index.html

4 DailyDialog
  https://www.aclweb.org/anthology/I17-1099/

5 Emotion Stimulus
  http://www.site.uottawa.ca/∼diana/resources/emotion_stimulus_data

6 MELD
  https://github.com/SenticNet/MELD

7 SMILE dataset
  https://figshare.com/articles/smile_annotations_final_csv/3187909 

---

For more information, please see [Emotion Avatar](http://emotionavatar.com/).

[![Emotion Avatar Website](https://i.imgur.com/mM2eWXg.png "Emotion Avatar Website")](http://emotionavatar.com/)


---

### References:

[1] Acheampong, FA, Wenyu, C, Nunoo-Mensah, H. Text-based emotion detection: Advances, challenges, and opportunities. Engineering Reports. 2020; 2:e12189. https://doi.org/10.1002/eng2.12189

---

### Usage:

1. Install pytorch to train the model. Training the model requires CUDA, 
   for which you must go to pytorch.org. 

2. Install everything required by EmotionDetection. Run:

   pip install -r requirements.txt 

3. Manually acquire roberta-large_fine-tuned and insert it inside the 
   ./models folder. 