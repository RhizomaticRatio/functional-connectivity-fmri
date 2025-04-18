#  Functional Connectivity Analysis of fMRI Data (Single Subject)

This project is a step-by-step walkthrough of how I analyzed a single-subject fMRI dataset to compute **ROI-based and network-based functional connectivity**. It documents the full analysis pipeline — from preprocessed BOLD data to time series extraction, connectivity matrices, and visual interpretation.

>  This notebook was part of my personal learning journey to understand how brain regions interact functionally using real fMRI data.


## Dataset Description

This project uses the **resting-state and arithmetic task fMRI dataset** from [OpenNeuro (ds002422)](https://openneuro.org/datasets/ds002422) -I have used only one subject in resting state-:

- **Title:** *fMRI: Resting State and Arithmetic Task*  
- **Dataset DOI:** [10.18112/openneuro.ds002422.v1.0.2](https://doi.org/10.18112/openneuro.ds002422.v1.0.2)  
- **BIDS Version:** 1.2.1  
- **Task:** `rest`  
- **Repetition Time (TR):** 2.0 seconds !! However, in fMRI metadata I used for the single subject it is indicated 3.56 second TR.
- **License:** [CC0 (Public Domain)](https://creativecommons.org/publicdomain/zero/1.0/)

**Authors:**  
Yana Panikratova, Alexander Tomyshev, Ekaterina Pechenkova, Roza Vlasova  

**Acknowledgments:**  
The authors thank Elena Mershina for help with study organization, Maria Fomina for BIDS formatting, and Mihail Levitchii for automating data preparation.

**Funding:**  
This research did not receive specific funding from any public, commercial, or nonprofit agency.

**Reference:**  
Panikratova, Y., et al. (2020). *Context-dependency in the Cognitive Bias Task and Resting-state Functional Connectivity of the Dorsolateral Prefrontal Cortex*.  
**Journal of the International Neuropsychological Society**, 26(8), 749–762. [DOI](https://doi.org/10.1017/S1355617720000302)

---

## Tools Used

- `Nilearn`: for loading, masking, plotting fMRI data
- `TemplateFlow`: for loading atlases
- `XCP-D`: denoising and postprocessing pipeline
- `fMRIPrep`: BIDS-compliant preprocessing
- `Matplotlib & Seaborn`: for plots and matrix visualizations

---

## Contact

Feel free to reach out for collaborations, feedback, or just to geek out about neuroscience and neuroimaging!

Oğulcan ULU  
Padova, Italy  
ogulcan.ulu7@gmail.com | ogulcan.ulu@studenti.unipd.it
