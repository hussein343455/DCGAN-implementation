# DCGAN-implementation
-an implementation of DCGAN to create new images of numbers, the network is trained on the MINST dataset for (21000 steps) but it can be trained for longer to get better results.


-as shown in the gif is the training process we can see how the Generator is learning to create similar images
DCGAN .ipynb : DCGAN building and training code
disc.pt : discriminator model
gen.pt : generator model
## Training:
![ezgif com-gif-maker (2)](https://user-images.githubusercontent.com/57813196/110002610-9f504800-7d26-11eb-9b7f-c37e849b32ab.gif)

# Morphing generated images into Zero's
-first i created a classifier using the MNIST dataset ,which classify images into (zero's ,other).

build_zeror_classifier.ipynb : the classifier code used to update the noise vector
digit_morphing.ipynb :digit morphing code used to create the gif

steps: 
1. generate images using the DCGAN generator 
2. get the classifier predictions on the generated images
3. optimize the noise vector to get the best looking zero image (without updating the generator or classifiers weights)


![22](https://user-images.githubusercontent.com/57813196/110349506-d5057180-8043-11eb-89ad-aa5e793f7f63.gif)

## This Image Best Explains What The Morphing images is:


![asdfx](https://user-images.githubusercontent.com/57813196/110352590-29f6b700-8047-11eb-9472-3e15c94955dd.PNG)

