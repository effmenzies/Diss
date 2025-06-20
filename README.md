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
|Project Plan draft|send draft on monday - brief, not in details|
|Sections of lit review|start writing just to get going|
|Test GPU Server|look at instructions again - been updated|
|Explore datasets|can use 4 - all good|

### Project plan draft
|Area|Papers|Strengths|Limitations|
|-|-|-|-|
|Pruning existing models||Reducing parameters of pre-trained models improves performance and reduces size|Requires a pre-trained model, pre-trained models designed for imagenet are over-parameterised for specific medical datasets|
|SNNs||Highly efficient, accurate, fewer energy resources|Hardware limitations, limited to 128x128, more complex models require more advnaced neuromorphic chips|
|New architectures|Plexus|Massive reduction in parameters, comparable performance|Different blocks for different image modalities, data driven - relies on accuracy of data and labels|

### Sections of lit review
|Header|Content|
|-|-|
|**Intro**|Why need automated diagnosis, current models, limitations of current models, chosen area being addressed|
|**Background** Current architectures|CNN vs Transformer vs Hybrid architectures wrt accuracy, efficiency, and resources|
|**Methodology**|What areas are being compared,what metrics are being used to comapre them: development time and cost; accuracy vs efficiency trade off;
|**Techniques**||
|New architectures|New module designs to improve efficiency and reduce parameter count|
|Spiking networks|Implementation of SNNs for energy efficiency|
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
- should i also use multiple resolutions to see how scalable models are with input?
