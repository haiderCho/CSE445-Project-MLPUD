# Exploratory Data Analysis (EDA) Notebook

This contains a comprehensive exploratory data analysis (EDA) pipeline performed using Python. It includes data cleaning, visualization, and preprocessing techniques to better understand the dataset and prepare it for further modeling or analysis.

## 📊 Dataset Overview

- **Initial View:** Display the first few rows to understand the basic structure.
- **Duplicate Removal:** Identifying and removing duplicate rows to reduce redundancy.
- **Missing Values:** Checking for missing values and handling them by imputing with the median.
    

## 📈 Visualization Sections

### Scatter Plots

- **Without Hue:** Basic scatter plots to visualize relationships between pairs of numerical features.
<p float="left">
  <img src="eda/scatter plots (without hue)/CharContinuationRate_vs_DegitRatioInURL.png" width="33%" />
  <img src="eda/scatter plots (without hue)/LetterRatioInURL_vs_DegitRatioInURL.png" width="33%" />
  <img src="eda/scatter plots (without hue)/CharContinuationRate_vs_SpacialCharRatioInURL.png" width="33%" />
</p> 

- **With Hue:** Adds a categorical feature as color to highlight group-wise distributions.
<p float="left">
  <img src="eda/scatter plots (with hue)/CharContinuationRate_vs_URLCharProb.png" width="33%" />
  <img src="eda/scatter plots (with hue)/DomainLength_vs_URLCharProb.png" width="33%" />
  <img src="eda/scatter plots (with hue)/URLCharProb_vs_LetterRatioInURL.png" width="33%" />
</p>



### KDE Plots
KDE plots differentiated by a categorical feature.
  <img src="eda/kde plots/KDE_WithHue.png"/>

  
### Histograms

<p float="left">
  <img src="eda/histogram (with hue)/hist_DomainLength.png" width="33%" />
  <img src="eda/histogram (with hue)/hist_DomainTitleMatchScore.png" width="33%" />
  <img src="eda/histogram (with hue)/hist_LetterRatioInURL.png" width="33%" />
</p> 
<p float="left">
  <img src="eda/histogram (with hue)/hist_NoOfSubDomain.png" width="33%" />
  <img src="eda/histogram (with hue)/hist_NoOfURLRedirect.png" width="33%" />
  <img src="eda/histogram (with hue)/hist_SpacialCharRatioInURL.png" width="33%" />
</p> 
<p float="left">
  <img src="eda/histogram (with hue)/hist_TLDLegitimateProb.png" width="33%" />
  <img src="eda/histogram (with hue)/hist_TLDLength.png" width="33%" />
  <img src="eda/histogram (with hue)/hist_URLCharProb.png" width="33%" />
</p> 


### Boxplot

- Summary of distributions for all numerical features, showing medians, quartiles, and potential outliers.

<p float="left">
  <img src="eda/box plots/boxplot_CharContinuationRate.png" width="33%" />
  <img src="eda/box plots/boxplot_DomainLength.png" width="33%" />
  <img src="eda/box plots/boxplot_LetterRatioInURL.png" width="33%" />
</p>
<p float="left">
  <img src="eda/box plots/boxplot_SpacialCharRatioInURL.png" width="33%" />
  <img src="eda/box plots/boxplot_TLDLength.png" width="33%" />
  <img src="eda/box plots/boxplot_URLCharProb.png" width="33%" />
</p>

### Swarm Plot

- Used to display individual data points along a categorical axis — helps to detect patterns and clusters.
    

### Strip Plot

- Similar to swarm plots but can overlap — great for visualizing dense distributions with less emphasis on separation.
    

### Violin Plot

- Combines boxplot and KDE to give a richer view of the data's distribution and variability.
<p float="left">
  <img src="eda/violin plots/violin_Bank_vs_label.png" width="33%" />
  <img src="eda/violin plots/violin_CharContinuationRate_vs_label.png" width="33%" />
  <img src="eda/violin plots/violin_DomainLength_vs_label.png" width="33%" />
</p>
<p float="left">
  <img src="eda/violin plots/violin_DomainTitleMatchScore_vs_label.png" width="33%" />
  <img src="eda/violin plots/violin_HasCopyrightInfo_vs_label.png" width="33%" />
  <img src="eda/violin plots/violin_HasHiddenFields_vs_label.png" width="33%" />
</p>
<p float="left">
  <img src="eda/violin plots/violin_HasPasswordField_vs_label.png" width="33%" />
  <img src="eda/violin plots/violin_HasSocialNet_vs_label.png" width="33%" />
  <img src="eda/violin plots/violin_HasSubmitButton_vs_label.png" width="33%" />
</p>
<p float="left">
  <img src="eda/violin plots/violin_HasTitle_vs_label.png" width="33%" />
  <img src="eda/violin plots/violin_IsResponsive_vs_label.png" width="33%" />
  <img src="eda/violin plots/violin_LetterRatioInURL_vs_label.png" width="33%" />
</p>
<p float="left">
  <img src="eda/violin plots/violin_NoOfSelfRedirect_vs_label.png" width="33%" />
  <img src="eda/violin plots/violin_NoOfSubDomain_vs_label.png" width="33%" />
  <img src="eda/violin plots/violin_NoOfURLRedirect_vs_label.png" width="33%" />
</p>
<p float="left">
  <img src="eda/violin plots/violin_Robots_vs_label.png" width="33%" />
  <img src="eda/violin plots/violin_SpacialCharRatioInURL_vs_label.png" width="33%" />
  <img src="eda/violin plots/violin_TLDLegitimateProb_vs_label.png" width="33%" />
</p>
<p float="left">
  <img src="eda/violin plots/violin_TLDLength_vs_label.png" width="33%" />
  <img src="eda/violin plots/violin_URLCharProb_vs_label.png" width="33%" />
  <img src="eda/violin plots/violin_URLTitleMatchScore_vs_label.png" width="33%" />
</p>
