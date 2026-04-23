# face

Ansigtsgenkendelse med CNN

1. Projekt den indledende tilgang "9face_bedre.ipynb"
Dette projekt implementerer et Convolutional Neural Network (CNN) til genkendelse af ansigtsudtryk ved hjælp af deep learning. Modellen er udviklet og trænet i Google Colab med TensorFlow og Keras.
Formålet med projektet er at klassificere ansigtsbilleder i ni forskellige følelseskategorier:
Angry, Contempt, disgust, fear, happy, natural, sad, sleepy, surprised 
Datasættet udtrækkes fra en komprimeret fil og omstruktureres fra YOLO-format til et format, der er kompatibelt med TensorFlow.
Billedstørrelse: 64×64 pixels 
Batch-størrelse: 32 
Træningsdata: 64.864 billeder 
Valideringsdata: 1.720 billeder 
Modellen er et simpelt CNN bestående af:
Rescaling-lag (normalisering), To konvolutionslag (Conv2D) med ReLU-aktivering, MaxPooling-lag, Output-lag med 9 neuroner (softmax) 
Modellen trænes i 10 epochs og evalueres løbende på et valideringssæt.
Træningsnøjagtighed: ca. 95,2 % 
Valideringsnøjagtighed: ca. 66,6 % 
Modellen opnår høj nøjagtighed på træningsdata, men væsentligt lavere præcision på valideringsdata. Dette indikerer overfitting, hvor modellen ikke generaliserer godt til nye data.
Mulige forbedringer som bliver anvendt i
•	Anvend data augmentation (rotation, zoom, spejling, lysændringer) 
•	Tilføj Dropout-lag for at reducere overfitting 
•	Brug Early Stopping under træning 
•	Undersøg klassefordeling og anvend class weights 
•	Evaluer modellen med en confusion matrix 
Teknologier
•	Python, TensorFlow, Keras, Google Colab 

