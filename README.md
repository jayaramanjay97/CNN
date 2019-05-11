# CNN

# Neural Style Transfer

The process of using CNN’s to render a content image in different styles is called as Neural Style Transfer.
The content image and the style image are merged to generate an
image which combines the content from the content image and the
style from the style image

DATA: A content image and a style image

VGG19 network pretrained on ImageNet dataset is used here to extract content and style features. The style and content features are obtained from the middle layers of VGG19. The loss function is designed in a way to minimize the content loss (difference between features of content image and target image) and also to minimize the style loss (difference between features of style image and target image). Then we train for few iterations to minimize the total loss (content loss + style loss).

After 2000 steps:
![alt text](https://raw.githubusercontent.com/jayaramanjay97/CNN/master/epoch2000.png)


After 4000 steps:
![alt text](https://raw.githubusercontent.com/jayaramanjay97/CNN/master/epoch4000.png)
