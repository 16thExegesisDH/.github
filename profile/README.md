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
- [Guideline](#guideline)
  - [I. Guideline for Segmentation](#i-guideline-for-segmentation)
  - [II. Guideline for Transcription](#ii-guideline-for-transcription)
  - [III. Encoding Problem](#iii-encoding-problem)
- [Citations](#citations)

## Data 

**Corpus HTR et Segmentation**

* 2026 (spring-summer): []() digital library corpus
* 2025: [HTR_1-Timotheus](https://github.com/16thExegesisDH/HTR_1-Timotheus) (Roman characters): Contains the best dataset :white_check_mark:
  - Commentaries on Timotheus and PHD students dataset `_test`
* 2024: [HTR_Lambertus_prototype](https://github.com/FourbeFlo/Lambertus) (Roman characters):
  - The beta-test corpus 2023-2024, more information on https://github.com/FourbeFlo/Lambertus, data now uploaded with a new version  

## Corpus 

The complete corpus is available in the HTR_Paul_corpus repository.

[Corpus: 7-10-24](https://github.com/16thExegesisDH/HTR_beta_corpus_2023/blob/main/corpus_ocr.csv)

## Models 
* Layout Analysis : 
* HTR :  - best model to use now (trained by collegues with a set of our datas :  
         -old model trained for the projet : 

# Guideline 

The guidelines for segmentation and transcription are available in the following [README](https://github.com/16thExegesisDH/HTR_Paul_corpus/blob/main/README.md).

## I. Guideline for Segmentation

The main documentation is here: [Annotation Guide on GitHub](https://github.com/DEFI-COLaF/LADaS/blob/main/AnnotationGuide.md).

### Examples of Specific Cases in Our Corpus

#### Legend
- **RunningTitleZone**: pink
- **MainZone:Head**: yellow
- **MainZone:P**: dark green
- **MainZone:P#Continued**: light blue
- **NumberingZone**: rosa (specific examples provided)
- **DropCapitalZone**: dark viola
- **QuireMarkZone**: viola
- **MainZone-ListItem**: brown
- **MarginTextZone-ManuscriptAddendum**: red

#### Examples

| Description | Example |
|-------------|---------|
| **RunningTitleZone**: pink <br/> **MainZone:Head**: yellow <br/> **MainZone:P**: dark green <br/> **MainZone:P#Continued**: light blue <br/> **NumberingZone**: rosa for "section 12" and "102" <br/> **QuireMarkZone**: viola | <img src="../profile/pictures/segmentationGL/Bucer_Eph_1.png" width="300"/> |
| **RunningTitleZone**: pink <br/> **DropCapitalZone**: dark viola <br/> **MainZone:Head**: yellow <br/> **MainZone:P**: dark green <br/> **MainZone:P#Continued**: light blue <br/> **NumberingZone**: rosa for "456", "II", "III" <br/> **QuireMarkZone**: viola | <img src="../profile/pictures/segmentationGL/Bucer_Rm_1.png" width="300"/> |
| **RunningTitleZone**: pink for "VII" (Epistle number) and "Col" (Epistle name) <br/> **MainZone:Head**: yellow <br/> **MainZone:P**: dark green <br/> **MainZone:P#Continued**: light blue <br/> **NumberingZone**: rosa for "7", "8", "184" | <img src="../profile/pictures/segmentationGL/Lefevre_1.png" width="300"/> |
| **RunningTitleZone**: pink for "COM" <br/> **DropCapitalZone**: dark viola <br/> **MainZone:Head**: yellow <br/> **MainZone:P**: dark green <br/> **MainZone:P#Continued**: light blue <br/> **NumberingZone**: rosa for "1", "C4", "D4", "5", "6" | <img src="../profile/pictures/segmentationGL/Lefevre_2.png" width="300"/> |
| **RunningTitleZone**: pink <br/> **MainZone-ListItem**: brown for "II ad liberalitatem [...] etc" <br/> **MainZone:Head**: yellow <br/> **MainZone:P**: green <br/> **NumberingZone**: rosa <br/> **QuireMarkZone**: viola | <img src="../profile/pictures/segmentationGL/ListItem.png" width="300"/> |
| **TitlePageZone**: light light viola <br/> **MarginTextZone-ManuscriptAddendum**: red <br/> _for the manuscript annotation around the text_ | <img src="../profile/pictures/segmentationGL/TitlePage.png" width="300"/> |

## II. Guideline for Transcription

We follow, as much as possible, the transcription standards proposed by [CATMuS standard](https://catmus-guidelines.github.io):

**Citation:**

Ariane Pinche, Thibault Clérice, Alix Chagué, Jean-Baptiste Camps, Malamatenia Vlachou-Efstathiou, et al., *CATMuS-Medieval: Consistent Approaches to Transcribing ManuScripts: A generalized set of guidelines and models for Latin scripts from Middle Ages (8th–16th century)*. 2023. [hal-04346939](https://hal.archives-ouvertes.fr/hal-04346939).

### Special Cases

* Special cases are documented in the examples below. The relevant letters or signs are encoded in **Junicode** and added to the [_exegesis_ keyboard](keyboard/exegesis.json).
* Greek text is fully transcribed and edited without preserving any abbreviations or ligatures.
* Hebrew letters may appear in the data but are not corrected as of now (19.02.2025).

### Tools for Building the Transcription

* **Download the keyboard for special letters:** /
  - If a letter is not already included in the keyboard, take a screenshot and store the image in `pictures/mysteria_litterae`.
* **Greek Transcription:**
  - Greek is transcribed fully.
  - Issues related to transcribing ligatures can be resolved using:
    - [Greek_Abbreviations.pdf](Greek_Abbreviations.pdf)
    - [_Alphabetum Graecum_ by Theodore de Bèze](https://doi.org/10.3931/e-rara-6065), see vignettes 27-39.

### Examples of Special Cases

| **Sign** | **Example** | **Source** | **Transcription** | **Unicode/Junicode** |
|----------|-------------|------------|-------------------|----------------------|
| Pilcrow | <img src="https://github.com/FourbeFlo/Lambertus/blob/main/images/piedDeMouche_1.jpg" alt="Pillcrow" width="85" height="47"> | [e-rara, p.11](https://doi.org/10.3931/e-rara-6338) | ¶ | `U+00B6` |
| Semicolon (shaped) | <img src="https://github.com/FourbeFlo/Lambertus/blob/main/images/semi-colon%20shapped.png" alt="semi-colon" width="27" height="48"> | | <img src="/.github/blob/main/profile/pictures/mysteria_litterae/que_acute_semicolon2.png" alt="que accentue" width="60" height="67"> | q `U+0071` + acute `U+0301` <br> Junicode (`F1AC`) |
| Cumque Abbreviation | <img src="/.github/blob/main/profile/pictures/mysteria_litterae/cumque_abreviation.png" alt="cumque" width="27" height="48"> | | <img src="/.github/blob/main/profile/pictures/mysteria_litterae/que_ligature.png" alt="cumque" width="76" height="45"> | Junicode (`00E8BF`) + tilde (`000303`) |
| Tur Abbreviation | <img src="/.github/blob/main/profile/pictures/mysteria_litterae/tur_abreviation.png" alt="tur" width="27" height="48"> | | <img src="/.github/blob/main/profile/pictures/mysteria_litterae/tur_online.png" alt="tur" width="48" height="75"> | Junicode (`000303`) + t Unicode |

## III. Encoding Problem

### Reading Hidden Characters in Junicode on eScriptorium

| Original state | Encoding Failure | Encoding Success |
|:----------------:|:-----------------:|:----------------:|
| <img src="./pictures/stylus/qligature.png" width="80"> |  <img src="./pictures/stylus/encodingfail.png" width="80"> | <img src="./pictures/stylus/encoding_working.png" width="80">|

---

### Steps to Resolve Encoding Issues with Stylus:

1. **Use Google Chrome:**  
   Ensure you are using Chrome as your web browser. The following steps require the Stylus extension.

2. **Download the Stylus Extension:**  
   Install Stylus from the Chrome Web Store:  
   [Stylus Extension](https://chromewebstore.google.com/detail/stylus/clngdbkpkpeebahjckkjfobafhncgmne)

3. **Upload the MUFI Style for eScriptorium:**  
   Download the MUFI style from this link:  
   [MUFI for eScriptorium](https://userstyles.world/style/3915/mufi-for-escriptorium)

4. **Implement and Apply the Style:**  
   - Open the Stylus extension in Chrome.  
   - Upload the downloaded MUFI style.  
   - Apply the style to the **e-Scriptorium** domain
---

<img src="./pictures/stylus/change_stylecss.png" > <br/>
<img src="./pictures/stylus/plugin_stylus.png" > <br/>

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
