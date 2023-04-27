# IRAS_ML_Predictions
This project uses ML to model the interstellar molecular abundances and predict new molecules for detection in source B of the binary Class 0 protostar IRAS 16293-2422. 

In order to predict the column density of a molecule of interest toward IRAS 16293-2422B, you will need to first download the following files:

1) mol2vec_model_final_70.pkl
2) scaler.pkl
3) gpr_model.pkl
4) br_model.pkl
5) main_predictions.ipynb

These should all be saved to the same folder on your device.

The trained mol2vec model file is too large to upload to GitHub. It can be found at https://doi.org/10.5281/zenodo.7869214 

Next you will need to activate an RDKit environment to allow for the RDKit module to be used within a Jupyter notebook. A tutorial for this can be found at the following link (https://depth-first.com/articles/2020/08/17/getting-started-rdkit-and-jupyter/).

Following this, you need to open the main_predictions.ipynb Jupyter notebook and follow the instructions within. In summary, run all import statements and function definitions. Then in the final cell, replace the "smile" input of the getPrediction() function with the SMILES string of the molecule you are interested in and define whether the molecule is a rare isotopologue or not by adjusting the isIso input. Setting isIso = True will denote that the molecule is a rare isotopologue and vice versa. The predicted column density of the molecule will be returned and printed!  

Also contained in this GithHub repository are PDF files that report the predicted column densities of many molecules and rare isotopologues that may be excellent candidates for radioastronomical detection toward IRAS 16293-2422B.

Finally, the remaining folders in the repository contain the files and Jupyter notebooks used to generate the results and Figures displayed in the paper. Several of these notebooks depend on files that are too large to upload to GitHub, including the full dataset of over 3,000,000 SMILES strings and feature vectors. These large files can also be found at https://doi.org/10.5281/zenodo.7869214

If you have questions, feel free to reach out! (zfried@mit.edu)


