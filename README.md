# Towards more patient friendly clinical notesthrough language models and ontologies

This repo contains the data for the paper "Towards more patient friendly clinical notesthrough language models and ontologies" which will be published in the Proceedings of the American Medical Informatics Association Annual Symposium (AMIA) 2021.

The MTSamples dataset comprises around 5000 sample medical transcription reports from a wide variety of specialities uploaded to a community platform website ( https://mtsamples.com). However, publicly available annotations are limited to only include high-level metadata, e.g. the medical speciality of a report.


We create a parallel corpus of clinician-simplified medical sentences on the basis of the raw MTSamples dataset. We pre-process the entire original dataset by tokenising all sentences and expanding abbreviations based on a custom list of common medical ontologies compiled by clinicians. We then review and exclude sentences that have too little context (i.e. are confusing or ambiguous to a clinician) or grammatically incorrect. Finally, three clinicians (native British English speakers) create a new version of each sentence using layman terms, ensuring consistency of both structure and medical context and accuracy. Only one simple sentence is generated for each original sentence for which simplification is possible. The resulting dataset contains 1250 sentence pairs, of which 597 (47.76%) have been simplified. The remainder have been left unchanged because they could not be further simplified. The average number of tokens in the original sentences is 66.96, and in the simplified sentences 68.60.
We divide the data into a 250 sentence development set and a 1000 sentence test set.
