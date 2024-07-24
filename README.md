## Machine learning-based models, molecular docking and simulation for the prediction of novel small molecules as potential TGR5 agonists in diabetes treatment

## *Table of Contents
- [Background](#Background)
- [Objectives](#Objectives)
- [Data](#Data)
- [Methods](#Methods)
- [Results](#Results)
- [Conclusion](#Conclusion)
- [Team](#Team)


## *Background
Diabetes is a major health burden worldwide, and the development of novel and effective therapies is crucial for improving patient outcomes.
A promising new class of medications for the management of type 2 diabetes is TGR5 agonists. Since it has been demonstrated that activating TGR5 receptors improves glucose homeostasis and increases energy expenditure, these receptors are an attractive target for diabetes treatment.
The development of novel TGR5 agonists holds great promise for diabetes treatment. These agonists have the potential to not only regulate glucose levels but also address other important aspects of diabetes management, such as body weight and associated complications. In addition, the stimulation of GLP-1 secretion by TGR5 agonists can lead to improved glycemic control through glucose-dependent insulin secretion.

Machine learning has emerged as a powerful tool in medical research, revolutionizing the field by enabling the prediction and diagnosis of various diseases, including diabetes. This has led to significant advancements in the monitoring and treatment of diabetes, allowing for personalized care and improved patient outcomes. By utilizing machine learning techniques, researchers have been able to analyze vast amounts of data related to diabetes, such as genetic information, environmental factors, and health behaviors. These techniques have led to the development of predictive models that can accurately identify individuals at risk for diabetes and provide personalized recommendations for treatment and management. 

Machine learning-based models, molecular docking, and simulation techniques play a crucial role in the prediction of novel small molecules as potential TGR5 agonists in diabetes treatment. These advancements in machine learning have not only improved our understanding of diabetes but have also opened up new possibilities for the development of novel treatments. Machine learning algorithms have been applied to the discovery of potential therapeutic molecules for diabetes treatment. These algorithms have the capability to analyze molecular structures, predict their interactions with target proteins, and identify small molecules that can act as TGR5 agonists, which have shown promising potential for diabetes treatment. By combining machine learning models with molecular docking and simulation techniques we can efficiently screen large libraries of compounds and identify novel small molecules that have the potential to activate TGR5 and contribute to the treatment of diabetes. 


## *Objectives

1. To Develop machine learning models to predict potential TGR5 agonist based on bioactivity data from Chembl
2. Identify lead compounds that could serve as potential drugs; this will be achived by carrying out molecular docking to dtermine the binding affinity of the compound(s) to the target protein.
3. Determine the stability of the binding of the compound(s) to the target protein, through Molecular Dynamics Simulations

## *Data
The data that was used for machine learning modelling in this study was obtained from (https://www.ebi.ac.uk/chembl/g/#search_results/all/query=TGR5). The training dataset used in the study is in (https://www.ebi.ac.uk/chembl/g/#search_results/targets/query=tgr5%0A)



## *Methods
### Workflow
![figures](https://github.com/omicscodeathon/tgr5t2d/blob/main/workflow/TGR5_FlowChart.png)

### 1.Machine Learning


### 2.Molecular Docking 
Molecular docking predicts the preferred orientation of a small molecule to a protein target to form a stable complex.

### 3.Molecular Dynamics Simulation (MDS)
This is a computational method used to examine how atoms and molecules behave over time. Using Newton's equations of motion, MDS determines the stability,  typically tracking the positions and velocities of atoms as they evolve in accordance with classical mechanics. This makes it possible for scientists to look into the atomic-level dynamic features of molecular systems.




## *Results

##Chemical Space Analysis
##Frequency plot of the two bioactivity classes  and scatter plot of MW versus LogP

![figures](https://github.com/omicscodeathon/tgr5t2d/blob/main/figures/Bioactivity%20class.png)

##Box plots of TGR5 agonists using Lipinski's descriptors

![figures](https://github.com/omicscodeathon/tgr5t2d/blob/main/figures/Lipinski.png)


![figures](https://github.com/omicscodeathon/tgr5t2d/blob/main/figures/HBDA.png)

##Scatter Plot of Experimental vs Predicted pEC50 Values (a) and Experimental vs Predicted pEC50 for Training Data (b)

![figures](https://github.com/omicscodeathon/tgr5t2d/blob/main/figures/pEC50graphs.png)

##Predicted binding scores of compounds docked in the TGR5 binding pocket
![figures](https://github.com/omicscodeathon/tgr5t2d/blob/main/figures/TGR5_Docked_scores.png)


## *Conclusion
The findings of the study provide valuable insights into the potential of TGR5 agonists as a novel therapeutic option for the treatment of type 2 diabetes.



## *Team
- Ojochenemi Enejoh (Genomics and Bioinformatics Department, National Biotechnology Development Agency, Abuja, Nigeria) chenemidala@gmail.com
- Hector Nortey norteyhector@gmail.com
- Chinelo Okonkwo  chinokonkwo@gmail.com 
- Oluwasegun Adesina Babaleye olajideolusegun01@gmail.com
- David Olatunji odavididowu@gmail.com
- Olalekan Kemiki kemikio@babcock.edu.ng
- Florence Mbaoji florence.mbaoji@unn.edu.ng
- Abdulrazak Sale abdulsaleyusuf93@gmail.com
- Olaitan I Awe laitanawe@gmail.com
