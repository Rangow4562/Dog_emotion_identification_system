# Dog_emotion_identification_system

### TOPIC TITLE : Emotion Recognition in Dogs
#### PROGRESS-
##### • We follow the ICML's official training, validation, and test sets while training on our dataset (FER2013 dataset reference). Our dataset contains 5954 pictures of four main emotions: anger, fear, happiness, and sadness.
##### •  Training and Inference:We run all experiments for 300 epochs optimizing the cross-entropy loss. In the following sections, we vary the optimizer used as well as the learning rate schedulers and maintain other parameters constant.
##### • We use a fixed momentum of 0.9 and a weight decay of 0.0001. All experiments are run with gradient scaling to prevent gradient underflow. The models are evaluated using validation accuracy and tested using standard ten-crop averaging.
##### • CNN Architecture

[![image](https://www.linkpicture.com/q/ddd_2.jpg)](https://www.linkpicture.com/view.php?img=LPic6217311e118b61936798411)

##### • Performance
 summarizes reported classification accuracies FER2013. Most reported methods perform better than the estimated human performance (~ 72.75 %). 
 
 ##### Method Accuracy Rate
       CNN(26)train 0.726%
       CNN(26)test 0.6889%

##### The best-reported single-network accuracy is 72.7 % . In this work, we achieve the state-of-the-art accuracy 70.6% as compared to the human emotion detection techniques.

##### • OUTPUT
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

##### • Saliency map
The ‘black box’ nature of deep learning models makes it difficult to understand how the model processes the input image to obtain the final result. Visualizing the information captured inside deep neural networks is important in evaluating the effectiveness of the model and understanding how it computes its prediction.
Thus, generating an understandable visualization of our CNN can help describe how it differentiates between and captures different facial emotions.
The above images show model learned to focus on the mouth for happy.We generate the saliency map using our best performing network to understand how it classifies each emotion. The above figure shows a saliency map for each emotion before and after being superimposed on the image it is generated from. Judging by all the images, our CNN can effectively capture most of the critical regions for each emotion.Our approach is also efficiently removing regions such as the backdrop, which are unhelpful in conveying dog emotions

##### Conclusion

The purpose of this research was to determine if a deep learning system can classify various facial emotion classes in dogs, such as happiness, sadness, anger, and neutral. For this we proposed three different convolutional networks for this: a shallow CNN, sequential CNN, and MBCC-CNN. Following the experiments with the mentioned structures, we acquired accuracy of 58 percent, 61.28 percent, and 71.26 percent, respectively. The results indicate that by using mbcc-cnn, an accuracy of  71.26% can be obtained. The findings prove that, when compared to the other models, the suggested model mbcc-cnn outperforms in terms of facial expression recognition in dogs.
This study might help us better understand how dogs react to different items and stimuli in their surroundings, which could be important in veterinary science and other studies. It may also be used to track down missing dogs.
We propose further research on emotions in different animals. Additional efforts may be taken to increase classification performance, such as experimenting with alternative deep learning models on similar datasets, adding pre-processing methods, and combining other feature extraction tools. This research can be further expanded by doing a real-time detection.
