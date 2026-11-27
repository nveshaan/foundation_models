# Foundation Models

This repo contains a checklist of open-weight foundation models explored through visualization, interpretability, and analysis of their behaviour and embeddings. The models are used as released (no fine-tuning), so the focus stays on what the pretrained weights have learned. It is the companion to [deep_learning](https://github.com/nveshaan/deep_learning), where the underlying components are implemented from first principles.

> For a better experience with notebooks, it is recommended to view the repository at
> https://nbviewer.org/github/nveshaan/foundation_models/tree/main/

> Everything here is meant to run on a 24 GB Apple silicon Mac (PyTorch `mps` or MLX), so models are chosen to fit. Check each model card for license and gated access.

## Models

### General

**Language: Encoders**
- [ ] BERT
- [ ] RoBERTa
- [ ] DeBERTa
- [ ] ELECTRA
- [ ] DistilBERT
- [ ] XLM-R
- [ ] ModernBERT

**Language: Encoder-Decoder**
- [ ] T5 / Flan-T5
- [ ] mT5
- [ ] BART

**Language: Decoders**
- [ ] GPT-2
- [ ] Pythia (with intermediate checkpoints)
- [ ] OLMo
- [ ] Llama 3.2 (1B)
- [ ] Qwen 2.5 (0.5B, 1.5B)
- [ ] Gemma
- [ ] Phi
- [ ] Falcon
- [ ] Mistral (7B, quantized)
- [ ] DeepSeek (distilled variants)

**Language: Alternative Architectures**
- [ ] Mamba
- [ ] RWKV

**Code**
- [ ] StarCoder (small variants)
- [ ] Qwen-Coder
- [ ] Code Llama

**Text Embeddings**
- [ ] sentence-transformers (MiniLM)
- [ ] BGE
- [ ] E5

**Vision: CNNs**
- [ ] ResNet
- [ ] ConvNeXt
- [ ] EfficientNet
- [ ] MobileNet

**Vision: Transformers**
- [ ] ViT
- [ ] DeiT
- [ ] Swin
- [ ] EVA

**Vision: Self-Supervised**
- [ ] DINO / DINOv2
- [ ] MAE
- [ ] SimCLR

**Vision: Dense Prediction**
- [ ] DETR
- [ ] Mask2Former
- [ ] YOLO
- [ ] SAM / SAM 2
- [ ] Depth Anything
- [ ] MiDaS

**Vision-Language**
- [ ] CLIP / OpenCLIP
- [ ] EVA-CLIP
- [ ] SigLIP
- [ ] BLIP / BLIP-2
- [ ] LLaVA
- [ ] PaliGemma
- [ ] Qwen-VL
- [ ] InternVL
- [ ] SmolVLM

**Generative Media**
- [ ] Stable Diffusion (VAE, UNet, text encoder)
- [ ] DiT
- [ ] ControlNet
- [ ] VQGAN

**Audio**
- [ ] Whisper
- [ ] wav2vec 2.0
- [ ] HuBERT
- [ ] WavLM
- [ ] CLAP
- [ ] AST
- [ ] EnCodec
- [ ] MusicGen

### Science

**Biology: Protein**
- [ ] ESM-2
- [ ] ESM C
- [ ] ProtBERT
- [ ] ProtT5
- [ ] ProteinMPNN

**Biology: DNA**
- [ ] DNABERT-2
- [ ] Nucleotide Transformer
- [ ] HyenaDNA
- [ ] Caduceus

**Biology: Single-Cell**
- [ ] Geneformer
- [ ] scGPT

**Chemistry**
- [ ] ChemBERTa-2
- [ ] MolFormer
- [ ] MolT5
- [ ] MACE (MP-0, OFF)
- [ ] Orb

**Medicine**
- [ ] PubMedBERT
- [ ] BioBERT
- [ ] BioGPT
- [ ] BioMistral
- [ ] MedGemma
- [ ] BiomedCLIP
- [ ] MedSAM
- [ ] RAD-DINO
- [ ] UNI
- [ ] CONCH

> Medical models are explored for learning only, not for clinical use.

### Other Domains

**Time Series**
- [ ] TimesFM
- [ ] Chronos
- [ ] Moirai

**Robotics**
- [ ] Octo
- [ ] OpenVLA

**Weather**
- [ ] GraphCast
- [ ] Pangu-Weather

<!--
## Analysis

**Visualization**
- [ ] Attention Maps
- [ ] Embedding Projections (PCA, t-SNE, UMAP)
- [ ] Saliency & Attribution (Grad-CAM, Integrated Gradients)
- [ ] Feature Visualization

**Interpretability**
- [ ] Attention Head Analysis
- [ ] Induction Heads
- [ ] Logit Lens & Tuned Lens
- [ ] Activation Patching
- [ ] Linear Probing (frozen backbone)
- [ ] Sparse Autoencoders

**Embedding Analysis**
- [ ] Similarity & Retrieval
- [ ] Layer-wise Evolution
- [ ] Anisotropy
- [ ] Intrinsic Dimensionality
- [ ] Neighborhood & Cluster Structure
- [ ] CKA (cross-layer, cross-model)

**Comparative Studies**
- [ ] Scale: same family across sizes (ESM-2 8M to 650M, Pythia)
- [ ] Training Dynamics: Pythia intermediate checkpoints
- [ ] Architecture: ResNet vs ViT vs DINOv2 representations
- [ ] Modality: ESM-2 vs DNABERT-2 vs ChemBERTa

tooling - transformerlens, hugging face transformers, timm, open_clip, mlx-lm
interp - neel nanda's mech interp glossary, transformer circuits thread, distill.pub, nostalgebraist's logit lens
protein - rao et al. (attention to contact maps)
pythia - eleutherai suite, checkpoints every 1000 steps
-->
