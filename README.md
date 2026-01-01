# Unsupervised Model Selection for Object Detection
Implementation of Flatness Index Score (FIS) by Yu et al (2024) found at https://github.com/HenryYu23/DAS.  The metric has been updated to save a checkpoint with the best FIS during training.  Implemented with the ALDI framework by Kay et al (2025) for unsupervised domain adaptation (UDA) for object detection 

### How to use
The code is written to be used with domain adaptation object detection code base found at https://github.com/justinkay/aldi from the ALDI++ paper.  See reference below.

After installing the aldi github repository, c the model_selection directory to the top directory.  

tools/train_net.py provides an example of using the model selection metric in a training script.  It behaves in the same way as the checkpoint using AP50 to save the best model.

### References

Justin Kay, Timm Haucke, Suzanne Stathatos, Siqi Deng, Erik Young, Pietro
Perona, Sara Beery, and Grant Van Horn. Align and Distill: Unifying and
Improving Domain Adaptive Object Detection. Transactions on Machine
Learning Research, 2025. ISSN 2835-8856.

Hengfu Yu, Jinhong Deng, Wen Li, and Lixin Duan. Towards Unsupervised Model
Selection for Domain Adaptive Object Detection. In The Thirty-eighth Annual
Conference on Neural Information Processing Systems, 2024.
