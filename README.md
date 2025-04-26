# Benchmark of core capabilities

## Instruction-Following-Benchmarks
Instruction-following benchmarks have evolved from single-task NLP sets to rich, real-world, and automated evaluations. Early datasets focused on mapping input to output on held-out tasks, giving way to instruction-tuning collections and prompt generalization. Modern evaluations incorporate human prompts, automated judges, style-control, and constraint-based tests. We also highlight recent benchmarks targeting specialized domains, evaluator robustness, and long-context stability.

### 1. Single-Task & Instruction Tuning  
Early instruction tuning aggregated diverse NLP tasks under descriptive prompts, enabling held-out-task evaluation.  
- **GPT-2 Language Modeling**: Foundations of zero-shot mapping $p(y\mid x)$ to $p(y\mid x,\text{task})$   
- **Natural Instructions**: Multi-task QA and classification   
- **TO-Eval**: Text-only prompts across tasks   
- **InstructEval**: Fine-grained held-out task splits   
- **FLAN**: Instruction-tuned on 1,800 tasks   
- **SuperNI-Test**: Held-out instruction evaluation 

### 2. Prompt Generalization  
As tuning scaled, models began handling arbitrary user prompts, moving beyond narrow task descriptions.  
- **ShareGPT**: Real user prompts from ChatGPT logs   
- **FreeDolly**: Crowdsourced web prompts   
- **OpenAssistant**: Community-driven prompt bank   
- **Chatbot Arena**: Elo-based human comparisons   

### 3. Automated Evaluation  
To reduce human labeling costs, LLMs themselves judge instruction adherence.  
- **AlpacaEval**: GPT-based pairwise scoring   
- **VicunaEval**: Multi-model automated ranking   
- **Arena Hard Auto**: Large-scale GPT-4 judging   

### 4. Style-Control  
Benchmarks disentangling style biases from content accuracy.  
- **StyleControl Arena**: Balancing verbosity and clarity   
- **Human-Length Eval**: Controlling response length   
- **Disentangling Styles**: Evaluating prompt style influence   

### 5. Constraint-Based Tests  
Absolute evaluation via rule-verifiable constraints.  
- **IfEval**: 25 rule-based prompt constraints   
- **FollowBench**: LLM-verified constraints   
- **WildBench**: Human-annotated checklists
- **CoDI-Eval**: Controllable generation under constraints 

### 6. Meta-Evaluation & Robustness  
Recent works challenge LLM evaluators and extend instruction testing to expert domains.  
- **LLMBar**: Adversarial meta-evaluation of instruction following 
- **IfIR**: Instruction-following IR in finance, law, science, healthcare 
- **DRFR**: Decomposed Requirements Following Ratio metric 
- **LIFBench**: Long-context instruction stability   
- **HREF**: Human-response guided evaluation 
- **CIF-Bench**: Chinese instruction generalizability 
- **MedS-Bench**: Clinical instruction following 
- **Knowledge-Task IF Eval**: Instruction tests over QA tasks 
---



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
