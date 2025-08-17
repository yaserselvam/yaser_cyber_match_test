# Cybersecurity Spend Record Matching – Assessment Submission

This repository contains my completed submission for the **Cybersecurity Spend Record Matching** assessment.  
The goal of this task was to normalize and map raw cybersecurity spend data to a curated product catalog, producing structured and reliable outputs.

---

## 📂 Files in this Repository

- **approach_summary.pdf**  
  A detailed step-by-step explanation of my methodology, covering data preparation, normalization, keyword mapping, and record matching.

- **yaser_matched_spend_records.csv**  
  Full set of matched spend records, including product IDs, names, vendor alignment, and confidence levels.

- **yaser_matched_spend_records_hard.csv**  
  Matched subset of the “hard” spend records provided separately in the assessment.

---

## 🛠️ Approach Overview

1. **Data Preparation**  
   - Cleaned and normalized supplier and text fields (`supplier_norm`, `text_norm`, `text_norm_compact`).  
   - Standardized vendor names into `vendor_norm`.

2. **Keyword Mapping**  
   - Built a `KeywordMapTbl` with canonical product names, vendors, short keys, and priorities.  
   - Added high-value aliases (e.g., *falcon*, *zscaler ia*, *firepower 2000*) to improve matching accuracy.

3. **Matching Logic**  
   - Used a combination of exact matches, compact matches, and manual product keys where required.  
   - Introduced confidence levels (`high`, `medium`, `low`) and a `method` field to indicate whether the match came from keyword search, manual entry, or vendor alignment.

4. **Outputs**  
   - Exported structured CSVs (`matched_spend_records` and `matched_spend_records_hard`).  
   - Ensured consistency in product_id, product_name, vendor_name, and supporting metadata.

---

## ✅ Reproducibility

- All outputs are generated from formula-driven Excel models.  
- The workflow is documented in **approach_summary.pdf** so the process can be replicated or adapted with minimal configuration changes.  
- Vendor and keyword mapping can be extended by editing the `KeywordMapTbl`.

---

## 🚀 How to Use

1. Review **approach_summary.pdf** for methodology.  
2. Open **yaser_matched_spend_records.csv** to see the full matched dataset.  
3. Open **yaser_matched_spend_records_hard.csv** to see the matched subset of harder records.  

---

## Author

**Yaser Selvam**  
📧 yaseruk259@gmail.com  
🔗 [LinkedIn](https://www.linkedin.com/in/yaserselvam) | [GitHub](https://github.com/yaserselvam)
