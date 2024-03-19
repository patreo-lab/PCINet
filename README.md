# PCINet
Código referente ao paper _Automatic mapping of high-risk urban areas for Aedes aegypti infestation based on building facade image analysis_ publicado na PLOS One em 2024.
- ```facades.ipynb```: Notebook principal com o treinamento k-fold e extração de métricas resultado. Treinamento e testes realizados nas fotos tiradas por agentes de saúde pública.
- ```inferencias_5classes.csv```: inferências do PCI 5 classes sobre as fotos dos agentes de saúde (separados por fold).
- ```models/folds.dict```: dicionário com as amostras associadas a cada fold
- ```models/best_fold0*.pt```: modelo treinado em cada um dos folds listados em ```folds.dict```.
- ```results/activations*.pdf```: distribuição de ativações para diferentes cenários (por fold, por classe, etc.)
- ```results/cm_fold0*.pdf```: matrizes de confusão por fold.
- ```streetview/data.ipynb```: exploração de dados das imagens coletadas via streetview e rotuladas por agentes de saúde.
-  ```streetview/inference.ipynb```: **Pipeline de inferência** com os modelos treinados nas fotos dos agentes de saúde, aqui testados nas imagens coletadas do streetview.
- ```streetview/inferences.csv```: inferências com os 5 diferentes modelos sobre as imagens do streetview.
