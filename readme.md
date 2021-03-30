## EECS 738 - Hidden Markov Model
The aim of this repository/project is to generate a new text from text corpus and perform prediction based on provided sequence of words

## Dataset
<a src="https://www.kaggle.com/kingburrito666/shakespeare-plays?select=Shakespeare_data.csv">Shakespeare-plays</a>

**Text-corpus:** <a src="./data/alllines.txt" >allines.txt</a>

## Process

1.  Dataset is loaded into pandas and cleaned which gives us all  list of all player-lines
2. Markov model is build and trained(Building State pairs)
     * First of all, each line is tokenized from player-lines of dataset
     * Markov chains are built based on generated tokens
3. Determining probability distribution

The second stage consists of forming the previous and current state pairs. Since we are building a 2nd-order Markov model, our previous state will consist of two words.

In stage 3 we need to  perform simple counts and calculate the probability of the next states possible for a given current state as previosuly.

* Text-corpus genneration capture
  <img src="./text_generation.png" >

* Text-prediction capture
  <img src="./text_prediction.PNG" >

## References
1. https://towardsdatascience.com/markov-and-hidden-markov-model-3eec42298d75
2. https://en.wikipedia.org/wiki/Hidden_Markov_model
3. https://medium.com/@kangeugine/hidden-markov-model-7681c22f5b9

 





