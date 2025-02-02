# Facial-Expression-Recognition
Source code for facial expression recognition. Uses fer 2013 dataset and classifies images based on 7 emotions.

Built a CNN-based model to classify faces into seven emotions using the FER2013 dataset, which contains 48x48 grayscale images. 

The dataset was split into 20,709 training and 3,809 testing images. The model's first convolutional layer detected low-level features like edges and corners, while deeper layers captured high-level facial structures such as the eyes, nose, mouth, and eyebrows. 

I applied 3x3 convolutional filters to extract features and used ReLU activation to introduce non-linearity and improve learning. To enhance robustness against distortions and reduce computational complexity, I incorporated MaxPooling, which downsampled feature maps by selecting the maximum value in 2x2 regions. 

The model classified emotions by analyzing the ratio between detected facial features—such as a wider mouth-to-eye ratio indicating a likely open-mouth expression. After feature extraction, a Flatten layer converted spatial data into a vector, followed by a Dense layer for final classification. 

The model achieved 96% accuracy, demonstrating its effectiveness in recognizing facial expressions. This project strengthened my understanding of CNN architectures, feature extraction, and optimization techniques for image-based classification tasks
