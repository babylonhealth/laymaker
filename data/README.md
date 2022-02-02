# Data

`test-set.csv` contains our test set of 1000 sentence pairs (original, simplified), and the generated sentences from all methods and benchmarks.

Columns:
ID \
ORIGINAL : original sentence, extracted from MTSamples \
REFERENCE : sentence simplified by the physicians \
REDDIT-NGRAM : sentence simplified by frequency + ngram LM trained on Reddit medical data \
REDDIT-GPT1 : sentence simplified by frequency + GPT1 LM trained on Reddit medical data \
GENERAL-GPT2 : sentence simplified by frequency + GPT2 LM out of the box \
NTS : sentence simplified by the NTS system (MT model trained on Simple Wikipedia) \
ClinicalNTS : sentence simplified by the ClinicalNTS system (MT model trained on medical sentences from Simple Wikipedia with medical Phrase Table) \
replaceWithShardlowPT : sentence simplified by the Phrase Table from Clinical NTS \



`dev-set-(alpha).csv` contains our dev set of 250 sentence pairs (original, simplified), used to tune our alpha parameter.
Columns are similar as `test-set.csv`
