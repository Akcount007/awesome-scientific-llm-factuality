# Verified References

## Survey and Review Papers
- **Survey of Hallucination in Natural Language Generation**
  Ji, Z., Lee, N., Frieske, R., et al., 2023, *ACM Computing Surveys*
  [DOI: 10.1145/3571730](https://doi.org/10.1145/3571730)
  Provides a comprehensive taxonomy and theoretical background of the hallucination phenomenon across various generation tasks.
- **Siren's Song in the AI Ocean: A Survey on Hallucination in Large Language Models**
  Zhang, Y., Li, Y., Cui, L., et al., 2023, *arXiv*
  [arXiv:2309.01219](https://arxiv.org/abs/2309.01219)
  Examines the underlying causes of hallucinations specifically in LLMs and categorizes current mitigation strategies.
- **A Multitask, Multilingual, Multimodal Evaluation of ChatGPT on Reasoning, Hallucination, and Interactivity**
  Bang, Y., Cahyawijaya, S., Lee, N., et al., 2023, *arXiv*
  [arXiv:2302.04023](https://arxiv.org/abs/2302.04023)
  A massive evaluation demonstrating how advanced conversational agents still fail on specialized reasoning and factual recall tasks.

## Foundational Papers
- **Training language models to follow instructions with human feedback**
  Ouyang, L., Wu, J., Jiang, X., et al., 2022, *arXiv*
  [arXiv:2203.02155](https://arxiv.org/abs/2203.02155)
  Demonstrates that training language models to follow instructions using human feedback (RLHF) improves helpfulness and reduces toxicity[cite: 2].
- **Chain-of-Thought Prompting Elicits Reasoning in Large Language Models**
  Wei, J., Wang, X., Schuurmans, D., et al., 2022, *arXiv*
  [arXiv:2201.11903](https://arxiv.org/abs/2201.11903)
  Shows that step-by-step reasoning significantly improves the ability of large models to perform complex reasoning tasks[cite: 2].
- **Retrieval-Augmented Generation for Knowledge-Intensive NLP Tasks**
  Lewis, P., Perez, E., Piktus, A., et al., 2020, *NeurIPS*
  [Paper Link](https://proceedings.neurips.cc/paper/2020/hash/6b493230205f780e1bc26945df7481e5-Abstract.html)
  The foundational paper introducing RAG to anchor language models to external, verifiable knowledge bases.
- **QAGS: Towards Automated Evaluation of Factuality in Abstractive Summarization**
  Wang, A., Cho, K., & Lewis, M., 2020, *ACL*
  [DOI: 10.18653/v1/2020.acl-main.671](https://aclanthology.org/2020.acl-main.671/)
  Introduces a question-answering framework for evaluating whether generated text remains factually consistent with its source.

## Recent Research and Methods
- **FreshLLMs: Refreshing Large Language Models with Search Engine Augmentation**
  Vu, T., Iyyer, M., Wang, X., et al., 2024, *Findings of ACL*
  [DOI: 10.18653/v1/2024.findings-acl.813](https://aclanthology.org/2024.findings-acl.813/)
  Demonstrates that advanced models struggle with false premises on fast-changing facts unless augmented by real-time search engine data[cite: 2].
- **Shall We Pretrain Autoregressive Language Models with Retrieval? A Comprehensive Study**
  Wang, B., Ping, W., Xu, P., et al., 2023, *EMNLP*
  [DOI: 10.18653/v1/2023.emnlp-main.482](https://aclanthology.org/2023.emnlp-main.482/)
  Concludes that pretraining autoregressive language models with retrieval can moderately improve factual accuracy[cite: 2].
- **SelfCheckGPT: Zero-Resource Black-Box Hallucination Detection for Generative Large Language Models**
  Manakul, P., Liusie, A., & Gales, M. J. F., 2023, *arXiv*
  [arXiv:2303.08896](https://arxiv.org/abs/2303.08896)
  Uses a sampling-based approach to fact-check responses, relying on the premise that hallucinated facts will diverge across multiple stochastic samples[cite: 2].
- **Multi-FAct: Assessing Factuality of Multilingual LLMs using FActScore**
  Shafayat, S., Kim, E., Oh, J., & Oh, A., 2024, *arXiv*
  [arXiv:2402.18045](https://arxiv.org/abs/2402.18045)
  Extends factual evaluation across multiple languages, demonstrating that complex text can be broken down into atomic facts[cite: 2].
- **Fact-Checking Complex Claims with Program-Guided Reasoning**
  Pan, L., Wu, C., Lu, X., et al., 2023, *ACL*
  [DOI: 10.18653/v1/2023.acl-long.385](https://aclanthology.org/2023.acl-long.385/)
  Introduces a methodology to decompose complex scientific claims into logical programs for verifiable fact-checking.
- **FacTool: Factuality Detection in Generative AI - A Tool Augmented Framework**
  Chern, S., Chern, E., Chen, Z., et al., 2023, *arXiv*
  [arXiv:2307.13528](https://arxiv.org/abs/2307.13528)
  Proposes an agnostic framework using external tools (like code interpreters and search) to verify LLM facts in scientific writing.

## Evaluation Methods and Benchmarks
- **TruthfulQA: Measuring How Models Mimic Human Falsehoods**
  Lin, S., Hilton, J., & Evans, O., 2022, *ACL*
  [DOI: 10.18653/v1/2022.acl-long.229](https://aclanthology.org/2022.acl-long.229/)
  A benchmark of adversarial questions designed to trigger false beliefs, revealing that larger language models can imitate widespread human falsehoods[cite: 2].
- **HaluEval: A Large-Scale Hallucination Evaluation Benchmark for Large Language Models**
  Li, J., Cheng, X., Zhao, X., et al., 2023, *EMNLP*
  [DOI: 10.18653/v1/2023.emnlp-main.397](https://aclanthology.org/2023.emnlp-main.397/)
  Utilizes a sampling-then-filtering framework to generate and annotate hallucinated samples[cite: 2].
- **Fact or Fiction: Verifying Scientific Claims**
  Wadden, D., Lin, S., Lo, K., et al., 2020, *EMNLP*
  [DOI: 10.18653/v1/2020.emnlp-main.609](https://aclanthology.org/2020.emnlp-main.609/)
  Introduces the SciFact dataset, containing expert-written scientific claims paired with evidence-containing abstracts[cite: 2].
- **PubMedQA: A Dataset for Biomedical Research Question Answering**
  Jin, Q., Dhingra, B., Liu, Z., et al., 2019, *EMNLP-IJCNLP*
  [DOI: 10.18653/v1/d19-1259](https://aclanthology.org/d19-1259/)
  A question-answering dataset collected directly from PubMed abstracts that requires models to reason over technical biomedical texts[cite: 2].
- **FActScore: Fine-grained Atomic Evaluation of Factual Precision in Long Form Text Generation**
  Min, S., Krishna, K., Lyu, X., et al., 2023, *EMNLP*
  [arXiv:2305.14251](https://arxiv.org/abs/2305.14251)
  Introduces a metric that breaks generated text into atomic facts and verifies them individually against external knowledge bases.
- **GPQA: A Graduate-Level Google-Proof Q&A Benchmark**
  Rein, D., Hou, B., Pang, R. Y., et al., 2023, *arXiv*
  [arXiv:2311.12022](https://arxiv.org/abs/2311.12022)
  A highly challenging dataset of multiple-choice questions in biology, physics, and chemistry.
- **Med-HALT: Medical Domain Hallucination Test for Large Language Models**
  Pal, A., Umapathi, L. K., & Mala, M., 2023, *EMNLP*
  [arXiv:2307.15343](https://arxiv.org/abs/2307.15343)
  Introduces a specific benchmark testing reasoning and memory-based hallucinations in healthcare contexts.
