# Jonathan Mamou

Senior AI Research Scientist & Engineer at **Intel** | 20+ years of industrial research (Intel Labs, IBM Research)

I work on making LLM inference faster and more efficient -- speculative decoding, CPU optimization, and serving infrastructure.

---

## What I'm working on

- **Speculative decoding** -- adaptive token scheduling, vocabulary-aware drafting, heterogeneous vocabularies (TLI, SLEM)
- **CPU inference optimization** -- bringing speculative decoding and high-throughput serving to Intel Xeon platforms
- **LLM serving infrastructure** -- contributing to vLLM and SGLang for production-grade inference

## Selected publlic contributions

### Speculative Decoding with Heterogeneous Vocabularies -- ICML 2025 (top 1%)
Enabling speculative decoding when draft and target models use different tokenizers.
- [TLI](https://github.com/sgl-project/sglang/pull/22883) -- Token-Level Intersection enabling any draft model regardless of tokenizer
- [SLEM](https://github.com/vllm-project/vllm/pull/45018) -- cross-vocabulary speculative decoding 

### Hugging Face Transformers
- [Dynamic speculative token count](https://github.com/huggingface/transformers/pull/33258) -- adaptive scheduling that improves acceptance rates
- [Adaptive dynamic speculative tokens](https://github.com/huggingface/transformers/pull/34156) -- further acceleration via heuristic scheduling
- [LM Head pruning for USD](https://github.com/huggingface/transformers/pull/36695) -- vocabulary mismatch handling for Universal Speculative Decoding
- [Default behavior of assisted decoding](https://github.com/huggingface/transformers/pull/33657) -- setting speculative decoding defaults for the ecosystem

### vLLM
- [Grammar-aware draft token sampling for structured outputs](https://github.com/vllm-project/vllm/pull/47885) -- constrained decoding during speculative drafting
- [Dynamic speculation length with confidence-threshold early exit](https://github.com/vllm-project/vllm/pull/35301) -- adaptive draft length based on model confidence
- [CPU spec decode stream fix](https://github.com/vllm-project/vllm/pull/47162) -- removing incorrect overrides in CPUModelRunner
- [Spec decode kernel compatibility](https://github.com/vllm-project/vllm/pull/44991) -- Triton-CPU integration
- [CPU rotary embedding fix](https://github.com/vllm-project/vllm/pull/44419) -- fixing CPU path without flash-attn ops

### SGLang
- [Vocabulary compatibility validation](https://github.com/sgl-project/sglang/pull/23838) -- safety checks for speculative decoding in standalone mode
- [SPEED-Bench dataset support](https://github.com/sgl-project/sglang/pull/24149) -- new benchmark dataset for serving evaluation

### Distributed Speculative Inference
- [Distributed Speculative Inference (DSI)](https://github.com/keyboardAnt/distributed-speculative-inference) -- co-developed implementation for distributed draft-target decoding
- [Redistributing Drafter Kernels](https://github.com/jmamou/redistributing-drafter-kernels) -- target distribution pruning and analysis for speculative decoding efficiency

## Connect

[<img src="https://img.shields.io/badge/LinkedIn-0A66C2?style=flat&logo=linkedin&logoColor=white" alt="LinkedIn" />](https://www.linkedin.com/in/jonathan-mamou-65366564/)
&nbsp;
[<img src="https://img.shields.io/badge/Google_Scholar-4285F4?style=flat&logo=google-scholar&logoColor=white" alt="Google Scholar" />](https://scholar.google.com/citations?user=96pR-j0AAAAJ&hl=en)
&nbsp;
[<img src="https://img.shields.io/badge/Patents-34A853?style=flat&logo=google&logoColor=white" alt="Google Patents" />](https://patents.google.com/?inventor=jonathan+mamou&oq=jonathan+mamou)
