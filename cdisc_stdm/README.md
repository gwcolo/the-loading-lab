# `sdtm` README

This folder contains a demo for working with **SDTM (Study Data Tabulation Model)** datasets.  
The data used here comes from the [PHUSE scripts repository](https://github.com/phuse-org/phuse-scripts/tree/master/data/sdtm), in particular the [`cdiscpilot01`](https://github.com/phuse-org/phuse-scripts/tree/master/data/sdtm/cdiscpilot01) example.

**Note: I'm using the updated 2018 version avaialble at: <https://github.com/phuse-org/phuse-scripts/blob/master/data/sdtm/cdiscpilot_update2.zip>.**

---

## Background

The Clinical Data Interchange Standards Consortium (CDISC) originally published these datasets as part of a **pilot electronic submission package**:  
<http://www.cdisc.org/sdtmadam-pilot-project>  

- The complete pilot package is available to CDISC members.  
- Within that archive, the SDTM datasets are located under:  
  ```
  updated Pilot Submission Package\900172\m5\datasets\cdiscpilot01\tabulation\sdtm\datasets\
  ```  

For further details, check the `README.md` included with the PHUSE/CDISC data.

---

## Dataset Contents

The demo dataset includes the following files:

- `ae.xpt` – Adverse Events  
- `blankcrf.pdf` – Blank Case Report Form  
- `cm.xpt` – Concomitant Medications  
- `define-v1-updated-html.xsl` – Define-XML Stylesheet  
- `define.pdf` – Define Document (PDF)  
- `define.xml` – Define-XML Metadata  
- `dm.xpt` – Demographics  
- `ds.xpt` – Disposition  
- `ex.xpt` – Exposure  
- `lb.xpt` – Laboratory  
- `mh.xpt` – Medical History  
- `qs.xpt` – Questionnaires  
- `relrec.xpt` – Related Records  
- `sc.xpt` – Subject Characteristics  
- `se.xpt` – Study Events  
- `suppae.xpt` – Supplemental Adverse Events  
- `suppdm.xpt` – Supplemental Demographics  
- `suppds.xpt` – Supplemental Disposition  
- `supplb.xpt` – Supplemental Laboratory  
- `sv.xpt` – Subject Visits  
- `ta.xpt` – Trial Arms  
- `te.xpt` – Trial Elements  
- `ti.xpt` – Trial Inclusion/Exclusion Criteria  
- `ts.xpt` – Trial Summary  
- `tv.xpt` – Trial Visits  
- `vs.xpt` – Vital Signs  

---

## Notes

- These files are provided in **XPT (SAS transport) format**, the FDA-required format for regulatory submissions.  
- The demo notebooks will show how to:
  1. Load `.xpt` files into Python.  
  2. Explore key structures (variables, metadata, relationships).  
  3. Make simple plots or summaries.  

---

## How to Use

1. Download the SDTM sample data from the [PHUSE GitHub repository](https://github.com/phuse-org/phuse-scripts/tree/master/data/sdtm/cdiscpilot01).  
2. Place the files into the `data/raw/` folder.  
3. Use the notebooks in this directory to load and explore the datasets.  


---

## Downloading the SDTM Data (single folder)

You don’t need to download the entire PHUSE repository — you can grab just the `cdiscpilot01` directory using Subversion (`svn`).

- **macOS**  
  Install Subversion if needed:  
  ```bash
  brew install svn
  ```  
  Then run:  
  ```bash
  svn export https://github.com/phuse-org/phuse-scripts/trunk/data/sdtm/cdiscpilot01
  ```

- **Windows**  
  1. Download and install [TortoiseSVN](https://tortoisesvn.net/downloads.html).  
  2. In File Explorer, right-click in your target folder and select:  
     **SVN Checkout...**  
  3. Enter this URL:  
     ```
     https://github.com/phuse-org/phuse-scripts/trunk/data/sdtm/cdiscpilot01
     ```  
  4. Click **OK** — only the `cdiscpilot01` folder will be downloaded.  