# Large Vision Language Models for Computational Pathology: A Comprehensive Survey of the Emerging Paradigm Shift

![](fig/image8.gif)

This is the summation of all the methods, datasets, and other survey mentioned in our survey 'A Comprehensive Survey of the Emerging Paradigm Shift' 🔥. Any problems, please contact [HuangPengyuan@csuft.edu.cn]. Any other interesting papers or codes are welcome. If you find this repository useful to your research or work, it is really appreciated to star this repository ❤️.

## Datasets

| Dataset         | Year | Link                                                         | Dataset           | Year | Link                                                         |
| --------------- | ---- | ------------------------------------------------------------ | ----------------- | ---- | ------------------------------------------------------------ |
| Camelyon16      | 2017 | [[link]](https://camelyon16.grand-challenge.org/)            | ACROBAT           | 2022 | [[link]](https://acrobat.grand-challenge.org)                |
| CoNIC           | 2024 | [[link]](https://conic-challenge.grand-challenge.org/)       | BCI               | 2022 | [[link]](https://bci.grand-challenge.org)                    |
| CoNSeP          | 2019 | [[link]](https://opendatalab.com/OpenDataLab/CoNSeP)         | EMPaCT            | 2023 | [[link]](https://zenodo.org/records/10066853)                |
| DigestPath      | 2022 | [[link]](https://digestpath2019.grand-challenge.org)         | ARCH              | 2021 | [[link]](https://warwick.ac.uk/fac/cross_fac/tia/data/arch)  |
| Glas            | 2016 | [[link]](https://www.kaggle.com/datasets/sani84/glasmiccai2015-gland-segmentation) | HEST-1k           | 2024 | [[link]](https://huggingface.co/datasets/MahmoodLab/HEst)    |
| Lizard          | 2021 | [[link]](https://www.kaggle.com/datasets/aadimator/lizard-dataset) | OpenPath          | 2023 | [[link]](https://huggingface.co/spaces/vinid/webplip)        |
| MoNuSeg         | 2020 | [[link]](https://monuseg.grand-challenge.org/)               | PathCap           | 2024 | [[link]](https://huggingface.co/datasets/jamessyx/PathCap)   |
| PanNuke         | 2019 | [[link]](https://huggingface.co/datasets/RationAI/PanNuke)   | PatchGastricADC22 | 2021 | [[link]](https://zenodo.org/records/6021442)                 |
| TUPAC           | 2019 | [[link]](https://tupac.grand-challenge.org)                  | QUILT-1M          | 2025 | [[link]](https://zenodo.org/records/8239942)                 |
| BACH            | 2019 | [[link]](https://zenodo.org/records/3632035)                 | SNOW              | 2023 | [[link]](https://zenodo.org/records/6633721)                 |
| BreakHis        | 2016 | [[link]](https://web.inf.ufpr.br/vri/databases/breakhis)     | PathGen-1.6M      | 2024 | [[link]](https://huggingface.co/datasets/jamessyx/PathGen)   |
| Camelyon17      | 2019 | [[link]](https://camelyon17.grand-challenge.org/)            | PathMMU           | 2024 | [[link]](https://huggingface.co/datasets/jamessyx/PathMMU)   |
| LC25000         | 2020 | [[link]](https://huggingface.co/datasets/1aurent/LC25000)    | PathText          | 2024 | [[link]](https://github.com/cpystan/Wsi-Caption)             |
| NCT-CRC-HE-100K | 2018 | [[link]](https://zenodo.org/records/1214456)                 | PathVQA           | 2020 | [[link]](https://huggingface.co/datasets/flaviagiammarino/path-vqa) |
| PANDA           | 2022 | [[link]](https://panda.grand-challenge.org)                  | PMC-VQA           | 2024 | [[link]](https://huggingface.co/datasets/RadGenome/PMC-VQA)  |
| PatchCamelyon   | 2018 | [[link]](https://github.com/basveeling/pcam)                 | QUILT-VQA         | 2024 | [[link]](https://huggingface.co/datasets/wisdomik/Quilt_VQA) |
| TCGA-BRCA       | 2022 | [[link]](https://portal.gdc.cancer.gov/projects/TCGA-BRCA)   | WSI-VQA           | 2025 | [[link]](https://github.com/cpystan/WSI-VQA)                 |



## Comparison of Datasets

| Dataset           | Modality    | Stain Type | Size                 |
| ----------------- | ----------- | ---------- | -------------------- |
| Camelyon16        | WSI         | H&E        | 400 WSIs             |
| CoNIC             | Patch       | H&E        | 4981 images          |
| CoNSeP            | Patch       | H&E        | 41 images            |
| DigestPath        | Patch       | H&E        | 1559 images          |
| Glas              | Patch       | H&E        | 165 images           |
| Lizard            | Patch       | H&E        | 495179 nuclei        |
| MoNuSeg           | Patch       | H&E        | 29000 nuclei         |
| PanNuke           | Patch       | H&E        | 7901 images          |
| TUPAC             | WSI         | H&E        | 573 cases            |
| BACH              | Patch, WSI  | H&E        | 400+ images          |
| BreakHis          | Patch       | H&E        | 9709 images          |
| Camelyon17        | WSI         | H&E        | 1399 WSIs            |
| LC25000           | Patch       | H&E        | 25000 images         |
| NCT-CRC-HE-100K   | Patch       | H&E        | 100000 images        |
| PANDA             | WSI         | H&E        | 11000 WSIs           |
| PatchCamelyon     | Patch       | H&E        | 327680 images        |
| TCGA-BRCA         | WSI         | H&E        | 1098 cases           |
| ACROBAT           | WSI         | H&E, IHC   | 4212 WSIs            |
| BCI               | WSI         | H&E, IHC   | 9746 images          |
| EMPaCT            | Patch       | H&E, IHC   | 420 images           |
| ARCH              | Patch       | /          | 15164 images         |
| HEST-1k           | WSI, omics  | H&E        | 1229 cases           |
| OpenPath          | Patch, Text | /          | 208414 images        |
| PathCap           | Patch, Text | /          | 207K pairs           |
| PatchGastricADC22 | Patch, Text | H&E        | 262K images          |
| QUILT-1M          | Patch       | /          | 1M pairs             |
| SNOW              | Patch       | H&E        | 20000 images         |
| PathGen-1.6M      | Patch, Text | Multiple   | 1.6M pairs           |
| PathMMU           | Patch, Text | /          | 24K images / 33K QA  |
| PathText          | Patch, Text | /          | 9009 WSI-text pairs  |
| PathVQA           | Patch, Text | /          | 5K images / 32K QA   |
| PMC-VQA           | Patch, Text | Multiple   | 227K VQA             |
| QUILT-VQA         | Patch, Text | /          | 985 images / 1283 QA |
| WSI-VQA           | WSI, Text   | H&E        | 977 WSIs / 8672 QA   |



## LVLMs for Computational Pathology

| Model                                                        | Architecture | Input              | Link                                                         |
| ------------------------------------------------------------ | ------------ | ------------------ | ------------------------------------------------------------ |
| PathologyGAN: Deep representations of cancer tissue for classification and generation | GAN          | Patch              | [[link]](https://arxiv.org/abs/1907.02644)                   |
| HistoGAN: Dataset augmentation with selective synthetic images for classification | GAN          | Patch              | [[link]](https://arxiv.org/abs/2111.06399)                   |
| Optimising Diffusion Models: Generating images conditioned on HPV status for improved classification | Diffusion    | Patch, HPV Status  | [[link]](https://bmvc2024.org/proceedings/727/)              |
| InsMix: Generating realistic data for augmenting nuclei instance segmentation tasks | GAN          | Patch              | [[link]](https://arxiv.org/abs/2206.15134)                   |
| MFDPM: Synthesizing histopathology images preserving morphological details | Diffusion    | Patch              | [[link]](https://arxiv.org/abs/2209.13167)                   |
| ViT-DAE: Transformer-driven diffusion autoencoder for augmentation and classification | Diffusion    | Patch              | [[link]](https://arxiv.org/abs/2304.01053)                   |
| ProGleason-GAN: Synthesizing prostate cancer images with controllable Gleason grades | GAN          | Patch              | [[link]](https://www.sciencedirect.com/science/article/pii/S0169260723003607) |
| DiffMix: Synthesizing balanced image-label pairs to improve segmentation | Diffusion    | Patch              | [[link]](https://arxiv.org/abs/2306.14132)                   |
| AnoDDPM: Detecting out-of-distribution samples in digital pathology images | Diffusion    | Patch              | [[link]](https://pubmed.ncbi.nlm.nih.gov/38228075/)          |
| ADD: Simulating progressive pathological transitions for classification tasks | Diffusion    | Patch              | [[link]](https://arxiv.org/abs/2311.12316)                   |
| MoPaDi: Generating counterfactual images for mechanistic explanation of AI models | Diffusion    | Patch              | [[link]](https://pmc.ncbi.nlm.nih.gov/articles/PMC11565818.1/) |
| USegMix: Unsupervised segment mix for data augmentation in classification | Diffusion    | Patch              | [[link]](https://arxiv.org/abs/2502.16160)                   |
| PDSeg: Patch-wise mask distillation for weakly-supervised tissue segmentation | Diffusion    | Patch, Mask        | [[link]](https://ieeexplore.ieee.org/document/10888097)      |
| dcGAN: Data augmentation with synthetic Gleason patterns to improve Gleason grading | GAN          | Patch              | [[link]](https://www.mendeley.com/catalogue/a93054c0-c74f-36b8-8c6d-7cac142f3746/) |
| AttributeGAN: Synthesizing histopathology images with control over cellular attributes | GAN          | Cellular Attribute | [[link]](https://arxiv.org/abs/2111.06398)                   |
| Sharp-GAN: Enhancing boundary resolution in mask-to-image synthesis for segmentation | GAN          | Patch              | [[link]](https://arxiv.org/abs/2110.14709)                   |
| NASDM: Generating nuclei-aware semantic tissue from segmentation masks | Diffusion    | Patch, Mask        | [[link]](https://arxiv.org/abs/2303.11477)                   |
| DISC: Self-distillation for prostate cancer grading and classification | Diffusion    | Patch              | [[link]](https://arxiv.org/abs/2404.13097)                   |
| DiffInfinite: Large-scale mask-to-image synthesis using parallel random patch diffusion | Diffusion    | Patch              | [[link]](https://arxiv.org/abs/2306.13384)                   |
| STEDM: Zero-shot, style-based synthesis of image-mask pairs from semantic layouts | Diffusion    | Patch, Layout      | [[link]](https://arxiv.org/abs/2403.14429)                   |
| SynCLay: Interactive synthesis of images from cellular layouts with co-generated masks | GAN          | Layout             | [[link]](https://www.sciencedirect.com/science/article/pii/S1361841523002554) |
| HADiff: Hierarchy-aggregated diffusion for mask-based segmentation | Diffusion    | Patch              | [[link]](https://link.springer.com/article/10.1007/s00371-024-03746-z) |
| PathoPainter: Tumor-aware image inpainting for segmentation data augmentation | Diffusion    | Patch              | [[link]](https://arxiv.org/abs/2503.04634)                   |
| MSSA-GAN: Pathology image restoration using multi-scale self-attention | GAN          | Patch              | [[link]](https://link.springer.com/article/10.1007/s00371-022-02592-1) |
| ArtiFusion: Restoring artifacts in histopathology images to improve classification | Diffusion    | Patch              | [[link]](https://arxiv.org/abs/2307.14262)                   |
| AR-CycleGAN: Detecting and restoring various histological artifacts | GAN          | Patch              | [[link]](https://ieeexplore.ieee.org/document/10160043)      |
| Restore-GAN: Enhancing pathology image quality (deblurring, super-res) for downstream tasks | GAN          | Patch              | [[link]](https://www.sciencedirect.com/science/article/pii/S0002944023000275) |
| HARP: Artifact restoration through unsupervised detection and diffusion-based inpainting | Diffusion    | Patch              | [[link]](https://openreview.net/forum?id=bVunbe4hoV)         |
| LatentArtiFusion: Restoring histological artifacts efficiently in a low-dimensional latent space | VAE/Diff.    | Patch              | [[link]](https://arxiv.org/abs/2407.20172)                   |
| ArtiDiffuser: Unified framework for histological artifact restoration and synthesis | Diffusion    | Patch              | [[link]](https://www.sciencedirect.com/science/article/abs/pii/S1361841525001148) |
| ProGAN: High-quality patch/WSI generation for data augmentation and classification | GAN          | Patch, WSI         | [[link]](https://pubmed.ncbi.nlm.nih.gov/32686118/)          |
| SAFRON: Generating seamless, large-scale histology images via patch-stitching GAN | GAN          | Mask               | [[link]](https://arxiv.org/abs/2008.04526)                   |
| STAR-RL: Hierarchical reinforcement learning for interpretable super-resolution | RL           | Patch              | [[link]](https://arxiv.org/html/2406.18310v1)                |
| PathUp: Synthesizing large, multi-class pathology images with high fidelity | Diffusion    | Patch, Text        | [[link]](https://dl.acm.org/doi/10.1145/3664647.3681295)     |
| URCDM: Ultra-resolution WSI synthesis using a cascaded conditional diffusion model | Diffusion    | Patch, WSI         | [[link]](https://arxiv.org/abs/2407.13277)                   |
| Histo-Diffusion: Super-resolution with quality assessment for classification | Diffusion    | Patch              | [[link]](https://arxiv.org/abs/2408.15218)                   |
| ToPoFM: Generating images with cellular topology control for segmentation | LLM/VLM      | Patch              | [[link]](https://ieeexplore.ieee.org/document/10915718)      |
| PathLDM: Generating histopathology images conditioned on descriptive text prompts | Diffusion    | Patch, Text        | [[link]](https://arxiv.org/abs/2309.00748)                   |
| VIMs: Synthesizing virtual multiplex IHC stains from H&E images using text prompts | Diffusion    | Patch, Text        | [[link]](https://arxiv.org/abs/2407.19113)                   |
| SST: Stain normalization and style transfer to improve classification robustness | GAN          | Patch              | [[link]](https://arxiv.org/abs/1710.08543)                   |
| PC-StainGAN: Unpaired stain transfer (e.g., H&E to IHC) with pathology-consistency constraints | GAN          | Patch              | [[link]](https://ieeexplore.ieee.org/document/9389763)       |
| Residual CycleGAN: Improving domain transformation robustness for segmentation tasks | GAN          | Patch              | [[link]](https://www.sciencedirect.com/science/article/pii/S1361841521000505) |
| CAGAN: Semi-supervised stain normalization via dual-decoder consistency learning | GAN          | Patch              | [[link]](https://www.sciencedirect.com/science/article/abs/pii/S1361841522002195) |
| StainDiff: Transferring stain styles between histology images using diffusion models | Diffusion    | Patch              | [[link]](https://link.springer.com/chapter/10.1007/978-3-031-43987-2_53) |
| AV-GAN: Virtual staining for unevenly stained tissue using an attention-based varifocal GAN | GAN          | Patch              | [[link]](https://arxiv.org/abs/2404.10714)                   |
| StainFuser: Controlling diffusion for fast neural style transfer in multi-gigapixel images | Diffusion    | Patch              | [[link]](https://arxiv.org/abs/2403.09302)                   |
| StainDiffuser: Multitask virtual staining and segmentation from the same model | Diffusion    | Patch              | [[link]](https://arxiv.org/abs/2403.11340)                   |
| PPHM-GAN: High-resolution any-to-any stain translation for classification | GAN          | Patch              | [[link]](https://www.sciencedirect.com/science/article/pii/S0010482524012344) |
| MDDP: Pre-training via H&E-to-IHC translation for improved WSI classification | Diffusion    | Patch              | [[link]](https://dl.acm.org/doi/10.1145/3664647.3680882)     |
| VirtualMultiplexer: AI-based virtual multiplexing for tumor profiling, prognosis, and classification | Other        | Patch              | [[link]](https://www.nature.com/articles/s42256-024-00889-5) |
| TT-SaD: Improving classification robustness through test-time stain adaptation | Diffusion    | Patch              | [[link]](https://link.springer.com/chapter/10.1007/978-3-031-72761-0_15) |
| PST-Diff: Achieving high-consistency stain transfer with pathological/structural constraints | Diffusion    | Patch              | [[link]](https://ieeexplore.ieee.org/document/10601703)      |
| F2FLD: Unpaired frozen-FFPE translation for classification   | Diffusion    | Patch              | [[link]](https://arxiv.org/abs/2404.12650)                   |
| ULSA: Unsupervised latent stain adaptation for WSI segmentation | GAN          | Patch, WSI         | [[link]](https://arxiv.org/abs/2406.19081)                   |
| Diffusion-L: Image-to-image translation with robust uncertainty quantification | Diffusion    | Patch              | [[link]](https://link.springer.com/chapter/10.1007/978-3-031-53767-7_15) |
| DUST: A unified diffusion framework for versatile (any-to-any) stain transfer | Diffusion    | Patch              | [[link]](https://ieeexplore.ieee.org/document/10980971)      |
| ODA-GAN: IHC staining via orthogonal decoupling of morphological and staining features | GAN          | Patch              | [[link]](https://ieeexplore.ieee.org/document/11095140)      |
| CC-WSI-Net: Generating seamless virtual IHC whole-slide images with content consistency | GAN          | Patch              | [[link]](https://arxiv.org/abs/2410.01072)                   |
| VM-GAN: A value mapping framework for large-scale histological image-to-image translation | GAN          | Patch              | [[link]](https://arxiv.org/abs/2501.03592)                   |
| DSTGAN: Deeply supervised two-stage GAN for stain normalization and segmentation | GAN          | Patch              | [[link]](https://www.nature.com/articles/s41598-025-91587-8) |
| RBDM: Virtual staining from label-free polarimetric imaging for report generation | Diffusion    | Patch              | [[link]](https://arxiv.org/abs/2503.01352)                   |
| SGMT: Generating WSI reports guided by cancer information using a masked transformer | VLM          | Patch, WSI         | [[link]](https://arxiv.org/abs/2310.20607)                   |
| HistGen: Employing a local-global hierarchical encoder for comprehensive WSI report generation | VLM          | WSI                | [[link]](https://arxiv.org/abs/2403.05396)                   |
| TraP-VQA: Achieving interpretable VQA by a vision encoder with multimodal attention mechanisms | VLM          | Patch, Text        | [[link]](https://ieeexplore.ieee.org/document/9745795)       |
| LLaVA-Med: Building a biomedical VQA assistant through cost-efficient instruction tuning | VLM          | Patch, Text        | [[link]](https://arxiv.org/abs/2306.00890)                   |
| PathChat: Developing a general-purpose multimodal AI assistant for interactive VQA and reporting | VLM          | Patch, Text        | [[link]](https://www.nature.com/articles/s41586-024-07618-3) |
| PathologyVLM: A large vision-language model foundational for diverse pathology VQA and reports | VLM          | Patch, Text        | [[link]](https://link.springer.com/article/10.1007/s10462-025-11190-1) |
| PathCoT: Improving reliability of zero-shot CoT reasoning via expert-guided prompting | VLM          | Patch, Text        | [[link]](https://arxiv.org/abs/2507.01029)                   |
| SlideChat: Enabling interactive WSI-level VQA through a hierarchical processing approach | VLM          | WSI                | [[link]](https://arxiv.org/abs/2410.11761)                   |



## Milestone Papers

| Date    | keywords             | Institute            | Paper                                                        |
| ------- | -------------------- | -------------------- | ------------------------------------------------------------ |
| 2017-06 | Transformer          | Google               | [Attention Is All You Need](https://arxiv.org/pdf/1706.03762.pdf) |
| 2018-06 | GPT 1.0              | OpenAI               | [Improving Language Understanding by Generative Pre-Training](https://www.cs.ubc.ca/~amuham01/LING530/papers/radford2018improving.pdf) |
| 2018-10 | BERT                 | Google               | [BERT: Pre-training of Deep Bidirectional Transformers for Language Understanding](https://aclanthology.org/N19-1423.pdf) |
| 2019-02 | GPT 2.0              | OpenAI               | [Language Models are Unsupervised Multitask Learners](https://d4mucfpksywv.cloudfront.net/better-language-models/language_models_are_unsupervised_multitask_learners.pdf) |
| 2019-10 | T5                   | Google               | [Exploring the Limits of Transfer Learning with a Unified Text-to-Text Transformer](https://jmlr.org/papers/v21/20-074.html) |
| 2020-05 | GPT 3.0              | OpenAI               | [Language models are few-shot learners](https://papers.nips.cc/paper/2020/file/1457c0d6bfcb4967418bfb8ac142f64a-Paper.pdf) |
| 2021-01 | Switch Transformers  | Google               | [Switch Transformers: Scaling to Trillion Parameter Models with Simple and Efficient Sparsity](https://arxiv.org/pdf/2101.03961.pdf) |
| 2021-08 | Codex                | OpenAI               | [Evaluating Large Language Models Trained on Code](https://arxiv.org/pdf/2107.03374.pdf) |
| 2021-08 | Foundation Models    | Stanford             | [On the Opportunities and Risks of Foundation Models](https://arxiv.org/pdf/2108.07258.pdf) |
| 2021-09 | FLAN                 | Google               | [Finetuned Language Models are Zero-Shot Learners](https://openreview.net/forum?id=gEZrGCozdqR) |
| 2021-10 | T0                   | HuggingFace et al.   | [Multitask Prompted Training Enables Zero-Shot Task Generalization](https://arxiv.org/abs/2110.08207) |
| 2022-01 | COT                  | Google               | [Chain-of-Thought Prompting Elicits Reasoning in Large Language Models](https://arxiv.org/pdf/2201.11903.pdf) |
| 2022-03 | InstructGPT          | OpenAI               | [Training language models to follow instructions with human feedback](https://arxiv.org/pdf/2203.02155.pdf) |
| 2022-10 | Flan-T5/PaLM         | Google               | [Scaling Instruction-Finetuned Language Models](https://arxiv.org/pdf/2210.11416.pdf) |
| 2022-10 | GLM-130B             | Tsinghua             | [GLM-130B: An Open Bilingual Pre-trained Model](https://arxiv.org/pdf/2210.02414.pdf) |
| 2022-11 | HELM                 | Stanford             | [Holistic Evaluation of Language Models](https://arxiv.org/pdf/2211.09110.pdf) |
| 2022-11 | BLOOM                | BigScience           | [BLOOM: A 176B-Parameter Open-Access Multilingual Language Model](https://arxiv.org/pdf/2211.05100.pdf) |
| 2022-11 | Galactica            | Meta                 | [Galactica: A Large Language Model for Science](https://arxiv.org/pdf/2211.09085.pdf) |
| 2022-12 | OPT-IML              | Meta                 | [OPT-IML: Scaling Language Model Instruction Meta Learning through the Lens of Generalization](https://arxiv.org/pdf/2212.12017) |
| 2023-01 | Flan 2022 Collection | Google               | [The Flan Collection: Designing Data and Methods for Effective Instruction Tuning](https://arxiv.org/pdf/2301.13688.pdf) |
| 2023-02 | LLaMA                | Meta                 | [LLaMA: Open and Efficient Foundation Language Models](https://research.facebook.com/publications/llama-open-and-efficient-foundation-language-models/) |
| 2023-02 | Kosmos-1             | Microsoft            | [Language Is Not All You Need: Aligning Perception with Language Models](https://arxiv.org/abs/2302.14045) |
| 2023-03 | PaLM-E               | Google               | [PaLM-E: An Embodied Multimodal Language Model](https://palm-e.github.io/) |
| 2023-03 | GPT 4                | OpenAI               | [GPT-4 Technical Report](https://openai.com/research/gpt-4)  |
| 2023-04 | LLaVA                | UW–Madison&Microsoft | [Visual Instruction Tuning](https://arxiv.org/abs/2304.08485) |
| 2023-04 | Pythia               | EleutherAI et al.    | [Pythia: A Suite for Analyzing Large Language Models Across Training and Scaling](https://arxiv.org/abs/2304.01373) |
| 2023-05 | Dromedary            | CMU et al.           | [Principle-Driven Self-Alignment of Language Models from Scratch with Minimal Human Supervision](https://arxiv.org/abs/2305.03047) |
| 2023-05 | PaLM 2               | Google               | [PaLM 2 Technical Report](https://ai.google/static/documents/palm2techreport.pdf) |
| 2023-05 | RWKV                 | Bo Peng              | [RWKV: Reinventing RNNs for the Transformer Era](https://arxiv.org/abs/2305.13048) |
| 2023-05 | DPO                  | Stanford             | [Direct Preference Optimization: Your Language Model is Secretly a Reward Model](https://arxiv.org/pdf/2305.18290.pdf) |
| 2023-05 | ToT                  | Google&Princeton     | [Tree of Thoughts: Deliberate Problem Solving with Large Language Models](https://arxiv.org/pdf/2305.10601.pdf) |
| 2023-07 | LLaMA2               | Meta                 | [Llama 2: Open Foundation and Fine-Tuned Chat Models](https://arxiv.org/pdf/2307.09288.pdf) |
| 2023-10 | Mistral 7B           | Mistral              | [Mistral 7B](https://arxiv.org/pdf/2310.06825.pdf)           |
| 2023-12 | Mamba                | CMU&Princeton        | [Mamba: Linear-Time Sequence Modeling with Selective State Spaces](https://arxiv.org/pdf/2312.00752) |
| 2024-01 | DeepSeek-v2          | DeepSeek             | [DeepSeek-V2: A Strong, Economical, and Efficient Mixture-of-Experts Language Model](https://arxiv.org/abs/2405.04434) |
| 2024-02 | OLMo                 | Ai2                  | [OLMo: Accelerating the Science of Language Models](https://arxiv.org/abs/2402.00838) |
| 2024-05 | Mamba2               | CMU&Princeton        | [Transformers are SSMs: Generalized Models and Efficient Algorithms Through Structured State Space Duality](https://arxiv.org/abs/2405.21060) |
| 2024-05 | Llama3               | Meta                 | [The Llama 3 Herd of Models](https://arxiv.org/abs/2407.21783) |
| 2024-06 | FineWeb              | HuggingFace          | [The FineWeb Datasets: Decanting the Web for the Finest Text Data at Scale](https://arxiv.org/abs/2406.17557) |
| 2024-09 | OLMoE                | Ai2                  | [OLMoE: Open Mixture-of-Experts Language Models](https://arxiv.org/abs/2409.02060) |
| 2024-12 | Qwen2.5              | Alibaba              | [Qwen2.5 Technical Report](https://arxiv.org/abs/2412.15115) |
| 2024-12 | DeepSeek-V3          | DeepSeek             | [DeepSeek-V3 Technical Report](https://arxiv.org/abs/2412.19437v1) |
| 2025-01 | DeepSeek-R1          | DeepSeek             | [DeepSeek-R1: Incentivizing Reasoning Capability in LLMs via Reinforcement Learning](https://arxiv.org/abs/2501.12948) |
| 2025-02 | Qwen2.5-VL           | Alibaba              | [Qwen2.5-VL Technical Report](https://arxiv.org/pdf/2502.13923) |
| 2025-03 | Qwen2.5-Omni         | Alibaba              | [Qwen2.5-Omni Technical Report](https://arxiv.org/pdf/2503.20215) |
| 2025-03 | QwQ                  | Alibaba              | [QwQ-32B: Embracing the Power of Reinforcement Learning](https://qwenlm.github.io/blog/qwq-32b/) |
| 2025-05 | Qwen3                | Alibaba              | [Qwen3 Technical Report](https://arxiv.org/abs/2505.09388)   |



## Open LLM

- Meta
  - [Llama-2-7B|13B|70B](https://github.com/meta-llama/llama)
  - [Llama-3-8B|70B](https://github.com/meta-llama/llama3)
  - [Llama-3.1-8B|70B|405B](https://github.com/meta-llama/llama3)
  - [Llama-3.2-1B|3B|8B|70B](https://github.com/meta-llama/llama3.2)
  - [CodeLlama-7B|13B|70B](https://github.com/meta-llama/codellama)
  - [CodeLlama-Python-7B|13B|70B](https://github.com/meta-llama/codellama)

- Mistral
  - [Mistral-7B-v0.1|v0.2|v0.3](https://github.com/mistralai/mistral-src)
  - [Mixtral-8x7B-v0.1](https://github.com/mistralai/mistral-src)
  - [Mixtral-8x22B-v0.1](https://github.com/mistralai/mistral-src)
  - [Mistral-Nemo-12B](https://github.com/mistralai/mistral-src)

- Alibaba
  - [Qwen-1.8B|7B|14B|72B](https://github.com/QwenLM/Qwen)
  - [Qwen-2-0.5B|1.5B|7B|14B|32B|72B](https://github.com/QwenLM/Qwen2)
  - [Qwen-VL-7B|14B](https://github.com/QwenLM/Qwen-VL)
  - [Qwen-Coder-1.5B|7B|14B|32B](https://github.com/QwenLM/Qwen-Coder)
  - [Qwen-Math-7B|14B](https://github.com/QwenLM/Qwen-Math)

- GLM
  - [ChatGLM-6B](https://github.com/THUDM/ChatGLM-6B)
  - [ChatGLM2-6B](https://github.com/THUDM/ChatGLM2-6B)
  - [ChatGLM3-6B](https://github.com/THUDM/ChatGLM3)
  - [GLM-4-9B|40B](https://github.com/THUDM/GLM-4)
  - [GLM-4V-9B](https://github.com/THUDM/GLM-4)
  - [CodeGeeX2-6B](https://github.com/THUDM/CodeGeeX2)

- DeepSeek
  - [DeepSeek-Math-7B](https://github.com/deepseek-ai/DeepSeek-Math)
  - [DeepSeek-Coder-1.3|6.7|7|33B](https://github.com/deepseek-ai/DeepSeek-Coder)
  - [DeepSeek-VL-1.3|7B](https://github.com/deepseek-ai/DeepSeek-VL)
  - [DeepSeek-MoE-16B](https://github.com/deepseek-ai/DeepSeek-MoE)
  - [DeepSeek-v2-236B-MoE](https://github.com/deepseek-ai/DeepSeek-LLM)
  - [DeepSeek-Coder-v2-16|236B-MOE](https://github.com/deepseek-ai/DeepSeek-Coder)
  - [DeepSeek-V2.5](https://github.com/deepseek-ai/DeepSeek-LLM)
  - [DeepSeek-V3](https://github.com/deepseek-ai/DeepSeek-LLM)
  - [DeepSeek-R1](https://github.com/deepseek-ai/DeepSeek-R1)

- Baichuan
  - [Baichuan-7B](https://github.com/baichuan-inc/Baichuan-7B)
  - [Baichuan-13B](https://github.com/baichuan-inc/Baichuan-13B)
  - [Baichuan-2-7B|13B](https://github.com/baichuan-inc/Baichuan2)
  - [Baichuan-3-4B|8B|24B](https://github.com/baichuan-inc/Baichuan3)

- InternLM
  - [InternLM-7B|20B](https://github.com/InternLM/InternLM)
  - [InternLM2-7B|20B](https://github.com/InternLM/InternLM)
  - [InternLM2.5-7B|20B](https://github.com/InternLM/InternLM)
  - [InternLM-Math-7B|20B](https://github.com/InternLM/InternLM-Math)

- Google
  - [Gemma-2B|7B](https://github.com/google/gemma_pytorch)
  - [Gemma-2-2B|9B|27B](https://github.com/google/gemma_pytorch)











