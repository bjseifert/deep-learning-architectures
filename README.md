Reflection

1. Which architecture was most effective for its task?
In my experience with this assignment, the Convolutional Neural Network (CNN) was the standout performer for image classification. While the MLP was able to recognize digits, the CNN reached a higher accuracy much faster on the Fashion-MNIST dataset. This is likely because the CNN uses filters to "see" spatial patterns like edges and textures, whereas the MLP treats the image like a flat list of numbers and loses that structural information. For the RNN, the LSTM was much more effective than a standard RNN for sentiment analysis because it actually "remembered" the context of the movie reviews.

2. What challenges did you face during training or implementation?
The biggest challenge was definitely training the DCGAN. It was very unstable; at one point, my Discriminator became "too smart," and the Generator stopped improving because it couldn't figure out how to fool the judge. I also ran into a few Shape Misalignment errors when transitioning from MNIST (1 channel) to CIFAR-10 (3 channels), which required me to carefully adjust the input layers of my CNN. Additionally, managing the data dimensions in the RNN/LSTM was tricky at first, specifically ensuring the embedding layer matched the hidden layer sizes.

3. How do you see these models being used in real-world applications?
I can see these architectures everywhere in daily technology:

CNNs: Are clearly the backbone of facial recognition on our phones and autonomous driving systems that need to "see" pedestrians.

RNNs/LSTMs: Are what power the predictive text on my keyboard and the sentiment analysis tools companies use to track customer feedback on social media.

DCGANs: Have huge potential in creative industries, like generating synthetic textures for video games or even helping doctors create "fake" medical data to train other AI models without compromising patient privacy.
