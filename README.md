This project aims to screen the input resumes against a job description (We have used data scientist job description for this project) using BERT and rank the resumes using intuitionistic fuzzy decision support systems (MAUT and Fuzzy TOPSIS). After classifying the resumes using BERT, to rank the resumes, a panel of 3 judges are taken and given 3 different weights ranging from 0-1 according to their experience and qualifications. These 3 judges score the candidate on a 5-level scale (VL, L, M, H, VH) based on 7 criteria (Educational background, programming skills, basic mathematics and statistics, data manipulation skills, communication skills, Internship experience and learning ability) with each criterion having different weights ranging from 0-1 according to their importance. These scores are converted into 3 linguistic matrices and these linguistic matrices are then converted into a fuzzy matrix using triangular intuitionistic fuzzy number. These 3 fuzzy matrices are then combined into a single matrix using CIFCS algorithm. This final matrix is then used to calculate utility score using MAUT algorithm and closeness coefficient using Fuzzy TOPSIS algorithm. These two scores are combined into a single score by average and then the resumes are ranked accordingly (resume having the highest score is ranked high).