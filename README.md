<div align="center">
  <img src="static/images/logo.png" alt="ReCamDriving Logo" style="height: 120px; margin-bottom: 5px;" />
  <h1 style="border-bottom: none;">ReCamDriving: LiDAR-Free Camera-Controlled Novel Trajectory Video Generation</h1>
</div>
<div align="center">
  <p>
    <a href="https://iron-lyk.github.io/" target="_blank">Yaokun Li</a><sup>1</sup>,
    <a>Shuaixian&nbsp;Wang</a><sup>1,3</sup>,
    <a href="https://scholar.google.com/citations?user=0_LPgUYAAAAJ&hl=zh-CN" target="_blank">Mantang Guo</a><sup>2</sup>,
    <a href="https://jackailab.github.io/" target="_blank">Jiehui Huang</a><sup>4</sup>,
    <a href="https://openreview.net/profile?id=~Taojun_Ding1" target="_blank">Taojun Ding</a><sup>2</sup>
    <br>
    <a href="https://scholar.google.com.hk/citations?user=Zac1-owAAAAJ&hl=zh-TW" target="_blank">Mu Hu</a><sup>4</sup>,
    <a href="https://scholar.google.com/citations?user=mSyd3BcAAAAJ&hl=zh-CN" target="_blank">Kaixuan Wang</a><sup>2</sup>,
    <a href="https://scholar.google.com/citations?user=u8Q0_xsAAAAJ&hl=zh-CN" target="_blank">Shaojie Shen</a><sup>4</sup>,
    <a href="https://ise.sysu.edu.cn/teacher/TanGuang" target="_blank">Guang Tan</a><sup>1</sup>
  </p>
  <p>
    <sup>1</sup> Sun Yat-sen University &nbsp;&nbsp;
    <sup>2</sup> ZYT &nbsp;&nbsp;
    <sup>3</sup> Shenzhen Polytechnic University &nbsp;&nbsp;
    <br>
    <sup>4</sup> The Hong Kong University of Science and Technology
  </p>
</div>

<p align="center">
  <a href='https://recamdriving.github.io/'><img src='https://img.shields.io/badge/Project-Page-Green'></a>
  &nbsp;
  <a href=""><img src="https://img.shields.io/static/v1?label=Arxiv&message=2512.xxxx&color=red&logo=arxiv"></a>
  &nbsp;
  <a href=''><img src='https://img.shields.io/badge/%F0%9F%A4%97%20Hugging%20Face-Data(soon)-orange'></a>
</p>

***

## 📷 Abstract

We propose **ReCamDriving**, a purely vision-based, camera-controlled novel-trajectory video generation framework. While repair-based methods fail to restore complex artifacts and LiDAR-based approaches rely on sparse and incomplete cues, ReCamDriving leverages dense and scene-complete **3DGS renderings** for explicit geometric guidance, achieving precise camera-controllable generation. To mitigate overfitting to restoration behaviors when conditioned on 3DGS renderings, ReCamDriving adopts a **two-stage training paradigm**: the first stage uses camera poses for coarse control, while the second stage incorporates 3DGS renderings for fine-grained viewpoint and geometric guidance. Furthermore, we present a **3DGS-based cross-trajectory data curation strategy** to eliminate the train–test gap in camera transformation patterns, enabling scalable multi-trajectory supervision from monocular videos. Based on this strategy, we construct the **ParaDrive** dataset, containing over 110K parallel-trajectory video pairs. Extensive experiments demonstrate that ReCamDriving achieves state-of-the-art camera controllability and structural consistency.

<div align="center">
<br>
  <img width="80%" src="assets/teaser.png" alt="ReCamDriving Teaser Image: Comparison of novel-trajectory generation methods">
<br>
</div>

<p align="center"><b>Comparison of novel-trajectory generation.</b> Repair-based methods (e.g., Difix3D+) suffer from severe artifacts under novel viewpoints, while LiDAR-based camera-controlled methods (e.g., StreetCrafter) show geometric inconsistencies in occluded or distant regions due to incomplete cues. In contrast, ReCamDriving employs a coarse-to-fine two-stage training strategy that leverages dense scene-structure information from novel-trajectory 3DGS renderings for precise camera control and structurally consistent generation.</p>

***


## 🌐 ParaDrive Dataset
Based on our data curation strategy, we constructed the **ParaDrive** dataset, which contains **over 110K parallel-trajectory video pairs**, enabling scalable multi-trajectory supervision.

***

## ✅ TODO List
Code and dataset will be made public as soon as possible.
- [x] arXiv paper released.
- [ ] Release Training and Inference code.
- [ ] Release Dataset (ParaDrive).

***

## 🔗 Citation
If you find our work helpful, please consider citing:
```bibtex
@article{li2025recamdriving,
  title={ReCamDriving: LiDAR-Free Camera-Controlled Novel Trajectory Video Generation},
  author={xxx},
  journal={arXiv preprint arXiv:2510.22213},
  year={2025}
}
