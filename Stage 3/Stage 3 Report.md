**Stage 3 Report**

Contributors: <b>Ntsieni Midalo Shaka , Babatunde OWOLOYE</b>

**Phase 1**

**Pancreatic Cancer and EGFR Inhibition**

Pancreatic cancer is a highly aggressive and lethal disease, with a five-year survival rate of less than 10%. The epidermal growth factor receptor (EGFR) is a key target for cancer therapies, as its mutations and overexpression are linked to various cancers.

Artemisia afra, a medicinal plant, contains phytochemicals with potential anti-cancer properties. This study investigated the binding affinity of 50 Artemisia afra phytochemicals to EGFR using molecular docking simulations.

**Methods**

The 3D structure of EGFR was obtained from the Protein Data Bank (PDB). Phytochemical structures were sourced from PubChem. Active site identification was performed using CASTp, and molecular docking simulations were conducted using PyRx and AutoDock Vina.

**Results**

The phytochemicals exhibited varying binding affinities, with lupeol demonstrating the strongest affinity (-12.8 kcal/mol). Lupeol formed hydrogen bonds with Met769 and Lys721 and hydrophobic interactions with Thr766.

![Aspose Words 69d32307-332d-47ed-8a87-d75cd0bad659 001](https://github.com/user-attachments/assets/1a894aa3-a0c5-4563-975d-247ad30e828a)
 **Figure 1**: The 3D structure of the EGFR tyrosine kinase domain (PDB ID: 1M14) obtained from the Protein Data Bank. The figure displays the key features of the protein, including the ATP-binding pocket and the residues involved in ligandinteractions, such as Met769 and Lys721.

![Aspose Words 69d32307-332d-47ed-8a87-d75cd0bad659 002](https://github.com/user-attachments/assets/4ce051f1-643d-4c5b-bbea-81cc2d16b488)
 **Figure 1.2**: Visualization of *Lupeol* docked within the active site of EGFR (PDB ID: 1M14), generated using Biovia Discovery Studio. The compound formed multiple hydrogen bonds with key EGFR residues, including Met769 and Lys721.

![Aspose Words 69d32307-332d-47ed-8a87-d75cd0bad659 003](https://github.com/user-attachments/assets/8ea69ee4-2043-4213-9f0f-07e1abf09d3d)
**Figure 1.3**: Docking pose of *Lupeol* within the EGFR active site, highlighting hydrophobic interactions with Thr766, visualized in Biovia Discovery Studio

**Discussion**

The study revealed significant binding affinities between EGFR and Artemisia afra phytochemicals. Lupeol's strong binding affinity and favorable interactions with key residues suggest potential as an EGFR inhibitor. Structure-activity relationship analysis highlighted the importance of hydroxyl groups in enhancing binding potential.

**Conclusion**

This study demonstrates the potential of Artemisia afra phytochemicals as EGFR inhibitors, warranting further investigation into their mechanisms of action. These findings highlight the therapeutic potential of Artemisia afra phytochemicals as EGFR inhibitors for EGFR-related cancers, such as pancreatic cancer.

**References**

1. American Cancer Society, 2023. *Pancreatic Cancer.* [online] Available at: https://www.cancer.org/cancer/pancreatic-cancer/about.html [Accessed 25 September 2024].
1. Berman, T., et al., 2000. "Pancreatic Cancer: A Review." *Oncology,* 14(7), pp. 793-801.
1. Hänsel, R., et al., 1993. "Terpenes from Artemisia afra." *Phytochemistry,* 32(5), pp. 1349-1352.
1. Lai, K. and Roy, S., 2004. "Phytochemical Analysis of Artemisia afra." *Journal of Ethnopharmacology,* 95(1), pp. 1-5.
1. Lynch, T.J., et al., 2004. "Activating mutations in the epidermal growth factor receptor underlying responsiveness of non-small-cell lung cancer to gefitinib." *N Engl J Med,* 350(21), pp. 2129-2139.
1. Mimica-Dukić, N., et al., 2003. "Phenolic Compounds and Flavonoids in Medicinal Plants." *Natural Product Communications,* 1(1), pp. 67-72.
1. Mok, T.S., et al., 2009. "Gefitinib or carboplatin-paclitaxel in pulmonary adenocarcinoma." *N Engl J Med,* 361(10), pp. 947-957.
1. Tshikalange, T.E., et al., 2005. "Antimicrobial activity of extracts from Artemisia afra." *South African Journal of Botany,* 71(3), pp. 456-459.
1. Van Wyk, B.-E. and Gericke, N., 2000. *People's Plants: A Guide to Useful Plants of Southern Africa.* Briza Publications.
1. Viljoen, A., et al., 2006. "Chemical composition and biological activity of Artemisia afra." *Journal of Ethnopharmacology,* 107(2), pp. 206-211.



**Phase 2**

Data Analysis and Machine Learning Pipeline for EGFR Inhibition

**Dataset Overview**

This analysis explores bioactivity data for EGFR, sourced from ChEMBL, comprising compound information and target details.

**Preprocessing Steps**

1\. Data Retrieval: ChEMBL client (EGFR bioactivity data)

2\. Molecule Preparation: RDKit (structure management, descriptor calculation, preprocessing)

3\. Drug-Likeness Filtering: Lipinski's Rule of Five

**Preprocessing Outputs**

\- Data Cleaning: 15900 rows × 46 columns

\- Data Transformation: Combined key columns

\- Bioactivity classification

\- Molecular Descriptors: Calculated Lipinski descriptors

\- IC50 Conversion: Transformed to pIC50

Training Phase

\- Feature Generation: RDKit, Mordred (molecular descriptors)

\- Model Development: Dataset split (80% train, 20% test), Linear Regression, Random Forest, Ridge Regression, Decision Trees

Testing Phase

1\. Model Evaluation: Compared predicted bioactivity values (pIC50) against actual data.

2\. Performance Metrics: Mean RMSE, R-squared, Mean Absolute Error (MAE)

3\. Cross-Validation

**Results**

The random forest model outperformed others, yielding:

\- RMSE: 0.254858016129063

\- R-squared: 0.8975385921910887

Molecular Descriptors Influencing EGFR Bioactivity

1\. Hydrogen Bond Donors/Acceptors

2\. Molecular Structure

3\. Electrostatic Properties

4\. Hydrophobicity/Hydrophilicity

5\. Steric Hindrance

6\. Rotatable Bonds

7\. Solubility and Stability

**Conclusion**

Understanding these descriptors aids in designing and optimizing EGFR inhibitors. By considering molecular characteristics influencing binding and activity, researchers can develop effective drugs.** The random forest model's strong performance indicates potential for predictive modeling in EGFR inhibition.
