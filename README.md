# Awesome LTX-2

A curated list of models, text encoders, and tools for the LTX-2 video generation suite.

## Models

LTX-2 models are available in various formats including full weights, transformers-only, and GGUF quantizations for efficient inference.

### Official & Full Models
* **[Lightricks/LTX-2](https://huggingface.co/Lightricks/LTX-2)** - Official repository.
* **[Kijai/LTXV2_comfy](https://huggingface.co/Kijai/LTXV2_comfy/blob/main/diffusion_models/ltx-2-19b-dev_transformer_only_bf16.safetensors)** - BF16 Transformer Only.

### GGUF Quantized Models
These models are optimized for lower memory usage. Note that in ComfyUI, these are typically loaded as transformer-only models.

#### **Unsloth GGUFs**
| File Name | Size | Download |
| :--- | :--- | :--- |
| `ltx-2-19b-dev-BF16.gguf` | 37.8 GB | [Download](https://huggingface.co/unsloth/LTX-2-GGUF/resolve/main/ltx-2-19b-dev-BF16.gguf?download=true) |
| `ltx-2-19b-dev-Q8_0.gguf` | 20.4 GB | [Download](https://huggingface.co/unsloth/LTX-2-GGUF/resolve/main/ltx-2-19b-dev-Q8_0.gguf?download=true) |
| `ltx-2-19b-dev-Q6_K.gguf` | 16.0 GB | [Download](https://huggingface.co/unsloth/LTX-2-GGUF/resolve/main/ltx-2-19b-dev-Q6_K.gguf?download=true) |
| `ltx-2-19b-dev-Q4_K_M.gguf` | 12.8 GB | [Download](https://huggingface.co/unsloth/LTX-2-GGUF/resolve/main/ltx-2-19b-dev-Q4_K_M.gguf?download=true) |
| `ltx-2-19b-dev-Q4_0.gguf` | 11.3 GB | [Download](https://huggingface.co/unsloth/LTX-2-GGUF/resolve/main/ltx-2-19b-dev-Q4_0.gguf?download=true) |

#### **Vantage AI GGUFs (Dev)**
| File Name | Size | Download |
| :--- | :--- | :--- |
| `ltx-2-19b-dev-Q8_0.gguf` | 20.4 GB | [Download](https://huggingface.co/vantagewithai/LTX-2-GGUF/resolve/main/dev/ltx-2-19b-dev-Q8_0.gguf?download=true) |
| `ltx-2-19b-dev-Q6_K.gguf` | 15.9 GB | [Download](https://huggingface.co/vantagewithai/LTX-2-GGUF/resolve/main/dev/ltx-2-19b-dev-Q6_K.gguf?download=true) |
| `ltx-2-19b-dev-Q4_K_M.gguf` | 12.8 GB | [Download](https://huggingface.co/vantagewithai/LTX-2-GGUF/resolve/main/dev/ltx-2-19b-dev-Q4_K_M.gguf?download=true) |

*   **Other GGUF Sources:** [QuantStack/LTX-2-GGUF](https://huggingface.co/QuantStack/LTX-2-GGUF)

---

## Text Encoders

LTX-2 requires Gemma-3-12b variants.

### **Comfy-Org Optimized Encoders**
Official and optimized versions for ComfyUI.

| Model Name | Size | Download |
| :--- | :--- | :--- |
| `gemma_3_12B_it.safetensors` | 24.1 GB | [Link](https://huggingface.co/Comfy-Org/ltx-2/blob/main/split_files/text_encoders/gemma_3_12B_it.safetensors) |
| `gemma_3_12B_it_fpmixed.safetensors` | 12.2 GB | [Link](https://huggingface.co/Comfy-Org/ltx-2/blob/main/split_files/text_encoders/gemma_3_12B_it_fpmixed.safetensors) |
| `gemma_3_12B_it_fp8_scaled.safetensors` | 12.3 GB | [Link](https://huggingface.co/Comfy-Org/ltx-2/blob/main/split_files/text_encoders/gemma_3_12B_it_fp8_scaled.safetensors) |
| `gemma_3_12B_it_fp4_mixed.safetensors` | 7.02 GB | [Link](https://huggingface.co/Comfy-Org/ltx-2/blob/main/split_files/text_encoders/gemma_3_12B_it_fp4_mixed.safetensors) |

### **FusionCow Gemma-3-12b Abliterated**
Fixed versions of the abliterated Gemma-3-12b-it model, modified specifically for compatibility with LTX-2.

| Model Name | Size | Download |
| :--- | :--- | :--- |
| `gemma_ablit_fixed_bf16.safetensors` | 24.1 GB | [Link](https://huggingface.co/FusionCow/Gemma-3-12b-Abliterated-LTX2/blob/main/gemma_ablit_fixed_bf16.safetensors) |
| `gemma_ablit_fixed_fp8.safetensors` | 12.3 GB | [Link](https://huggingface.co/FusionCow/Gemma-3-12b-Abliterated-LTX2/blob/main/gemma_ablit_fixed_fp8.safetensors) |

---

## Separated Components

### VAE (Video & Audio)
| Component | Download Link |
| :--- | :--- |
| **Video VAE (BF16)** | [Download](https://huggingface.co/Kijai/LTXV2_comfy/blob/main/VAE/LTX2_video_vae_bf16.safetensors) |
| **Audio VAE (BF16)** | [Download](https://huggingface.co/Kijai/LTXV2_comfy/blob/main/VAE/LTX2_audio_vae_bf16.safetensors) |

### Diffusion Models (Transformer Only)
*   [ltx-2-19b-dev-bf16](https://huggingface.co/Kijai/LTXV2_comfy/blob/main/diffusion_models/ltx-2-19b-dev_transformer_only_bf16.safetensors)
*   [ltx-2-19b-dev-fp8](https://huggingface.co/Kijai/LTXV2_comfy/blob/main/diffusion_models/ltx-2-19b-dev-fp8_transformer_only.safetensors)
*   [ltx-2-19b-distilled-fp8](https://huggingface.co/Kijai/LTXV2_comfy/blob/main/diffusion_models/ltx-2-19b-distilled-fp8_transformer_only.safetensors)

### Embedding Connectors
*   [Dev BF16 Connector](https://huggingface.co/Kijai/LTXV2_comfy/blob/main/text_encoders/ltx-2-19b-embeddings_connector_dev_bf16.safetensors)
*   [Distill BF16 Connector](https://huggingface.co/Kijai/LTXV2_comfy/blob/main/text_encoders/ltx-2-19b-embeddings_connector_distill_bf16.safetensors)

---

## LoRA
*   [LTX-2-19b-LoRA-SPROUT](https://huggingface.co/oumoumad/LTX-2-19b-LoRA-SPROUT)

---

##  Workflow & Technical Notes
