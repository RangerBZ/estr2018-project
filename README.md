# estr2018-project
## Introduction
this project is the requirement of ESTR2018 Probability for Engineers

## Implementation Process
our main procedure for contructing the model come mostly from [this paper](https://www.researchgate.net/profile/Anbang-Xu/publication/221414811_Spam_email_filtering_with_Bayesian_belief_network_using_relevant_words/links/560d981e08ae6cf681540164/Spam-email-filtering-with-Bayesian-belief-network-using-relevant-words.pdf)
Our data set comes from [here](https://www.kaggle.com/datasets/jokerak/acllmdb)
### Text preprocess
we represent the words in one review as one feature/word vector, the $i$-th component $w_i$ is the number of times the word appears in one review.
In this process, we apply word stemming, i.e. converting the words into base forms, "kicked" and "kicking" to "kick";
and we remove the stop-word which carry useless information, like "and, a, the, we".
and to be more specific, we use nltk when doing it.