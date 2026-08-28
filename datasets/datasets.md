# Datasets

Curated datasets relevant to **Evaluating Multilingual Reliability of Large Language Models in Scientific Literature Analysis**. Each entry includes name, source, description, application, and access link. All links verified as of August 2026.

---

## 1. XNLI — Cross-lingual Natural Language Inference

| Field | Details |
|-------|---------|
| **Name** | XNLI (Cross-lingual Natural Language Inference) |
| **Source** | Facebook AI Research (Conneau et al., EMNLP 2018) |
| **Languages** | 15 languages (English, French, Spanish, German, Greek, Bulgarian, Russian, Turkish, Arabic, Vietnamese, Thai, Chinese, Hindi, Swahili, Urdu) |
| **Size** | ~5,000 hypothesis-premise pairs per language for dev/test |
| **License** | Creative Commons Attribution-ShareAlike 4.0 |
| **Link** | [https://github.com/facebookresearch/XNLI](https://github.com/facebookresearch/XNLI) |

**Description**: XNLI extends MultiNLI to 15 languages through human translation. Each sentence pair is labeled as entailment, neutral, or contradiction. It is the standard benchmark for evaluating cross-lingual language understanding.

**Application in this topic**: Used to evaluate whether LLMs can consistently classify the logical relationship between scientific claims across languages — a direct proxy for scientific claim verification reliability.

---

## 2. SciERC — Scientific Information Extraction Corpus

| Field | Details |
|-------|---------|
| **Name** | SciERC |
| **Source** | University of Washington NLP (Luan et al., EMNLP 2018) |
| **Languages** | English |
| **Size** | 500 scientific abstracts with entity, relation, and coreference annotations |
| **Domain** | NLP, machine learning, and AI research papers |
| **License** | Research use |
| **Link** | [http://nlp.cs.washington.edu/sciIE/](http://nlp.cs.washington.edu/sciIE/) |

**Description**: SciERC provides fine-grained annotations of scientific entities (Task, Method, Metric, Material, Generic, Other Scientific Term), coreference links, and semantic relations from AI/ML paper abstracts.

**Application in this topic**: Baseline dataset for evaluating scientific named entity recognition and relation extraction; used to test whether multilingual models can perform equivalent extraction in non-English scientific text.

---

## 3. PubMedQA — Biomedical Question Answering

| Field | Details |
|-------|---------|
| **Name** | PubMedQA |
| **Source** | Jin et al., EMNLP 2019 |
| **Languages** | English (multilingual extension available) |
| **Size** | 1,000 expert-annotated QA pairs + 61,000 unlabeled + 211,000 artificially generated |
| **Domain** | Biomedical/PubMed literature |
| **License** | CC BY 4.0 |
| **Link** | [https://pubmedqa.github.io/](https://pubmedqa.github.io/) |

**Description**: PubMedQA is a biomedical QA dataset where each question is derived from a PubMed abstract title, and answers (yes/no/maybe) are drawn from the abstract conclusions. It evaluates reasoning over scientific literature.

**Application in this topic**: Core benchmark for scientific QA reliability; when combined with translated versions, it enables cross-lingual reliability comparison for LLMs on biomedical literature.

---

## 4. FEVER — Fact Extraction and VERification

| Field | Details |
|-------|---------|
| **Name** | FEVER 1.0 |
| **Source** | Thorne et al., NAACL 2018 |
| **Languages** | English (with cross-lingual extensions) |
| **Size** | 185,445 claims with evidence annotations from Wikipedia |
| **License** | CC BY-SA 3.0 |
| **Link** | [https://fever.ai/](https://fever.ai/) |

**Description**: FEVER requires systems to verify claims against a large text corpus, labeling each as SUPPORTED, REFUTED, or NOT ENOUGH INFO with evidence retrieval. It is the standard fact-verification benchmark adapted for scientific claim checking.

**Application in this topic**: Scientific claim verification pipeline evaluation; extended multilingual FEVER datasets test whether LLMs maintain factual reliability across languages.

---

## 5. CC-100 — Multilingual Web Crawl Corpus

| Field | Details |
|-------|---------|
| **Name** | CC-100 |
| **Source** | Conneau et al., ACL 2020 (used for XLM-R pre-training) |
| **Languages** | 100 languages |
| **Size** | ~2.5 TB of deduplicated web text |
| **License** | Common Crawl Terms of Use |
| **Link** | [http://data.statmt.org/cc-100/](http://data.statmt.org/cc-100/) |

**Description**: CC-100 is a massive multilingual web text corpus derived from Common Crawl, filtered and deduplicated per language. It is the pre-training corpus for XLM-R and a standard resource for studying language representation imbalances.

**Application in this topic**: Analyzing training data composition across languages to understand why LLMs show reliability gaps in lower-resource languages for scientific tasks; also used for fine-tuning multilingual scientific models.

---

## 6. S2ORC — Semantic Scholar Open Research Corpus

| Field | Details |
|-------|---------|
| **Name** | S2ORC (Semantic Scholar Open Research Corpus) |
| **Source** | Lo et al., ACL 2020 |
| **Languages** | English-dominant, with multilingual documents |
| **Size** | 81.1 million English papers + metadata; full-text available for ~8.1 million |
| **License** | ODC-By 1.0 |
| **Link** | [https://github.com/allenai/s2orc](https://github.com/allenai/s2orc) |

**Description**: S2ORC is a large-scale scholarly paper corpus spanning 19 scientific domains. It includes structured full-text, citations, and metadata. Increasingly used as source for multilingual scientific NLP benchmarks.

**Application in this topic**: Provides structured scientific literature for pre-training and evaluation; can be filtered by language to study cross-lingual scientific text understanding.

---

*All datasets listed have been verified for accessibility as of August 2026.*
