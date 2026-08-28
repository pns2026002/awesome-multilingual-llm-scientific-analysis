# GitHub Implementations

Curated high-quality GitHub repositories relevant to **Evaluating Multilingual Reliability of LLMs in Scientific Literature Analysis**. Selected based on documentation quality, maintenance activity, reproducibility, and direct relevance to the research topic.

---

## 1. allenai/scibert

| Field | Details |
|-------|---------|
| **Repository** | [https://github.com/allenai/scibert](https://github.com/allenai/scibert) |
| **Stars** | 1,800+ |
| **Maintained by** | Allen Institute for AI (AllenAI) |
| **License** | Apache 2.0 |
| **Related Paper** | SciBERT: A Pretrained Language Model for Scientific Text (Beltagy et al., EMNLP 2019) |

**What it implements**: Fine-tuning and evaluation pipelines for SciBERT — a BERT model pre-trained on 1.14M scientific papers from Semantic Scholar. Includes scripts for NER, PICO extraction, relation classification, and text classification on scientific benchmarks.

**Why relevant**: SciBERT is the primary domain-adapted scientific language model baseline. Understanding its architecture and limitations is essential before extending evaluations to multilingual scientific settings.

---

## 2. facebookresearch/XNLI

| Field | Details |
|-------|---------|
| **Repository** | [https://github.com/facebookresearch/XNLI](https://github.com/facebookresearch/XNLI) |
| **Stars** | 500+ |
| **Maintained by** | Facebook AI Research |
| **License** | CC BY-SA 4.0 |
| **Related Paper** | XNLI: Evaluating Cross-lingual Sentence Representations (Conneau et al., EMNLP 2018) |

**What it implements**: Official XNLI dataset, evaluation scripts, and baseline models for cross-lingual natural language inference across 15 languages. Includes training and evaluation code for multilingual transfer learning baselines.

**Why relevant**: XNLI provides the standard cross-lingual inference evaluation framework; directly applicable to evaluating whether LLMs consistently understand scientific claims across languages.

---

## 3. bigscience-workshop/bigscience

| Field | Details |
|-------|---------|
| **Repository** | [https://github.com/bigscience-workshop/bigscience](https://github.com/bigscience-workshop/bigscience) |
| **Stars** | 2,000+ |
| **Maintained by** | BigScience Workshop (international collaboration) |
| **License** | Apache 2.0 |
| **Related Paper** | BLOOM: A 176B-Parameter Open-Access Multilingual Language Model (2022) |

**What it implements**: Training configurations, evaluation scripts, and documentation for BLOOM — the first open-access 176B multilingual LLM trained on 46 languages. Includes multilingual benchmark evaluation code.

**Why relevant**: BLOOM is the key open-access multilingual LLM for this research topic. Its evaluation framework and training data composition directly inform studies of multilingual scientific text reliability.

---

## 4. allenai/s2orc

| Field | Details |
|-------|---------|
| **Repository** | [https://github.com/allenai/s2orc](https://github.com/allenai/s2orc) |
| **Stars** | 700+ |
| **Maintained by** | Allen Institute for AI (AllenAI) |
| **License** | ODC-By 1.0 |
| **Related Paper** | S2ORC: The Semantic Scholar Open Research Corpus (Lo et al., ACL 2020) |

**What it implements**: Dataset processing pipeline for the Semantic Scholar Open Research Corpus including metadata parsing, full-text extraction, citation linking, and filtering scripts. Handles 81M+ scientific papers.

**Why relevant**: Provides programmatic access to a massive multilingual scientific corpus — the primary data source for training and evaluating multilingual scientific LLMs.

---

## 5. UKPLab/sentence-transformers

| Field | Details |
|-------|---------|
| **Repository** | [https://github.com/UKPLab/sentence-transformers](https://github.com/UKPLab/sentence-transformers) |
| **Stars** | 16,000+ |
| **Maintained by** | UKP Lab, TU Darmstadt |
| **License** | Apache 2.0 |
| **Related Paper** | Sentence-BERT: Sentence Embeddings using Siamese BERT-Networks (Reimers & Gurevych, EMNLP 2019) |

**What it implements**: Training and inference code for multilingual sentence embedding models. Includes pre-trained multilingual models supporting 50+ languages, fine-tuning scripts, and evaluation on semantic textual similarity (STS) benchmarks.

**Why relevant**: Multilingual sentence embeddings enable cross-lingual scientific document similarity search; directly applicable to comparing scientific claim embeddings across languages for consistency analysis.

---

## 6. allenai/longformer

| Field | Details |
|-------|---------|
| **Repository** | [https://github.com/allenai/longformer](https://github.com/allenai/longformer) |
| **Stars** | 2,100+ |
| **Maintained by** | Allen Institute for AI |
| **License** | Apache 2.0 |
| **Related Paper** | Longformer: The Long-Document Transformer (Beltagy et al., 2020) |

**What it implements**: Longformer model code — a Transformer model that scales linearly with sequence length using a combination of local and global attention. Supports processing of full scientific papers (not just abstracts).

**Why relevant**: Scientific papers are long-form documents; Longformer provides the foundation for evaluating LLM comprehension of full multilingual scientific papers beyond 512-token limits.

---

## 7. nlpyang/PRIMERA

| Field | Details |
|-------|---------|
| **Repository** | [https://github.com/allenai/PRIMERA](https://github.com/allenai/PRIMERA) |
| **Stars** | 200+ |
| **Maintained by** | Allen Institute for AI |
| **License** | Apache 2.0 |
| **Related Paper** | PRIMERA: Pyramid-based Masked Sentence Pre-training for Multi-document Summarization (Xiao et al., ACL 2022) |

**What it implements**: Multi-document summarization model for scientific papers trained on the S2ORC corpus. Includes training, inference, and evaluation scripts for cross-document scientific summarization.

**Why relevant**: Multi-document scientific summarization is a key task in evaluating LLM reliability on scientific literature; extending PRIMERA to multilingual settings is a direct research direction for this topic.

---

*Repositories selected based on: documentation quality, maintenance activity, direct relevance to multilingual scientific NLP, reproducible code, and connection to peer-reviewed research. All repository links verified as of August 2026.*
