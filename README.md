# EMOTION-ANALYSER

The problem in emotion analysis is to predict in what emotion is the person texting. We do not
know whether the person texting is in anger, fear, sadness, disgust, joy or surprise. Hence our
main objective in this project is to implement an algorithm for automatically classifying whether
the message typed or spoken indicates anger, fear, sadness, disgust, joy or surprise. Emotion
analysis is done to determine the emotion of individual while sending the message. We have not
limited our project to sentimental analysis of just a given text but have also incorporated
sentimental analysis of audio as well.
The idea behind the project is to study the basic human emotions that can be depicted by a text
written by a person or something spoken by a person. It takes in a text or a voice message, and
identifies the emotion related to the text or audio. The program takes multimodal input, i.e. it can
take input in either text or using your voice. The program includes a speech-to-text Google API
that helps it to recognize the words that are said. The program gives output as one of the six basic
emotions, which are anger, fear, sadness, disgust, joy and surprise.


 METHODOLOGY:
• Dataset Optimization: The dataset file location would be put in the code, then two
different variables are read for putting the words of the first and the second column in
two different variables. The words in the first columns would be the various kind of
words found in a dictionary and the second columns would show the emotion related to
their corresponding words. Each words in the first columns would be reduced to their
base or root form. The words in the first column would be put as the key of a dictionary
with the values of the second column as their values.

• Input Conversion: In our program we would be taking input from the voice of a person.
This would then be converted into a text using a Google speech-to-text API. In case the
program is unable to understand what the user has spoken, it would show an error
message.

• Stopwords Removal: The String of words generated as an input would be sent to a
function rem_stopw(). The function would then take the string as an input, change it all to
lowercase, and would then remove all the stopwords.

• Stemming Input: In this part of the code, the program would first take the list of word,
that it got from the rem_stopw() function, and stems each and every word present in it so
that it could be matched from the dataset. 

• Find Max Emotion: It finds all the words in this list in the key of the dictionary formed
by the dataset. If the word matches the key of any of the dictionary, it adds the
corresponding value to another list. Like this all the words would be searched in the
dictionary and their values would be added in the list. The list of values of the dictionary
would be then taken into another dictionary, where keys would be all the unique values of
the list and the values would be the number of occurrences of each of these values. The
key with the maximum value would be printed as output, which turns out to be the
emotion of the inputted sentence. 
