# Teeth Mold Point Cloud Completion Via Data Augmentation and Hybrid RL-GAN (Official Implementation)

## Abstract

Teeth scans are essential for many applications in orthodontics, where the teeth structures
are virtualized to facilitate the design and fabrication of the prosthetic piece. Nevertheless,
due to the limitations caused by factors such as viewing angles, occlusions, and sensor resolution, the 3D scanned point clouds (PCs) could be noisy or incomplete. Hence, there is a
critical need to enhance the quality of the teeth PCs to ensure a suitable dental treatment.
Toward this end, we propose a systematic framework including a two-step data augmentation (DA) technique to augment the limited teeth PCs and a hybrid deep learning (DL)
method to complete the incomplete PCs. For the two-step DA, we first mirror and
combine the PCs based on the bilateral symmetry of the human teeth and then augment
the PCs based on an iterative generative adversarial network (GAN). Two filters are
designed to avoid the outlier and duplicated PCs during the DA. For the hybrid DL, we
first use a deep autoencoder (AE) to represent the PCs. Then, we propose a hybrid approach
that selects the best completion to the teeth PCs from AE and a reinforcement learning (RL)
agent-controlled GAN. Ablation study is performed to analyze each component’s contribution. We compared our method with other benchmark methods including point cloud
network (PCN), cascaded refinement network (CRN), and variational relational point completion network (VRC-Net), and demonstrated that the proposed framework is suitable for
completing teeth PCs with good accuracy over different scenarios.

## Citation
@article{toscano2023teeth,
  title={Teeth Mold Point Cloud Completion Via Data Augmentation and Hybrid RL-GAN},
  author={Toscano, Juan Diego and Zuniga-Navarrete, Christian and Siu, Wilson David Jo and Segura, Luis Javier and Sun, Hongyue},
  journal={Journal of Computing and Information Science in Engineering},
  volume={23},
  number={4},
  pages={041008},
  year={2023},
  publisher={American Society of Mechanical Engineers}
}
