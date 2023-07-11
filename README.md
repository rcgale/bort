# BORT

BORT is a pretrained LLM that is designed to accept a mixture of English phonemes (in IPA) and orthography, made with clinical language evaluation tasks in mind. From the paper:

Robert Gale, Alexandra C. Salem, Gerasimos Fergadiotis, and Steven Bedrick. 2023. [**Mixed Orthographic/Phonemic Language Modeling: Beyond Orthographically Restricted Transformers (BORT).**](./2023-acl-bort.pdf) In Proceedings of the 8th Workshop on Representation Learning for NLP (RepL4NLP-2023), pages TBD, Online. Association for Computational Linguistics.

## Limitations

The models presented here were trained with the basic inventory of English phonemes found in CMUDict. However, a more fine-grained phonetic analysis would require a pronunciation dictionary with more narrowly defined entries. Additionally, while this paper focused on models trained with English-only resources (pre-trained BART-BASE, English Wikipedia text, CMUDict, and the English AphasiaBank), the techniques should be applicable to non-English language models as well. Finally, from a clinical standpoint, the model we describe in this paper assumes the existence of transcribed input (from either a manual or automated source, discussed in detail in §2.1 of the paper; in its current form, this represents a limitation to its clinical implementation, though not to its use in research settings with archival or newly-transcribed datasets.

## Ethics Statement

Our use of the AphasiaBank data was governed by the TalkBank consortium's data use agreement, and the underlying recordings were collected and shared with approval of the contributing sites' institutional review boards.
Limitations exist regarding accents and dialect, which in turn would affect the scenarios in which a system based on our model could (and should) be used.
It should also be noted that these models and any derived technology are not meant to be tools to diagnose medical conditions, a task best left to qualified clinicians.



## Pre-trained Model Variants

- **BORT-PR** (upload ETA ≤ ACL 2023)
- **BORT-SP** (upload ETA ≤ ACL 2023)
- **BORT-PR-SP** (upload ETA ≤ ACL 2023)
- **BORT-PR-NOISY** (upload ETA ≤ ACL 2023)
- **BORT-SP-NOISY** (upload ETA ≤ ACL 2023)
- **BORT-PR-SP-NOISY** (upload ETA ≤ ACL 2023)

## Wikipedia Dataset Used in Pre-Training

The BPE-tokenized version of the dataset, including metadata used in word transforms.

- **Dataset** (upload ETA ≤ ACL 2023)

## Acknowledgements

This work was supported by the National Institute on Deafness and Other Communication Disorders of the National Institutes of Health under award 5R01DC015999 (Principal Investigators: Bedrick \& Fergadiotis). The content is solely the responsibility of the authors and does not necessarily represent the official views of the National Institutes of Health. 
