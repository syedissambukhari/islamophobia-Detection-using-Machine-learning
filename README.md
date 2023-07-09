# islamophobia detection
#Ist install all the require libraries:
----------------------------------------------
import os
import cv2
import pytesseract
import numpy as np
from sklearn.feature_extraction.text import TfidfVectorizer
from sklearn.svm import SVC
from sklearn.metrics import accuracy_score, precision_score, recall_score, f1_score
import joblib
from tensorflow.keras.models import Sequential
from tensorflow.keras.layers import Conv2D, MaxPooling2D, Flatten, Dense
import tensorflow.keras as keras
-----------------------------------------
SVM model to detect islamophobic text in the picture. and CNN model to detect islamophobic nature in image
----------------------------------------------------
#the data_folder consist of 4 sub folders which is:

islamophobic_text_folder = 'C:/Users/Syed Issam Bukhari/Documents/projects all/projects/islamop/Memes/islamophobic text'

not_islamophobic_text_folder = 'C:/Users/Syed Issam Bukhari/Documents/projects all/projects/islamop/Memes/Non islamophobic text'

islamophobic_nature_folder = 'C:/Users/Syed Issam Bukhari/Documents/projects all/projects/islamop/Memes/Islamophobic image'

not_islamophobic_nature_folder = 'C:/Users/Syed Issam Bukhari/Documents/projects all/projects/islamop/Memes/Non Islamophobic image'

----------------------------------------------------------------
