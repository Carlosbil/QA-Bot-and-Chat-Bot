# BDP
 ChatBots based on bert, every step is fully explained inside the ipynb 

 ## BDPBot
 English lenguage bot, trained to answer questions in english
 
 ## BDP_ESPBot
 Spanish lenguage bot, trained to answer questions in spanish

 ## BDP_MultilingualBot
 English an Spanish bot, trained to answer questions in spanish and english

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
