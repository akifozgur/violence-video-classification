## Introduction

Detecting violence in various forms, such as physical altercations or aggressive behavior, is crucial for maintaining safety and security in society. The aim of violence detection systems is to automatically identify instances of violence in real-time using advanced technologies like computer vision and machine learning. These systems analyze visual and auditory cues from surveillance cameras, social media platforms, or other sources to recognize violent actions or events. The motivation behind developing violence detection technology stems from the pressing need to prevent and respond to violent incidents effectively. By swiftly detecting and alerting authorities to potentially dangerous situations, these systems can help mitigate the impact of violence and enhance public safety. Furthermore, in contexts like law enforcement, security monitoring, or crowd management, the ability to identify and intervene in violent situations promptly is paramount for maintaining order and preventing harm. Additionally, violence detection systems can aid in the monitoring and enforcement of policies and regulations aimed at curbing violence in various settings, including public spaces, schools, or online platforms. By providing valuable insights into patterns of violent behavior and facilitating data-driven decision-making, these systems contribute to the development of proactive strategies for violence prevention and intervention. In summary, the aim of violence detection technology is to automatically identify instances of violence using advanced technologies like computer vision and machine learning. The motivation behind this technology is to prevent and respond to violent incidents effectively, enhance public safety, and enforce policies aimed at curbing violence.

## Model

https://drive.google.com/file/d/1SkD6J82fFItEdNsdu0QOT-y9WvxahUFp/view?usp=sharing

## Dataset

https://drive.google.com/drive/folders/1lV3nD6-jQYj9s18GRYlQ54wPQqeS0Ezi?usp=sharing

https://drive.google.com/drive/folders/1ylavlDyf46qKypB_4JWob-5tZkv8nhzJ?usp=sharing

We have utilized the Real Life Violence Situations Dataset dataset for our project. This dataset contains 1000 violence and 1000 non-violence videos collected from YouTube videos. The videos in the violence class contain many real street fight situations in several environments and conditions. Also, the videos in the non-violence class were collected from various human actions like sports, eating, walking, etc.

<h2> Model</h2>

In this project, we used the pretrained ResNet-101 model, which has proven to be an important model in classification tasks, as the backbone. We passed our data through the ResNet to extract feature maps. Next, we fed the obtained feature maps into an LSTM layer. Finally, we took the output from the LSTM layer and passed it through a fully connected layer to perform the classification. Throughout this process, we set the initial learning rate to 1e-5. We used Adam as the optimizer and Binary Cross-Entropy Loss as the loss function.

<p align="center"> 
<img src=https://github.com/akifozgur/violence-video-classification/blob/main/img/model.png>
  </p>


<h2>Accuracy and Loss Curves</h2>
<p align="center"> 
<img src=https://github.com/akifozgur/violence-video-classification/blob/main/img/acc_loss.png>
</p>
