# Hangman
<h2>Trexquant Hangman Project</h2>
This project implements an algorithm that can play the game of Hangman. The algorithm uses a variety of strategies to determine the best guess, including letter frequency, ngrams, and semantic similarity.

<h3>Getting Started</h3>
To get started, you will need to install the following dependencies:

pip install requests
Once you have installed the dependencies, you can run the following command to start a new game:

python hangman.py
The game will prompt you to enter your access token, which you can obtain from Trexquant. Once you have entered your access token, the game will start.

<h3>Playing the Game</h3>
To play the game, you will need to guess a letter at a time. The game will tell you whether your guess is correct or incorrect. If you guess a letter correctly, the letter will be revealed in the word. If you guess a letter incorrectly, you will lose one life.

The game ends when you either guess all the letters in the word or when you lose all your lives.

<h3>Strategies</h3>
The algorithm uses a variety of strategies to determine the best guess, including:

Letter frequency: The algorithm calculates the frequency of each letter in the English language and uses this information to determine which letters are most likely to be in the word.
Ngrams: The algorithm uses ngrams to identify patterns of letters that are likely to occur together. This information is used to determine which letters are most likely to be in the word.
Semantic similarity: The algorithm uses semantic similarity to identify words that are similar to the revealed word. This information is used to determine which letters are most likely to be in the word.

<h3>Results</h3>
The algorithm has been tested on a variety of words and has achieved a high accuracy rate. The algorithm has also been tested on words with multiple meanings and has been able to correctly guess the correct meaning of the word.

<h3>Future Work</h3>
There are a number of ways to improve the algorithm in the future. For example, the algorithm could be improved by using a more sophisticated model of language, such as a neural network. The algorithm could also be improved by using a more sophisticated strategy for selecting the next word to guess.

<h3>Conclusion</h3>
The Trexquant Hangman Project is a challenging but rewarding project. The project teaches you about the game of Hangman, the different strategies that can be used to play the game, and how to implement an algorithm that can play the game effectively.

<h2>CODE DESCRIPTION</h2>

<h3>def is_valid_word(self, word):</h3>
This function returns a Boolean value of the word being a valid word or not.

<h3>def should_use_optimal_guess(self, word):</h3>
This function determines when to use the ‘optimal_guess method’
Example logic:
        If the word length is short (e.g., 3 letters), use optimal_guess
        If there are only a few remaining attempts left (e.g., 2 or 3), use optimal_guess
        If the revealed word is almost complete (few underscores left), use optimal_guess
        You can adjust the conditions based on your observations and testing

<h3>def should_use_semantic_guess(self, ngram_guess, semantic_guess, word):</h3>
This function determines when to use the ‘semantic_guess method’
Example logic:
        If the word length is long (e.g., 7 letters), use semantic_guess with confidence
        If there are plenty of remaining attempts (e.g., more than 6), use semantic_guess
        If the revealed word has many unknown letters (more than half), use semantic_guess
        You can adjust the conditions based on your observations and testing

<h3>def letter_frequency_score(self, word):</h3>
This function calculates a score based on letter frequency in the English language higher frequency letters get a higher score.

<h3>def pick_best_semantic_guess(self, similar_words):</h3>
This function picks the best guess based on the semantics of the similar words. This iterates through a list of valid similar words and returns the best guess based on letter frequency score.

<h3>def semantic_similarity_guess(self, word):</h3>
This function picks the closest valid similar word based on the frequency score after iterating through a list of valid similar words.

<h3>def possible_ngrams_3(self, inp):</h3>
This function generates possible ngrams value and returns it for the optimized guesses. The main difference between this and the “possible_ngrams” function is the fallback strategy, for this we fallback on the “possible_ngrams” function.

<h3>def possible_ngrams(self, inp):</h3>
This function returns the best possible ngrams strategy for the current scenario and in case of fallback uses the “guess_fallback_letter()” function to help re-evaluate the scenario.

<h3>def remove_letters_from_string(self, letters_to_remove, input_string):</h3>
This function just removes the letters to remove from the required string and trims it as required.

<h3>def is_substring_with_wildcard(self,word, ngram):</h3>
This function returns the best match using the ngrams technique with the input word.

<h3>def optimal_guess(self, word):</h3>
This function combines multiple guess strategies and decides which one to use given the input of a specific word, the strategies at hand consists of “ngram_guess” and “semantic_guess”.

<h2>VIDEO EXPLAINATION:-</h2> https://drive.google.com/file/d/1M2EN2ByRyb0K4jAcKAlD5w0UnPvsg8jy/view?usp=drive_link
