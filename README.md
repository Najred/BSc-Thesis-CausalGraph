# BSc-Thesis-CausalGraph
This repository contains the implementation of TRACE, the framework developed and presented in the thesis “Emergent Causal Graphs from LLM-Guided Tree Exploration of Latent Variables”. TRACE is a tree-based method for autonomous causal structure discovery using Large Language Models (LLMs). It recursively builds partial causal graphs by performing localized cause-effect queries between variable pairs, enabling scalable exploration of latent causal structures without relying on external context or fine-tuning. This codebase reflects the core architecture and development environment described in the thesis.

---

The repository accompanies the B.Sc. thesis:  
**"Emergent Causal Graphs from LLM-Guided Tree Exploration of Latent Variables"**   
_TU-Darmsatdt_  
_Computer Science / AIML_ 

---

## 📂 Repository Structure

### Main Folder

- **`causality_finder_parallel.ipynb`**  
  Contains the full TRACE framework:
  - Core implementation
  - Execution control wrapper
  - Parameter specifications
  - Evaluation and grading of TRACE outputs

- **`direct_crab.ipynb`** and **`direct_tubing.ipynb`**  
  Direct dataset inspections for benchmarking TRACE with the Crab and Tubing datasets.

### `manual_safes/`
Includes the CRAB and tubing datasets as well as old execution outputs:
- Original and cleaned versions of the Crab and Tubing datasets
- Residual files from development, including earlier TRACE versions used for various analysis stages

### `log_dump/`
Contains raw outputs of all prompts executed during TRACE runs.

### `recent/`
The default output folder for all TRACE executions:
- Individual runs are saved directly here
- Automated batch runs are organized into respective subfolders
- Each execution includes:
  - A `.txt` file with the output in a custom format
  - A graph in its written and pdf form in the `pngs/` subfolder
