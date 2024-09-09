# Face Recognition with FaceNet

## Overview

This project aims to evaluate the FaceNet model for face recognition tasks by leveraging a pre-trained version of the model provided by Hiroki Taniai. FaceNet, proposed by Florian Schroff in their 2015 paper "FaceNet: A Unified Embedding for Face Recognition and Clustering," is a deep convolutional neural network that maps face images to a compact Euclidean space, where the distances directly correspond to a measure of facial similarity. Inspired by the tutorial from Machine Learning Mastery, this project utilizes the MTCNN (Multi-task Cascaded Convolutional Networks) library for face detection to extract faces from images.

## About the dataset
The dataset used in this project is the 5 Celebrity Faces Dataset, a curated collection of images featuring five well-known celebrities: Ben Affleck, Elton John, Jerry Seinfeld, Madonna, and Mindy Kaling. This dataset is specifically designed for face recognition tasks and consists of a variety of face images that include variations in pose, expression, lighting, etc.

## Steps
The process begins by using MTCNN to detect faces in a dataset containing images of celebrities, such as Ben Affleck, Elton John, and Madonna. Each detected face is extracted and resized to the required input shape for the FaceNet model (160x160 pixels). The pre-trained FaceNet model is then used to generate a 128-dimensional embedding vector for each face, which serves as a unique identifier for face recognition. These embeddings are further processed and normalized for use in a Support Vector Machine (SVM) classifier.
The classifier is trained and tested on the extracted face embeddings from the dataset, achieving high accuracy in recognizing faces both in the training and testing sets. The results demonstrate the effectiveness of FaceNet embeddings combined with a simple SVM classifier for face recognition tasks. This project provides a practical approach to face detection and recognition using deep learning techniques and pre-trained models, highlighting the potential for real-world applications in security, authentication, and personal identification systems.

