# Benchmark of core capabilities
## Knowledge-Benchmarks

This page organizes LLM knowledge-evaluation benchmarks into four major types—**Breadth**, **Depth**, **Truthfulness**, and **Dynamic/Timely**—and lists representative datasets for each. We’ve also added a handful of the latest 2024–2025 works.

### 1. General Knowledge (Breadth)  
Benchmarks testing broad world knowledge (often QA over Wikipedia or ConceptNet).  
- **LAMA**: Language Models as Knowledge Bases   
- **TriviaQA**: Open-domain QA from trivia sites   
- **NaturalQuestions**: Real queries from Google logs   
- **WebQuestions**: QA over Freebase   
- **CommonsenseQA**: Commonsense reasoning QA   

### 2. Domain-Specific Expertise (Depth)  
Probing specialized knowledge in finance, law, etc.  
#### Finance
- **FinanceBench**: Financial question answering   
- **FinBEN**: Chinese financial QA   
- **CFinBench**: Corporate finance QA
#### Law
- **LawBench**: Legal QA   
- **LexEval**: Legal entity understanding   
- **LegalAgentBench**: Agentic legal reasoning   

### 3. Truthfulness & Hallucination Detection  
Datasets that distinguish correct answers from plausible-but-false ones.  
- **TruthfulQA**: Known false claims   
- **HaluEval**: Unanswerable or trick questions   

### 4. Dynamic / Timely Knowledge  
Benchmarks that account for **new** or **time-sensitive** facts.  
#### Temporal
- **TimeQA**: Chronological QA over timelines   
- **SituatedQA**: Contextualized QA with temporal info   
- **StreamingQA**: Continual knowledge streams   
- **RealtimeQA**: Live news QA   
- **KoLA**: Knowledge-of-Language Assessment
#### Data Contamination
- **UntangleQA**: Disentangling pretraining contamination   
- **LiveBench**: News-driven QA updates   
- **EvoWiki**: Evolving Wikipedia evaluation   
- **AntiLeak**: Anti-contamination QA   
#### Evolving Benchmarks  
- **Benchmark Self-Evolving**: multi-agent framework for dynamic evaluation
- **DARG**: adaptive reasoning graph to generate complexity-controlled test data
- **DyVal 2**: meta-probing agents for psychometric-inspired dynamic eval
- **KG-LLM-Bench**: reasoning over textualized knowledge graphs
---
