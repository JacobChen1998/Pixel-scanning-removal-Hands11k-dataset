# Fit-hand-size-based-on-pixel-scanning-on-Hands11k-dataset

**Discription:**

This is the data preprocess of my master thesis.
We want to training CNN that learning from hand features with less noise.
Most of hand dataset doesn't fit the hand size. Therefore we need a process to remove useless part for our training work.
However, hand detection process sometime will cut fingers which we undesired.
Also, using cv2.findcontour function are not satisfying to us.
Therefore, we write this process for fit size.

**Hands11k dataset:** 

Hand 11k are a hand dataset contain 11076 hand images (1600x1200 pixels) and filming at white wall.

**About This process** 

This process can fit hand size based on scanning white/black ratio from binarization image through adjust ratio you wanted.
Here we have 4 ratio (top-to-down/down-to-top/right-to-left/left-to-right) you can adjust.
In addition, you can adjust binarization min/max to adjust more serious shadaw.

**Shortcome:**

The parameters at a set is not suitable for all the images.
At similar images, you can use same set of parameters.
And at another simuliar images, using another set of parameters.

**Flowchart of our process**

![image](https://github.com/JacobChen1998/Fit-hand-size-based-on-pixel-scanning-on-Hands11k-dataset/blob/main/data_preprocess_flowchart.png)

**Cutting area histogram based on parameters setting in the code**
![image](https://github.com/JacobChen1998/Fit-hand-size-based-on-pixel-scanning-on-Hands11k-dataset/blob/main/area.png)
