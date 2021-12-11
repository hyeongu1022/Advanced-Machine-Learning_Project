# Personality Prediction System Based on Graphology using Machine Learning

Team Members:

Lucy Hwang, Archit Patel, Yashaswini Kalva, Hyeon Gu Kim, Kaushik Kumaran

## Abstract

Graphology is a method of identifying, evaluating and understanding human personality traits through the strokes and patterns revealed by handwriting. Handwriting reveals the true personality including emotional outlay, fears, honesty, defences and many others. Professional handwriting examiners called graphologists often identify the writer with a piece of handwriting. Accuracy of handwriting analysis depends on how skilled the Analyst is. Although human intervention in handwriting analysis has been effective, it is costly and prone to error. Hence the proposed methodology focuses on developing a system that can predict personality traits with the aid of machine learning without human intervention. To make this happen, we plan to consider handwriting features such as size of letters, slant of the writing, baseline, pen pressure, spacing between letters, spacing between words, top margin in a document to predict eight personality traits of a writer.  For the project, handwriting samples of 657 writers are acquired.

## Application and Motivation

Handwriting analysis is one among several methods to understand the psychology of a person. Some applications of graphology are listed here.
* Psychological analysis: Graphology is used clinically by counsellors and psychotherapists. But it is generally used alongside other projective personality assessment tools, and not in isolation.
* Employment profiling: Companies use handwriting analysis for recruitment. A graphological report is meant to be used in conjunction with other tools, such as comprehensive background checks, practical demonstration or record of work skills.
An employer needs to understand the employees they hire; a counsellor needs to understand his/her client; an individual needs to understand his/her friends for a good and long-lasting relationship. A graphologist studies handwriting based on its graphic structures, some aspects of which can be automated to speed up the analysis and produce accurate results with the help of machine learning. Hand-writing analysis with a computer is fast, accurate and identifies the patterns better than visual inspection. Moreover, machine learning assisted analysis is efficient and devoid of human errors.

## Problem Statement

A system is proposed to automate the basic handwriting analysis tasks of graphology to determine a few important personality traits. Seven features/characteristics of a handwriting are considered to be extracted from a sample handwriting image. Each of the seven resulting raw values will be put into corresponding categories of respective feature variations. A combination of these discrete values will be used to train each support vector machine for a personality trait. The classifier will then be able to predict the personality traits of the writer. An overview is represented in figure 1.1.

## Data sourcing

Data from the IAM Handwriting Database of Research Group on Computer Vision and Artificial Intelligence INF, University of Bern, Switzerland is obtained. The data is readily available for download to be used for non-pro t research purposes. The database contains 1538 pages of scanned text for which 657 writers contributed samples of their handwriting. Each handwriting sample is labelled with the corresponding psychological traits by manually studying each document. (https://fki.tic.heia-fr.ch/databases/iam-handwriting-database). These images will be cropped and saved as PNG images with an automatic action script.

## Approaches

The proposed project phases have been mentioned in the Figure 1.1 
We will first pre-process the images. The handwriting images we obtained contain unwanted noise, printed texts and lines. The original images also have a very big resolution by default. The aim of pre-processing is to make the image data suitable for feature extraction by filtering unwanted attributes, enhancing the quality, and performing transformations. The methods which we plan to perform in pre-processing are given below:
* Image Resolution and Cropping: The original images contain unwanted printed texts, lines and free space which are not suitable for further processing. We will be writing a script to crop out the left and right margins, resize all the images with 850 pixels width and perspective height, and save the images in PNG format. 
* Noise Removal: Image noise is defined as random variation of brightness or colour information in images. Noise can be removed by filtering the images.

We will then move onto feature extraction to determine each sample’s features and their measurement. The set of features we will be evaluating handwriting on are shown in Figure 1.3. These features are: letter size, letter slant, pen pressure, baseline, and word spacing. Each of these has their own measurements and what those measurements say about a person’s personality. We plan to explore SVM classifiers to predict the personality type based on the feature values scored by the user in each feature.

## References

https://nanonets.com/blog/handwritten-character-recognition/ 
https://towardsdatascience.com/build-a-handwritten-text-recognition-system-using-tensorflow-2326a3487cd5 
https://medium.com/the-andela-way/applying-machine-learning-to-recognize-handwritten-characters-babcd4b8d705 
https://www.researchgate.net/publication/284205700_Handwriting_Analysis_for_Detection_of_Personality_Traits_using_Machine_Learning_Approach
https://data-flair.training/blogs/python-deep-learning-project-handwritten-digit-recognition/
https://www.pyimagesearch.com/2020/08/24/ocr-handwriting-recognition-with-opencv-keras-and-tensorflow/InternationalResearchJournalofEngineeringandTechnology(IRJET),e-ISSN:2395-0056

