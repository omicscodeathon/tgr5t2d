## Machine learning-based Models, Molecular Docking and Molecular Dynamics Simulations for the Prediction of Potential TGR5 Agonists in Type 2 Diabetes Treatment

## *Table of Contents
- [Background](#Background)
- [Objectives](#Objectives)
- [Methods](#Methods)
- [Results](#Results)
- [Conclusion](#Conclusion)
- [Team](#Team)


## *Background
Diabetes is a major health burden worldwide, and the development of novel and effective therapies is crucial for improving patient outcomes.
A promising new class of medications for the management of type 2 diabetes is Takeda G Protein-Coupled Receptor 5 (TGR5) agonists. Since it has been demonstrated that activating TGR5 receptors improves glucose homeostasis and increases energy expenditure, these receptors are an attractive target for diabetes treatment.
The development of novel TGR5 agonists holds great promise for diabetes treatment. These agonists have the potential to not only regulate glucose levels but also address other important aspects of diabetes management, such as body weight and associated complications. In addition, the stimulation of glucagon-like peptide 1 secretion by TGR5 agonists can lead to improved glycemic control through glucose-dependent insulin secretion.

Machine learning has emerged as a powerful tool in medical research, revolutionizing the field by enabling the prediction and diagnosis of various diseases, including diabetes. This has led to significant advancements in the monitoring and treatment of diabetes, allowing for personalized care and improved patient outcomes. By utilizing machine learning techniques, researchers have been able to analyze vast amounts of data related to diabetes, such as genetic information, environmental factors, and health behaviors. These techniques have led to the development of predictive models that can accurately identify individuals at risk for diabetes and provide personalized recommendations for treatment and management. 

Machine learning-based models, molecular docking, and simulation techniques play a crucial role in the prediction of novel small molecules as potential TGR5 agonists in diabetes treatment. These advancements in machine learning have not only improved our understanding of diabetes but have also opened up new possibilities for the development of novel treatments. Machine learning algorithms have been applied to the discovery of potential therapeutic molecules for diabetes treatment. These algorithms have the capability to analyze molecular structures, predict their interactions with target proteins, and identify small molecules that can act as TGR5 agonists, which have shown promising potential for diabetes treatment. By combining machine learning models with molecular docking and simulation techniques we can efficiently screen large libraries of compounds and identify novel small molecules that have the potential to activate TGR5 and contribute to the treatment of diabetes. 


## *Objectives

1. To Develop machine learning models to predict potential TGR5 agonist based on bioactivity data from ChEMBL
2. Screen the COC
3. Identify lead compounds that could serve as potential drugs; this will be achieved by carrying out molecular docking to determine the binding affinity of the compound(s) to the target protein.
4. Determine the stability of the binding of the compound(s) to TGR5, through Molecular Dynamics Simulations


## *Methods
### Workflow
![figures](https://github.com/omicscodeathon/tgr5t2d/blob/main/workflow/TGR5_Methods_Flowchart.png)

### 1.Machine Learning
The Jupyter Notebook was used to create and run the machine learning module's code. Bioactivity data was retrieved from the ChEMBL database (https://www.ebi.ac.uk/chembl/)  The data was cleaned and classified as active, intermediate, or inactive. 

The EC50 values were converted into pEC50 measurements, and Lipinski's descriptors were calculated. After the intermediate bioactivity category was removed, only active and inactive compounds were the subject of exploratory data analysis. Data matrices were created in accordance with the fingerprint descriptors produced using PaDEL. The dataset was split in an 80:20 ratio for training and testing after features with low variance were eliminated. Using a random forest algorithm, a regression model was produced, signifying the end of the machine learning training procedure. 

The coconut database (https://coconut.naturalproducts.net/) was screened using the trained model, and the predicted dataset was used to prepare ligands for docking experiments against the  TGR5 protein.


### 2.Molecular Docking 
Molecular docking predicts the preferred orientation of a small molecule to a protein target to form a stable complex. Here, the TGR5 protein was downloadrd from the protein data bank (https://www.rcsb.org/), prepared and used for docking along with the prepared ligands.

### 3.Molecular Dynamics Simulation (MDS)
This is a computational method used to examine how atoms and molecules behave over time. Using Newton's equations of motion, MDS determines the stability,  typically tracking the positions and velocities of atoms as they evolve in accordance with classical mechanics. This makes it possible for scientists to look into the atomic-level dynamic features of molecular systems.




## *Results

## Chemical Space Analysis
## The bioactivity classes are spanning similar chemical spaces as evident by the scatter plot of MW vs LogP
![figures](https://github.com/omicscodeathon/tgr5t2d/blob/main/figures/Bioactivity%20class.png)

## Frequency plot of the two bioactivity classes  and scatter plot of MW versus LogP



![figures](https://github.com/omicscodeathon/tgr5t2d/blob/main/figures/Lipinski.png)

![figures](https://github.com/omicscodeathon/tgr5t2d/blob/main/figures/HBDA.png)
## Box plots of TGR5 agonists using Lipinski's descriptors




![figures](https://github.com/omicscodeathon/tgr5t2d/blob/main/figures/pEC50graphs.png)
## Scatter Plot of Experimental vs Predicted pEC50 Values (a) and Experimental vs Predicted pEC50 for Training Data (b)



![figures](https://github.com/omicscodeathon/tgr5t2d/blob/main/figures/TGR5_Docked_scores.png)
## Predicted binding scores of compounds docked in the TGR5 binding pocket

## *Conclusion
Our study identified four (4) novel molecules, notably, CNP0209363, CNP0424850, CNP0417335 and CNP0224616, as potential TGR5 agonists which may be considered for the treatment of T2D 
The findings of the study provide valuable supporting data for predicting potential TGR5 agonists that combines machine learning-based models, molecular docking, and molecular dynamics simulations, which demonstrate the potential of the proposed approach for predicting novel small molecules as TGR5 agonists. 


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
