Heart Disease UCI

https://www.kaggle.com/ronitf/heart-disease-uci/discussion/105877

For some unknown reason, the dataset for download on Kaggle is VERY different from the one you can download at https://archive.ics.uci.edu/ml/datasets/heart+Disease And what's worse: the description here on Kaggle is the same as the one in the Cleveland page, that means every interpretation you make based on the Kaggle dataset is WRONG. So here it goes, the CORRECT description of the kaggle dataset.

cp: chest pain type -- Value 0: asymptomatic -- Value 1: atypical angina -- Value 2: non-anginal pain -- Value 3: typical angina

restecg: resting electrocardiographic results -- Value 0: showing probable or definite left ventricular hypertrophy by Estes' criteria -- Value 1: normal -- Value 2: having ST-T wave abnormality (T wave inversions and/or ST elevation or depression of > 0.05 mV)

slope: the slope of the peak exercise ST segment 0: downsloping; 1: flat; 2: upsloping

thal: 1 = fixed defect; 2 = normal; 7 = reversable defect

target (maybe THE most important feature): 0 = disease, 1 = no disease

A few more things to consider: data #93, 139, 164, 165 and 252 have ca=4 which is incorrect. In the original Cleveland dataset they are NaNs (so they should be removed) data #49 and 282 have thal = 0, also incorrect. They are also NaNs in the original dataset.

I'll copy a sentence so you get more insight about the "thal" column (thal is for Thalium, a radioactive tracer injected during a stress test): --Nuclear stress testing requires the injection of a tracer, commonly technicium 99M (Myoview or Cardiolyte), which is then taken up by healthy, viable myocardial cells. A camera (detector) is used afterwards to image the heart and compare segments. A coronary stenosis is detected when a myocardial segment takes up the nuclear tracer at rest, but not during cardiac stress. This is called a "reversible defect." Scarred myocardium from prior infarct will not take up tracer at all and is referred to as a "fixed defect." --

You can check all of this by comparing the Kaggle and the UCI datasets. Feel free to ask/correct/comment/say hi.

To open a .data file, change the extension to a .txt and then open it with excel or similars.

You're welcome!
