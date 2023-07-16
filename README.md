# Fake-Hand-Digit-Generation-using-GANS
To create fake hand digit images DC GAN's were used. The coding is done in pytorch.
The dataset used was MNIST hand digit dataset. The standard training dataset given was used along with the test dataset provided by MNIST by default.
First the dataset was downloaded and loaded for processing. 
Next images were resized for 28*28*1 size. This size was chosen because it’s easy to process. 
First a standard GAN architecture was used to generate images with batch size 128 and 100 latent size as given. 
Though it generated results which were acceptable it was not good accurate enough. 
So, DC GAN was used as the next step. Many architectures were tried with DC GAN. 
The discriminator architecture and generator architecture were changed, and results were observed. 
Learning rates were also changed and results were observed. After several testing the best learning rate which gave results was 0.0003. 
There were some research articles which have stated that 0.0003 is the best learning rate with Adam optimizer. 
The 10-training epochs gave the best results.
