# Intro to Artificial Intelligence  
**Master of Science in Health Informatics**

## Course Purpose
This course is designed to build **AI literacy** for health informatics students. Rather than teaching mathematical or programming foundations, the goal is to equip students with the **vocabulary, conceptual frameworks, and critical thinking skills** needed to:

- Speak intelligently about different domains of artificial intelligence
- Evaluate AI tools and vendor claims in healthcare
- Collaborate effectively with technical teams
- Understand strengths, weaknesses, risks, and appropriate use cases of AI systems

The course consists of **four 3-hour sessions** and assumes **no prerequisite knowledge**.

---

## Guiding Learning Objectives
By the end of the course, students will be able to:

1. Identify major domains of artificial intelligence and machine learning  
2. Match AI approaches to appropriate healthcare problems  
3. Describe data requirements, performance tradeoffs, and limitations of each domain  
4. Recognize risks related to bias, interpretability, validation, and governance  
5. Critically evaluate real-world healthcare AI applications  

---

# Core Domains of Artificial Intelligence

## 1. Rule-Based Systems & Expert Systems
**Overview**  
Early forms of AI based on explicit human-defined logic. Many healthcare “AI” tools still rely heavily on rules.

**Key Concepts**
- If/then logic
- Decision trees
- Deterministic behavior
- Knowledge engineering

**Strengths**
- Transparent and interpretable  
- Predictable behavior  
- Easy to validate and audit  

**Weaknesses**
- Brittle and hard to scale  
- Requires frequent manual updates  
- Performs poorly with complex variability  

**Healthcare Examples**
- Sepsis alerts  
- Triage protocols  
- Order sets  

**Exercise: Build a Triage Algorithm**
- Students design a rule-based triage or deterioration algorithm
- Introduce edge cases (missing data, conflicting symptoms)

**Teaching Point:** Rule-based systems break down quickly as complexity increases.

---

## 2. Classical Machine Learning (Supervised Learning)
Focus on **terminology and intuition**, not math.

**Common Techniques**
- Logistic regression  
- Decision trees  
- Random forest  
- k-Nearest Neighbor (kNN)  

**Key Concepts**
- Features and labels  
- Training vs testing data  
- Overfitting  
- Bias–variance tradeoff  
- Performance metrics (accuracy, sensitivity, AUROC)  

**Strengths**
- Effective with structured/tabular data  
- Often interpretable (especially trees)  
- Strong performance with modest datasets  

**Weaknesses**
- Requires labeled data  
- Feature engineering burden  
- Limited use with unstructured data  

**Healthcare Examples**
- Readmission prediction  
- Risk stratification  
- Throughput and capacity prediction  
- No-show prediction  

**Exercise: Same Dataset, Different Models**
- Run multiple models on the same dataset using prebuilt tool in Codespaces
- Compare accuracy, interpretability, and stability

**Teaching Point:** More complex models are not always better.

---

## 3. Unsupervised Learning
Used for **pattern discovery**, not direct prediction.

**Key Techniques**
- Clustering (k-means, hierarchical clustering)  
- Dimensionality reduction (PCA, t-SNE)  

**Key Concepts**
- No labeled outcomes  
- Latent structure  
- Exploratory analysis  
- Hypothesis generation  

**Strengths**
- Works without labeled data  
- Useful for population discovery  
- Can reveal hidden structure  

**Weaknesses**
- Black box phenomenon. Difficult to validate  
- Subjective interpretation  
- Not decision-ready on its own  

**Healthcare Examples**
- Patient phenotyping  
- Utilization patterns  
- Disease subtyping  

**Exercise: Find the Patient Groups**
- Perform clustering on a patient dataset
- Define and interpret clusters
- Discuss whether results are clinically actionable

**Teaching Point:** Unsupervised learning suggests insights—it does not answer questions.

---

## 4. Neural Networks & Deep Learning (Conceptual)
Introduced at a **high level only**.

**Key Concepts**
- Neurons and layers  
- Representation learning  
- Why depth matters  
- Data requirements  

**Strengths**
- Handles complex, nonlinear patterns  
- Works with unstructured data  
- State-of-the-art performance in many domains  

**Weaknesses**
- Black box phenomenon. Poor interpretability  
- Data-intensive  
- Difficult to validate and govern  

**Healthcare Examples**
- Medical imaging  
- Physiologic waveforms (ECG, EEG)  
- Predictive monitoring  

**Exercise: Why Can’t a Random Forest Read an X-ray?**
- Compare tabular vs unstructured data
- Discuss why deep learning is needed for images and signals

---

## 5. Natural Language Processing (NLP)
Critical domain for health informatics.

**Subdomains**
- Rule-based NLP  
- Classical NLP (bag-of-words, TF-IDF)  
- Transformer-based NLP  

**Key Concepts**
- Tokenization  
- Embeddings  
- Context  
- Named entity recognition (NER)  

**Strengths**
- Unlocks clinical notes  
- Enables large-scale text analysis  
- Reduces documentation burden  

**Weaknesses**
- Ambiguity in clinical language  
- Bias from documentation practices  
- PHI and privacy risks  

**Healthcare Examples**
- Chart abstraction  
- Clinical coding  
- Quality reporting  
- Prior authorization  

**Exercise: From Keywords to Meaning**
- Compare keyword extraction with LLM-based summarization
- Discuss tradeoffs in accuracy, nuance, and risk

---

## 6. Large Language Models (LLMs) & Generative AI
Seismic shift in workflows in the past decade.

**Key Concepts**
- Foundation models  
- Pretraining vs fine-tuning  
- Prompt engineering  
- Hallucinations  
- Retrieval-augmented generation (RAG)  

**Strengths**
- General-purpose  
- Natural language interfaces  
- Rapid prototyping and automation  

**Weaknesses**
- Not able to vet truth vs fiction
- Non-deterministic outputs (can also be a strength)
- Regulatory, safety, and governance challenges  

**Healthcare Examples**
- Clinical documentation support  
- Patient communication  
- Ambient scribing
- Education and training  

**Exercise: Same Question, Three Prompts**
- Summarize a discharge note
- Explain it to a patient
- Extract structured data
- Introduce an error and discuss mitigation strategies

**Teaching Point:** LLMs are assistants, not decision-makers.

---

## 7. Evaluation, Ethics, and Governance (Cross-Cutting)
This domain applies to **all AI approaches**.

**Core Vocabulary**
- Bias and fairness  
- Model drift  
- Explainability  
- Validation vs verification  
- Human-in-the-loop  
- Regulatory considerations (conceptual FDA pathways)  

**Exercise: Would You Deploy This?**
- Evaluate a hypothetical AI tool
- Identify risks, safeguards, and monitoring metrics

---

# Suggested Course Structure

## Session 1: What Is (and Isn’t) AI?
- Rule-based systems  
- Supervised machine learning  
- Triage and prediction exercises  

## Session 2: Finding Patterns and Meaning
- Unsupervised learning  
- NLP fundamentals  
- Patient clustering and note analysis  

## Session 3: Deep Learning and Generative AI
- Neural networks  
- Large language models  
- Prompting and hallucination exercises  

## Session 4: Using AI Responsibly in Healthcare
- Evaluation and governance  
- Bias and safety  
- Capstone: critique a real AI product or paper  

---

## Unifying Framework
Each AI domain is evaluated using three questions:

1. What problem is this good at?  
2. What data does it require?  
3. What can go wrong in healthcare?  

---

## License
This content is intended for educational use within the Master of Science in Health Informatics program. Adaptation and reuse are encouraged with attribution.
