# Anonymous Text-Simplification Corpus  

This repo contains a tiny **data bundle** and a few supporting notebooks.  
Everything here is referenced in the paper; the README is only for quick
orientation.

---

## 1. Data (`/data`)

| file | what’s inside | columns |
|------|---------------|---------|
| `ground_truth.csv` | human-written simplifications for every sentence | `source`, `level1`, `level2`, `level3` |
| `200_generated*.csv` | model outputs on the **same fixed 200 sentences**<br>pattern:<br>`200_generated[_<model>][_few_shot].csv` | `source`, `level1`, `level2`, `level3` |

---

## 2. Research (`/research`)

- `complexity_analysis.ipynb` – computes classical readability metrics (SMOG, ASL, …) for both ground-truth and model outputs.  
- `few_shot/` & `zero_shot/` – notebooks that produced the corresponding `200_generated*.csv` files.

---