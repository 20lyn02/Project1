
<h1>Workforce Restructuring with Predictive Analytics & Optimization</h1>

<h2>Description</h2>
This project was based on the INSEAD case Integration Planning at SFB (A), where Big American Pharmaceuticals (BAP) acquired Société Française de Biotechnologie (SFB). As part of the integration, the Lyon office was to be closed, requiring at least €3 million in salary savings and 40 voluntary employee departures under France’s rupture conventionnelle collective (RCC) framework. The challenge was to design a data-driven restructuring strategy that balanced cost savings, legal compliance, and fairness.
<br />


<h2>Languages and Utilities Used</h2>

- <b>Python</b> 
- <b>Supervised Machine Learning (Tree Based Models)</b>
- <b>Excel Solver</b>
- <b>Data Ethics & Fairness Assessment</b>


<h2>Methodology</h2>

1. <b>Prediction Model</b>  
   Trained machine learning models (e.g., Gradient Boosting) on historical attrition data to estimate the probability of employees accepting an RCC. Validated model choice and analysed feature importance such as overtime status, tenure, and salary.  

2. <b>Attrition Forecasting</b>  
   Applied the trained model to the Lyon office dataset to generate RCC acceptance likelihoods. Results were saved as <code>attrition_prediction.csv</code>.  

3. <b>Group Formation</b>  
   Designed an algorithm to create “objective” non-discriminatory employee groups. Groups were first split by department (HR, Sales, R&D), then subdivided using key features such as overtime status and tenure. Group sizes were kept between 5–20 employees to balance control and fairness.  

4. <b>Cost Optimisation</b>  
   Built an Excel Solver model to minimise severance costs under the following constraints:  
   - ≥ €3M annual salary savings  
   - ≥ 40 employees leaving  
   - ≥ 80% of employees retained in each department  
   Decision variables represented whether or not to offer RCCs to each group.  

5. <b>Evaluation</b>  
   Assessed model assumptions and limitations, including uncertainty in predictions and peer effects. Checked groups for proportional representation to mitigate risks of indirect discrimination.  


<h2>Findings</h2>

- The <b>Gradient Boosting model</b> delivered the strongest predictive performance.  
- <b>Overtime</b> and <b>tenure</b> were the most influential factors in RCC acceptance.  
- Employees working overtime showed significantly higher probabilities of leaving.  
- Optimal group sizes of 6–10 employees provided a balance between fairness and manageability.  
- Solver optimisation successfully reduced costs but struggled to meet all departmental retention constraints simultaneously.  
- Overall, the integrated <b>prediction + optimisation framework</b> offered a transparent, adaptable, and fairer approach to workforce restructuring compared to manual or subjective decision-making.  

