# icaars: Prediction and Classification of Aminoacyl tRNA Synthetases

Welcome to the official documentation for **aaRSPred**, a computational method developed for the prediction and classification of Aminoacyl tRNA synthetases (aaRSs) using PROSITE domains and Support Vector Machines (SVM). aaRSs are essential enzymes that catalyze the attachment of amino acids to their cognate transfer RNAs, playing a vital role in protein synthesis across all organisms.

**Web Server:** [http://www.imtech.res.in/raghava/aarspred/](http://www.imtech.res.in/raghava/aarspred/)(https://webs.iiitd.edu.in/raghava/icaars/)

---

## Citation

Panwar, B., & Raghava, G. P. S. (2010). 
**Prediction and classification of aminoacyl tRNA synthetases using PROSITE domains.** *BMC Genomics*, 11, 507. 
[https://doi.org/10.1186/1471-2164-11-507](https://doi.org/10.1186/1471-2164-11-507)
Zenodo:-(https://doi.org/10.5281/zenodo.20133931)

---

## About the Platform

aaRSPred was developed to address the need for accurate identification and classification of aaRSs. These enzymes are divided into two distinct classes (Class I and Class II), each comprising ten enzymes. aaRSPred utilizes a variety of features, including amino acid composition, dipeptide composition, and domain-based information, to effectively discriminate aaRSs from non-aaRSs and to classify them into their respective classes and sub-classes.

### Key Features
* **SVM-Based Classification**: Employs Support Vector Machines to provide high-accuracy discrimination and classification.
* **PROSITE Domain Integration**: Utilizes specific functional domains (e.g., PS50862, PS00178) to improve prediction reliability.
* **Hybrid Approach**: Combines domain information with dipeptide composition to achieve superior performance.
* **Multi-Level Classification**: Capable of classifying enzymes into Class I or Class II, and further into specific types based on the amino acid they carry.

---

## Technical Overview

The models were developed using a non-redundant dataset of 117 aaRSs and 117 non-aaRSs, where no two sequences shared more than 30% similarity.

| Method / Feature | Accuracy (%) | MCC |
| :--- | :--- | :--- |
| **BLAST (Similarity Search)** | 67.52% | - |
| **SVM (Dipeptide Composition)** | 83.73% | 0.68 |
| **Hybrid (SVM + Domains)** | 88.00% | 0.77 |

---

## Model Functionality

* **aaRS Identification**: Accurately predicts whether a query protein sequence is an aminoacyl tRNA synthetase.
* **Class Prediction**: Classifies identified aaRSs into Class I (enzymes that acylate the 2'-OH of the adenosine) or Class II (enzymes that acylate the 3'-OH).
* **Detailed Sub-classification**: Provides further classification into specific types corresponding to the twenty natural amino acids.

---

## Applications

* **Functional Genomics**: Annotating aaRSs in newly sequenced genomes across all domains of life.
* **Protein Synthesis Research**: Understanding the precise mechanisms and evolutionary relationships of tRNA charging.
* **Evolutionary Biology**: Studying the classification and divergence of these ancient and essential enzymes.

---

## Contact & Authors

**Gajendra P. S. Raghava** Bioinformatics Centre, Institute of Microbial Technology (CSIR), Chandigarh, India.  
**Email**: raghava@imtech.res.in

---

## License

This project is open-access and distributed under the terms of the **Creative Commons Attribution License**, which permits unrestricted use and distribution provided the original author and source are properly credited.
