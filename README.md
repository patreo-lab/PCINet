# PCINet
Code refering to the paper _Automatic mapping of high-risk urban areas for Aedes aegypti infestation based on building facade image analysis_ (in review - PLOS One 2024)
- ```facades.ipynb```: Main Notebook containing the k-fold training procedure and resulting metrics. The training and testing are performed with the photos taken in place by the public health agents.
- ```inferencias_5classes.csv```: PCI inferences for the photos taken by the agends (separated by fold).
- ```models/folds.dict```: dictionary with the samples associated with each fold.
- ```models/best_fold0*.pt```: models trained with each of the folds listed in ```folds.dict```. 
- ```results/activations*.pdf```: distribution of activations for different scenarios (per fold, per class, etc.).
- ```results/cm_fold0*.pdf```: confusion matrix per fold.
- ```streetview/data.ipynb```: data exploration of the images collected from Google Street View and labeled by public health agents.
-  ```streetview/inference.ipynb```: **Inference Pipeline** with the models trained on top of the photos taken by the agents, here tested with Street View images.
- ```streetview/inferences.csv```: inferences with the 5 diffente models (for each fold) for the Street View images.
