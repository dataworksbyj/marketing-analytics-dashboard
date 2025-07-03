# Marketing Campaign Performance & Optimization Case Study

This repository contains an end-to-end analysis of a digital marketing campaign dataset to identify conversion drivers and recommend optimal budget allocations.

## Project Overview

In this case study, we analyze a digital marketing campaign dataset from Kaggle to uncover the key factors driving customer conversions for a mid-sized e-commerce brand. Through exploratory analysis, predictive modeling, and what-if budget simulations, we quantify channel performance, evaluate engagement metrics, and recommend the optimal marketing mix under a fixed budget.

## Objectives

- **Quantify Channel Performance:** Compute CTR, Conversion Rate, Ad Spend and Cost per Acquisition (CPA) for each campaign channel.  
- **Segment Audience Cohorts:** Create demographic (AgeGroup, IncomeBracket) and engagement (EmailEngagementRate, SocialEngagementScore) segments to identify high-value users.  
- **Build & Evaluate Models:** Train and compare Logistic Regression and Random Forest classifiers to predict conversion likelihood and assess feature importance.  
- **Simulate Budget Scenarios:** Develop a simulation function to estimate conversions for different spend allocations and recommend the mix that maximizes ROI under a $50 K budget.  


## Dataset
The dataset is available on Kaggle:
https://www.kaggle.com/datasets/rabieelkharoua/predict-conversion-in-digital-marketing-dataset

## Requirements
Install the required Python packages:
```bash
pip install -r requirements.txt
```

## Notebook
Open and run `marketing_campaign_analysis.ipynb` to perform:
1. Data Loading & Initial Exploration  
2. Data Cleaning & Preprocessing  
3. Exploratory Data Analysis (EDA)  
4. Predictive Modeling (Logistic Regression & Random Forest)  
5. Budget Allocation Simulation & Recommendations  

## Screenshots

### Channel‐Level Performance  
![Channel‐Level Performance: Avg CTR & Conversion Rate](images/channel_level_performance.png)

### IncomeBracket Cohort Analysis  
![IncomeBracket Cohort: Conversion & Engagement](images/income_cohort.png)

## Intereactive Tableau Dashboard

<div class='tableauPlaceholder' id='viz1751573574130' style='position: relative'><noscript><a href='#'><img alt='Marketing Analytics Dashboard ' src='https:&#47;&#47;public.tableau.com&#47;static&#47;images&#47;Ma&#47;MarketingAnalyticsDashboard_17496729206370&#47;Dashboard1&#47;1_rss.png' style='border: none' /></a></noscript><object class='tableauViz'  style='display:none;'><param name='host_url' value='https%3A%2F%2Fpublic.tableau.com%2F' /> <param name='embed_code_version' value='3' /> <param name='site_root' value='' /><param name='name' value='MarketingAnalyticsDashboard_17496729206370&#47;Dashboard1' /><param name='tabs' value='no' /><param name='toolbar' value='yes' /><param name='static_image' value='https:&#47;&#47;public.tableau.com&#47;static&#47;images&#47;Ma&#47;MarketingAnalyticsDashboard_17496729206370&#47;Dashboard1&#47;1.png' /> <param name='animate_transition' value='yes' /><param name='display_static_image' value='yes' /><param name='display_spinner' value='yes' /><param name='display_overlay' value='yes' /><param name='display_count' value='yes' /><param name='language' value='en-US' /></object></div>                <script type='text/javascript'>                    var divElement = document.getElementById('viz1751573574130');                    var vizElement = divElement.getElementsByTagName('object')[0];                    if ( divElement.offsetWidth > 800 ) { vizElement.style.width='1000px';vizElement.style.height='827px';} else if ( divElement.offsetWidth > 500 ) { vizElement.style.width='1000px';vizElement.style.height='827px';} else { vizElement.style.width='100%';vizElement.style.height='1377px';}                     var scriptElement = document.createElement('script');                    scriptElement.src = 'https://public.tableau.com/javascripts/api/viz_v1.js';                    vizElement.parentNode.insertBefore(scriptElement, vizElement);                </script>

**Or view it directly on Tableau Public:**  
[Open the dashboard in a new tab](https://public.tableau.com/views/MarketingAnalyticsDashboard_17496729206370/Dashboard1?:language=en-US&:sid=&:redirect=auth&:display_count=n&:origin=viz_share_link)

## Key Insights
- **Social Media** delivers the highest conversion rate (0.1066) and the lowest cost per acquisition (~$46.6K).  
- **PPC** has the highest click-through rate (0.158) and, when allocated 40% of the budget, maximizes conversions (~38.6 per $50K).  
- **Behavioral Metrics**: TimeOnSite and PagesPerVisit are the strongest predictors of conversion.  
- **Cohort Uniformity**: AgeGroup and IncomeBracket show minimal variation in conversion and engagement metrics.  
- **Model Performance**:  
  - Scaled Logistic Regression: ROC-AUC ≈ 0.78, balanced precision/recall.  
  - Random Forest: ROC-AUC ≈ 0.80, high recall for converters but low recall for non-converters.

## Usage
Adjust budget scenarios in the "Budget Simulation" section of the notebook to test different spend allocations and expected conversion outcomes.
-----

This project is part of a broader portfolio showcasing real-world data analysis. Visit [My GitHub Portfolio](https://github.com/dataworksbyj/real-world-data-case-studies) to explore more case studies.