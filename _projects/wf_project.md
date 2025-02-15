---
layout: page
title: Quality Assurance Process Automation
description: Conducted at Wells Fargo 
img: assets/img/wf/all_interns_v.jpg
importance: 1
category: work
tags: ["machine learning", spacy, "product management"]
row: 2
---
<div class="post">
  <header class="post-header">
    {% if page.tags %}
    <div class="project-tags">
      {% for tag in page.tags %}
        <span class="tag">{{ tag }}</span>
      {% endfor %}
    </div>
    {% endif %}
    <br>
    <br>
    <link rel="stylesheet" href="style.css">
    <!-- <h1 class="post-title">{{ page.title }}</h1> -->
    <!-- <p class="post-description">{{ page.description }}</p> -->
    
  </header>
</div>

- [Background](#background)
- [Methodology](#methodology)
- [Results](#results)
- [What I Learned](#what-i-learned)

### Background
- My task was to propose an automation strategy for the Validation Quality Assurance (VQA), which:
    - ensure proper data validation process
    - satisfies banking regulations compliance
- VQA entails:
    - taking about 100-300 rows of data checks
    - manually check if each of them satisfy 20 criteria
    - return VQA success / fail

- an example criteria:
<table class="criteria-table">
<tr>
<th>Criteria</th>
<th>Successful Example</th>
<th>Unsuccessful Example</th>
</tr>
<tr>
<td>Frequency Compliance</td>
<td>On a <strong>daily</strong> basis, X database checks the transaction amount of Y database</td>
<td>The interface prevent users from entering improper entries</td>
</tr>
</table>
<br>

### Methodology
- My approach:
    - 10+ surveys with internal staff, learning the cognitive model of completing VQA manually
    - match the model to script, machine learning and pre-trained deep learning models
- Ultimately, I designed three deliverables to present to my manager and the Chief Data Analytics Officer

1. **Automation Analysis**
    - Analyzed the feasability and importance for each criteria's automation
2. **Criteria-wise Automation**
   - Implemented protocols to showcases automation effectiveness
3. **Holistic Automation**
   - Designed hollistic framework and foundation for future full automation of VQA
   - Predict success probability of a check based on historical data
   - Return criteria importance scores

## Results

1. **Automation Analysis**
    - Created comprehensive report on 6 criteria that can be quickly auotmated, 12 criteria that can be partially automated, and two criteria that computational strategies do not have the power to accurately automate yet 
2. **Criteria-wise Automation**
   - Implemented 5 protocols backed by script, linear regression, XGBoost and Name Entity Recognition (NER)
   - On average, automated 83% of VQA
3. **Holistic Automation**
   - Conducted data preparating through feature engineering, Word2Vec mapping, addressing imbalanced dataset (oversampling and creating synethetic training data using SMOTE) 
   - Trained XGBoost Classifier, reaching 94% accuracy
   - Created data pipeline suggestions for future complete automation

```
Deployed at my department, actively automating 20% of VQA right now!
```

## What I Learned
In terms of technical skills, I learned many [spaCy](https://spacy.io/) techniques such as NER, rule-based matching, and part-of-speech dependency visualizations. 

More broadly, though, I learned how to scope out my own project. The entire process of figuring out how to take an idea to a finished product was very rewarding. I practiced designing a solution that aligns with business objectives while balancing diverse stakeholder interests.
