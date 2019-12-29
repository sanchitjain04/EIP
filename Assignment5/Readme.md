# Assignment 5

In this i tried experimenting many things in a ways to achieve good accuracy, was unable to debug the data augmentation error in my code hence the expected accuracy is quite low as per me, tried with diiferent models such as VGG16,resnet50,VGG19,Xception,MobileNetV2,InceptionV3,resnet_v2,inception_v3,inception_resnet_v2 as a backbone network, increased layers, decreased droupout, played with batch size as well,changing of epochs as well for every scenarios, tried with changing optimizer to adam and checked with decaying the learning rate with SGD.

Studied few of the solutions for various other techniques to improve accuracy for image classification also people sharing on the group as well how they implemented and achieved excellent accuracies but i understood a little less and hence did not try to do experimentation with that as understanding is also the key apart from achieving higher accuracies as per me. hence including the results i obtained after 70 epochs as the accuracy became constant:

val_gender_output_acc: 0.6381 
val_image_quality_output_acc: 0.5328 
val_age_output_acc: 0.4012 
val_weight_output_acc: 0.6164 
val_bag_output_acc: 0.5665 
val_footwear_output_acc: 0.6159 
val_pose_output_acc: 0.6109 
val_emotion_output_acc: 0.7092


