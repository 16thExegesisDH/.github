## 16th Century Exegesis of Paul

# Website 

* Website: https://16thexegesisdh.github.io/ReformingPaul/ 
* Migration to TEI Publisher scheduled for **summer 2026**

# Project

The digital component of the project on the exegesis of Paul aims to build up a corpus of commentaries dating from the 16th century.

This digital corpus will make it possible to develop specific textual analysis tools for texts in Latin from the 16th century and models for the automatic processing of printed material in Latin from this period. A major digital dimension is therefore planned for this project, with the digitisation of a large number of printed documents on the one hand and the computational exploitation of this data on the other, in particular using distant reading and topic modeling.


## Funder

This project is funded by the Swiss National Science Foundation (SNSF). Project number: [207696](https://data.snf.ch/grants/grant/207696)

# Table of Contents

- [Data](#data)
- [Corpus](#corpus)
- [Models](#model)
- [Workflow](#Workflow)
- [Guideline](#guideline)
  - [I. Segmentation](#i-segmentation)
  - [II. Transcription](#ii-transcription)
- [Citations](#citations)

## Data 

**Corpus HTR et Segmentation**

* 2026 (spring-summer): []() digital library corpus
* 2025: [HTR_1-Timotheus](https://github.com/16thExegesisDH/HTR_1-Timotheus) (Roman characters): Contains the best dataset :white_check_mark:
  - Commentaries on Timotheus and PHD students dataset `_test`
* 2024: [HTR_Lambertus_prototype](https://github.com/FourbeFlo/Lambertus) (Roman characters):
  - The beta-test corpus 2023-2024, more information on https://github.com/FourbeFlo/Lambertus, data now uploaded with a new version  

## Corpus 

| Corpus | Description | File |
|--------|-------------|------|
| **Corpus A** | Gold-standard corpus (manually corrected) | [Corpus_A_2.csv](https://github.com/16thExegesisDH/HTR_1-Timotheus/blob/main/corpus/digital_library_set/Corpus_A_2.csv) |
| **Corpus B** | Automatically processed version of the same book (segmentation + HTR) | [Corpus_B_2.csv](https://github.com/16thExegesisDH/HTR_1-Timotheus/blob/main/corpus/digital_library_set/Corpus_B_2.csv) |
| **Corpus C** | Digital library corpus (reviewed segmentation, corrected verse-level HTR) | [Corpus_C_2.csv](https://github.com/16thExegesisDH/HTR_1-Timotheus/blob/main/corpus/digital_library_set/Corpus_C_2.csv) |



## Models 

* **Layout Analysis:**
  - [Repository – Segmentation-model](https://github.com/16thExegesisDH/Segmentation_model)
  - best model (20.01.26) :[Download](https://github.com/16thExegesisDH/Segmentation_model/releases/download/segmentation/best.pt)
* **HTR:** 
  - Best model to use now (trained by colleagues with a set of our data): 
  - Old model trained for the project:
    * [Reposoitory – OCR](https://github.com/FourbeFlo/OCR_test)
    - old model (25.06.2024): [Download](https://github.com/FourbeFlo/OCR_test/releases/download/ml.model/lambertus_test_mai_best.mlmodel)
## Workflow

The complete pipeline and all scripts are described and available in the following repository:  
**[Workflow Repository – PipeLineThm](https://github.com/16thExegesisDH/PipeLineThm)**  

For further explanations and examples, see our training materials:  
**[Training Materials – CUSO 2025 Ed-Num Online](https://github.com/CUSO-2025-Ed-Num-online?view_as=public)**  
- **Sonia Solfrini**, Doctorante (Université de Genève | IHR, Projet FNS *SETAF*), **Floriane Goy**, Post-doctorante (Université de Genève | IHR, Projet FNS *16th Century Exegesis of Paul* )*

# Guidelines 

The guidelines for building Segmentation's and Transcription's datas. 

## I. Segmentation
The main documentation for segmentation is here: [Annotation Guide on GitHub](https://github.com/DEFI-COLaF/LADaS/blob/main/AnnotationGuide.md).
* Examples of specific cases in our corpus : [here](https://github.com/16thExegesisDH/HTR_Paul_corpus/blob/main/README.md)

  
## II: Transcription 
We follow, as much as possible, the transcription standards proposed by [Catmus standard](https://catmus-guidelines.github.io):
**Citation:**
Ariane Pinche, Thibault Clérice, Alix Chagué, Jean-Baptiste Camps, Malamatenia Vlachou-Efstathiou, et al., *CATMuS-Medieval: Consistent Approaches to Transcribing ManuScripts: A generalized set of guidelines and models for Latin scripts from Middle Ages (8th–16th century)*. 2023. [hal-04346939](https://hal.archives-ouvertes.fr/hal-04346939).
* Examples of specific cases in our corpus : [here](https://github.com/16thExegesisDH/HTR_Paul_corpus/blob/main/README.md)

# Citations

## Citation: Project

Ueli Zahnd, Stefan Krauter, Matteo Colombo, Floriane Goy, Benjamin Manig, Noemi Schürmann, _16th Century Exegesis of Paul_, Geneva; Zürich, Universities of Geneva and Zürich, 2023.

```bibtex
@misc{Goy_exegesisofPaul_2023,
  author={Ueli Zahnd, Stefan Krauter, Matteo Colombo, Floriane Goy, Benjamin Manig, Noemi Schürmann},
  title={16th Century Exegesis of Paul},
  address={Geneva; Zürich},
  publisher={University of Geneva; University of Zürich},
  year={2023},
  url={https://www.theologie.uzh.ch/de/faecher/neues-testament/Professur-f%C3%BCr-neutestamentliche-Wissenschaft/16th_century_exegesis_of_paul.html},
  note={Grant number SNFS: 207696},
}
```

## On the Project

- Reformation Readings of Paul: [RRP](https://rrp.zahnd.be/) – database for the 16th century printed commentaries on Paul.
- In Zürich: [Exegesis of Paul](https://www.theologie.uzh.ch/de/faecher/neues-testament/Professur-f%C3%BCr-neutestamentliche-Wissenschaft/16th_century_exegesis_of_paul.html)
- In Geneva: [L'exégèse des épîtres pauliniennes](https://www.unige.ch/ihr/fr/accueil/exegese-paulinienne/)
