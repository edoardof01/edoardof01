# Edoardo Fanciullacci

**Ingegnere Informatico** con un percorso non convenzionale: da Gestionale a Informatica, entrambe con **110/110 con Lode** — un background che unisce visione sistemica e rigore tecnico.

Mi specializzo in **sistemi distribuiti**, **infrastrutture cloud-native** e **AI applicata**. Non mi interessa solo far funzionare le cose: voglio capire *perché* funzionano, costruire con rigore formale e lasciare codice che resiste al tempo.

> 📍 Firenze, Italia · Aperto a opportunità remote e ibride

[![LinkedIn](https://img.shields.io/badge/LinkedIn-Edoardo_Fanciullacci-0077B5?style=flat&logo=linkedin)](https://linkedin.com/in/edoardo-fanciullacci)
[![Email](https://img.shields.io/badge/Email-edoardofanciullacci01@gmail.com-D14836?style=flat&logo=gmail)](mailto:edoardofanciullacci01@gmail.com)

---

## 🎓 Formazione

| Titolo | Ateneo | Voto |
|---|---|---|
| **Laurea Magistrale** — Ingegneria Informatica | Università di Firenze | 110/110 con Lode |
| **Laurea Triennale** — Ingegneria Gestionale | Università di Firenze | 110/110 con Lode |

---

## 🚀 Progetti in Evidenza

### 📐 [Tesi Magistrale] Valutazione e Rifattorizzazione di Topologie SAGA
> *Framework per l'analisi stocastica della consistenza in architetture a microservizi*

Architetture a microservizi promettono scalabilità, ma nascondono un problema sottile: **come garantire la consistenza finale quando una transazione distribuita fallisce parzialmente?**

Ho costruito un framework teorico ed empirico per analizzare e ottimizzare il **Time to Consistency** in pattern SAGA con ramificazioni parallele (AND) e condizionali (XOR).

**Contributo chiave:** un algoritmo Greedy di rifattorizzazione basato sulla **dominanza stocastica delle CDF**, che minimizza i tempi di recupero scegliendo l'ordine ottimale di esecuzione dei compensating transactions.

```
Stack: Java (Sirio/Eulero) · Kubernetes · Apache Kafka
Risultati: +15.29% performance · MAE < 0.02 (validazione empirica)
```

---

### 🤖 [cf_ai_rag](https://github.com/edoardof01/cf_ai_rag) — Advanced Hybrid RAG System
> *Sistema RAG production-grade, completamente self-hosted su Kubernetes*

Un sistema di Retrieval-Augmented Generation che va oltre il semplice vector search. Il design ibrido combina **due paradigmi di retrieval** per massimizzare la qualità delle risposte:

- 🔍 **Dense retrieval** (semantico) via **Milvus**
- 📖 **Sparse retrieval** (lessicale) via **BM25 su Redis**
- 🎯 **Cross-Encoder reranking** per la selezione finale
- 🧠 **Memoria conversazionale multi-strategia**: Sliding Window · Summary · Vector Memory
- ✍️ **Query Rewriting** contestuale + gestione dinamica del budget dei token

```
Infrastruttura: Minikube · Ollama (Qwen 2.5) · Milvus · Redis
Deploy: completamente automatizzato con persistenza dei dati
```

---

## 🛠 Altri Progetti

### [SessionBuilder](https://github.com/edoardof01/sessionBuilder) — Java Desktop App con TDD rigoroso
Applicazione sviluppata con una disciplina ingegneristica end-to-end: ogni riga di codice coperta da test prima di essere scritta.

- **Pipeline CI/CD** completa con GitHub Actions
- **Analisi statica** con SonarCloud + **Mutation Testing** con PIT
- **Architettura** MVC + Service Layer con gestione transazionale custom via `ThreadLocal`

### [Multi-Label Emotion Classifier](https://github.com/edoardof01/fml-laboratory) — NLP con DistilBERT
Classificatore di emozioni multi-label che affronta il problema spesso ignorato del **rumore nelle label**.

- **Confident Learning** (CleanLab) per la pulizia automatica delle annotazioni rumorose
- **Optuna** per l'ottimizzazione bayesiana degli iperparametri
- **LIME** per la spiegabilità (XAI) delle predizioni

---

## 🧰 Tech Stack

| Area | Tecnologie |
|---|---|
| **Languages** | Java (Spring, JPA/Hibernate), Python (PyTorch, LangChain, Pandas), SQL (Postgres), C |
| **Cloud & DevOps** | Docker, Kubernetes, Apache Kafka, GitHub Actions, Maven |
| **AI & Data** | Vector DBs (Milvus), Redis, RAG Architectures, LLM Self-hosting (Ollama), NLP, XAI |
| **Software Engineering** | TDD, Design Patterns, Microservices, DDD |

---

## 📚 Apprendimento continuo

Costruire sistemi non basta: bisogna capire il *perché* dietro ogni scelta. Per questo studio in modo sistematico e continuo — libri di testo, paper, blog tecnici, documentazione originale. Alcune aree che sto esplorando in questo periodo:

- **Distributed Systems** — *Designing Data-Intensive Applications* (Kleppmann), paper su consensus algorithms
- **AI/ML** — paper su architetture RAG avanzate, agentic systems, model evaluation
- **Software Design** — *A Philosophy of Software Design* (Ousterhout), pattern architetturali

Credo che l'ingegneria del software sia un mestiere che richiede umiltà intellettuale costante: il panorama cambia, e stare al passo significa non smettere mai di essere studenti.

---

*Trovo che l'intersezione tra rigore formale e ingegneria creativa sia il posto più stimolante in cui costruire software — e la traiettoria Gestionale → Informatica mi ha dato gli strumenti per abitare entrambe le sponde.*
