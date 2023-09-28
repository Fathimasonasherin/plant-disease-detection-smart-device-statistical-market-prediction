# plant-disease-detection-smart-device-statistical-market-prediction
The prototype consists of four key components: the trained CNN model, the Raspberry Pi hardware
platform for processing, the camera module for capturing the images of the plant and the lcd to
display the results. The CNN model is trained on a comprehensive dataset of plant images, containing
various species and diseases. The model architecture is carefully designed to balance accuracy and
computational efficiency, taking into account the limitations of the Raspberry Pi's hardware resources.
The trained model is then integrated into the Raspberry Pi, which serves as the on-device inference
platform. The Raspberry Pi provides the necessary computing power, memory, and storage to perform
real-time disease detection, enabling farmers to obtain immediate results without relying on an
internet connection or external servers. Once an image is provided, the system processes it through
the trained CNN model, performs disease classification, and displays the results on the lcd. The final
prototype demonstrates the feasibility and practicality of using CNNs on a Raspberry Pi for on-site
plant disease detection, providing farmers with an accessible and efficient tool to manage crop health
effectively.

Algorithms and Frameworks –

 Tensorflow and Keras
 
 Scikit Learn, Numpy, Matplotlib, Seaborn
 
Dataset - The dataset consists of around 20.6 k .jpg files belonging to 15 classes of the healthy,
bacterial, fungal, and viral diseased leaves of plants like tomato, pepper, and potato.

Data Preprocessing - The data was normalised, splitted into train, and test in 80-20 manner, also
some data augmentation was applied so that the dataset increases and generalizes well.The data
was converted into a One vs Rest Format using sklearn’s Label Binarizer.

ML Modelling - Custom CNN architecture having 5 layers with dropout and max pooling was used to
perform the detection and a dense neural network at the end as the classifier.
