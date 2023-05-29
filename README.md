# Student attendance record using facial recognition
 
The facial recognition roll call project uses facial recognition technology to identify 
and verify the identity of people, streamlining and improving the roll call process 
in various situations, that's what we are doing with this project. We aplly the necesary methods
to recognize the face of registraded students, and recognized them with a camera. 

We used the next method mentionated:

• The MTCNN (Multi-task Cascaded Convolutional Networks) model.

• The InceptionResnetV1 model.

• And finally used a multiple images of all four group members that have been included to 
create reference feature vectors for each person.

# Face recognition 

Additional techniques or algorithms that qe used are:

• MTCNN: It is a model based on convolutional neural networks that consists of three stages: 
face detection, detection refinement and extraction of facial reference points. It is used to
locate and extract the faces present in the images.

• InceptionResnetV1: It is a deep neural network architecture that combines the Inception 
model and the ResNet architecture. It is used to extract feature vectors from the detected 
faces. These vectors represent unique features of each face and are used to compare the 
similarity between faces.

Performance or efficiency improvements:
The addition of MTCNN makes it possible to detect and extract only the faces present in the 
images, which reduces processing time and avoids the need to analyze the entire image.
Using pre-trained models like InceptionResnetV1 avoids the need to train a model from scratch,
saving training time and resources.
By calculating the cosine similarity between feature vectors, the need for pixel-by-pixel 
comparisons is avoided, which improves system efficiency.
The addition of similarity thresholds allows for more efficient and accurate classification 
of the test image based on similarity to persons of interest.


## Motivación

For the implementation of the project, the aim was to improve the efficiency, precision and 
security in the process of calling the list and registering attendance, by taking advantage 
of facial recognition technology to identify and verify the identity of people quickly and reliably.

## Technologies/Frameworks used
  
- Colab.
- CPU.
- Camera.

## Most important features

In this project, the MTCNN model is used for face detection and extraction, while the 
InceptionResnetV1 model is used for feature extraction from the detected faces.
MTCNN – A convolutional neural network model used for face detection, refinement, and 
extraction of facial landmarks. Helps locate and extract faces from images.
InceptionResnetV1 – A deep neural network architecture that combines the Inception model
and the ResNet architecture. Extracts feature vectors of detect

## Instalation of diferent libraries we used

* Instalation torch:
* * 1. Open code terminal
* * 2. Run the following command
*      !pip install torch;

* Instalation facenet-pytorch:
* *  1. Open code terminal
* *  2. Run the following command
*      !pip install facenet-pytorch;

* Intalation of matplotlib:
* *   1. Open code terminal.
* *   2. Run the following command
*      !pip install matplotlib;

* Importation of scipy:
* *   1. Open code terminal.
* *   2. Run the following command
*      !pip install scipy;

## Credits

Name of the participants:
* David Andre Alarcon
* Nestor Barrientos
* Massiel Solano
* Carlos Michel

And our inspiration and knolegde based on this papers:
- https://uctunexpo.autanabooks.com/index.php/uct/article/view/126/182
- https://zhzhanp.github.io/papers/SPL2016.pdf
- https://scontent.flpb2-1.fna.fbcdn.net/v/t39.8562-6/240890413_887772915161178_4705912772854439762_n.pdf
- https://www.cv-foundation.org/openaccess/content_cvpr_2015/papers/Schroff_FaceNet_A_Unified_2015_CVPR_paper.pdf
- https://uctunexpo.autanabooks.com/index.php/uct/article/view/126/182
- https://upcommons.upc.edu/bitstream/handle/2117/331277/TFG_Análisis%20de%20un%20sistema%20de%20reconocimiento%20facial%20a%20partir%20de%20una%20base%20de%20datos%20realizado%20mediante%20Python.pdf?sequence=1&isAllowed=y
- http://repositorio.ug.edu.ec/bitstream/redug/32954/1/B-CINT-PTG-N.297%20Portilla%20Jimenez%20Jonathan%20Javier.pdf
- https://arxiv.org/pdf/2301.01922.pdf

## Licencia

The MIT License

Copyright (c) 2020 Red_no_disponible

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in
all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
THE SOFTWARE.
