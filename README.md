---
license: apache-2.0
---

# Constitution Multi Lang

A collection of multiple nation, constitutional legal documents, with their official language translation.

## Rationale behind this

This project aims to get the official translation pairs of various **non-english** constitutions, of various nations.
Due to the importance of such documents on a nation, it is expected that the translation pairs are of high quality.
Additional in many cases, official goverment documents are "copyright free", removing any legal issues in the training process.

This also provides an easy scalable way to get reliable translation pairs for AI training.

## Repo links

Github: https://github.com/PicoCreator/constitution-multi-lang
Huggingface: https://huggingface.co/datasets/picocreator/constitution-multi-lang

## How to contribute (a public contributor)

1) Obtain official copies, and/or links and place them within the respective country folder in `raw-copies`

2) Cleanup and convert raw copies, into language markdown pairs. Line number content must 1:1 match one another into the `cleaned` folder.

3) Submit a pull request - via github

## How to followup with a completed contribution

1) Validate the cleaned markdown pairs, and ensure they are 1:1 match with the official copies.

2) Convert into translation training pairs, on the "vocab", "section", and "document" level. Generate the .jsonl files into the `parsed` folder.

3) Split out some vocab and section pairs, for them to be used in validation dataset.

## Example

Canada
- has an english copy : https://laws-lois.justice.gc.ca/eng/const/FullText.html
- and a french copy : https://laws-lois.justice.gc.ca/fra/const/TexteComplet.html

The converted markdown pairs (for en/fr) would be:
- https://github.com/PicoCreator/constitution-multi-lang/blob/main/cleaned/canada/fr.md
- https://github.com/PicoCreator/constitution-multi-lang/blob/main/cleaned/canada/fr.md