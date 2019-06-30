---
title: "About Pose Estimation Evaluation"
date: 2019-07-01 03:28:00 -0400
categories: PoseEstimation Evaluation
---
첫번째 포스팅은 제가 연구중인 Pose Estimation Evaluation Metric에 대해 소개하겠습니다.

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


`_posts` directory. Go ahead and edit it and re-build the site to see your changes. You can rebuild the site in many different ways, but the most common way is to run `jekyll serve`, which launches a web server and auto-regenerates your site when a file is updated.

To add new posts, simply add a file in the `_posts` directory that follows the convention `YYYY-MM-DD-name-of-post.ext` and includes the necessary front matter. Take a look at the source for this post to get an idea about how it works.

Jekyll also offers powerful support for code snippets:

​```python
def print_hi(name):
  print("hello", name)
print_hi('Tom')
​```

Check out the [Jekyll docs][jekyll-docs] for more info on how to get the most out of Jekyll. File all bugs/feature requests at [Jekyll’s GitHub repo][jekyll-gh]. If you have questions, you can ask them on [Jekyll Talk][jekyll-talk].

[jekyll-docs]: https://jekyllrb.com/docs/home
[jekyll-gh]:   https://github.com/jekyll/jekyll
[jekyll-talk]: https://talk.jekyllrb.com/
