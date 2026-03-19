# Content Generation Models in Computational Pathology: A Comprehensive Survey on Methods, Applications, and Challenges

![](fig/image8.gif)

This is the summation of all the methods, datasets, and other survey mentioned in our survey 'Content Generation Models in Computational Pathology: A Comprehensive Survey on Methods, Applications, and Challenges' 🔥. Any problems, please contact [HuangPengyuan@csuft.edu.cn]. Any other interesting papers or codes are welcome. If you find this repository useful to your research or work, it is really appreciated to star this repository ❤️.

## Datasets

| Dataset         | Year | Link                                                         | Dataset           | Year | Link                                                      |
| --------------- | ---- | ------------------------------------------------------------ | ----------------- | ---- | --------------------------------------------------------- |
| Camelyon16      | 2017 | https://camelyon16.grand-challenge.org/                      | BCI               | 2022 | https://bci.grand-challenge.org                           |
| CoNIC           | 2024 | https://conic-challenge.grand-challenge.org/                 | EMPaCT            | 2023 | https://zenodo.org/records/10066853                       |
| CoNSeP          | 2019 | https://opendatalab.com/OpenDataLab/CoNSeP                   | ARCH              | 2021 | https://warwick.ac.uk/fac/cross_fac/tia/data/arch         |
| DigestPath      | 2022 | https://digestpath2019.grand-challenge.org                   | HEST-1k           | 2024 | https://huggingface.co/datasets/MahmoodLab/HEst           |
| Glas            | 2016 | https://www.kaggle.com/datasets/sani84/glasmiccai2015-gland-segmentation | OpenPath          | 2023 | https://huggingface.co/spaces/vinid/webplip               |
| Lizard          | 2021 | https://www.kaggle.com/datasets/aadimator/lizard-dataset     | PathCap           | 2024 | https://huggingface.co/datasets/jamessyx/PathCap          |
| MoNuSeg         | 2020 | https://monuseg.grand-challenge.org/                         | PatchGastricADC22 | 2021 | https://zenodo.org/records/6021442                        |
| PanNuke         | 2019 | https://huggingface.co/datasets/RationAI/PanNuke             | QUILT-1M          | 2025 | https://zenodo.org/records/8239942                        |
| TUPAC           | 2019 | https://tupac.grand-challenge.org                            | SNOW              | 2023 | https://zenodo.org/records/6633721                        |
| BACH            | 2019 | https://zenodo.org/records/3632035                           | PathGen-1.6M      | 2024 | https://huggingface.co/datasets/jamessyx/PathGen          |
| BreakHis        | 2016 | https://web.inf.ufpr.br/vri/databases/breakhis               | PathMMU           | 2024 | https://huggingface.co/datasets/jamessyx/PathMMU          |
| Camelyon17      | 2019 | https://camelyon17.grand-challenge.org/                      | PathText          | 2024 | https://github.com/cpystan/Wsi-Caption                    |
| LC25000         | 2020 | https://huggingface.co/datasets/1aurent/LC25000              | PathVQA           | 2020 | https://huggingface.co/datasets/flaviagiammarino/path-vqa |
| NCT-CRC-HE-100K | 2018 | https://zenodo.org/records/1214456                           | PMC-VQA           | 2024 | https://huggingface.co/datasets/RadGenome/PMC-VQA         |
| PANDA           | 2022 | https://panda.grand-challenge.org                            | QUILT-VQA         | 2024 | https://huggingface.co/datasets/wisdomik/Quilt_VQA        |
| PatchCamelyon   | 2018 | https://github.com/basveeling/pcam                           | WSI-VQA           | 2025 | https://github.com/cpystan/WSI-VQA                        |
| TCGA-BRCA       | 2022 | https://portal.gdc.cancer.gov/projects/TCGA-BRCA             |                   |      |                                                           |
| ACROBAT         | 2022 | https://acrobat.grand-challenge.org                          |                   |      |                                                           |



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



## Models

// TODO

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











