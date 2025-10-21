# Awesome-LLM-based-Text2SQL

<div align="center">
    <a href="https://awesome.re"><img src="https://awesome.re/badge.svg"/></a>
    <a href="http://makeapullrequest.com"><img src="https://img.shields.io/badge/PRs-welcome-green.svg"/></a>
    <a href="http://makeapullrequest.com"><img src="https://img.shields.io/github/stars/DEEP-PolyU/Awesome-LLM-based-Text2SQL"/></a>
    <a href="http://makeapullrequest.com"><img src="https://img.shields.io/github/forks/DEEP-PolyU/Awesome-LLM-based-Text2SQL"/></a>
      <a href="http://makeapullrequest.com"><img src="https://img.shields.io/github/last-commit/DEEP-PolyU/Awesome-LLM-based-Text2SQL?color=blue"/></a>
</div>

This repository provides a comprehensive collection of research papers, benchmarks, and open-source projects on **large language model-based text-to-SQL (LLM-based Text-to-SQL)**. It includes all the contents from our survey paper 📖<em>"[**Next-Generation Database Interfaces: A Survey of LLM-based Text-to-SQL**](https://arxiv.org/pdf/2406.08426)"</em> and will be continuously updated to incorporate the up-to-date advances and notable contributions from the text-to-SQL community. Stay tuned!!

🤗 **You are vey welcome to contribute to this repository** by launching an issue or a pull request. If you find any missing resources or come across interesting new research works, please don’t hesitate to open an issue or submit a PR!

📫 **Contact us via emails:**  `zijin[dot]hong[at]connect[dot]polyu[dot]hk`

**📃 Please [cite our paper](#-citation)** if you find our survey or repository helpful!

## 🔥 News

* **[2025-10-21]** 🎉🎉 Our paper *"Knapsack Optimization-based Schema Linking for LLM-based Text-to-SQL Generation"* has been **accepted by *IEEE International Conference on Data Engineering (ICDE)*!**
* **[2025-09-21]** 🔥🔥 Finished building the benchmarks, datasets, and taxonomy for this repository.
* **[2025-09-14]** 🔥🔥 Repository launched based on our survey paper to keep track of recent progress in LLM-based text-to-SQL.
* **[2025-09-02]** 🎉🎉 Our paper *"Next-Generation Database Interfaces: A Survey of LLM-based Text-to-SQL"* has been **accepted by *IEEE Transactions on Knowledge and Data Engineering (TKDE)*!**
* **[2025-05-01]** 🎉🎉 Our paper *"Struture-Guided Large Language Models for Text-to-SQL Generation"* has been **accepted by *International Conference of Machine Learning (ICML)*!**

---

<div>
<h3 align="center">
       <p align="center"><img width="80%" src="figures/overview.svg" /></p>
    <p align="center"><em>Overview of LLM-based Text-to-SQL Workflow </em></p>
</div>
A user asks a question about football leagues. The LLM takes this question together with the schema of the corresponding database as input and generates an SQL query as output. The generated SQL is then executed on the database, retrieving the result <em>"The 5 leagues with the highest matches"</em>, which answers the user's question.

## 📜 Catalog

> **[Awesome-LLM-based-Text2SQL](#-awesome-llm-based-text2sql)**
>
>  - **[🔥 News](#-news)**
>  - **[📜 Catalog](#-catalog)**
>  - **[📈 Trends](#-trends)**
>  - **[📰 Surveys](#-surveys)**
>  - **[🏆 Benchmarks](#-benchmarks)**
>  - **[🗃️ Datasets](#️-datasets)**
>    - [Original Datasets](#original-datasets)
>    - [Post-annotated Datasets](#post-annotated-datasets)
>  - **[🪴 Taxonomy](#-taxonomy)**
>    - [In-cotext Learning](#in-context-learning)
>    - [Fine-tuning](#fine-tuning)
>  - **[📦 Projects](#-projects)**
>  - **[📃 Citation](#-citation)**

---


## 📈 Trends

<div>
<h3 align="center">
       <p align="center"><img width="100%" src="figures/trends.svg" /></p>
    <p align="center"><em>A Sketch of Research Trends in the Field of Text-to-SQL with Representative Works </em></p>
</div>
Before 2023, the focus is on a selection of representative traditional studies. However, from 2023 onward, the emphasis shifts to the rapid advancements driven by LLMs, marking a significant acceleration in the field.

## 📰 Surveys

* ![TKDE](https://img.shields.io/badge/TKDE2025-FF6347) Next-Generation Database Interfaces: A Survey of LLM-based Text-to-SQL [[Paper](https://ieeexplore.ieee.org/abstract/document/11160657)] [[Code]()]
* ![CSUR2025](https://img.shields.io/badge/CSUR2025-3CB371) A Survey on Employing Large Language Models for Text-to-SQL Tasks [[Paper]()]
* ![TKDE](https://img.shields.io/badge/TKDE2025-FF6347?style=flat) A Survey of Text-to-SQL in the Era of LLMs: Where are We, and Where are We Going? [[Paper]()]
* ![TKDE](https://img.shields.io/badge/TKDE2024-FF6347?style=flat) Natural Language Interfaces for Tabular Data Querying and Visualization: A Survey [[Paper]()]
* ![arXiv2024](https://img.shields.io/badge/arXiv2024-B31B1B) Large Language Model Enhanced Text-to-SQL Generation: A Survey [[Paper]()]
* ![VLDBJ2023](https://img.shields.io/badge/VLDBJ2023-4B0082) A Survey on Deep Learning Approaches for Text-to-SQL [[Paper]()]
* ![VLDB2023](https://img.shields.io/badge/VLDB2023-800080) Natural Language Interfaces for Databases with Deep Learning [[Paper]()]
* ![arXiv2022](https://img.shields.io/badge/arXiv2022-B31B1B) A Survey on Text-to-SQL Parsing: Concepts, Methods, and Future Directions [[Paper]()]
* ![COLING2022](https://img.shields.io/badge/COLING2022-00CED1) Recent Advances in Text-to-SQL: A Survey of What We Have and What We Expect [[Paper]()]

## 🏆 Benchmarks

In the era of LLMs, two benchmarks and their variants/extensions are widely recognized for evaluating text-to-SQL capabilities. **We will continually update the top five methods on each benchmark** to showcase the latest advances in the text-to-SQL community. These benchmarks, along with other text-to-SQL dataset papers, are listed in the [datasets section](#-datasets) below.

#### [BIRD](https://bird-bench.github.io/) - A Big Bench for Large-Scale Database Grounded Text-to-SQL


| Method/Model | Dev EX (%) | Test EX (%) | Paper/Code | Date |
|--------------|------------|-------------|------------|------|
| ![arXiv2025](https://img.shields.io/badge/Proprietary-lightgray) Agentar-Scale-SQL | 74.90 | **81.67** | [[Paper](https://arxiv.org/pdf/2509.24403)] | 2025-09-25 |
| ![arXiv2025](https://img.shields.io/badge/arXiv2025-B31B1B) AskData + GPT-4o | **76.14** | 80.88 | [[Paper](https://arxiv.org/pdf/2505.19988)] | 2025-03-11 |
| ![Proprietary](https://img.shields.io/badge/Proprietary-lightgray) LongData-SQL | 74.32 | 77.53 | [<u>Proprietary</u>] | 2025-07-14 |
| ![ICLR2025](https://img.shields.io/badge/ICLR2025-7CFC00) CHASE-SQL + Gemini | 74.90 | 76.02 | [[Paper](https://openreview.net/pdf?id=CvGqMD5OtX)] | 2025-04-16 |
| ![Proprietary](https://img.shields.io/badge/Proprietary-lightgray) JoyDataAgent-SQL | 74.25 | 75.74 | [[Report](https://github.com/jd-opensource/joyagent-jdgenie/blob/data_agent/README_DataAgent.md)] [[Code](https://github.com/jd-opensource/joyagent-jdgenie/tree/data_agent)] | 2025-09-22 |
| ![Proprietary](https://img.shields.io/badge/Proprietary-lightgray) TCDataAgent-SQL | 74.12 | 75.74 | [[Report](https://cloud.tencent.com/developer/article/2537769)] | 2025-05-30 |
| ![Proprietary](https://img.shields.io/badge/Proprietary-lightgray) Contextual-SQL | 73.50 | 75.63 | [[Report](https://contextual.ai/blog/open-sourcing-the-best-local-text-to-sql-system/)] [[Code](https://github.com/ContextualAI/bird-sql)] | 2025-02-27 |
| ![arXiv2024](https://img.shields.io/badge/arXiv2024-B31B1B) XiYan-SQL | 73.34 | 75.63 | [[Paper](https://arxiv.org/pdf/2411.08599)] [[Code](https://github.com/XGenerationLab/XiYan-SQL)] | 2024-12-17 |

---

#### [Spider1.0](https://yale-lily.github.io/spider) - Semantic Parsing and Text-to-SQL Challenge

| Method/Model | Dev EX (%) | Test EX (%) | Paper/Code | Date |
|--------------|------------|-------------|------------|------|
| ![Proprietary](https://img.shields.io/badge/Proprietary-lightgray) MiniSeek | - | **91.2** | [[Report](https://www.seek.ai/blog/miniseek-first-model-to-surpass-90-accuracy-on-spider-test-benchmark)] | 2023-11-02 |
| ![VLDB2024](https://img.shields.io/badge/VLDB2024-800080) DAIL-SQL + GPT-4 | **82.4** | 86.6 | [[Paper](https://www.vldb.org/pvldb/vol17/p1132-gao.pdf)] [[Code](https://github.com/BeachWang/DAIL-SQL)] | 2023-08-20 |
| ![NeurIPS2025](https://img.shields.io/badge/NeurIPS2025-2E8B57) DIN-SQL + GPT-4 | 74.2 | 85.3 | [[Paper](https://openreview.net/pdf?id=p53QDxSIc5)] [[Code](https://github.com/MohammadrezaPourreza/Few-shot-NL2SQL-with-prompting)] | 2023-04-21 |
| ![arXiv2023](https://img.shields.io/badge/arXiv2023-B31B1B) C3 + ChatGPT | 81.8 | 82.3 | [[Paper](https://arxiv.org/pdf/2307.07306)] [[Code](https://github.com/bigbigwatermalon/C3SQL)] | 2023-06-01 |
| ![AAAI2025](https://img.shields.io/badge/AAAI2025-006400) RESDSQL-3B + NatSQL | 84.1 | 79.9 | [[Paper](https://arxiv.org/pdf/2302.05965)] [[Code](https://github.com/RUCKBReasoning/RESDSQL)] | 2023-02-27 |

---

#### [Spider2.0](https://spider2-sql.github.io/) - Evaluating Language Models on Real-World Enterprise Text-to-SQL Workflows

| Method/Model | Snow Score | Lite Score | Paper/Code | Date |
|--------------|------------|----------------|------------|------|
| ![arXiv2025](https://img.shields.io/badge/arXiv2025-B31B1B) AgenticData + Qwen3 | - | **44.5** | [[Paper](https://arxiv.org/pdf/2508.05002)] | 2025-08-07 |
| ![ICLR2025](https://img.shields.io/badge/ICLR2025Workshop-7CFC00) ReFoRCE + o3 | **37.11** | 37.84 | [[Paper](https://openreview.net/pdf?id=OuFIfDBwQd)] [[Code](https://github.com/Snowflake-Labs/ReFoRCE)] | 2025-05-22 |
| ![arXiv2024](https://img.shields.io/badge/arXiv2024-B31B1B) RSL-SQL + o3 | - | 33.09 | [[Paper](https://arxiv.org/pdf/2411.00073)] [[Code](https://github.com/Laqcce-cao/RSL-SQL)] | 2025-07-10 |
| ![EMNLP2025](https://img.shields.io/badge/EMNLP2025-00BFFF) LinkAlign + DeepSeek-R1 | - | 33.09 | [[Paper](https://arxiv.org/pdf/2503.18596)] [[Code](https://github.com/Satissss/LinkAlign)] | 2025-04-27 |
| ![ICLR2025](https://img.shields.io/badge/ICLR2025-7CFC00) Spider-Agent + Claude-3.7-Sonnet | - | 28.52 | [[Paper](https://openreview.net/pdf?id=XmProj9cPs)] [[Code](https://github.com/xlang-ai/Spider2)] | 2025-03-16 |

---

#### [BIRD-CRITIC](https://bird-critic.github.io/) - Can LLMs Fix User Issues in Real-World Database Applications?


| Model | SR (%) | Date |
|-------|--------|------|
| ByteBrain-Agent | **43.33** | 2025-06-10 |
| GPT-5-High | 34.96 | 2025-09-04 |
| grok-4 | 33.68 | 2025-07-18 |
| DeepSeek-R1 | 33.51 | 2025-04-20 |
| o3-Mini | 33.33 | 2025-04-20 |

---

#### [BIRD-INTERACT](https://bird-interact.github.io/) - Re-imagining Text-to-SQL Evaluation via Lens of Dynamic Interactions


| Model/Method | Reward | Date |
|--------------|--------|------|
| Gemini-2.5-Pro | **20.92** | 2025-08-22 |
| o3-Mini | 20.27 | 2025-08-22 |
| Claude-Sonnet-4 | 18.35 | 2025-08-22 |
| Qwen-3-Coder-480B | 17.75 | 2025-08-22 |
| DeepSeek-V3 | 15.15 | 2025-08-22 |

## 🗃️ Datasets

**We categorize the datasets into *Original Datasets* and *Post-annotated Datasets*** based on whether they were released with the original dataset (question–SQL pairs) and databases, or were developed by adapting existing datasets and databases with special settings. The *Post-annotated Datasets* rely on the databases from [Spider 1.0](https://yale-lily.github.io/spider). For each original dataset, we list its characteristics, number of examples, and number of databases under the dataset title.

### Original Datasets

* ![arXiv2025](https://img.shields.io/badge/arXiv2025-B31B1B) **BIRD-CRITIC** | SWE-SQL: Illuminating LLM Pathways to Solve User SQL Issues in Real-World Applications [[Paper]()] [[Code]()] [[Dataset]()]<br>
  *Knowledge-augmented, Long-context; #Example: 600; #DB: 95*
* ![ICLR2025](https://img.shields.io/badge/ICLR2025-7CFC00) **Spider2.0** | Spider 2.0: Evaluating Language Models on Real-world Enterprise Text-to-SQL Workflows [[Paper](https://openreview.net/pdf?id=XmProj9cPs)] [[Code](https://github.com/xlang-ai/Spider2)] [[Dataset](https://github.com/xlang-ai/Spider2/blob/main/spider2-lite/spider2-lite.jsonl)]<br>
  *Knowledge-augmented, Long-context; #Example: 632; #DB: 213*
* ![SIGMOD2025](https://img.shields.io/badge/SIGMOD2025-8A2BE2) **BULL** | FinSQL: Model-Agnostic LLMs-based Text-to-SQL Framework for Financial Analysis [[Paper](https://arxiv.org/pdf/2401.10506)] [[Code](https://github.com/bigbigwatermalon/FinSQL)] [[Dataset](https://drive.google.com/file/d/1OtyFdH9cs-6bEVj8yKK4Zt53N52L_dBH/view?usp=sharing)]<br>
  *Knowledge-augmented, Long-context; #Example: 4,966; #DB: 3*
* ![NeurIPS2023](https://img.shields.io/badge/NeurIPS2023-2E8B57) **BIRD** | Can LLM Already Serve as A Database Interface? A BIg Bench for Large-Scale Database Grounded Text-to-SQLs [[Paper](https://openreview.net/pdf?id=dI4wzAE6uV)] [[Code]()] [[Dataset]()]<br>
  *Cross-domain, Knowledge-augmented; #Example: 12,751; #DB: 95*
* ![ACL2021](https://img.shields.io/badge/ACL2021-1E90FF) **KaggleDBQA** | KaggleDBQA: Realistic Evaluation of Text-to-SQL Parsers [[Paper](https://aclanthology.org/2021.acl-long.176.pdf)] [[Code](https://github.com/Chia-Hsuan-Lee/KaggleDBQA)] [[Dataset]()]<br>
  *Cross-domain; #Example: 272; #DB: 8*
* ![EMNLP2020](https://img.shields.io/badge/EMNLP2020-00BFFF) **DuSQL** | DuSQL: A Large-Scale and Pragmatic Chinese Text-to-SQL Dataset [[Paper](https://aclanthology.org/2020.emnlp-main.562.pdf)] [[Dataset](https://www.luge.ai/#/luge/dataDetail?id=13)]<br>
  *Cross-domain, Cross-lingual; #Example: 23,797; #DB: 200*
* ![Findings2020](https://img.shields.io/badge/EMNLP2020Findings-87CEFA) **SQUALL** | On the Potential of Lexico-logical Alignments for Semantic Parsing to SQL Queries [[Paper](https://aclanthology.org/2020.findings-emnlp.167.pdf)] [[Code](https://github.com/tzshi/squall)] <br>
  *Cross-domain, Cross-lingual; #Example: 11,468; #DB: 1,679*
* ![EMNLP2019](https://img.shields.io/badge/EMNLP2019-00BFFF) **CoSQL** | CoSQL: A Conversational Text-to-SQL Challenge Towards Cross-Domain Natural Language Interfaces to Databases [[Paper](https://aclanthology.org/D19-1204.pdf)] [[Code](https://github.com/taoyds/cosql)] [[Dataset](https://drive.usercontent.google.com/download?id=1Y3ydpFiQQ3FC0bzdfy3groV95O_f1nXF&export=download&authuser=0)]<br>
  *Cross-domain, Context-dependent; #Example: 15,598; #DB: 200*
* ![EMNLP2018](https://img.shields.io/badge/EMNLP2018-00BFFF) **Spider** | Spider: A Large-Scale Human-Labeled Dataset for Complex and Cross-Domain Semantic Parsing and Text-to-SQL Task [[Paper](https://aclanthology.org/D18-1425.pdf)] [[Code](https://github.com/taoyds/spider)] [[Dataset](https://drive.google.com/file/d/1403EGqzIDoHMdQF4c9Bkyl7dZLZ5Wt6J/view)]<br>
  *Cross-domain; #Example: 10,181; #DB: 200*
* ![arXiv2017](https://img.shields.io/badge/arXiv2017-B31B1B) **WikiSQL** | Seq2SQL: Generating Structured Queries from Natural Language using Reinforcement Learning [[Paper](https://arxiv.org/pdf/1709.00103)] [[Code](https://github.com/salesforce/WikiSQL)] [[Dataset](https://github.com/salesforce/WikiSQL/tree/master/collection)]<br>
  *Cross-domain; #Example: 80,654; #DB: 26,521*

### Post-annotated Datasets

* ![ICLR2023](https://img.shields.io/badge/ICLR2023-7CFC00) **Dr. Spider** | Dr.Spider: A Diagnostic Evaluation Benchmark towards Text-to-SQL Robustness [[Paper](https://openreview.net/pdf?id=Wc5bmZZU9cy)] [[Code](https://github.com/awslabs/diagnostic-robustness-text-to-sql)]<br>
  *Robustness; Perturbations in DB, query and SQL*
* ![ACL2022](https://img.shields.io/badge/ACL2022-1E90FF) **ADVETA** | Towards Robustness of Text-to-SQL Models Against Natural and Realistic Adversarial Table Perturbation [[Paper](https://aclanthology.org/2022.acl-long.142.pdf)] [[Code](https://github.com/microsoft/ContextualSP/tree/master/robustness_of_text_to_sql)] [[Dataset](https://github.com/microsoft/ContextualSP/blob/master/robustness_of_text_to_sql/adveta_1.0.zip)]<br>
  *Robustness; Adversarial table perturbation*
* ![Findings2022](https://img.shields.io/badge/NAACL2022Findings-87CEFA) **Spider-SS&CG** | Measuring and Improving Compositional Generalization in Text-to-SQL via Component Alignment [[Paper](https://aclanthology.org/2022.findings-naacl.62.pdf)] [[Code](https://github.com/ygan/SpiderSS-SpiderCG)] [[Dataset](https://github.com/ygan/SpiderSS-SpiderCG/tree/main/Spider-SS)]<br>
  *Context-dependent; Splitting example into sub-examples*
* ![EMNLP2021](https://img.shields.io/badge/EMNLP2021-00BFFF) **Spider-DK** | Exploring Underexplored Limitations of Cross-Domain Text-to-SQL Generalization [[Paper](https://aclanthology.org/2021.emnlp-main.702.pdf)] [[Code](https://github.com/ygan/Spider-DK)]<br>*Knowledge-augmented; Adding domain knowledge*
*  ![ACL2021](https://img.shields.io/badge/ACL2021-1E90FF) **Spider-SYN** | Towards Robustness of Text-to-SQL Models against Synonym Substitution [[Paper](https://aclanthology.org/2021.acl-long.195.pdf)] [[Code](https://github.com/ygan/Spider-Syn)]<br>*Knowledge-augmented; Adding domain knowledge*
* ![Findings2020](https://img.shields.io/badge/EMNLP2020Findings-87CEFA) **Spider-Vietnames** | A Pilot Study of Text-to-SQL Semantic Parsing for Vietnamese [[Paper](https://aclanthology.org/2020.findings-emnlp.364.pdf)] [[Code](https://github.com/VinAIResearch/ViText2SQL)]<br>
  *Cross-lingual; Vietnamese version of Spider*
* ![NAACL2021](https://img.shields.io/badge/NAACL2021-4682B4) **Spider-Realistic** | Structure-Grounded Pretraining for Text-to-SQL [[Paper](https://aclanthology.org/2021.naacl-main.105.pdf)] [[Dataset](https://zenodo.org/records/5205322)]<br>*Robustness; Removing column names in question*
* ![EMNLP2019](https://img.shields.io/badge/EMNLP2019-00BFFF) **CSpider** | A Pilot Study for Chinese SQL Semantic Parsing [[Paper](https://aclanthology.org/D19-1377.pdf)] [[Code](https://github.com/taolusi/chisp)]<br>*Cross-lingual; Chinese version of Spider*
* ![EMNLP2019](https://img.shields.io/badge/EMNLP2019-00BFFF) **SParC** | SParC: Cross-Domain Semantic Parsing in Context [[Paper](https://aclanthology.org/P19-1443.pdf)] [[Code](https://github.com/taoyds/sparc)] [[Dataset](https://drive.usercontent.google.com/download?id=1Uu7NMHTR1tdQw1t7bAuM7OPU4LElVKfg&export=download&authuser=0)]<br>*Context-dependent; Annotate conversational contents*

## 🪴 Taxonomy

The implementation of recent LLM-based text-to-SQL methods primarily relies on in-context learning and fine-tuning, enabled by the release of both powerful proprietary and well-architected open-source LLMs. **A detailed categorization of text-to-SQL methods can be found in [our paper](https://arxiv.org/pdf/2406.08426#page=3), and subsequent latest research papers will be continually updated and aligned with this taxonomy.** 

### In-context Learning

* ![EMNLP2025](https://img.shields.io/badge/EMNLP2025-00BFFF) LinkAlign: Scalable Schema Linking for Real-World Large-Scale Multi-Database Text-to-SQL  [[Paper](https://arxiv.org/pdf/2503.18596)] [[Code](https://github.com/Satissss/LinkAlign)]
* ![ICLR2025](https://img.shields.io/badge/ICLR2025Workshop-7CFC00) ReFoRCE: A Text-to-SQL Agent with Self-Refinement, Consensus Enforcement, and Column Exploration [[Paper](https://openreview.net/pdf?id=OuFIfDBwQd)] [[Code](https://github.com/Snowflake-Labs/ReFoRCE)]
* ![arXiv2025](https://img.shields.io/badge/arXiv2025-B31B1B) CSC-SQL: Corrective Self-Consistency in Text-to-SQL via Reinforcement Learning [[Paper](https://arxiv.org/pdf/2505.13271)] [[Code](https://github.com/CycloneBoy/csc_sql)]
* ![arXiv2025](https://img.shields.io/badge/arXiv2025-B31B1B) SAFE-SQL: Self-Augmented In-Context Learning with Fine-grained Example Selection for Text-to-SQL [[Paper](https://arxiv.org/pdf/2502.11438)]
* ![COLING2025](https://img.shields.io/badge/COLING2025-00CED1) Gen-SQL: Efficient Text-to-SQL by Bridging Natural Language Question and Database Schema with Pseudo-Schema [[Paper](https://aclanthology.org/2025.coling-main.256.pdf)] [[Code](https://github.com/jieshi10/gensql)]
* ![COLING2025](https://img.shields.io/badge/COLING2025-00CED1) In-Context Reinforcement Learning based Retrieval-Augmented Generation for Text-to-SQL  [[Paper](https://aclanthology.org/2025.coling-main.692.pdf)] 
* ![ICLR2025](https://img.shields.io/badge/ICLR2025-7CFC00) Spider 2.0: Evaluating Language Models on Real-world Enterprise Text-to-SQL Workflows [[Paper](https://openreview.net/pdf?id=XmProj9cPs)] [[Code](https://github.com/xlang-ai/Spider2)]
* ![arXiv2024](https://img.shields.io/badge/arXiv2024-B31B1B) RSL-SQL: Robust Schema Linking in Text-to-SQL Generation [[Paper](https://arxiv.org/pdf/2411.00073)] [[Code](https://github.com/Laqcce-cao/RSL-SQL)]
* ![ICLR2025](https://img.shields.io/badge/ICLR2025-7CFC00) CHASE-SQL: Multi-Path Reasoning and Preference Optimized Candidate Selection in Text-to-SQL [[Paper](https://openreview.net/pdf?id=CvGqMD5OtX)]
* ![arXiv2024](https://img.shields.io/badge/arXiv2024-B31B1B) E-SQL: Direct Schema Linking via Question Enrichment in Text-to-SQL [[Paper](https://arxiv.org/pdf/2409.16751)] [[Code](https://github.com/HasanAlpCaferoglu/E-SQL)]
* ![NeurIPS202](https://img.shields.io/badge/NeurIPS2024Workshop-2E8B57) The Death of Schema Linking? Text-to-SQL in the Age of Well-Reasoned Language Models [[Paper](https://openreview.net/pdf?id=fglyh5pa7d)] 
* ![VLDB2024](https://img.shields.io/badge/VLDB2024-800080) The Dawn of Natural Language to SQL: Are We Fully Ready? [[Paper](https://www.vldb.org/pvldb/vol17/p3318-luo.pdf)]
* ![arXiv2024](https://img.shields.io/badge/arXiv2024-B31B1B) CHESS: Contextual Harnessing for Efficient SQL Synthesis [[Paper](https://arxiv.org/pdf/2405.16755)] [[Code](https://github.com/ShayanTalaei/CHESS)]
* ![COLING2025](https://img.shields.io/badge/COLING2025-00CED1) MCS-SQL: Leveraging Multiple Prompts and Multiple-Choice Selection For Text-to-SQL Generation [[Paper](https://aclanthology.org/2025.coling-main.24.pdf)]
* ![Findings2020](https://img.shields.io/badge/ACL2024Findings-87CEFA) Before Generation, Align it! A Novel and Effective Strategy for Mitigating Hallucinations in Text-to-SQL Generation [[Paper](https://aclanthology.org/2024.findings-acl.324.pdf)] [[Code](https://github.com/quge2023/TA-SQL)]
* ![arXiv2024](https://img.shields.io/badge/arXiv2024-B31B1B) Dubo-SQL: Diverse Retrieval-Augmented Generation and Fine Tuning for Text-to-SQL [[Paper](https://arxiv.org/pdf/2404.12560)] [[Code](https://github.com/mercatorhq/dubo-sql)]
* ![AAAI2025](https://img.shields.io/badge/AAAI2025-006400) MAGIC: Generating Self-Correction Guideline for In-Context Text-to-SQL [[Paper](https://arxiv.org/pdf/2406.12692)] [[Code](https://github.com/microsoft/SynQo)]
* ![NAACL2025](https://img.shields.io/badge/NAACL2025-4682B4) You Only Read Once (YORO): Learning to Internalize Database Knowledge for Text-to-SQL [[Paper](https://aclanthology.org/2025.naacl-long.94.pdf)]
* ![ICDE2024](https://img.shields.io/badge/ICDE2025-9370DB) PURPLE: Making a Large Language Model a Better SQL Writer [[Paper](https://ieeexplore.ieee.org/abstract/document/10597914)]
* ![arXiv2024](https://img.shields.io/badge/arXiv2024-B31B1B) PET-SQL: A Prompt-Enhanced Two-Round Refinement of Text-to-SQL with Cross-consistency [[Paper](https://arxiv.org/pdf/2403.09732)] [[Code](https://github.com/zhshLii/PETSQL)]
* ![ACL2025](https://img.shields.io/badge/ACL2025Workshop-1E90FF) **ℛ**³: "This is My SQL, Are You With Me?" A Consensus-Based Multi-Agent System for Text-to-SQL Tasks [[Paper](https://aclanthology.org/2025.trl-1.4.pdf)] [[Code](https://github.com/1ring2rta/R3)]
* ![ICDE2024](https://img.shields.io/badge/ICDE2025-9370DB) MetaSQL: A Generate-then-Rank Framework for Natural Language to SQL Translation [[Paper](https://ieeexplore.ieee.org/abstract/document/10597742)] [[Code](https://github.com/Kaimary/MetaSQL)]
* ![EMNLP2024](https://img.shields.io/badge/EMNLP2024-00BFFF) Middleware for LLMs: Tools Are Instrumental for Language Agents in Complex Environments [[Paper](https://aclanthology.org/2024.emnlp-main.436.pdf)] [[Code](https://github.com/OSU-NLP-Group/Middleware)]
* ![arXiv2024](https://img.shields.io/badge/arXiv2024-B31B1B) SQL-CRAFT: Text-to-SQL through Interactive Refinement and Enhanced Reasoning [[Paper](https://arxiv.org/pdf/2402.14851v1)]
* ![ICML2025](https://img.shields.io/badge/ICML2025-228B22) Structure-Guided Large Language Models for Text-to-SQL Generation [[Paper](https://openreview.net/pdf?id=gT8JSEFqaS)]
* ![Findings2020](https://img.shields.io/badge/ACL2024Findings-87CEFA) Knowledge-to-SQL: Enhancing SQL Generation with Data Expert LLM [[Paper](https://aclanthology.org/2024.findings-acl.653.pdf)] [[Code](https://github.com/Rcrossmeister/Knowledge-to-SQL)]
* ![Findings2024](https://img.shields.io/badge/EMNLP2024Findings-87CEFA) Improving Demonstration Diversity by Human-Free Fusing for Text-to-SQL [[Paper](https://aclanthology.org/2024.findings-emnlp.65.pdf)] [[Code](https://github.com/zirui-HIT/Fused)]
* ![Findings2020](https://img.shields.io/badge/ACL2024Findings-87CEFA) Decomposition for Enhancing Attention: Improving LLM-based Text-to-SQL through Workflow Paradigm [[Paper](https://aclanthology.org/2024.findings-acl.641.pdf)] [[Code](https://github.com/FlyingFeather/DEA-SQL)]
* ![COLING2025](https://img.shields.io/badge/COLING2025-00CED1) MAC-SQL: A Multi-Agent Collaborative Framework for Text-to-SQL [[Paper](https://aclanthology.org/2025.coling-main.36.pdf)] [[Code](https://github.com/wbbeyourself/MAC-SQL)]
* ![Findings2023](https://img.shields.io/badge/EMNLP2023Findings-87CEFA) ACT-SQL: In-Context Learning for Text-to-SQL with Automatically-Generated Chain-of-Thought [[Paper](https://aclanthology.org/2023.findings-emnlp.227.pdf)] [[Code](https://github.com/X-LANCE/text2sql-GPT)]
* ![Findings2023](https://img.shields.io/badge/EMNLP2023Findings-87CEFA) Selective Demonstrations for Cross-domain Text-to-SQL [[Paper](https://aclanthology.org/2023.findings-emnlp.944.pdf)] [[Code](https://github.com/shuaichenchang/ODIS-Text-to-SQL)]
* ![VLDB2024](https://img.shields.io/badge/VLDB2024-800080) Text-to-SQL Empowered by Large Language Models: A Benchmark Evaluation [[Paper](https://www.vldb.org/pvldb/vol17/p1132-gao.pdf)] [[Code](https://github.com/BeachWang/DAIL-SQL)]
* ![arXiv2023](https://img.shields.io/badge/arXiv2023-B31B1B) C3: Zero-shot Text-to-SQL with ChatGPT [[Paper](https://arxiv.org/pdf/2307.07306)] [[Code](https://github.com/bigbigwatermalon/C3SQL)]
* ![ICONIP2023](https://img.shields.io/badge/ICONIP2023-8FBC8F) Retrieval-augmented GPT-3.5-based Text-to-SQL Framework with Sample-aware Prompting and Dynamic Revision Chain [[Paper](https://link.springer.com/chapter/10.1007/978-981-99-8076-5_25)]
* ![TMLR2024](https://img.shields.io/badge/TMLR2024-556B2F) SQL-PaLM: Improved Large Language Model Adaptation for Text-to-SQL [[Paper](https://openreview.net/pdf?id=rlloVZoKrX)]
* ![EMNLP2023](https://img.shields.io/badge/EMNLP2023-00BFFF) Exploring Chain of Thought Style Prompting for Text-to-SQL [[Paper](https://aclanthology.org/2023.emnlp-main.327.pdf)]
* ![Findings2023](https://img.shields.io/badge/EMNLP2023Findings-87CEFA) Enhancing Text-to-SQL Capabilities of Large Language Models: A Study on Prompt Design Strategies [[Paper](https://aclanthology.org/2023.findings-emnlp.996.pdf)]
* ![EMNLP2023](https://img.shields.io/badge/EMNLP2023-00BFFF) StructGPT: A General Framework for Large Language Model to Reason over Structured Data [[Paper](https://aclanthology.org/2023.emnlp-main.574.pdf)] [[Code](https://github.com/RUCAIBox/StructGPT)] 
* ![NeurIPS2023](https://img.shields.io/badge/NeurIPS2023-2E8B57) DIN-SQL: Decomposed In-Context Learning of Text-to-SQL with Self-Correction [[Paper](https://openreview.net/pdf?id=p53QDxSIc5)] [[Code](https://github.com/MohammadrezaPourreza/Few-shot-NL2SQL-with-prompting)]
* ![PRICAI2023](https://img.shields.io/badge/PRICAI2023-8FBC8F) Prompting GPT-3.5 for Text-to-SQL with De-semanticization and Skeleton Retrieval [[Paper](https://link.springer.com/chapter/10.1007/978-981-99-7022-3_23)]
* ![ICLR2024](https://img.shields.io/badge/ICLR2025-7CFC00) Teaching Large Language Models to Self-Debug [[Paper](https://openreview.net/pdf?id=KuPixIqPiq)]
* ![ICML2023](https://img.shields.io/badge/ICML2023-228B22) LEVER: Learning to Verify Language-to-Code Generation with Execution [[Paper](https://openreview.net/pdf?id=Gj3zN9zs4v)] [[Code](https://github.com/niansong1996/lever)]
* ![ICML2023](https://img.shields.io/badge/ICML2023-228B22) Coder Reviewer Reranking for Code Generation [[Paper](https://openreview.net/pdf?id=tgXxVlWkmb)] 
* ![EMNLP2022](https://img.shields.io/badge/EMNLP2022-00BFFF) Natural Language to Code Translation with Execution [[Paper](https://aclanthology.org/2022.emnlp-main.231.pdf)] [[Code](https://github.com/facebookresearch/mbr-exec)]

### Fine-tuning

* ![ACL2025](https://img.shields.io/badge/ACL2025-1E90FF) SHARE: An SLM-based Hierarchical Action CorREction Assistant for Text-to-SQL [[Paper](https://aclanthology.org/2025.acl-long.552.pdf)] [[Code](https://github.com/quge2023/SHARE)] 
* ![ICLR2025](https://img.shields.io/badge/ICLR2025-7CFC00) ROUTE: Robust Multitask Tuning and Collaboration for Text-to-SQL [[Paper](https://openreview.net/pdf?id=BAglD6NGy0)] [[Code](https://github.com/D2I-ai/Route)]
* ![arXiv2024](https://img.shields.io/badge/arXiv2024-B31B1B) A Preview of XiYan-SQL: A Multi-Generator Ensemble Framework for Text-to-SQL [[Paper](https://arxiv.org/pdf/2411.08599)] [[Code](https://github.com/XGenerationLab/XiYan-SQL)]
* ![NAACL2025](https://img.shields.io/badge/NAACL2025-4682B4) MSc-SQL: Multi-Sample Critiquing Small Language Models For Text-To-SQL Translation [[Paper](https://aclanthology.org/2025.naacl-long.107.pdf)] [[Code](https://github.com/layer6ai-labs/msc-sql)]
* ![arXiv2025](https://img.shields.io/badge/ICDE2025-9370DB) Knapsack Optimization-based Schema Linking for LLM-based Text-to-SQL Generation [[Paper](https://arxiv.org/pdf/2502.12911)]
* ![Findings2024](https://img.shields.io/badge/EMNLP2024Findings-87CEFA) DTS-SQL: Decomposed Text-to-SQL with Small Large Language Models [[Paper](https://aclanthology.org/2024.findings-emnlp.481.pdf)] [[Code](https://github.com/MohammadrezaPourreza/DTS-SQL)]
* ![COLING2025](https://img.shields.io/badge/COLING2025-00CED1) MAC-SQL: A Multi-Agent Collaborative Framework for Text-to-SQL [[Paper](https://aclanthology.org/2025.coling-main.36.pdf)] [[Code](https://github.com/wbbeyourself/MAC-SQL)]
* ![NeurIPS202](https://img.shields.io/badge/NeurIPS2024Workshop-2E8B57) The Death of Schema Linking? Text-to-SQL in the Age of Well-Reasoned Language Models [[Paper](https://openreview.net/pdf?id=fglyh5pa7d)] 
* ![arXiv2024](https://img.shields.io/badge/arXiv2024-B31B1B) Dubo-SQL: Diverse Retrieval-Augmented Generation and Fine Tuning for Text-to-SQL [[Paper](https://arxiv.org/pdf/2404.12560)] [[Code](https://github.com/mercatorhq/dubo-sql)]
* ![COLM2024](https://img.shields.io/badge/COLM2024-20B2AA) StructLM: Towards Building Generalist Models for Structured Knowledge Grounding [[Paper](https://openreview.net/pdf?id=EKBPn7no4y)] [[Code](https://github.com/TIGER-AI-Lab/StructLM)]
* ![SIGMOD2024](https://img.shields.io/badge/SIGMOD2024-8A2BE2) CodeS: Towards Building Open-source Language Models for Text-to-SQL [[Paper](https://dl.acm.org/doi/10.1145/3654930)] [[Code](https://github.com/RUCKBReasoning/codes)]
* ![ACL2024](https://img.shields.io/badge/ACL2024-1E90FF) Symbol-LLM: Towards Foundational Symbol-centric Interface For Large Language Models [[Paper](https://aclanthology.org/2024.acl-long.707.pdf)] [[Code](https://github.com/xufangzhi/Symbol-LLM)] 
* ![VLDB2024](https://img.shields.io/badge/VLDB2024-800080) Text-to-SQL Empowered by Large Language Models: A Benchmark Evaluation [[Paper](https://www.vldb.org/pvldb/vol17/p1132-gao.pdf)] [[Code](https://github.com/BeachWang/DAIL-SQL)]
* ![ICML2024](https://img.shields.io/badge/ICML2024-228B22) CLLMs: Consistency Large Language Models [[Paper](https://openreview.net/pdf?id=8uzBOVmh8H)] [[Code](https://github.com/hao-ai-lab/Consistency_LLM)]

## 📦 Projects 

* [SQLGlot](https://github.com/tobymao/sqlglot) [![GitHub Repo stars](https://img.shields.io/github/stars/tobymao/sqlglot?style=social)](https://github.com/premAI-io/tobymao/sqlglot)
* [DB-GPT](https://github.com/eosphoros-ai/DB-GPT) [![GitHub Repo stars](https://img.shields.io/github/stars/eosphoros-ai/DB-GPT?style=social)](https://github.com/eosphoros-ai/DB-GPT/stargazers)
* [DB-GPT-Hub](https://github.com/eosphoros-ai/DB-GPT-Hub) [![GitHub Repo stars](https://img.shields.io/github/stars/eosphoros-ai/DB-GPT-Hub?style=social)](https://github.com/eosphoros-ai/DB-GPT-Hub/stargazers)
* [Awesome-Text2SQL](https://github.com/eosphoros-ai/Awesome-Text2SQL) [![GitHub Repo stars](https://img.shields.io/github/stars/eosphoros-ai/Awesome-Text2SQL?style=social)](https://github.com/premAI-io/premsql/stargazers)
* [PremSQL](https://github.com/premAI-io/premsql) [![GitHub Repo stars](https://img.shields.io/github/stars/premAI-io/premsql?style=social)](https://github.com/premAI-io/premsql/stargazers)

## 📃 Citation

```
@article{hong2025next,
  title={Next-generation database interfaces: A survey of llm-based text-to-sql},
  author={Hong, Zijin and Yuan, Zheng and Zhang, Qinggang and Chen, Hao and Dong, Junnan and Huang, Feiran and Huang, Xiao},
  journal={IEEE Transactions on Knowledge and Data Engineering},
  year={2025}
}
```
