# Spellchecker-NLP

Implemented functions to correct spelling mistakes in a document. There is no right way to perform spell checking and is totally dependent on the corpus or the vocabulary you have with you. The order in which you call these functions matters too.

I walk you through different types of tokens/ words that commonly occur in a document.

1) **Named entities** - These are tokens which represent a Organization, Place, Person or a Cardinal. These tokens shouldn't be pre-processed or spell-checked. Hence it is important to do Named Entity Recognition(NER) and seperate them.

2) **pyspellchecker** - This is a package in python that tells you if there is an error in spelling with spell.unknown and tries to correct the spelling on its own with spell.correction.

3) **Recurring character token**- These tokens occur more frequently than you expect, for Eg- Birthdayyyyyyyy needs to be corrected to Birthday. A simple ReGex can be used to solve this issue.

4) **Word split with wordninja** - Sometimes words are merged, or have an irrelevant character between them. Eg- handnwash needs to be corrected to hand and wash. Similarly cheesepizza needs to be corrected to cheese and pizza.

**Installation**
pip install wordninja
pip install pyspellchecker
