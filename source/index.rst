.. stGCL_Tutorials documentation master file, created by
   sphinx-quickstart on Tue Aug  1 15:43:58 2023.
   You can adapt this file completely to your liking, but it should at least
   contain the root `toctree` directive.



Welcome to stGCL's documentation!
===================================


stGCL: A versatile spatial transcriptomics cross-modality fusion method based on multi-modal graph contrastive learning for spatial transcriptomics
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
stGCL is a graph contrastive learning-based cross-modality fusion model that incorporates transcriptional profiles, histological profiles and spatial information to learn the spot joint embedding, enabling spatial domain detection, multi-slices integration and downstream comparative analysis. stGCL utilizes a novel H-ViT method to extract the latent representation of each spot image. Then stGCL employs multi-modal graph attention auto-encoder (GATE) and contrastive learning to extract discriminative information from each modality and fuse them efficiently to generate meaningful joint embeddings. Specifically, multi-modal GATE learns spot joint structured embedding by iteratively aggregating gene expression features and histological features from adjacent spots. In contrastive learning, stGCL maximizes the mutual information between each spot joint embedding and the global summary of the graph, which endows the learned joint representation with not only local (spot expression patterns) but also global features (tissue microenvironment patterns). Furthermore, with a pioneering spatial coordinate correcting and registering strategy, stGCL can precisely identify cross-sectional domains while reducing batch effects.

Citation
========
Na Yu, Daoliang Zhang, Wei Zhang, Zhiping Liu, Xu Qiao, Chuanyuan Wang, Miaoqing Zhao, Baoting Chao, Wei Li, Yang De Marinis, and Rui Gao. stGCL: A versatile spatial transcriptomics cross-modality fusion method based on multi-modal graph contrastive learning for spatial transcriptomics. 2023. (submitted).
