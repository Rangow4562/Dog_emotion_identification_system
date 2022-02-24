# Dog_emotion_identification_system

### TOPIC TITLE : Emotion Recognition in Dogs
#### PROGRESS-
##### • We follow the ICML's official training, validation, and test sets while 
training on our dataset (FER2013 dataset reference). Our dataset 
contains 5954 pictures of four main emotions: anger, fear, happiness, 
and sadness.
##### •  Training and Inference:
 We run all experiments for 300 epochs optimizing the cross-entropy 
loss. In the following sections, we vary the optimizer used as well as the 
learning rate schedulers and maintain other parameters constant.
##### • We use a fixed momentum of 0.9 and a weight decay of 0.0001. All 
experiments are run with gradient scaling to prevent gradient 
underflow. The models are evaluated using validation accuracy and 
tested using standard ten-crop averaging.
##### • CNN Architecture
##### • Performance
 
 
[![image](https://www.linkpicture.com/q/ddd_2.jpg)](https://www.linkpicture.com/view.php?img=LPic6217311e118b61936798411)

 summarizes reported classification accuracies FER2013. Most reported 
methods perform better than the estimated human performance (~ 72.75 %). 
Method Accuracy Rate
CNN(26)train 0.706%
CNN(26)test 0.6789%
The best-reported single-network accuracy is 72.7 % . In this work, we achieve 
the state-of-the-art accuracy 70.6% as compared to the human emotion 
detection techniques.
• OUTPUT
anger: 99.85%
 emotion prob
0 anger 0.998547
1 happy 0.001035
2 fear 0.000328
3 sad 0.000091
happy: 97.91%
 emotion prob
1 happy 0.979122
0 anger 0.012402
3 sad 0.008195
2 fear 0.000280
sad: 63.52%
 emotion prob
3 sad 0.635215
2 fear 0.362007
1 happy 0.002070
0 anger 0.000708
fear: 68.8%
 emotion prob
2 fear 0.688002
3 sad 0.256879
0 anger 0.048149
1 happy 0.006969
• Saliency map
The ‘black box’ nature of deep learning models makes it difficult to 
understand how the model processes the input image to obtain the final 
result. Visualizing the information captured inside deep neural networks 
is important in evaluating the effectiveness of the model and 
understanding how it computes its prediction.
Thus, generating an understandable visualization of our CNN can help 
describe how it differentiates between and captures different facial 
emotions.
The above images show model learned to focus on the mouth for happy.
We generate the saliency map using our best performing network to 
understand how it classifies each emotion. The above figure shows a 
saliency map for each emotion before and after being superimposed on 
the image it is generated from. Judging by all the images, our CNN can 
effectively capture most of the critical regions for each emotion.
Our approach is also efficiently removing regions such as the backdrop, 
which are unhelpful in conveying dog emotions
