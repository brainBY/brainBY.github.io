---
title: "About Pose Estimation Evaluation"
date: 2019-07-01 03:28:00 -0400
categories: PoseEstimation Evaluation
---
첫번째 포스팅은 제가 연구중인 Pose Estimation 분야의 Evaluation Metric에 대해 소개하겠습니다.

'PCK (Percentage of Correct Keypoints)'
We define a candidate keypoint to be correct if it falls within α · max(h, w) pixels of the ground-truth keypoint, where h and w are the height and width of the bounding box respectively, and α controls the relative threshold for considering correctness. (usually use torso)
A candidate keypoint to be correct if it falls within α · max(h, w) pixels of the groundtruth keypoint, where h and w are the height and width of the bounding box of human (usually use torso)
ex) PCK@0.2 : α를 0.2로 잡은 PCK 
ref) Articulated Human Detection with Flexible Mixtures-of-Parts

'PCKh: using head size instead of bounding box size'
MPII dataset엔 coordinates of the head rectangle 있음
ref) 2d human pose estimation: New benchmark and state of the art analysis

'PCP: Percentage of Correctly estimated body Parts'
Ref) V. Ferrari, M. Marin-Jimenez, and A. Zisserman, “Progressive search space reduction for human pose estimation,” in IEEE Conference on Computer Vision and Pattern Recognition, 2008.

'PCPm'

그밖의 metric : AP 등 https://darkpgmr.tistory.com/162 참고
