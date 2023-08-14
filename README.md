[![LinkedId][linkedin-shield]][linkedin-url]

 &nbsp;&nbsp;
 <div style="background: #6acc64; border-radius:30px; padding:10px"><h1 style="text-align: center; color:white; " class="list-group-item list-group-item-action active">LOAN DEFAULTERS PREDICTION WITH MACHINE LEARNING</h1>
 <h4 style="text-align: center; color:white; " class="list-group-item list-group-item-action active">Detecting default borrowers before it happens, reduce risk of loss from loans</h4>

 <p style="text-align: center; color:white; font-style: italic;">Ahmad Hafizh</p>
 <p style="text-align: center; color:white; font-style: italic;">RMT-20-FTDS</p>
</div>

&nbsp;&nbsp;&nbsp;
# Utilities
![Python](https://img.shields.io/badge/python-3670A0?style=for-the-badge&logo=python&logoColor=ffdd54)
![scikit-learn](https://img.shields.io/badge/scikit--learn-%23F7931E.svg?style=for-the-badge&logo=scikit-learn&logoColor=white)
![Jupyter Notebook](https://img.shields.io/badge/jupyter-%23FA0F00.svg?style=for-the-badge&logo=jupyter&logoColor=white)
![Kaggle](https://img.shields.io/badge/Kaggle-035a7d?style=for-the-badge&logo=kaggle&logoColor=white)

### What you can find in this notebook.
<ul style="list-style-type:none;">
</li>
<li><p class="list-group-item list-group-item-action" data-toggle="list" href="#1" role="tab"
        aria-controls="settings">1. Introduction</p>
</li>
<li><p class="list-group-item list-group-item-action" data-toggle="list" href="#2" role="tab"
        aria-controls="settings">2. Preparation</p>
</li>
<li><p class="list-group-item list-group-item-action" data-toggle="list" href="#3" role="tab"
        aria-controls="settings">3. Analysis</p>
</li>
<li><p class="list-group-item list-group-item-action" data-toggle="list" href="#4" role="tab"
        aria-controls="settings">4. Feature Engineering</p>
</li>
<li><p class="list-group-item list-group-item-action" data-toggle="list" href="#5" role="tab"
        aria-controls="settings">5. Creating Models</p>
</li>
<li><p class="list-group-item list-group-item-action" data-toggle="list" href="#6" role="tab"
        aria-controls="settings">6. Conclusion</p>
</li>
 </ul>

&nbsp;&nbsp;&nbsp;
# About the project
Loans, the term refers to a type of credit vehicle in which a sum of money is lent to another party in exchange for future repayment of the value. The lender, usually a financial institution, advances a sum of money to the borrower. In return, the borrower agrees to a certain set of terms including any finance charges, interest, repayment date, and other conditions. In some cases, the lender may require collateral to secure the loan and ensure repayment.

This study aims to gain insight of what causes the client to have defaulted their current installments which can be used to determine actions for future borrowers, and to generate a model able to detect which client have high probability to default. In other words, we want understand what are the causes that drive borrowers to default and therefore predict probable defaulters. This model can increase the company risk assessment capability and may reduce losses from loan department.

Several consideration were taken during the data exploration. The columns with high missing value were dropped, the previous application dataset were not used to create current version of the model, and there are many columns that do not have significant relevance to the default status. After doing feature engineering, handling some outliers, missing values, and created custom imputer, the model was then created using six classification algorithm from scikit-learn library to find the best result. The defaulters F1 score will be the main benchmark to detemine which model is the best. The current state of the data yield high imbalance that is only 8.1% of the data is a default. We resorted to balancing by increasing the amount of default entries using SMOTENC algorithm.

&nbsp;&nbsp;&nbsp;
# Conclusions
The final f1 score for the current made model is 17% with 43% recall and just a 10% precision. This means that the model perdicted over 20000 borrowers will default but actually only 10% of those is right and the right predicted defaulters are only 43% of the total customers that actually defaults. The dataset of loan defaulters having over 124 type of customer and a previous loan history, give an overall ambiguous reasons why the borrowers defaulted. Currently no features that have significant impact to the defaulting clients have been found. We get 33 correlated features from statistical testing and data visualization. This might explain why the model is having a hard time training and predicting the correct value.

> The model that has been generated only usable for demo purpose only, not for predicting defaulters in real application. This is because with a very low f1 score, the true values it predicts are fewer than the wrong values by a significant amount. The precision is so low that only 10% of the predicted data is actually correct and all the correct prediction only acounts for 43% of all the defaulters.


&nbsp;&nbsp;&nbsp;
# Check out other reference
[![Canva][canva-shield]][canva-url] 

[![Tableu][tableu-shield]][tableu-url] `Unfinished`




[linkedin-shield]: https://img.shields.io/badge/-LinkedIn-black.svg?style=for-the-badge&logo=linkedin&colorB=555
[linkedin-url]: https://www.linkedin.com/in/ahmad-hafizh-assegaf/
[canva-shield]: https://img.shields.io/badge/Canva-%2300C4CC.svg?style=for-the-badge&logo=Canva&logoColor=white
[canva-url]: https://www.canva.com/design/DAFrWn64tv8/DoejfThw0ovKkpO7wvuOpg/edit?utm_content=DAFrWn64tv8&utm_campaign=designshare&utm_medium=link2&utm_source=sharebutton

[tableu-shield]: https://img.shields.io/badge/Tableau-E97627?style=for-the-badge&logo=Tableau&logoColor=white
[tableu-url]: https://public.tableau.com/views/LoanDefaulters_16919738253650/DraftLoanDefaulters?:language=en-US&:display_count=n&:origin=viz_share_link

