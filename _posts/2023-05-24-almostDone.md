# Almost done!

Most of Question 2 and 3 is completed! Woohoo!

## Question 2 update

My only issues with Question 2 now is that both search_images and search_images_ddg (the later being the solution Brain provided to the bugs caused by the first) were both not working. This became an issue as I noted that I was potentially using the same images for my training and testing data set as I was downloading the images separately. To fix this, I downloaded all the images once, and separated the data with a some quick code chatGPT wrote (how handy!). Following this, I attempted to increase to amount of images to download, but this is where the image search functions stopped working. I plan to fix this tomorrow in the prac. After that question 2 will be complete. 

Issue with search_image: only downloads images for one directory. 

Issue with search_image_ddg:

![image](/images/screenshot.png)


## Question 3 update

Question 3 is also close to being done, however, at the moment I am trying to test different ResNet models to base my model off. ResNet18 worked well, but when I try ResNet50 and 101, the Kernal times out. This is super inconvenient! I will attempt to run these again, but the time it takes to run, and the likelihood of the kernel stopping makes it hard to keep attempting different ResNet models. 

## Everything else

Today I also got a better understand of why we are able to use the ResNet models to base our model off and wrote a blog post on that as well as a post on confusion matrices and T-SNE plots. 

Almost there!
