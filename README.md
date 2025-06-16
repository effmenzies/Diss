# Diss
## 04/06
- Initial meeting

## 12/06
|Topic|Notes|
|-|-|
|Datasets|Find datasets to test models on|
|Research area|Whittle down from parameter count, dealing with small datasets (augmentation methods), explainability|
|Search|Find some papers that do the research area, recent|

### Datasets
- MedMNIST
    - Chest X-Ray
    - Derma Dermatoscope
    - Retina Fundus cam
    - Breast ultrasound? Colon pathology? for additional modality
- SIPaKMeD
    - Pap smear (small set, unbalanced)

### Research area
- Parameter count
    - Better for smaller medical datasets
    - Fewer resources
    - Easier to implement on small devices

### Search
- Transformers
    - ViT
    - MaxCerVixT
- CNNs
    - CNN-LSTM
    - PlexusNet
- Hybrids
    - Spiking attention module
- Pruning
    - Chaos game optimisation
    - Evolutionary pruning + ensemble learning (connection pruning)

- Pruning methods
    - quantisation
    - knowledge distillation
    - low-rank decomposition
    - network pruning
        - filter
        - channel
        - connection

## 18/06
|Topic|Notes|
|-|-|
|Project Plan draft||
|Sections of lit review||
|Test GPU Server||
|Explore datasets||

### Project plan draft

[project plan](projectPlan.docx)

### Sections of lit review
|Header|Content|
|-|-|
|**Intro**|Why need automated diagnosis, current models, limitations of current models, chosen area being addressed|
|**Background** Current architectures|CNN vs Transformer vs Hybrid architectures wrt accuracy, efficiency, and resources|
|**Methodology**|What areas are being compared,what metrics are being used to comapre them: development time and cost; accuracy vs efficiency trade off;
|**Techniques**||
|New architectures|New module designs to improve efficiency and reduce parameter count|
|Pruning methods|Filter, channel, and connection: The differences, compare costs|
|Quantisation|?|
|Knowledge distillation|?|
|**Conclusion**|Best area of research and why, potential current models suitable to look at|

### GPU Server

### Datasets
- Want to add in a 4th\
*is this too many datasets*
    - adding in colon pathology or breast ultrasound introduces more image modalities
    - breast ultrasound dataset is small, maybe good to test the models training with smaller datasets