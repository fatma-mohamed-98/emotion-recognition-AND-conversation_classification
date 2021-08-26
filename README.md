
# Dataset:
In this task I used two different datasets 
1. DailyDialog dataset for emotion recognition to classify the input sentence. (multiclass classification) \
https://paperswithcode.com/dataset/dailydialog 
2. EMPATHETICDIALOGUES dataset for conversation classification. (binary classification) \
https://paperswithcode.com/dataset/empatheticdialogues

At first we need to find sentence boundary then we will tokenize it to get separate words then we apply embedding to convert the
input sentence to normalized numeric vector.So I used the Universal sentence encoder for sentence, phrase embedding.

# Deep learning model architecture:
there are two variations of Universal Sentence Encoder (USE). and I choose Transformer Encoder based architecture for this task. \
it has better accuracy on downstream tasks but higher memory and compute resource usage due to complex architecture. \
Also, the compute time scales dramatically with the length of sentence as self-attention has O(n2) time complexity with the length of the sentence. \
But for short sentences, it is only moderately slower. And our application we have short sentence and we need high accuracy so we
choose this architecture (universal-sentence-encoder-large-5).


# Results:
### Confusion_Matrix for emotion recognition task using USE on DailyDialoge dataset
![Confusion_Matrix for emotion recognition task using USE on DailyDialoge dataset](https://github.com/fatma-mohamed-98/emotion-recognition-AND-conversation_classification/blob/main/confusion%20matrix.png )

### F1_Score for emotion recognition task using USE on DailyDialoge dataset
![F1_Score for emotion recognition task using USE on DailyDialoge dataset](https://github.com/fatma-mohamed-98/emotion-recognition-AND-conversation_classification/blob/main/F1_Score.png)


### Accuracy for emotion recognition task using USE on DailyDialoge dataset
![Accuracy for emotion recognition task using USE on DailyDialoge dataset](https://github.com/fatma-mohamed-98/emotion-recognition-AND-conversation_classification/blob/main/Accuracy.png)




