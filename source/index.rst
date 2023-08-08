.. stGCL_Tutorials documentation master file, created by
   sphinx-quickstart on Tue Aug  1 15:43:58 2023.
   You can adapt this file completely to your liking, but it should at least
   contain the root `toctree` directive.



Welcome to stGCL's documentation!
===================================


Spatial domain identification and multi-slice integration analysis for spatial transcriptomics with multi-modal graph contrastive learning
=====================================================================================================================================================

.. toctree::
   :maxdepth: 1
   
   Installation
   Tutorial 1_Encoding histology image features using H-ViT
   Tutorial 2_10x Visium (DLPFC dataset)
   Tutorial 3_Slide-seqV2 (mouse hippocampus)
   Tutorial 4_Stereo-seq (mouse olfactory bulb)
   Tutorial 5_NanoString CosMx SMI (NSCLC dataset)
   Tutorial 6_Horizontal integration
   Tutorial 7_Vertical integration
   Tutorial 8_Manual region segmentation


.. image:: ../Figures/stGCL.png
   :width: 1400

Overview
========
stGCL is a multi-modal graph contrastive learning framework that integrates transcriptional profiles, histological profiles and spatial information learning the spot joint embedding, enabling spatial domain detection, spatial data integration and downstream analysis. First, stGCL utilizes the proposed H-ViT model to extract the latent representation of each spot image. Then stGCL employs multi-modal graph attention auto-encoder (GATE) and contrastive learning to extract discriminative information from each modality and fuse them efficiently to generate meaningful joint embeddings. Specifically, multi-modal GATE learns spot joint structured embedding by iteratively aggregating gene expression features and histological features from adjacent spots. In contrastive learning, stGCL maximizes the mutual information between each spot joint embedding and the global summary of the graph, which endows the learned joint representation with not only local (spot expression patterns) but also global features (tissue microenvironment patterns). Finally, stGCL offers simple and effective vertical and horizontal integration methods for analyzing multiple tissue slices, which encourages smoothing of adjacent spot features within and across slices and mitigates the batch effect.

Citation
========
Na Yu, Daoliang Zhang, Zhiping Liu, Xu Qiao, Wei Zhang, Chuanyuan Wang, Miao-Qing Zhao, Baoting Chao, Wei Li, Yang De Marinis, and Rui Gao. Spatial domain identification and multi-slice integration analysis for spatial transcriptomics with multi-modal graph contrastive learning. 2023. (submitted).