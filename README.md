# BDP
 ChatBots based on bert, every step is fully explained inside the ipynb 
 As I don't have enough resources to tune this great model, I'm going to make a stand by on this project for a while. on this project for a while
 ## BDP_Chatbot
 English lenguage bot, trained to be able to speak and answer questions without context. Based on T5

 ## BDP_MultilingualQA
 English an Spanish bot, trained to answer questions in spanish and english, required context. Based on BERT

 ## Datasets
 For this chatbot has been used the following datasets:
 - https://github.com/ccasimiro88/TranslateAlignRetrieve
 - http://nlp.cs.washington.edu/triviaqa/data/triviaqa-unfiltered.tar.gz
 - For multilingual model the datasets have been combined into one, using the most important commons characteristics:
   - Question
   - Context
   - Answers (array of possible answers)

## Tokenize
For this enhacement i have used the bert tokenizer, and apply it to the 3 columns, if you want to build a model that select an answer
you could not tokenize answers column.

Once it is tokenized, all the dataset are tensors of pytorch, letting me to use it, even with CUDA to process all the information faster
