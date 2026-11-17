# plp-da-a2-rainfall-advisory
# Rainfall Advisory & Planting Window Analysis

### Project Summary
This project cleans, analyzes, and summarizes monthly rainfall data across five Kenyan counties (Nairobi, Nakuru, Kisumu, Mombasa, and Machakos) for a farmer-support NGO. Using Python and NumPy, the pipeline handles manual data-entry errors via exception handling, computes vectorized seasonal metrics, and outputs a structured CSV summary to power targeted SMS planting advisories.

### How to Run
1. Clone this repository or open `rainfall_analysis.ipynb` directly in Google Colab:
   [Open in Colab](https://colab.research.google.com/github/CynthiahL/plp-da-a2-rainfall-advisory/blob/main/rainfall_analysis.ipynb)
2. Install the required dependency (`numpy`) using:
   ```bash
   pip install -r requirements.txt
   ```
3. Run all cells from top to bottom to view the printed diagnostics and regenerate `rainfall_summary.csv`.

### Planting Advisory
* **Universal Peak Planting Window:** All five counties experience their highest two-month consecutive rainfall during **April–May**, making late March to early April the optimal window for seed planting.
* **High-Moisture vs. Arid Zones:** **Kisumu** (1,371 mm/year, 0 dry months) and **Mombasa** (1,085 mm/year, 2 dry months) support full-season crops, whereas **Nairobi** and **Machakos** each face **5 dry months** (< 50 mm) and require drought-tolerant crop varieties.
* **Data Quality Caveat:** Missing manual readings for **Machakos** in April (`"N/A"`) and September (`""`) were imputed using the valid monthly average (**68 mm**), which likely underestimates Machakos's true April rainfall peak.
