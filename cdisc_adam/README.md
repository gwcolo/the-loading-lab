# `adam` README

This folder contains a demo for working with **ADaM (Analysis Data Model)** datasets.  
The data used here comes from the [PHUSE scripts repository](https://github.com/phuse-org/phuse-scripts/tree/master/data/adam), in particular the [`cdiscpilot01`](https://github.com/phuse-org/phuse-scripts/tree/master/data/adam/cdiscpilot01) example.

**I will be using the Updated 2018 Version of the data set at <https://github.com/phuse-org/phuse-scripts/blob/master/data/adam/cdiscpilot_update1.zip>.**

---

## Background

The Clinical Data Interchange Standards Consortium (CDISC) originally published these datasets as part of a **pilot electronic submission package**:  
<http://www.cdisc.org/sdtmadam-pilot-project>  
According to the ADaM-specific README file here: <https://github.com/phuse-org/phuse-scripts/blob/master/data/adam/cdiscpilot01/README.md>
- The complete pilot package is available to CDISC members.  
- Within that archive, the ADaM datasets are located under:  
updated Pilot Submission Package\900172\m5\datasets\cdiscpilot01\analysis\adam\datasets\

I have been able to retrieve the data from the cited CDISC pilot01 resource, but through that this direct reference might help.

For further details, check the `README.md` included with the PHUSE/CDISC data.

---

## Dataset Contents

The demo dataset includes the following files:

- `README.md`  
- `adae.xpt` – Adverse Events Analysis Dataset  
- `adlbc.xpt` – Laboratory Chemistry Analysis Dataset  
- `adlbh.xpt` – Laboratory Hematology Analysis Dataset  
- `adlbhy.xpt` – Laboratory Hy’s Law Analysis Dataset  
- `adqsadas.xpt` – Alzheimer’s Disease Assessment Scale (ADAS) Questionnaire  
- `adqscibc.xpt` – Clinical Global Impression of Change (CGI-C) Questionnaire  
- `adqsnpix.xpt` – Neuropsychological Inventory (NPI-X) Questionnaire  
- `adsl.xpt` – Subject-Level Analysis Dataset  
- `adtte.xpt` – Time-to-Event Analysis Dataset  
- `advs.xpt` – Vital Signs Analysis Dataset  
- `dataguide.pdf` – Data Guide  
- `define-v1-updated-html.xsl` – Define-XML Stylesheet  
- `define.pdf` – Define Document (PDF)  
- `define.xml` – Define-XML Metadata  

---

## Notes

- These files are provided in **XPT (SAS transport) format**, the FDA-required format for regulatory submissions.  
- The demo notebooks will show how to:
1. Load `.xpt` files into Python.  
2. Explore key structures (variables, metadata, relationships).  
3. Make simple plots or summaries.  

---

## How to Use

1. Download the ADaM sample data from the [PHUSE GitHub repository](https://github.com/phuse-org/phuse-scripts/tree/master/data/adam/cdiscpilot01).  
2. Place the files into the `data/raw/` folder.  
3. Use the notebooks in this directory to load and explore the datasets.  

## Downloading the ADaM Data (single folder)

You don’t need to download the entire PHUSE repository — you can grab just the `cdiscpilot01` directory using Subversion (`svn`).

- **macOS**  
  Install Subversion if needed:  
  ```bash
  brew install svn
  ```  
  Then run:  
  ```bash
  svn export https://github.com/phuse-org/phuse-scripts/trunk/data/adam/cdiscpilot01
  ```

- **Windows**  
  1. Download and install [TortoiseSVN](https://tortoisesvn.net/downloads.html).  
  2. In File Explorer, right-click in your target folder and select:  
     **SVN Checkout...**  
  3. Enter this URL:  
     ```
     https://github.com/phuse-org/phuse-scripts/trunk/data/adam/cdiscpilot01
     ```  
  4. Click **OK** — only the `cdiscpilot01` folder will be downloaded.  

---