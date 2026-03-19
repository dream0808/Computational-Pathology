# 多条件病理图像理解与生成

## 四个关键领域

- 图像生成
- 文本生成
- 分子轮廓-形态学生成
- 其他专业生成应用

## 技术范式与演进

- GAN(生成对抗网络)
- VAE(变分自编码器)
- 扩散模型
- 大语言模型/多模态大模型(LLM/VLM)
- ## 生成任务

   根据生成目标将现有工作分为六个子任务

  - 用于数据增强的合成图像生成（有条件和无条件）
  - 掩模引导生成以实现结构保真度
  - 伪影恢复，用于去除伪影并提高图像质量
  - 高分辨率/多分辨率生成，包括跨尺度图像和十亿像素全幻灯片生成
  - 根据诊断描述或提示生成文本到图像
  - 用于标准化和转移的染色风格生成

  1. synthetic image generation for data augmentation (conditional and unconditional)
  2. mask-guided generation for structural fidelity
  3. artifact restoration for removing artifacts and improving image quality
  4. high/multiple-resolution generation,including cross-scale images and gigapixel whole-slide generation
  5. text to image generation from diagnostic descriptions or prompts
  6. stain style generation for normalization and transfer

  

## Models

### VAE-based

| Model | Year | Link                             |
| ----- | ---- | -------------------------------- |
| VAE   | 2014 | https://arxiv.org/pdf/1505.04597 |

### GAN-based

| Model    | Year | Link                             |
| -------- | ---- | -------------------------------- |
| GAN      | 2014 | https://arxiv.org/pdf/1406.2661  |
| cGAN     | 2014 | https://arxiv.org/pdf/1411.1784  |
| Pix2Pix  | 2016 | https://arxiv.org/pdf/1611.07004 |
| CycleGAN | 2017 | https://arxiv.org/pdf/1703.10593 |
| StyleGAN | 2018 | https://arxiv.org/pdf/1812.04948 |

### Diffusion-based

| Model                         | Year | Link                             |
| ----------------------------- | ---- | -------------------------------- |
| DDPM                          | 2020 | https://arxiv.org/pdf/2006.11239 |
| DDIM                          | 2020 | https://arxiv.org/pdf/2010.02502 |
| Score-based Generative Models | 2020 | https://arxiv.org/pdf/2011.13456 |

### LLM/VLM-based

| Model        | Year | Link |
| ------------ | ---- | ---- |
| ChatGPT      |      |      |
| LLaVA        |      |      |
| TraP-VQA     |      |      |
| Med-PaLM M   |      |      |
| LLaVA-M      |      |      |
| Quilt-LLaVA  |      |      |
| HistoGPT     |      |      |
| PathCHAT     |      |      |
| PathologyVLM |      |      |
| TopoFM       |      |      |

### Other

| Model      | Year | Link                             |
| ---------- | ---- | -------------------------------- |
| PathoDuet  | 2023 | https://arxiv.org/pdf/2312.09894 |
| mSTAR      | 2024 | https://arxiv.org/pdf/2407.15362 |
| SlideSeek  | 2025 | https://arxiv.org/pdf/2506.20964 |
| PathFinder | 2025 | https://arxiv.org/pdf/2502.08916 |

## Datasets

### 1.Real-World Benchmark Datasets

#### A. Segmentation & Detection

| Dataset    | Organ    | Modality | Stain Type | Size          | Source                                                       |
| ---------- | -------- | -------- | ---------- | ------------- | ------------------------------------------------------------ |
| Camelyon16 | Breast   | WSI      | H&E        | 400 WSIs      | https://camelyon16.grand-challenge.org/                      |
| CoNIC      | Colon    | Patch    | H&E        | 4981 images   | https://conic-challenge.grand-challenge.org/                 |
| CoNSeP     | Colon    | Patch    | H&E        | 41 images     | https://opendatalab.com/OpenDataLab/CoNSeP                   |
| DigestPath | Multiple | Patch    | H&E        | 1559 images   | https://digestpath2019.grand-challenge.org                   |
| Glas       | Multiple | Patch    | H&E        | 165 images    | https://www.kaggle.com/datasets/sani84/glasmiccai2015-gland-segmentation |
| Lizard     | Colon    | Patch    | H&E        | 495179 nuclei | https://www.kaggle.com/datasets/aadimator/lizard-dataset     |
| MoNuSeg    | Multiple | Patch    | H&E        | 29000 nuclei  | https://monuseg.grand-challenge.org/                         |
| PanNuke    | Multiple | Patch    | H&E        | 7901 images   | https://huggingface.co/datasets/RationAI/PanNuke             |
| TUPAC      | Breast   | WSI      | H&E        | 573 cases     | https://tupac.grand-challenge.org                            |

#### B. Classification

| Dataset         | Organ    | Modality   | Stain Type | Size          | Source                                           |
| --------------- | -------- | ---------- | ---------- | ------------- | ------------------------------------------------ |
| BACH            | Breast   | Patch, WSI | H&E        | 400+ images   | https://zenodo.org/records/3632035               |
| BreakHis        | Breast   | Patch      | H&E        | 9709 images   | https://web.inf.ufpr.br/vri/databases/breakhis   |
| Camelyon17      | Breast   | WSI        | H&E        | 1399 WSIs     | https://camelyon17.grand-challenge.org/          |
| LC25000         | Multiple | Patch      | H&E        | 25000 images  | https://huggingface.co/datasets/1aurent/LC25000  |
| NCT-CRC-HE-100K | Colon    | Patch      | H&E        | 100000 images | https://zenodo.org/records/1214456               |
| PANDA           | Prostate | WSI        | H&E        | 11000 WSIs    | https://panda.grand-challenge.org                |
| PatchCamelyon   | Multiple | Patch      | H&E        | 327680 images | https://github.com/basveeling/pcam               |
| TCGA-BRCA       | Multiple | WSI        | H&E        | 1098 cases    | https://portal.gdc.cancer.gov/projects/TCGA-BRCA |

#### C. Stain Transfer

| Dataset | Organ    | Modality | Stain Type | Size        | Source                              |
| ------- | -------- | -------- | ---------- | ----------- | ----------------------------------- |
| ACROBAT | Breast   | WSI      | H&E, IHC   | 4212 WSIs   | https://acrobat.grand-challenge.org |
| BCI     | Breast   | WSI      | H&E, IHC   | 9746 images | https://bci.grand-challenge.org     |
| EMPaCT  | Prostate | Patch    | H&E, IHC   | 420 images  | https://zenodo.org/records/10066853 |

#### D. Multimodal & Other Tasks (Retrieval, Captioning, Biomarker Exploration)

| Dataset           | Organ    | Modality    | Stain Type | Size          | Source                                            |
| ----------------- | -------- | ----------- | ---------- | ------------- | ------------------------------------------------- |
| ARCH              | Multiple | Patch       | /          | 15164 images  | https://warwick.ac.uk/fac/cross_fac/tia/data/arch |
| HEST-1k           | Multiple | WSI, omics  | H&E        | 1229 cases    | https://huggingface.co/datasets/MahmoodLab/HEst   |
| OpenPath          | Multiple | Patch, Text | /          | 208414 images | https://huggingface.co/spaces/vinid/webplip       |
| PathCap           | Multiple | Patch, Text | /          | 207K pairs    | https://huggingface.co/datasets/jamessyx/PathCap  |
| PatchGastricADC22 | Stomach  | Patch, Text | H&E        | 262K images   | https://zenodo.org/records/6021442                |
| QUILT-1M          | Multiple | Patch       | /          | 1M pairs      | https://zenodo.org/records/8239942                |

### 2.Generative & Synthetic Datasets

#### A. Image-Synthetic

| Dataset | Organ  | Modality | Stain Type | Size         | Source                             |
| ------- | ------ | -------- | ---------- | ------------ | ---------------------------------- |
| SNOW    | Breast | Patch    | H&E        | 20000 images | https://zenodo.org/records/6633721 |

B. Text-Synthetic (for VQA & Report Generation)

| Dataset      | Organ    | Modality    | Stain Type | Size                 | Source                                                    |
| ------------ | -------- | ----------- | ---------- | -------------------- | --------------------------------------------------------- |
| PathGen-1.6M | Multiple | Patch, Text | Multiple   | 1.6M pairs           | https://huggingface.co/datasets/jamessyx/PathGen          |
| PathMMU      | Multiple | Patch, Text | /          | 24K images / 33K QA  | https://huggingface.co/datasets/jamessyx/PathMMU          |
| PathText     | Multiple | Patch, Text | /          | 9009 WSI-text pairs  | https://github.com/cpystan/Wsi-Caption                    |
| PathVQA      | Multiple | Patch, Text | /          | 5K images / 32K QA   | https://huggingface.co/datasets/flaviagiammarino/path-vqa |
| PMC-VQA      | Multiple | Patch, Text | Multiple   | 227K VQA             | https://huggingface.co/datasets/RadGenome/PMC-VQA         |
| QUILT-VQA    | Multiple | Patch, Text | /          | 985 images / 1283 QA | https://huggingface.co/datasets/wisdomik/Quilt_VQA        |
| WSI-VQA      | Breast   | WSI, Text   | H&E        | 977 WSIs / 8672 QA   | https://github.com/cpystan/WSI-VQA                        |



## Overview of Image Generation Methods in Computational Pathology

(计算病理学中的图像生成方法概述)







