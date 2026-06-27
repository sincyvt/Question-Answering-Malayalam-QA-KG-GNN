# Malayalam Knowledge Graph Question Answering (Malayalam-KGQA)

A manually curated **Malayalam Knowledge Graph (KG)** and **Question Answering (QA)** dataset for developing and evaluating **Knowledge Graph Question Answering (KGQA)** systems.

The dataset is intended for research in:

- Knowledge Graph Question Answering (KGQA)
- Natural Language Processing (NLP)
- Information Retrieval
- Graph Neural Networks (GNN)
- Retrieval-Augmented Generation (RAG)
- Entity Linking
- Question Classification
- Multilingual Language Models (mBERT, XLM-R, IndicBERT, MuRIL, etc.)

---

## Dataset Statistics

| Item | Count |
|------|------:|
| Knowledge Base Triples | 6000+ |
| Malayalam Questions | 700+ |
| Unique Entities | 1000+ |
| Relations | 50+ |
| Domains | 20+ |

---

## Dataset Structure

```
Malayalam-KGQA/
│
├── kgm.txt
├── data1.json
├── README.md
└── LICENSE
```

---

## Knowledge Base Format

Each line contains one RDF-style triple.

```
Subject|Relation|Object
```

Example

```text
കേരളം|തലസ്ഥാനം|തിരുവനന്തപുരം
കേരളം|സംസ്ഥാന രൂപീകരണ വർഷം|1956
ചന്ദ്രയാൻ-3|ലക്ഷ്യം|ചന്ദ്രൻ
ഇന്ത്യ|ദേശീയ മൃഗം|കടുവ
```

---

## Question Format

Questions are stored in JSON format.

```json
{
  "Question":"കേരളത്തിന്റെ തലസ്ഥാനം ഏതാണ്",
  "Question Entity":"കേരളം",
  "Answer":["തിരുവനന്തപുരം"]
}
```

Example

```json
{
  "Question":"ചന്ദ്രയാൻ-3ന്റെ ലക്ഷ്യം എന്താണ്",
  "Question Entity":"ചന്ദ്രയാൻ-3",
  "Answer":["ചന്ദ്രൻ"]
}
```

---

## Relation Types

Some commonly used relations include:

```
തലസ്ഥാനം
ജന്മസ്ഥലം
ജനന വർഷം
മരണ വർഷം
സ്ഥാപിതമായ വർഷം
ആസ്ഥാനം
സംസ്ഥാനം
രാജ്യം
നാണയം
ഭാഷ
ലിപി
രചിച്ച കൃതി
സംവിധാനം
പ്രധാന അഭിനേതാക്കൾ
ലഭിച്ച പുരസ്കാരം
കായികം
വിളിപ്പേര്
പ്രശസ്തം
നേട്ടം
ഉപയോഗം
തരം
മേഖല
ബന്ധപ്പെട്ട ദൗത്യം
ലക്ഷ്യം
```

---

## Domains Covered

The dataset covers multiple domains including:

- Kerala General Knowledge
- Indian History
- World History
- Geography
- Science
- Biology
- Physics
- Chemistry
- Space Science
- ISRO Missions
- Artificial Intelligence
- Machine Learning
- Computer Science
- Databases
- Networking
- Mathematics
- Literature
- Malayalam Literature
- Sports
- Awards
- Indian Constitution
- Economy
- Culture
- Wildlife
- UNESCO Heritage
- Festivals

---

## Example Knowledge Graph

```
ചന്ദ്രയാൻ-3
      │
      ├── ലക്ഷ്യം ─────────► ചന്ദ്രൻ
      │
      ├── ലാൻഡർ ─────────► വിക്രം
      │
      ├── റോവർ ─────────► പ്രഗ്യാൻ
      │
      └── വിക്ഷേപിച്ച വർഷം ─► 2023
```

---

## Possible Applications

This dataset can be used for

- Knowledge Graph Construction
- Knowledge Graph Question Answering
- Entity Linking
- Named Entity Recognition
- Question Classification
- Semantic Search
- Graph Embedding
- Retrieval-Augmented Generation
- Graph Neural Networks
- Large Language Model Evaluation

---

## Compatible Frameworks

- PyTorch
- TensorFlow
- HuggingFace Transformers
- NetworkX
- Neo4j
- RDFLib
- DGL
- PyTorch Geometric
- LangChain
- LlamaIndex

---

## Citation

If you use this dataset in your research, please cite:

```bibtex
@misc{malayalamkgqa,
  title={Malayalam Knowledge Graph Question Answering Dataset},
  author={Your Name},
  year={2026},
  note={GitHub Repository}
}
```

---

## License

This dataset is released for academic and research purposes.

---

## Future Work

Planned extensions include

- Multi-hop questions
- Complex reasoning questions
- Boolean questions
- Count-based questions
- Temporal questions
- Comparative questions
- Wikidata entity mapping
- RDF/TTL version
- Neo4j import files
- Graph embeddings

---

## Acknowledgement

This dataset was manually curated to facilitate research on Malayalam Knowledge Graph Question Answering (KGQA) and multilingual NLP. It aims to support the development of robust question answering systems for low-resource languages.
