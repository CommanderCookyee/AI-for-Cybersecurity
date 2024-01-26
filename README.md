# AI-for-Cybersecurity
Detecting Tampered Images with Malware 


### Intorduction 
In this report, we introduce an innovative strategy that integrates a modified CNN and autoencoder model for steganalysis & a Hybrid Adversarial Auto encoder for ensembling. Our approach comprises three essential stages: utilizing EfficientNetB2 as the underlying CNN model, extracting DCT features from the images, and constructing a dedicated steganalysis model. Alongside the hybrid model, we explore the utilization of unsupervised learning deep learning models, such as Adversarial Auto Encoders (AAEs), to facilitate model ensembling techniques (Hybrid CNN + AAEs) that enhance adversarial robustness against adversarial examples. 

Steganography is the art of hiding information within other data, such as an image, audio, or video file. It plays a crucial role   maintaining privacy and confidentiality in communication, especially in the digital age where data can easily be intercepted and analysed. By hiding sensitive information within innocent-looking data, steganography allows people to communicate covertly without arousing suspicion. For companies this might mean a leakage of confidential data like technology blueprints etc. For government’s stegnography in images might mean espionage and for day-to-day users such stegnograph images might hide executables which can introduce malware into our systems.
DARKCOMET 

To ensure a comprehensive analysis, we employ two CNN models that examine different spatial dimensions: RGB and YCCBBR colour spaces. The EfficientNetB2 model, pretrained on ImageNet, operates on the RGB colour space, while the SRNET model focuses on the YCCBBR colour space. Additionally, the DCT features are extracted specifically from the YCCBBR colour space for a different perspective. 
Despite the use of smaller image sizes (256x256), the proposed model manages to achieve comparable or superior performance compared to the standard CNN model, EfficientNetB2, which operates on larger images (512x512). This suggests that our approach maintains the model's effectiveness even with reduced image dimensions.
In addition to the CNN model, we incorporate the use of unsupervised learning AAEs to detect stegnograph images. The parameters for this would be images of size (512 X 512) and 1000 image from each class. 
