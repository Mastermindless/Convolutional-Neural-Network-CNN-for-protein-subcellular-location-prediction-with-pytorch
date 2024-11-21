# Exam SIB course: 
## Diving into deep learning - theory and applications with PyTorch 
### Martin Schwill, martin.schwill@uzh.ch
### date: 2024-Nov-08

## Summary

This Jupyter notebook implements and trains a Convolutional Neural Network (CNN) for protein subcellular location prediction with pytorch. It leverages the code from `04_chest_Xray_CNN.ipynb` notebook to achieve similar or better performance compared to Feedforward Neural Network (FFN) with flattening layer from the `02_protein_subcellular_localisation_classifier.ipynb` notebook.

The CNN architecture has been optimized to prioritize the first 150 positions (rows) of the input data, as protein translocation signals are often located at the N-terminus. To achieve this, additional layers were incorporated into the network. This focused approach resulted in improved validation accuracy compared to a model that did not specifically target this region. Dropout regularization could be considered as an alternative approach to further enhance the model's performance and prevent overfitting.

**Resources:**

* Main repository: https://github.com/sib-swiss/pytorch-practical-training
* Protein subcellular localization classifier notebook: https://github.com/sib-swiss/pytorch-practical-training/blob/master/02_protein_subcellular_localisation_classifier.ipynb
* Chest X-ray CNN notebook (reference for implementation): https://github.com/sib-swiss/pytorch-practical-training/blob/master/04_chest_Xray_CNN.ipynb
