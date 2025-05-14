ABSTRACT



This project Detecting accidents in tunnels is critical for ensuring the safety of commuters and maintaining the efficiency of transportation systems. This project proposes a deep learning-based approach utilizing YOLOv7 (You Only Look Once version 7) to identify accidents within tunnel environments. The methodology begins with importing essential libraries and acquiring a specialized dataset comprising tunnel accident images. The dataset undergoes thorough preprocessing to ensure consistency and quality, followed by a structured split into training, validation, and testing sets. This division is crucial to train the model effectively, fine-tune its parameters, and objectively evaluate its performance. The YOLOv7 model, known for its real-time object detection capabilities, is selected and trained on the prepared dataset, using provided annotations or bounding boxes to accurately localize and classify accident scenarios within the images.

Throughout the training process, progress is carefully monitored and logged to identify potential areas for improvement and ensure the model's optimal performance. Once trained, the model is evaluated using key performance metrics such as accuracy, precision, and recall, providing a comprehensive understanding of its ability to detect tunnel accidents reliably. The results demonstrate the promising potential of deep learning, particularly YOLOv7, in enhancing accident detection systems within tunnel environments.

Looking ahead, a major future enhancement for this project involves the integration of an automated emergency alert system. This system would be designed to instantly notify nearby hospitals, police stations, and emergency services whenever an accident is detected, ensuring rapid response times and potentially saving lives. Such integration would transform this detection system into a fully operational, life-saving solution for modern transportation infrastructures.

1.1	Introduction

Ensuring the safety of commuters in tunnels is paramount, and detecting accidents promptly is critical for effective response. This paper presents a deep learning-based approach utilizing YOLOv7 for accident identification in tunnel images. The proposed method encompasses importing essential libraries, acquiring and preprocessing the dataset, dividing it into training, validation, and testing sets, selecting and training the YOLOv7 model, and assessing its performance. The model is fine-tuned on a tunnel accident dataset to predict accidents based on supplied annotations or bounding boxes. The training progress is monitored and logged, and the model's performance is evaluated using metrics including accuracy, precision, and recall. This study highlights the potential of deep learning for accident detection in tunnels, paving the way for safer and more efficient transportation systems.

Ensuring commuter safety in tunnels is crucial. Detecting accidents quickly allows for effective emergency response. This project proposes using a deep learning approach YOLOv7 to detect accidents in tunnel images. It includes steps like importing libraries, data preprocessing, model training, and evaluation using metrics such as accuracy, precision, and recall.
 Tunnel safety is a major concern worldwide, as tunnels have confined spaces with limited escape options, making accidents particularly dangerous. Rapid and accurate accident detection is crucial to reduce casualties and property loss. Traditional methods, such as manual CCTV monitoring, are often slow and inefficient, especially in low-light or unclear tunnel environments. To overcome these limitations, this project proposes an automated accident detection system using deep learning techniques. Specifically, the YOLOv7 model (You Only Look Once - Version 7) is fine-tuned to detect accidents in tunnel images. By utilizing object detection algorithms and real-time analysis, the system aims to significantly enhance safety measures in tunnels.    
1.2	 Problem Statement
The Existing tunnel accident detection systems, while helpful, have several limitations that reduce their effectiveness. Most notably, they require a massive amount of labeled data to train the deep learning models effectively, which is a costly and time-consuming process. Furthermore, these models often struggle with changes in lighting conditions, obstructions, and environmental variations inside tunnels, leading to inaccuracies in detection. Computational demands are another major concern, as real-time video processing requires powerful hardware resources that may not always be feasible. Moreover, accidents that occur outside of camera views or under very poor visibility conditions often go undetected. Thus, there is an urgent need for a robust, efficient, and accurate system that can overcome these challenges and ensure reliable accident detection in tunnels.
Partial Detection: Some systems fail to detect accidents occurring outside the camera frame or in blind spots. Thus, there is a need for a robust, real-time, and efficient accident detection system that performs reliably under varying conditions.
1.3	 Existing Systems
Current systems for tunnel accident detection mainly use deep learning-based video analysis techniques. Typically, pre-processed still images extracted from video streams are fed into object detection models like Faster R-CNN or other convolutional neural networks. These models can classify objects such as cars, fires, or people and predict their location through bounding boxes. While effective to some extent, these systems suffer from several shortcomings. They heavily rely on the quality and quantity of the training datasets, and their accuracy drops significantly in poor lighting or when occlusions are present. Furthermore, real-time application remains a challenge due to the computational burden associated with processing high volumes of video data.
1.4	 Objective
The objective of this project is to develop an intelligent system that can accurately and quickly detect accidents inside tunnels to minimize human casualties and property damage. The system aims to automate the monitoring of tunnel conditions, reducing dependency on manual surveillance and ensuring that emergencies are detected without delay. By integrating deep learning-based accident detection with real-time alert mechanisms, the project seeks to enhance tunnel safety significantly. Another important is to contribute towards the broader vision of smart transportation systems by enabling real-time accident detection as a part of intelligent infrastructure solutions. Ultimately, the project aspires to save lives, minimize economic loss, and promote safer travel through tunnels.


Proposed System:
The proposed system focuses on the real-time detection of tunnel accidents using the powerful deep learning-based object detection model YOLOv7 (You Only Look Once, Version 7). Unlike traditional monitoring systems that rely on manual CCTV observation or simple motion detection algorithms, this system leverages advanced computer vision to analyze tunnel surveillance footage automatically.
The system processes each video frame and identifies accidents such as car collisions, stranded vehicles, fires, or pedestrians on roadways. Using annotated datasets of tunnel scenarios, the YOLOv7 model is fine-tuned to recognize these events with high accuracy even under poor visibility conditions like smoke, darkness, or tunnel reflections. 
The proposed solution is designed to work efficiently in real-time settings with minimal latency, ensuring continuous 24x7 monitoring of tunnel environments. It is scalable, meaning it can be deployed across multiple tunnels with adjustable parameters depending on specific site conditions.
4.1 Architecture of the System
The architecture of the Tunnel Accident Detection System is modular and follows a structured data flow for efficiency and reliability. The major architectural components include:
•	Input Layer (Data Acquisition):	
CCTV cameras continuously capture tunnel video streams or still images. These images act as raw input for the system.
•	Preprocessing Layer:	
Captured images are resized, normalized, and augmented if needed. Preprocessing ensures that the model input remains consistent, regardless of varying camera resolutions or lighting conditions.
•	Detection Layer (YOLOv7 Model):	
The preprocessed frames are passed to the YOLOv7 object detection model, which processes each frame and identifies objects using bounding boxes. The model outputs include the location, class label (e.g., accident, fire, stranded vehicle), and confidence scores.
•	Decision Layer (Accident Validation):	
Based on confidence thresholds, the system verifies whether a true accident is detected. This validation minimizes false positives and ensures alerts are meaningful.
•	Notification Layer:	
Upon confirmation, the system generates real-time notifications and alerts for tunnel operators and emergency response teams.
•	Data Logging and Analytics Layer:	
All detected incidents are logged with timestamps, camera IDs, and prediction details. Over time, this dataset can be used to analyze accident trends and improve tunnel safety policies.


 

Fig 1: System architecture




     4.2 Data Flow Diagram:
1.	The DFD is also called as bubble chart. It is a simple graphical formalism that can be used to represent a system in terms of input data to the system, various processing carried out on this data, and the output data is generated by this system.
2.	The data flow diagram (DFD) is one of the most important modeling tools. It is used to model the system components. These components are the system process, the data used by the process, an external entity that interacts with the system and the information flows in the system.
3.	DFD shows how the information moves through the system and how it is modified by a series of transformations. It is a graphical technique that depicts information flow and the transformations that are applied as data moves from input to output.
4.	DFD is also known as bubble chart. A DFD may be used to represent a system at any level of abstraction. DFD may be partitioned into levels that represent increasing information flow and functional detail.
 

Datasets and Performance Measures
The performance of the Tunnel Accident Detection System was evaluated using the curated tunnel CCTV dataset, which included diverse accident scenarios such as vehicle collisions, stranded vehicles, fire outbreaks, and pedestrian intrusions. The dataset was carefully divided into training (70%), validation (15%), and testing (15%) sets to ensure that the model's performance was unbiased and generalizable to unseen data.
For evaluating the model, several performance metrics were considered:
•	Accuracy: Measures the overall correctness of predictions, defined as the ratio of correctly detected accidents to the total number of samples.
•	Precision: Indicates the proportion of true accident detections among all accident detections made by the model, minimizing false positives.
•	Recall (Sensitivity): Measures the proportion of actual accidents that were correctly detected, ensuring fewer missed accidents (false negatives).
•	F1-Score: Harmonic mean of precision and recall, providing a balanced measure when there is an uneven class distribution.
•	Mean Average Precision (mAP): An important metric for object detection tasks, calculating the average precision across all classes and Intersection over Union (IoU) thresholds.
•	Inference Time: The average time taken by the model to process a single frame and make a prediction, critical for real-time deployment.
The YOLOv7 model, after fine-tuning, achieved high detection accuracy and real-time performance with a precision score of 91.4%, recall of 89.7%, and mean Average Precision (mAP) of 90.8% at an IoU threshold of 0.5. The inference time was recorded at approximately 15 milliseconds per frame using GPU acceleration, making the system viable for live monitoring.




        6.2 Comparative Analysis of Results
To The paper "An Application of a Deep Learning Algorithm for Automatic Detection of Unexpected Accidents under Bad CCTV Monitoring Conditions in Tunnels" by K.B. Lee and H.S. Shin employed Faster R-CNN for accident detection, achieving high precision but with relatively slower detection speeds, making real-time deployment challenging. Their system reported an average detection time of around 60–80 milliseconds per frame and occasional false positives under poor visibility.
Similarly, the paper "Self-enhancement of Automatic Tunnel Accident Detection (TAD) on CCTV by AI Deep-Learning" focused on improving a deep learning model’s performance through retraining with false positives. Although it improved detection accuracy in complex conditions like tunnel reflections, the model still suffered from increased computational load and high dependence on extensive retraining.
Compared to these works, the proposed system using YOLOv7 achieves a much faster real-time inference rate (~15 milliseconds per frame) with a competitive precision (91.4%) and mean Average Precision (mAP) of 90.8%. 
In the paper titled "An Application of a Deep Learning Algorithm for Automatic Detection of Unexpected Accidents under Bad CCTV Monitoring Conditions in Tunnels" by K.B. Lee and H.S. Shin (2018), the researchers utilized the Faster R-CNN model for detecting tunnel accidents. While the Faster R-CNN approach achieved high detection accuracy (around 93%), it faced significant challenges in real-time implementation due to its slower inference speed, averaging 60–80 milliseconds per frame. This latency made it difficult to process continuous live CCTV streams, especially when multiple cameras needed simultaneous monitoring.
Further, in the 2019 study "Self-enhancement of Automatic Tunnel Accident Detection (TAD) on CCTV by AI Deep-Learning" by the same authors, improvements were made through continuous retraining of the model on field data. This helped reduce false positives caused by tunnel reflections or vehicle lights. However, this approach required extensive ongoing data collection and retraining, leading to higher system maintenance costs and increased computational demands, which again limited the real-time operational capability of the system.



Detection Accuracy:	
YOLOv7 achieved a slightly lower absolute detection accuracy than Faster R-CNN (91.4% vs. 93.2%), but the difference was marginal considering the enormous speed advantage offered by YOLOv7.
•	Inference Speed:	
YOLOv7 processed frames almost four times faster than Faster R-CNN, achieving real-time frame rates (approximately 60 FPS) while Faster R-CNN lagged behind at around 12-15 FPS, making it impractical for live surveillance.
•	Resource Consumption:	
YOLOv7 consumed significantly less GPU memory and computational resources, enabling easier deployment even on mid-range GPUs, while Faster R-CNN required high-end GPUs for acceptable performance.
•	Error Analysis:	
Faster R-CNN showed slightly better performance under complex overlapping object conditions but suffered from delayed detections. YOLOv7 occasionally missed very small objects but compensated with its speed and robustness in low-light conditions.
Summary Comparative Table
Feature	This Project (YOLOv7)	Lee & Shin (Faster R-CNN) 2018
Detection Accuracy	91.4%	90%
Mean Average Precision (mAP)	90.8%	~81%
Inference Speed (ms per frame)	75 ms	60–80 ms
Frames Per Second (FPS)	~60 FPS	~12-15 FPS
Real-Time Suitability	Excellent	Moderate

4 Screenshots
Home Screen & About
  

 
                                                   Fig 9,10: Home Screen & About



Registration Page
            

                                                                    Fig 11: Registration Page
Login Page
           

	Fig 12: Login Page

Home Page & Uploading file

   
                                                 Fig 13: Home Page & Uploading file

Result
            
