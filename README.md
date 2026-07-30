# Generative AI in Structural Biology

Compares an experimental protein structure (PDB) against its AlphaFold
prediction — Cα distance matrices, per-residue error, contact maps, and
pLDDT-vs-error correlation, visualised with Plotly.

## Installation

```bash
git clone https://github.com/Harshith-Bathula/Generative-AI-in-Structural-Biology.git
cd Generative-AI-in-Structural-Biology
pip install -r requirements.txt
```

## Usage

Open `BioPythonTest.ipynb` and run the cells. Core logic is in the
`ProteinEvaluator` class:

```python
pipeline = ProteinEvaluator(pdb_id="1CRN")
pipeline.fetch_structures()
pipeline.parse_and_align_structures()
pipeline.compute_invariants()
pipeline.generate_visualisations()
```
