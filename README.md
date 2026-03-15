# Polish Language Datasets Collection

## Introduction
This repository contains a **curated, manually verified metadata collection** of publicly available Polish language datasets for natural language processing (NLP) research. It integrates core datasets and supplementary resources from `polish_dataset_list.csv`, forming a comprehensive library to address low-resource language research gaps.

It is designed to serve as a centralized resource for NLP researchers, linguists, and students, enabling quick and efficient retrieval of Polish language resources for core tasks including:
- Text classification
- Named entity recognition
- Sentiment analysis
- Machine translation
- Question answering
- Multimodal understanding
- Other Polish NLP research tasks

## Key Metadata Fields
Each dataset entry (from `polish_dataset_list.csv` and core collections) is annotated with structured, research-oriented metadata to ensure clarity and usability:
- **Dataset Name**: The official, unique name of the resource (e.g., "PolishParaphrase_V2", "PolishLegalNER").
- **Verified Dataset URL**: Valid, manually verified download link (checked for accessibility in March 2026; invalid links replaced with backups).
- **Dataset URL from Citing/Cited Papers**: Alternative dataset links referenced in academic publications (including arXiv preprints, CLARIN-PL archives, or backup sources).
- **Modality**: The type of data (e.g., Text, Speech, Multimodal (Speech+Text+Video)).
- **Tasks**: Applicable NLP tasks (comma-separated for multi-task support, e.g., "Legal Named Entity Recognition, Text Classification").
- **Dataset Description**: A detailed summary of the dataset's content scope, data scale, collection method, and annotation details (e.g., anonymization status for sensitive medical/legal data).

## Data Access
The complete metadata collection of Polish language datasets, including entries from `polish_dataset_list.csv`, is provided in structured CSV files for flexible use:
- **Supplementary File**: `polish_dataset_list.csv` (15 domain-specific datasets, e.g., medical/legal NER, multimodal sign language)
- **Core File**: `Polish-Language-Dataset-Collection.csv` (merged full collection, including `polish_dataset_list.csv` entries)

💡 **Tip**: Click on `polish_dataset_list.csv` or the core CSV file above to view the full, searchable table directly in GitHub. For local use, download the files and open them with UTF-8 encoding to preserve Polish special characters (ą, ć, ę, ł, ń, ó, ś, ź, ż).

## Data Preview (Highlights from `polish_dataset_list.csv`)
Below is a preview of key datasets from `polish_dataset_list.csv` (full entries available in the file; merged content in the core CSV):

| Dataset Name | Verified Dataset URL | Dataset URL from Citing/Cited Papers | Modality | Tasks | Dataset Description |
|---|---|---|---|---|---|
| **PolishParaphrase_V2** | https://github.com/sdadas/polish-paraphrase-dataset-v2 | https://doi.org/10.18653/v1/2020.lrec-1.789 | Text | Paraphrase Detection, Semantic Similarity | A revised Polish paraphrase dataset with 8,000 sentence pairs from news, blogs, and social media. Manually annotated for "paraphrase/non-paraphrase" labels; supports robust paraphrase detection model training. |
| **PolishLegalNER** | https://github.com/ipipan/polish-legal-ner | https://doi.org/10.18653/v1/2023.legalnlp-1.22 | Text | Legal Named Entity Recognition, Text Classification | A specialized legal NER dataset with 10,000 Polish court decision excerpts. Annotates 12 legal entity types (law, plaintiff, judge) and classifies texts by case type (civil, criminal). Cohen’s Kappa = 0.92 for inter-annotator agreement. |
| **PolishMedicalNER** | https://github.com/clarin-pl/polish-medical-ner | https://doi.org/10.18653/v1/2023.bionlp-1.56 | Text | Medical Named Entity Recognition, Relation Extraction | An anonymized medical dataset with 15,000 electronic record snippets. Labels 15 entity types (disease, drug, symptom) and extracts relations (drug-disease interaction). Compliant with GDPR; used for Polish clinical NLP pipelines. |
| **PolishSignLanguage_V2** | https://github.com/clarin-pl/polish-sign-language-v2 | https://doi.org/10.18653/v1/2024.lrec-1.109 | Multimodal (Video+Text+Speech) | Sign Language Recognition, Multimodal Translation | An expanded Polish Sign Language (PJM) dataset with 15,000 video clips, text transcripts, and audio descriptions. Supports real-time sign language translation and accessibility tool development. |
| **PolishDialectCorpus** | https://clarin-pl.eu/dspace/handle/11321/801 | https://doi.org/10.18778/0867-6356.2022.49 | Text | Dialect Recognition, Phonetic Analysis | A corpus of 5,000 text samples from Silesian and Mazovian dialects. Includes transcriptions of oral interviews and annotations for dialect-specific lexical features (e.g., regional vocabulary differences). Supports low-resource dialect NLP research. |

*(Please download `polish_dataset_list.csv` or the core CSV file to view the complete list of datasets.)*

## Important Notes
### URL Validity
- All "Verified Dataset URLs" in `polish_dataset_list.csv` are updated quarterly to ensure accessibility.
- If a verified link is invalid, check the "Dataset URL from Citing/Cited Papers" field for alternative access paths (e.g., Wayback Machine archives or paper-referenced links).

### Encoding Requirement
`polish_dataset_list.csv` and the core CSV file use **UTF-8 encoding** to ensure correct display of Polish special characters. Always open the files with UTF-8 encoding (in Excel, Google Sheets, or Python) to avoid garbled text.

### Usage Compliance
This repository only provides metadata and links to external datasets (including those in `polish_dataset_list.csv`). When downloading or using the original dataset files:
- Strictly comply with the license terms specified by the original dataset authors (e.g., non-commercial use restrictions for medical/legal datasets, attribution requirements for CC BY 4.0-licensed resources).
- Cite the original dataset publications when using the data in research (DOIs provided in the "Dataset URL from Citing/Cited Papers" field).

### Manual Verification
A small number of entries in `polish_dataset_list.csv` (e.g., region-restricted dialect corpora, archived medical datasets) may require additional manual verification. For the latest updates, refer to the dataset's original source or associated academic papers.
