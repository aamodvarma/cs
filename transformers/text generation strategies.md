**Greedy Search**
- Select the word with the highest probability as its next word $w_t = argmax_wP(w|w_{1:t-1})$
- Problem is it might miss high prob words hidden behind a relative lower prob word

**Beam Search**
- Reduces the risk of missing hidden high probaility word sequences by keeping most likely beams so using this it doesn't miss the high prob words.


**Sampling**
- We sample from a distribution instead of just picking the most probable one.
- This introduces randomness and makes the output non-deterministic

**Top K Sampling**
- We can make it so that the sampling only happens from the top k words rather than the entire distribution because the words after might just be useless.

**Top-p**
Only samples from the smallest num of words whose cummulative probability adds up to p.

So in cases where the distirbutino is to the left vs flat. Top p samples from lesser words for the first and more words for the second.



