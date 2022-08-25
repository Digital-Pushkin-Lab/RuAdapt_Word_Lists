# RuAdapt_Word_Lists

This repository contains word lists that were created from parallel simplification/adaptation data or from other dictionaries and word lists.

**RuAdapt_literature_word_list** is a list of monolingual word alignments taken from the [RuAdapt adapted literature subcorpus](https://github.com/Digital-Pushkin-Lab/RuAdapt/tree/main/Adapted_literature).

**RuAdapt_literature_word_list_only_good_pairs** is a shorter version of the previous list containing only "good" pairs with higher human evaluation scores. It also contains more information about each pair, including, for example, the words' CEFR grade levels.  

**dictionary synonyms** is a list of "regular" words and their synonyms from CEFR-graded vocabulary lists for students of Russian as a foreign language. The list was created for [this project](https://www.hse.ru/en/edu/vkr/182626286) (full text in Russian).  


### Columns in the word lists

* source: a word from source sentence, a "regular"/"complicated" word;
* target: a word from target sentence that corresponds to the source word, its "simple" synonym;
* score_1, score_2: scores given to the pair by human editors. Score 0 means that the words in the pair are not synonymous at all, score 1 means partial synonymity, and score 2 stands for synonymity in most contexts;
* editor_1, editor_2: human editor's ID;
* partition: whether the word pair was retrieved by eflomal (e), awesome-align (a), of both (e&a);
* agreement: agreement between editors (1 - two editors agreed on the score, 0 - disagreed);
* score_3: the resulting score of a pair, either the score the two editors agreed on or the third editor's score;
* source_pos, target_pos: POS tags of the source and target words (NB! all grammar info retrieved with the help of the Stanza Syntagrus model);
* source_lemma, target_lemma: source and target words' lemmas;
* source_sentence, target_sentence: source and target sentences the way they are present in the RuAdapt dataset;
(listed below are columns only present in the "only good pairs" list)
* source_cefr, target_cefr: source and target's CEFR grade levels, if the words are precent in the vocabulary lists;
* source_ipm, target_ipm: source and target's IPM, taken from the [Modern Russian frequency dictionary](http://dict.ruslang.ru/freq.php);
* target_sentence_level: the CEFR grade level for which the adapted text is intended, as specified by publisher;
* target_level_comparison: how the target sentence level compares to the target word's CEFR grade level.
