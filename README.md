# Awesome Scientific LLM Factuality

A curated collection of research papers, datasets, tools, implementations, and learning resources dedicated to benchmarking, evaluating, and improving the factual accuracy of Large Language Models (LLMs) across scientific domains[cite: 2, 3].

## Contents
- [Overview](#overview)
- [AI-Assisted Research Paper](#ai-assisted-research-paper)
- [Citation Integrity Audit](#citation-integrity-audit)
- [Survey and Review Papers](#survey-and-review-papers)
- [Foundational Papers](#foundational-papers)
- [Recent Research and Methods](#recent-research-and-methods)
- [Evaluation Methods and Benchmarks](#evaluation-methods-and-benchmarks)
- [Datasets](#datasets)
- [Tools and Libraries](#tools-and-libraries)
- [GitHub Implementations](#github-implementations)
- [Tutorials and Learning Resources](#tutorials-and-learning-resources)
- [License](#license)

## Overview
The rapid integration of Large Language Models (LLMs) into scientific workflows necessitates rigorous evaluation of their factual accuracy[cite: 2, 3]. While LLMs excel in open-ended text generation, they are prone to producing hallucinations—plausible but incorrect statements—which pose critical risks in high-stakes domains such as medicine, biology, and the physical sciences[cite: 2, 3]. This repository provides a comprehensive review of the current paradigms for benchmarking factual accuracy in LLMs across scientific domains[cite: 2, 3]. It covers foundational datasets (like SciFact and PubMedQA), automated factuality evaluation (like FActScore and SelfCheckGPT), and approaches like retrieval-augmented generation to mitigate factual drift[cite: 2, 3].

## AI-Assisted Research Paper
**Benchmarking Factual Accuracy of Large Language Models Across Scientific Domains**[cite: 2, 3]  
This paper provides a comprehensive review of the current paradigms for benchmarking factual accuracy in LLMs across scientific domains, examining foundational datasets, hallucination mechanisms, and advancements in automated factuality evaluation[cite: 2, 3].  
[View Paper](paper/AI_Assisted_Research_Paper.pdf)[cite: 1]

## Citation Integrity Audit
**Lab 1: AI-Assisted Citation Integrity Audit**[cite: 1, 4]  
This document contains a systematic audit of 10 references generated in the AI-assisted research paper, verifying that the publications exist, all bibliographic details match the scholarly record exactly, and the genuine references support the claims for which they were cited[cite: 1, 4].  
[View Audit](citation-audit/Citation_Integrity_Audit.pdf)[cite: 1]

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
  Demonstrates that training language models to follow instructions using human feedback (RLHF) improves helpfulness and reduces toxicity[cite: 2, 3].
- **Chain-of-Thought Prompting Elicits Reasoning in Large Language Models**
  Wei, J., Wang, X., Schuurmans, D., et al., 2022, *arXiv*
  [arXiv:2201.11903](https://arxiv.org/abs/2201.11903)
  Shows that step-by-step reasoning significantly improves the ability of large models to perform complex reasoning tasks[cite: 2, 3].
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
  Demonstrates that advanced models struggle with false premises on fast-changing facts unless augmented by real-time search engine data[cite: 2, 3].
- **Shall We Pretrain Autoregressive Language Models with Retrieval? A Comprehensive Study**
  Wang, B., Ping, W., Xu, P., et al., 2023, *EMNLP*
  [DOI: 10.18653/v1/2023.emnlp-main.482](https://aclanthology.org/2023.emnlp-main.482/)
  Concludes that pretraining autoregressive language models with retrieval can moderately improve factual accuracy[cite: 2, 3].
- **SelfCheckGPT: Zero-Resource Black-Box Hallucination Detection for Generative Large Language Models**
  Manakul, P., Liusie, A., & Gales, M. J. F., 2023, *arXiv*
  [arXiv:2303.08896](https://arxiv.org/abs/2303.08896)
  Uses a sampling-based approach to fact-check responses, relying on the premise that hallucinated facts will diverge across multiple stochastic samples[cite: 2, 3].
- **Multi-FAct: Assessing Factuality of Multilingual LLMs using FActScore**
  Shafayat, S., Kim, E., Oh, J., & Oh, A., 2024, *arXiv*
  [arXiv:2402.18045](https://arxiv.org/abs/2402.18045)
  Extends factual evaluation across multiple languages, demonstrating that complex text can be broken down into atomic facts[cite: 2, 3].
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
  A benchmark of adversarial questions designed to trigger false beliefs, revealing that larger language models can imitate widespread human falsehoods[cite: 2, 3].
- **HaluEval: A Large-Scale Hallucination Evaluation Benchmark for Large Language Models**
  Li, J., Cheng, X., Zhao, X., et al., 2023, *EMNLP*
  [DOI: 10.18653/v1/2023.emnlp-main.397](https://aclanthology.org/2023.emnlp-main.397/)
  Utilizes a sampling-then-filtering framework to generate and annotate hallucinated samples[cite: 2, 3].
- **Fact or Fiction: Verifying Scientific Claims**
  Wadden, D., Lin, S., Lo, K., et al., 2020, *EMNLP*
  [DOI: 10.18653/v1/2020.emnlp-main.609](https://aclanthology.org/2020.emnlp-main.609/)
  Introduces the SciFact dataset, containing expert-written scientific claims paired with evidence-containing abstracts[cite: 2, 3].
- **PubMedQA: A Dataset for Biomedical Research Question Answering**
  Jin, Q., Dhingra, B., Liu, Z., et al., 2019, *EMNLP-IJCNLP*
  [DOI: 10.18653/v1/d19-1259](https://aclanthology.org/d19-1259/)
  A question-answering dataset collected directly from PubMed abstracts that requires models to reason over technical biomedical texts[cite: 2, 3].
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

## Datasets
- **SciFact**: Contains expert-written scientific claims paired with evidence-containing abstracts, allowing researchers to evaluate whether an AI system can correctly identify if an abstract supports or refutes a claim[cite: 2, 3].
- **PubMedQA**: A novel question-answering dataset collected directly from PubMed abstracts that requires models to answer research questions with yes, no, or maybe[cite: 2, 3].
- **TruthfulQA**: A benchmark comprising adversarial questions designed to trigger false beliefs and measure how models adopt human misconceptions[cite: 2, 3].
- **GPQA**: A graduate-level, Google-proof dataset for testing expert-level domain reasoning in biology, chemistry, and physics.

## Tools and Libraries
- **FActScore**: An automated pipeline extending evaluation across complex text by breaking it down into atomic facts[cite: 2, 3].
- **SelfCheckGPT**: A zero-resource hallucination detection method that uses a sampling-based approach to check black-box model responses[cite: 2, 3].
- **FacTool**: A framework utilizing external code interpreters and search tools to verify AI-generated claims across domains.
- **TruLens**: An open-source tool specifically designed for evaluating and tracking the factual relevance of Retrieval-Augmented Generation (RAG) applications.
- **Ragas**: A metric-driven framework designed to quantitatively score RAG pipelines on factual accuracy and context precision.

## GitHub Implementations
- **[HaluEval Official Repo](https://github.com/RUCAIBox/HaluEval)**: Implements the large-scale hallucination evaluation collection and its generation framework[cite: 2, 3].
- **[SelfCheckGPT Scripts](https://github.com/potsawee/selfcheckgpt)**: Provides zero-resource implementations to test model consistency without external databases[cite: 2, 3].
- **[TruthfulQA Repo](https://github.com/sylinrl/TruthfulQA)**: Codebase for measuring how models mimic widespread human falsehoods[cite: 2, 3].
- **[SciFact Toolkit](https://github.com/allenai/scifact)**: Implementation of baseline models and verification tools for expert-written scientific claims[cite: 2, 3].
- **[FActScore Implementation](https://github.com/shmsw25/factscore)**: Official scripts for atomic fact extraction and scoring against external knowledge.

## Tutorials and Learning Resources
- **Evaluating Factuality in LLMs (Stanford CS224N)**: University-level lecture materials covering the technical mechanisms of hallucination and current mitigation strategies.
- **Hugging Face RAG Documentation**: Authoritative tutorials on integrating Retrieval-Augmented Generation to anchor language models to scientific texts.
- **OpenAI Prompt Engineering Guide**: Official strategies detailing how to force models to provide step-by-step reasoning and cite references to reduce fabrications.
- **LangChain Fact-Checking Guide**: Developer documentation on building AI chains that execute automated verification utilizing search APIs.
- **Survey on Hallucination Mitigation**: A continuously maintained GitHub index tracking the latest algorithmic research on scientific hallucination.

## License
This repository is licensed under the MIT License.
