# TIL6022 – Group 16

**TIL Python Programming**

### Students
- Emma ten Koppel – 5570484  
- Ties Timmerman – 5636965  
- Twan Guleij – 5072530  
- Gijs Bezemer – 5064481  
- Machtelt Boogers – 5416396  

---

 
## **An analysis of the impact of electric vehicles on emission intensity in Dutch road transport**

### Introduction  
This project investigates how the rise of electric passenger cars in the Netherlands between 2018 and 2023 has influenced emissions of CO₂, NOx, and PM₁₀. The electrification of passenger transport plays a key role in achieving climate goals, reducing air pollution, and improving air quality. Using national datasets from the Dutch Central Bureau of Statistics (CBS), the analysis explores how total and per-kilometre emissions have changed in relation to the increasing share of electric vehicles.

The main research question guiding this study is:  
**To what extent has the growth of electric passenger cars in the Netherlands between 2018 and 2023 correlated to changes in CO₂, NOx and PM₁₀ emissions from passenger cars, both in totals and per vehicle-kilometre?**

To answer this, four sub-questions were addressed:  
1. How do CO₂, NOx, and PM₁₀ totals and intensities evolve over 2018–2023?  
2. How does the BEV, FCEV, and PHEV population develop during this period?  
3. How are these vehicle types related to annual emission intensities?  
4. How might continued EV growth affect emission intensity by 2030?

---

### Data Sources  
All data used in this project are publicly available from CBS Open Data and RVO.  
- [Air emissions from road transport in the Netherlands](https://opendata.cbs.nl/#/CBS/nl/dataset/85347NED/table?ts=1760339509512)
- [https://duurzamemobiliteit.databank.nl/mosaic/nl-nl/elektrisch-vervoer/personenauto-s]
- [https://www.cbs.nl/nl-nl/cijfers/detail/85404NED]
These data cover the years 2018 to 2023 and include information on total vehicle kilometres, emissions per pollutant, and EV fleet composition.

---

### Methods and Tools  
All analyses were conducted in Python, using the following libraries:
- pandas, for data import and processing  
- numpy, for numerical operations and correlation analysis  
- plotly.express, for data visualization  
- matplotlib, for static plots  
- re, for text processing and data cleaning  

The datasets were merged and normalized to calculate annual emission intensities (g/km). Pearson’s correlation coefficient was used to assess the relationship between EV share and emission intensity.

---

### How to Run the Analysis  
1. **Download** the project files (`main_analysis.py` or `EV_emissions_analysis.ipynb`).  
2. **Install dependencies** by running:  
   ```bash
   pip install pandas numpy plotly matplotlib
