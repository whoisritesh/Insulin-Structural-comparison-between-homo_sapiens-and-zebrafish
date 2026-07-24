# Insulin-Structural-comparison-between-homo_sapiens-and-zebrafish
This project presents an in silico comparative analysis of the primary hormone Insulin between Homo sapiens (Human) and Danio rerio (Zebrafish). 
# Structural and Evolutionary Analysis of Preproinsulin Across Vertebrates (Human vs. Zebrafish)

![3D Structural Alignment](results/3d_structure_alignment/rcsb_3d_superposition.png)

## 📌 Project Overview
This project presents an *in silico* comparative analysis of the primary hormone **Insulin** between **Homo sapiens (Human)** and **Danio rerio (Zebrafish)**. 

The investigation combines sequence homology searches (**NCBI BLASTp**), structural predictions (**AlphaFold DB**), and 3D spatial superimposition (**RCSB PDB Pairwise Alignment**) to evaluate how evolutionary divergence affects 3D tertiary protein folding over 400+ million years.

---

## 🧬 Primary Sequence & Target Metadata

| Feature | Human Target | Zebrafish Target |
| :--- | :--- | :--- |
| **Organism** | *Homo sapiens* | *Danio rerio* |
| **UniProt ID** | `P01308` | `O73727` |
| **AlphaFold ID** | `AF-P01308-F1` | `AF-O73727-F1` |
| **Protein Name** | Insulin Precursor (Preproinsulin) | Preproinsulin b |
| **Sequence Length** | 110 amino acids | 108 amino acids |

---

## 🔬 Experimental Workflow & Methodology

```text
1. Sequence Data Mining (UniProtKB)
   └── Retrieved human (P01308) and zebrafish (O73727) preproinsulin records.

2. Sequence Homology Search (NCBI BLASTp)
   └── Queried human preproinsulin against RefSeq Danio rerio (taxid:7955).

3. 3D Structural Modeling & Retrieval (AlphaFold DB)
   └── Extracted full 3D coordinate PDB models for both targets.

4. Structural Superposition & Alignment (RCSB PDB TM-align)
   └── Conducted pairwise 3D alignment to extract RMSD, TM-score, and superposed coordinates.



# Structural and Evolutionary Analysis of Preproinsulin Across Vertebrates (Human vs. Zebrafish)

![3D Structural Alignment](rcsb_3d_superposition.png)

## 📌 Project Overview
This project presents an *in silico* comparative analysis of the primary hormone **Insulin** between **Homo sapiens (Human)** and **Danio rerio (Zebrafish)**. 

The investigation combines sequence homology searches (**NCBI BLASTp**), structural predictions (**AlphaFold DB**), and 3D spatial superimposition (**RCSB PDB Pairwise Alignment**) to evaluate how evolutionary divergence affects 3D tertiary protein folding over 400+ million years.

---

## 🧬 Primary Sequence & Target Metadata

| Feature | Human Target | Zebrafish Target |
| :--- | :--- | :--- |
| **Organism** | *Homo sapiens* | *Danio rerio* |
| **UniProt ID** | `P01308` | `O73727` |
| **AlphaFold ID** | `AF-P01308-F1` | `AF-O73727-F1` |
| **Protein Name** | Insulin Precursor (Preproinsulin) | Preproinsulin b |
| **Sequence Length** | 110 amino acids | 108 amino acids |

---

## 🔬 Experimental Workflow & Methodology

1. **Sequence Data Mining (UniProtKB):** Retrieved human (`P01308`) and zebrafish (`O73727`) preproinsulin records.
2. **Sequence Homology Search (NCBI BLASTp):** Queried human preproinsulin against RefSeq *Danio rerio* (taxid: 7955).
3. **3D Structural Modeling & Retrieval (AlphaFold DB):** Extracted full 3D coordinate PDB models for both targets.
4. **Structural Superposition & Alignment (RCSB PDB TM-align):** Conducted pairwise 3D alignment to extract RMSD, TM-score, and superposed coordinates.

---

## 📊 Results & Key Findings

### 1. Sequence Level Divergence (NCBI BLASTp)
* **Query Coverage:** 76%
* **E-value:** $2 \times 10^{-23}$
* **Percent Identity:** **53.57%** (Preproinsulin b, `NP_001034153.1`) / **48.89%** (`NP_571131.1`)
* **Observation:** Approximately $46\% - 51\%$ of amino acid residues have mutated since the mammalian-teleost evolutionary split. However, all **Cysteine (C)** residues involved in disulfide bridging are 100% conserved.

---

### 2. 3D Structural Superposition Metrics (RCSB PDB TM-align)
*Data extracted from `structure.json`:*

| Metric | Measured Value | Biological Interpretation |
| :--- | :--- | :--- |
| **Global RMSD** | **4.66 Å** | Driven by flexible C-peptide linker loops flaring outward. |
| **TM-score** | **0.42** | Reflects divergence in non-functional precursor regions. |
| **Aligned Core Residues** | **61 / 110 residues** | Represents the core mature A and B chains. |
| **Sequence Identity in 3D Core**| **36%** | Structural homology preserved across active binding regions. |

---

## 💡 Biological Conclusion
1. **Precursor Plasticity:** The overall RMSD ($4.66\,\text{Å}$) is elevated due to the **C-peptide and signal peptide regions**, which act as flexible linker loops and are cleaved off during post-translational processing inside the cell.
2. **Core Fold Conservation:** The 3D superposition tool successfully isolated a **61-residue structural core** corresponding to the mature A and B chains. 
3. **Evolutionary Constraint:** Despite $>50\%$ sequence divergence over evolutionary time, the spatial geometry of the **alpha-helical framework** and **disulfide bonds** remains structurally conserved to maintain insulin receptor binding capabilities.

---

## 📁 Repository Outputs & Data Files

* `raw_human_insulin.fasta`: Primary sequence file for `P01308`.
* `blast_results.csv`: Complete NCBI BLAST search output table.
* `alignment.fasta`: Structural sequence alignment exported from RCSB PDB.
* `structure.json`: Raw alignment metrics exported from RCSB PDB API.
* `transformed_structures.zip`: Superimposed 3D atomic coordinates.

---

## 📜 License
Distributed under the **MIT License**. Free for educational and research use.
