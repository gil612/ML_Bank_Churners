# ML_Bank_Churners
- - - -

The goal of this XML to predict bank’s customers who are likely to drop off.

I used LIME, the acronym for local interpretable model-agnostic explanations, is a technique that approximates any black box machine learning model with a local, interpretable model to explain each individual prediction.
With LIME we can review every instance and look over its attributes and their influences enabling to compare our predictions. On the following I’ll present some samples and their explanations.

In this first sample we have (actual 0, Predicted 0) for an existing customer. The major reason its classified as 0 is because of the attribute “Total_Trans_Ct” and it has the lowest (or most negative) value of weight.


<p align="center">
  <img src="https://github.com/gil612/ML_Bank_Churners/blob/main/Images/LIME%5B0%5D.png" width="600"/>
</p>
Up next we have sample #3: (Actual 0, Predicted: 0.16). Total_Revovlving_Bal, Total_Relationship_Count and Education_Level categorized as Doctorate have negative value and that’s why the selected instance is classified as class 0.  

<p align="center">
    <img src="https://github.com/gil612/ML_Bank_Churners/blob/main/Images/LIME%5B3%5D.png" width="600"/>
</p> 

In sample #7 we have (Actual 1, Predicted: 0.98). The major positive values are Total_Trans_ct, Total_Revolving_Bal, Total_Ct_chng_Q4_Q1 and Total_trans_amt with major positive values and this is good prediction for an attrited customer.
<p align="center">
    <img src="https://github.com/gil612/ML_Bank_Churners/blob/main/Images/LIME%5B7%5D.png" width="600"/>
  </p>
  In sample #34 we have (Actual: 1, Predicted: 0.57) the major attributes are Total_Trans_ct, Total_Revolving_Bal, Total_Ct_chng_Q4_Q1 and Total_trans_amt and Education_Level categorized as College with major positive values and this is good prediction for an attrited customer.
  <p align="center">
     <img src="https://github.com/gil612/ML_Bank_Churners/blob/main/Images/LIME%5B21%5D.png" width="600"/>
    </p>
    In sample #21 we have only one positive value of the attribute “Total_Trans_amt”. Here we have a case of False Positive

![ezcv logo](https://github.com/gil612/ML_Bank_Churners/blob/main/Images/LIME%5B21%5D.png?raw=true)
