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
