# `_folder_template` README

This folder is a template for creating new data type demos.  
Each data type should live in its own folder, following this structure for consistency.

---

## Folder Structure

_folder_template/
├── data/
│ └── raw/
│ └── .gitkeep # placeholder (keeps empty folder in git)
├── notebooks/
│ └── .gitkeep # placeholder
├── environment.yml # conda environment for this data type
└── README.md # folder-specific documentation

---

## Notes

- **`data/raw/`**  
  Store raw input files here. Use `.gitkeep` so the folder is tracked even if empty.  

- **`notebooks/`**  
  Place Jupyter notebooks here for loading, explaining, and plotting the data type.  

- **`environment.yml`**  
  A dedicated Conda environment for this data type to avoid conflicts with others.  

- **`README.md`**  
  Customize this file to explain what the demo does:  
  1. What the data format is (e.g., FCS, RNA-seq, microscopy, etc.)  
  2. Any important aspects of the file structure (data + metadata, etc.)  
  3. Simple example plots/analyses.  

---

## How to Use

1. Duplicate this `_folder_template` directory.  
2. Rename it to the new data type (e.g., `rna_seq/`, `mass_spec/`).  
3. Update the `README.md` and `environment.yml` for the new demo.  

