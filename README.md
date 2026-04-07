# DENZA Savings Calculator (Australia)

A high-fidelity, interactive web application designed for the Australian automotive market. This tool enables potential customers to compare the annual running costs of traditional Internal Combustion Engine (ICE) vehicles against **DENZA**'s lineup of Pure EV and Super Hybrid (PHEV) models.

## 🚀 Live Demo
[Insert your GitHub Pages link here, e.g., `https://your-username.github.io/denza-calculator/`]

## ✨ Features

* **Real-time Comparisons:** Instant calculation of annual and monthly savings.
* **Dual Mode Support:** Specialized logic for both Pure Electric (EV) and Plug-in Hybrid (PHEV) calculations.
* **Data Grounded:** Pre-loaded with Australian national averages for fuel and electricity from ABS, DISER, and AEMO.
* **Interactive UI:** Dynamic sliders for driving habits and a "Dark Mode" toggle for premium aesthetics.
* **PDF Generation:** Client-side PDF generation (using `jsPDF`) allowing users to download a professional summary of their results.
* **Transparency First:** An integrated "Assumptions & Data Sources" table that cites specific Green Vehicle Guide (GVG) data points.

---

## 📐 Calculation Logic

The tool uses specific formulas to ensure accuracy between different engine types:

### 1. General Metrics
* **Annual Distance ($D$):** $$D = \text{Daily km} \times \text{Days per week} \times 52 \text{ weeks}$$
* **ICE Annual Cost:** $$\text{Annual km} \times \frac{L/100\text{km}}{100} \times \text{Fuel Price}$$

### 2. DENZA Specifics
* **Pure EV (e.g., D9 AWD):** $$\text{Cost} = \frac{\text{Annual km}}{100} \times \text{kWh/100km} \times \text{Elec Price}$$
* **Super Hybrid (PHEV) (e.g., B5, B8):** $$\text{Cost} = \text{Annual km} \times \left( \frac{L/100\text{km}}{100} \times \text{Fuel Price} + \frac{Wh/\text{km}}{1000} \times \text{Elec Price} \right)$$

---

## 🛠️ Technical Stack

* **Frontend:** Semantic HTML5, CSS3 (using CSS Variables for theming).
* **Interactivity:** Vanilla JavaScript (ES6+).
* **Library:** [jsPDF](https://github.com/parallax/jsPDF) for client-side document generation.
* **Design:** Custom "Barlow" and "Barlow Condensed" typography for a modern, automotive-branded feel.

## 📂 Project Structure
```text
├── index.html      # Single-file application containing HTML, CSS, and JS
├── README.md       # Project documentation
```

## 📋 Data Sources
* **Consumption Data:** Green Vehicle Guide (GVG) / MY26 Spec Sheets.
* **Fuel Pricing:** ABS/DISER National Averages (2024).
* **Electricity Pricing:** AEMO National Averages (2024).

---

## 🔧 How to Use
1.  **Clone the repository:**
    ```bash
    git clone https://github.com/your-username/denza-calculator.git
    ```
2.  **Open the file:** Simply open `index.html` in any modern web browser.
3.  **Deployment:** This project is ready for **GitHub Pages**. Just upload the file and enable Pages in the repository settings.

## ⚖️ Disclaimer
This tool provides indicative figures only and does not constitute financial advice. Individual results will vary based on driving conditions, charging behavior, and local utility rates.

---
*Created as a Sales Consultation Tool for DENZA Australia.*
