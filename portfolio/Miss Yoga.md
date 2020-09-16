---
title: Miss Yoga
subtitle: A Yoga Assistant Mobile Application Based on Keypoint Detection
collaborators: Renhao Huang, Jiqing Wang, Haowei Lou, Haodong Lu, Bofei Wang 
date: '2020-09-17'
thumb_image: images/miss-yoga.png

video_url: https://youtu.be/f0u11IM4GR8
layout: project
---




As the accelerating pace of modern life, many students, peo- ple with jobs and elders prefer exercising at home to a GYM to avoid the limitations from the location, time or privacy. To meet these requirements, many fitness applications, such as Keep (https://www.gotokeep.com), have become popular during these years and provide services including professional training guidance, supervision and communication platforms. Users can follow the training steps, via videos or literal statements, to complete their home-training plans.

Yoga, as a category of light-weight exercises, can benefit the physical and psychological health with little demand on physical strength and locations requirement. It is suitable for people of all ages. However, trainees with no scientific guidance from the Yoga specialist are likely to ignore some important pose details, and nonstandard Yoga poses may result in bad harm on the bones and joints. Therefore, a mobile application with ”real supervision” is helpful for these trainees who decide to train at home. Unlike those applications that provide the instructions only, the ”real supervision” requires the mobile application to ”watch” trainee’s poses and provide them with warning once they are posing incorrectly. In order to imitate a real Yoga teacher who is watching the trainee doing Yoga, the mobile application needs to illustrate steps, analyse the postures in real-time, evaluate and provide correct suggestions.

Many Yoga self-assessment systems are being proposed through the years. [1] is a segmentation-based approach and uses two Kinects to analyse users’ poses from both front and side. [2] provides a Yoga self-assessment system based on OpenPose[3] and utilizes an angle score calculation without using hardware. [4] is an end-to-end Yoga Pose classification technique that using OpenPose and a Recurrent Neural Network structure. It is apparent that OpenPose is highly appreciated on Yoga Pose analysis.

In this project, We demonstrate a practical and humanized Yoga Assistant mobile application inspired by [2] but utilize an improved score calculation algorithm to adapt different Yoga Poses and appended with more humanized designs such as voice service. We also evaluated these models with different Yoga poses under different scenes to ensure its robustness.


#### Reference

1. Hua-Tsung Chen, Yu-Zhen He, and Chun-Chieh Hsu. Computer-assisted yoga training system. Multimedia Tools and Applications, 77:23969– 23991, 2018.

2.  M. C. Thar, K. Z. N. Winn, and N. Funabiki. A proposal of yoga pose assessment method using pose detection for self-learning. In 2019 International Conference on Advanced Information Technologies (ICAIT), pages 137–142, 2019.

3. Z. Cao, G. Hidalgo Martinez, T. Simon, S. Wei, and Y. A. Sheikh. Openpose: Realtime multi-person 2d pose estimation using part affinity fields. IEEE Transactions on Pattern Analysis and Machine Intelligence, 2019.

4. Santosh Kumar Yadav, Amitojdeep Singh, Abhishek Gupta, and Jagdish Lal Raheja. Real-time yoga recognition using deep learning. Neural Computing and Applications, 31:9349–9361, 2019.

5. Hao-ShuFang,ShuqinXie,Yu-WingTai,andCewuLu.RMPE:Regional multi-person pose estimation. In ICCV, 2017.

6. Daniil Osokin. Real-time 2d multi-person pose estimation on cpu: Lightweight openpose. In ICPRAM, 2019.