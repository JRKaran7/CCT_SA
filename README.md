# Subject Name: Critical and Creative Thinking
## Beyond the Blueprint: Crafting Innovative Prototypes with  Critical and Creative Thinking
## Task 1: Designing Digital Nomad Community App Prototype
## Name of the Project: Faint Detection System

Student ID: 1000130 <br>
Karan Amol Rajankar </br>
Delhi Public School Bangalore North </br>
Email ID: karan.rajankar07@gmail.com </br>

### Introduction
“Own only what you can always carry with you: known languages, known countries, known people. Let your memory be your travel bag." — Alexandr Solzhenitsyn </br> <br>
This fascinating quote by Alexandr Solzhenitsyn represents the mindset of a digital nomad. Digital nomads are people who travel freely while working remotely using technology and the internet. While travelling, digital nomads tend to understand the culture and the environment, giving them opportunities to understand the world’s diversity and handle software projects at the same time. <br> <br>
As a developer of RemoteVibe.inc, I researched the different constraints that digital nomads face. In fact, I had an interview session with one such person who has lived in 4 countries in her 1.5 years of being a digital nomad. During the interview, he mentioned that learning about the famous places in real time is an experience, but doing so and working becomes a problem because not only places offer smooth internet and efficient technologies. Many places do not have the right requirements that digital nomads need for their work. So, it is a necessity, as an organisation, to come up with a product that can overcome these constraints and fulfil their needs. <br> <br>
This project will provide a solution in the form of a prototype that fulfils every digital nomad's requirements and makes their work-travel time highly efficient.

### Problem Definition
In the rapidly growing community of digital nomads, several challenges hinder productivity, learning, and overall well-being, leading to reduced effectiveness and poor quality of work. These challenges include: </br> <br>
1. Language Learning Inefficiency: According to a study by the Education Data Initiative, 70% of digital nomads find it difficult to learn a new language despite the necessity to communicate effectively while traveling. Only 40% of these individuals engage in language learning consistently, with a significant portion citing lack of structured time, motivation, and suitable resources. </br> <br>
2. Inefficient Co-working Sessions: Research by WeWork suggests that 65% of digital nomads report inefficient co-working experiences. These include poor collaboration, distractions, and lack of proper resources. The inefficiencies in co-working spaces lead to a decrease in overall productivity, as 55% of nomads express frustration over inconsistent or low-quality work environments. </br> <br>


About 30–40% of adults experience a fall-related injury in their homes. Not only this, about 35–40% of fainting episodes lead to injuries that require immediate medical attention. (Syncope (fainting) 2020) </br>
Looking at the statistics, I feel that this issue must be taken into deep consideration and addressed. Also, while addressing the issue, conditions like accuracy and quicker messaging must be taken into consideration along with the main goal of saving the individual.

### Goal and Objective
• To develop a system that can detect a person standing, sitting, and fainting. Along with this, the system should alert the closest family member if the model detects the target user facing a fainting episode. <br>
• To develop a heart rate detector using photoplethysmography that will share the last recorded heart rate of the person after fainting.

### Existing projects
1. Wait Kit Wong: https://www.researchgate.net/publication/228792571_Home_Alone_Faint_Detection_Surveillance_System_Using_Thermal_Camera <br>
2. IEEE Explore: http://ieeexplore.ieee.org/document/5489510/
### Approach
Here is how the Software Development Life Cycle (SDLC) helped me create the faint detection system: - </br>
#### 1. Planning: 
After discussing with my teachers and family members, I found out that there is a higher rate of injuries due to falling in homes and fainting episodes. This is an issue that needs to be efficiently resolved. So, I thought of using computer vision to make a faint detection system that can detect a person fainting. Along with this, if fainting is detected, it will message the closest family member on WhatsApp. Another reason for coming up with this idea is because my grandparents had recently met with two fainting episodes that my family feels that it should be detected immediately so that help can be provided on time. <br>
Keeping this in mind, I generated a base problem statement with statistics, that helped me work on my project. I had first thought of detecting only fainting, but then I decided to even detect sitting and standing so that the accuracy of detecting fainting increases. After researching about pose detection, I went through the concept of combining advanced computer vision techniques with photoplethysmography (ppg). This made me think about combining heart rate detection with faint detection so that the affected individual's vitals can also be recorded. <br>

#### 2. Defining:-
• Required Python Computer Vision, Mediapipe, and WhatsApp message coding experience. I learnt about it through many YouTube videos and websites like GeeksForGeeks, Java Tutorials, etc. <br>
• Used websites like vector images and Shutterstock to download different sitting, standing, and fainting videos. Added 10 videos for each pose to increase accuracy. <br>
• Asked ChatGPT to provide the different landmarks of the body to detect three different poses. <br>
• Finally, understood the use of pywhatkit and advanced computer vision techniques for the code to send the WhatsApp message to the provided number and record the heartbeat respectively. This will be the final output of the code. <br>
 
#### 3. Designing: 
• Began designing the faint detection. It is a working detection system that checks three different poses. If fainting is detected, then it sends a WhatsApp message to the given number saying that fainting has been detected along with the last recorded heartbeat. <br>
• Designed a storyboard to express how this detection system can be beneficial and a requirement for all houses. <br>
• Finally, designed a flowchart to show the system process from the start to the end. <br> <br>
![image](https://github.com/user-attachments/assets/41718f8f-9709-4117-add2-2a955c31c8d2) <br>
(Figure 2: Storyboard for the model, https://www.canva.com/) <br> <br>
![image](https://github.com/user-attachments/assets/2e43c485-0073-4831-9825-5c2d592049b2) <br>
(Figure 3: Flowchart for Data Structure, https://www.canva.com/)

#### 3. Building: 
• Started building my faint detection system on Visual Studio Code. <br>
• Used modules like mediapipe, pywhatkit, cv2, and sklearn to extract features from different training videos. <br>
• Trained three different models (Random Forest Classifier, Decision Tree Classifier, and KNN Classifier) on the dataset and saved the model that had the highest accuracy using the joblib library. <br>
• Used CV2 in order to capture real-time frames and make this system functional in real time. <br>
• Python Libraries Used: - <br>
1. CV2: - To access webcamera for extracting real time information (Get started 2024)<br>
2. mediapipe as mp: - To access body landmarks (Mediapipe)<br>
3. numpy as np: - To flatten landmark vectors for the machine learning model to process data (Numpy Introduction &amp; Guide for beginners 2024)<br>
4. os: - To extract videos from the folder (W3schools.com)<br>
5. sklearn.model_selection.train_test_split: - Split the dataset into training and test set (Learn: Machine learning in python - scikit-learn 0.16.1 documentation)<br>
6. sklearn.ensemble.RandomForestClassifier: - Machine Learning Model (Learn: Machine learning in python - scikit-learn 0.16.1 documentation)<br>
7. sklearn.neighbors.KNeighborsClassifier: - Machine Learning Model (Learn: Machine learning in python - scikit-learn 0.16.1 documentation)<br>
8. sklearn.tree. DecisionTreeClassifier: - Machine Learning Model (Learn: Machine learning in python - scikit-learn 0.16.1 documentation)<br>
9. sklearn.metrics.accuracy_score: - To check accuracy of the model and evaluate it (Learn: Machine learning in python - scikit-learn 0.16.1 documentation)<br>
10. joblib: - To store the model so that it can be accessed again without the need of processing it (Sharma, 2023)<br>

 
#### 4. Testing:
I tested my system by introducing it to my peers, teachers, and family members. They found the idea and the system quite interesting, and they all agreed that the system has a greater scope in the future. Finally, I introduced a feedback survey to make sure that the system was fulfilling the objective. <br>
Forms Link: https://docs.google.com/forms/d/e/1FAIpQLSf63XT3TAY2lBdupnTlUIrUfD75gXnOa8nRc6XESU9MCMKTgQ/viewform?usp=sf_link <br>
Forms Response Sheet: https://docs.google.com/spreadsheets/d/171L4dBcxADU1JaSF3q4bnnEjV5oubl93SErVe220ILo/edit?usp=sharing
 
#### 5. Model Deployment:
• The entire code is uploaded to Github for the users to understand the code and gain insights from it. <br>
• Along with this, a detailed ReadMe file includes screenshots of the output window and the frame window. <br>
• Finally, a presentation that gives a brief idea about my project.

### Detailed Understanding about the Code
#### Data Selection
To train the model with the proper frames extracted from videos, I have taken videos of different poses from websites like Shutterstock and vector images. Around 10 videos were taken for each pose recorded in different angles so that the model can successfully detect any pose without any hesitance. To differentiate between the poses, I have made separate folders for each pose and provided that for the respective pose variable. 

#### Data preprocessing and Exploratory Data Analysis (EDA)
This process is applicable for both model training and real-time detection.
• For the model training, we defined a function that can process every single video. Once the function is called, it takes in the video from the video path. An empty list feature[] will be used to store the landmark values. We then check whether the model can process the video. If yes, then the process begins. First, a loop is created that processes every frame of the video. The frame is then converted to RGB and is processed by the pose class from mediapipe to detect any body landmarks. If the pose detects landmarks, then it begins extracting 15 different body landmarks. Once this is done, the model then flattens the vectors for the machine learning model to process. Now this will then be appended in the features list, and frame count increases by 1. This whole process is looped over all videos in the dataset. Finally, the dataset is split into a training and test set with a ratio of 80:20. <br>
• For the real-time detection, a conditional statement about whether the frame is running or not is compiled. Then a loop runs over each frame. Similar landmarks are drawn after converting the frame to RGB. Then, the vectors are flattened, and predictions are made. <br> <br>
![Screenshot 2024-11-11 114715](https://github.com/user-attachments/assets/bf1259a6-e197-4bd5-98ca-0b983b3b532f) <br>
(Figure 4: Code for Video Processing)<br> <br>
![Screenshot 2024-11-11 114804](https://github.com/user-attachments/assets/557b67fa-ce57-420c-82d4-7e26bd8dde67) <br>
(Figure 5: Code for Dataset Splitting and Processing)

#### Model Selection and Training
Once the data is preprocessed, we take in three different classification models to examine which one is better. For extracting features, mediapipe was used. But for the predictions, we will choose from DecisionTreeClassifier, RandomForestClassifier, and K Nearest Neighbors. We train it with the training data collected from the dataset. <br> <br>
![image](https://github.com/user-attachments/assets/f626ff50-41c4-404f-a522-89735c39ac52) <br>
(Figure 6: Training the three models)

#### Model Evaluation and Testing
Once the data is trained, it is tested on the test dataset, and the accuracy is checked. The model with the best accuracy will be chosen and will be dumped as a permanent pretrained model that can be used without the need of processing it again. <br> <br>
![image](https://github.com/user-attachments/assets/3c1ddd05-734e-4b64-84a1-c2786e37ded7) <br>
(Figure 7: Evaluating and deciding the best model)

#### Model Deployment
Finally, the main code is the file where we load the pretrained model and begin detecting real-time poses. If there is a faint detected, the model uses PyWhatKit to immediately open WhatsApp and send a message that also includes the last recorded heart rate to the provided number in the code. <br>

### Heart Rate Detection
This system uses mediapipe and advanced computer vision techniques to detect the heart rate of a person based on changes in facial colour channels linked to the blood flow. Now this system is not 100% accurate but is a trial implementation. In the main loop, the face detection variable detects the colour intensity of the face in each frame. This draws an invisible line around the face that it uses for the calculation. Then a low-pass filter is coded that prevents any noise or abrupt changes in colour intensity, thereby smoothening the detection process. To minimise fluctuations and save memory storage, only the last 30 recorded frames will be appended to a list whose mean value is calculated to provide the normalised heart rate after every 2 seconds. 

### Screenshots of the Real Time Detection Code
![image](https://github.com/user-attachments/assets/4381b324-14bf-4e3a-aae1-5f22927b35a6)
![image](https://github.com/user-attachments/assets/b0e7e0ef-ad90-41f9-a099-cfc313fb5cff)
<br>
(Figure 8: Importing Pose model, Machine Learning model, and Declaring variables) <br> <br>
![image](https://github.com/user-attachments/assets/9e698fca-1af7-4286-b2f2-7e985158ce94) <br>
(Figure 9: Function For Calculating Heart Rate) <br> <br>
![image](https://github.com/user-attachments/assets/50907d60-b4fa-47f2-a7c0-b4ab45f3dd75) <br>
(Figure 10: Flattening Vectors for Model Prediction and Probability Calculation) <br> <br>
![image](https://github.com/user-attachments/assets/d7287a60-fd22-43ba-8e02-800904dce0ef) <br>
(Figure 11: Loop for drawing landmarks)

### Screenshots of the Output
(Note that the probabilities of the poses are not dependent on each other) <br>
1. Standing Threshold Probability: 5 % <br>
2. Sitting Threshold Probability: 90 % <br>
3. Faint Threshold Probability: 85 % <br>
(The model must detect a value greater than these threshold values to detect the respective pose) <br> <br>
![image](https://github.com/user-attachments/assets/ae072d8e-7483-4b27-9a01-7d1c06bfc6b5) <br>
(Figure 12: Model Accuracies) <br> <br>
![Screenshot 2024-11-13 135755](https://github.com/user-attachments/assets/26136d5d-b9cf-43aa-8b35-4586ba74c55a) <br>
(Figure 13: Sitting Pose Detection) <br> <br>
![Screenshot 2024-11-13 135854](https://github.com/user-attachments/assets/fc86964d-1434-4c5d-a54d-ecf0d24eb80f) <br>
(Figure 14: Standing Pose Detection) <br> <br>
![Screenshot 2024-11-13 140445](https://github.com/user-attachments/assets/024e0f05-b724-4481-a14e-f20d2caaf8f3) <br>
(Figure 15: - Fainting Pose Detection) <br> <br>
![image](https://github.com/user-attachments/assets/7e0ce8e2-7106-4732-99b3-35141ba5bc74) <br>
(Figure 16: WhatsApp Message Sent) <br> <br>
![image](https://github.com/user-attachments/assets/f2daeb6b-69dc-4991-9e11-3868bef07665) <br>
(Figure 16: Output Screen)

### Monitoring and Maintenance
Now that we have deployed the model, it is to be monitored to prevent false alarms and continuously update the training data to increase accuracy. Once we get a deeper understanding about advanced computer vision, I would continue to integrate this model with hardware devices to make it a fully functional product. Monitoring this model will prevent any issues arising in the code.
### Limitations
• Can only send a WhatsApp message as Twilio requires a subscription for calling services <br>
• Not much detailed feature extraction and limited to only one person at a time <br>
• Cannot completely differentiate between sleeping and fainting.
### Benefits
• Provides additional safety for individuals prone to fainting, such as those with certain medical conditions, elderly individuals, or people recovering from surgeries. <br>
• Offers around-the-clock monitoring without requiring the constant presence of a caregiver, making it ideal for home or assisted-living environments.
• Provides last recorded heart beat so that doctors can find out the cause of the faint easily.
### Future Scope
This system can be made much better by introducing it in the public surveillance cameras as well as improving and adding new features to the vital systems so that the camera provides the accurate recorded vitals when the person has fainted. Along with this, immediate ambulance services and increased accuracy can make the project better. 

### Conclusion
While coding this faint detection system, I learnt about how Python can be used to code computer vision applications to create systems for fulfilling basic necessities in society. I also learnt about how to provide a proper dataset as all the videos were put in a list. So, the best videos were found by surfing through the internet. <br>
Coding with different libraries like Mediapipe and Scikit Learn helped me understand advanced computer vision techniques and how to implement them with machine learning. Along with this, researching about the colour channels and different methods led to the creation of a heart rate detection system that I felt was not possible to do without any sensors. The use of photoplethysmography helped me integrate the use of vitals in my faint detection system. Finally, the discussion with peers, family members, and my teachers not only developed my communication skills, but they also gave me ideas and suggestions on how I can make my faint detection system better.

### PPT Link
https://www.canva.com/design/DAGWJt5h7O0/W7nnbCF_XAAMC00j8nf63A/view?utm_content=DAGWJt5h7O0&utm_campaign=designshare&utm_medium=link&utm_source=editor
