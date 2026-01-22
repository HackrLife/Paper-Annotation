# Annotations

## "Augmenting Organizational Decision-Making with Deep Learning Algorithms: Principles, Promises, and Challenges"

**Shrestha, Krishna, & von Krogh (2021)**

*A Comprehensive Analysis of Deep Learning-Augmented Decision-Making (DLADM) in Organizations*

Critical Commentary, Technical Analysis, Organisational Implications, and Research Gaps

---

## Table of Contents

1. Executive Summary and Research Significance
2. Paper Overview and Key Contributions
3. Section-by-Section Annotations
4. Methodological Deep Dive
5. Theoretical Framework Analysis
6. Critical Assessment and Limitations
7. Implications for AI Governance Research
8. Glossary of Technical Terms
9. Suggested Further Reading

---

# PART 1: DETAILED ANALYSIS

# 1. Executive Summary and Research Significance

## 1.1 Why This Paper Matters

This paper represents a significant contribution to bridging the gap between technical deep learning (DL) research and management/organization studies. Published in the *Journal of Business Research*, it provides management scholars with an accessible yet rigorous introduction to DL algorithms while demonstrating their practical applications through two illustrative case studies. The paper conceptualizes **Deep Learning-Augmented Decision-Making (DLADM)** as a framework for understanding how DL outputs can enhance organisational decision processes.

| **🟡 Historical Context** |
|:----|
| *Before this paper, management scholars largely treated AI/ML as a "black box," focusing on outcomes rather than mechanisms. The Carnegie School tradition (March & Simon, 1958) emphasised information processing as central to organizational decision-making, but the AI-specific literature remained fragmented between highly technical computer science papers and superficial business applications. This paper explicitly aims to open the "black box" of DL for management researchers (citing Orlikowski & Scott, 2008), positioning itself as a bridge between disciplines.* |

## 1.2 The Paradigm Shift

The paper positions contemporary AI as fundamentally different from earlier conceptions. While early AI was characterised as "systems of knowing" that attempted to emulate human reasoning and fell short of expectations, contemporary AI—enabled by advanced algorithms, big data, and GPU/TPU computing—now demonstrates genuine learning capabilities and "simple agency" within organizational structures.

| **🔴 Critical Analysis** |
|:----|
| *The framing of AI as having "simple agency" is provocative but underexplored. The paper invokes Kaplan & Haenlein (2020) but does not deeply engage with what agency means in an organisational context, or how such algorithmic agency interacts with human accountability structures. This represents a significant gap given the paper's focus on organisational decision-making. The agency framing raises questions: Can an algorithm be accountable? Who bears responsibility when DLADM fails?* |

---

# 2. Paper Overview and Key Contributions

## 2.1 Core Contributions

1. **Conceptualisation of DLADM**: Introduces "Deep Learning-Augmented Decision-Making" as a framework for understanding DL integration into organisational decision processes across marketing, finance, operations, HR, and strategy.

2. **Accessible DL Tutorial**: Provides management scholars with a readable explanation of neural network architectures, training procedures, and the distinction between traditional ML and DL.

3. **Application Taxonomy**: Categorises DLADM applications into **targeting**, **monitoring**, and **scheduling** clusters with industry examples.

4. **Empirical Demonstrations**: Two case studies (fashion image classification using Zalando data, sentiment analysis using Rotten Tomatoes) demonstrating DL superiority over traditional ML.

5. **Challenge Synthesis**: Systematic discussion of economic challenges (costs, data, computing) and organisational challenges (errors, bias, opacity, privacy) with managerial recommendations.

## 2.2 Author Team and Institutional Context

All authors are from **ETH Zurich**, a leading technical university. Georg von Krogh is a prominent strategy and innovation scholar known for work on knowledge management. This combination of technical institution and management expertise positions the paper well for its bridge-building aims.

| **🟡 Attribution Analysis** |
|:----|
| *The paper is funded by the Swiss National Science Foundation (grant 169441), suggesting a broader research programme. The authors note they have made code publicly available on GitHub, demonstrating commitment to reproducibility. However, the absence of industry co-authors or organisational field research limits the paper's ability to speak to actual implementation challenges.* |

---

# 3. Section-by-Section Annotations

## 3.1 Abstract Analysis

The abstract positions DL as enabling employees to transition "to more creative work" through information processing assistance. This reflects techno-optimist assumptions common in the AI-augmentation literature.

| **🔴 Critical Analysis** |
|:----|
| *The claim that DL will help workers transition to "more creative work" is stated without evidence or qualification. This echoes earlier claims about IT that were not borne out in practice. The labour implications of DL augmentation—including potential deskilling, job displacement, and changes to work meaning—are not addressed in the abstract and receive only cursory attention in the challenges section.* |

## 3.2 Introduction

The introduction effectively situates the paper within the Carnegie School tradition, citing foundational works (March & Simon, 1958; Tushman & Nadler, 1978) and Simon's famous dictum that organisational structure is fundamentally about information processing. This provides strong theoretical grounding for examining AI's role in organisations.

| **🟢 Key Insight** |
|:----|
| *The paper makes an important empirical observation: while **80% of marketing data is unstructured**, only a fraction of organisations possess capabilities to utilise it (citing Balducci & Marinova, 2018). This identifies a genuine capability gap that DL might address. The statistic provides concrete justification for the paper's focus on image and text data.* |

## 3.3 DLADM in Practice (Section 2)

The taxonomy of **targeting**, **monitoring**, and **scheduling** provides a useful organising framework. Examples include:
- Unilever-Alibaba partnerships for demand generation
- Bloomberg sentiment analysis for market movements
- Amazon fraud detection
- Cainiao logistics optimisation

| **🔴 Critical Analysis** |
|:----|
| *The examples are drawn predominantly from large technology companies or their partners (Google, Amazon, Alibaba, Bloomberg). This selection bias limits generalisability to smaller organisations or non-technology sectors. The paper acknowledges DLADM is "no longer limited to large technology companies" but provides little evidence for this claim. Implementation details for non-tech firms remain unaddressed.* |

## 3.4 Technical Overview (Section 3)

The technical tutorial progresses from basic ML concepts through neural networks to CNN architectures. The explanation of neurons, activation functions, and layer hierarchies is accessible to non-technical readers while maintaining accuracy.

| **🔵 Technical Note** |
|:----|
| *The paper correctly identifies that DL's advantage over traditional ML comes from **automatic feature extraction** (no manual feature engineering required) and the ability to capture complex non-linear patterns in large datasets. Figure 5 effectively illustrates the data quantity/performance relationship that favours DL at scale.* |

## 3.5 Case Studies (Section 4)

### 3.5.1 Fashion Image Classification

The **Fashion-MNIST** dataset (60,000 training, 10,000 test images) demonstrates CNN superiority: **92.48% accuracy** versus 84.82% for best traditional ML (Random Forest). Transfer learning with ResNet18 achieves **93.98%**.

| **🟡 Design Analysis** |
|:----|
| *Fashion-MNIST is deliberately designed as a more challenging benchmark than original MNIST. However, its 28x28 grayscale images are far simpler than production fashion e-commerce images, which include multiple angles, varying backgrounds, models wearing garments, and style context. The 8.5% accuracy improvement, while statistically meaningful, may not translate to business-meaningful improvement in actual deployment.* |

### 3.5.2 Sentiment Analysis

Using **Rotten Tomatoes** movie reviews, the paper demonstrates BERT fine-tuning achieving **90.4% accuracy** versus 79.24% for Linear SVM. The **11.2% improvement** is substantial.

| **🟡 Measurement Validity** |
|:----|
| *The sentiment classification is binary (positive/negative), collapsing the original fine-grained labels. This simplification may overstate model performance in nuanced business contexts where distinguishing degrees of sentiment matters. The domain (movie reviews) may not generalise to product reviews, social media sentiment, or employee feedback—all mentioned as potential DLADM applications.* |

---

# 4. Methodological Deep Dive

## 4.1 Research Design

The paper employs a **tutorial + case study methodology**. This is appropriate for introducing technical concepts to a new audience but limits causal inference and generalisability.

| **🟢 Methodological Strength** |
|:----|
| *The authors provide complete reproducibility through GitHub code availability. They correctly use held-out test sets to evaluate generalisation. The comparison across multiple algorithms (Decision Tree, KNN, SVC, Random Forest, CNN variants) provides robust benchmarking.* |

## 4.2 Key Results Summary

| Task | Best Traditional ML | Best DL | Improvement |
|------|---------------------|---------|-------------|
| Fashion Image Classification | Random Forest: 84.82% | CNN+ResNet18: 93.98% | +9.16% |
| Sentiment Analysis | Linear SVM: 79.24% | BERT Fine-tuned: 90.40% | +11.16% |

---

# 5. Theoretical Framework Analysis

## 5.1 Information Processing as Core Mechanism

The paper's theoretical contribution lies in connecting DL capabilities to the **information processing view of organisations** (Galbraith, 1974; Tushman & Nadler, 1978). DL is positioned as a technology that expands organisational information processing capacity, particularly for unstructured data.

| **🔵 Theoretical Integration** |
|:----|
| *The information processing framing is apt but underutilised. The paper could have developed hypotheses about which organisational structures or decision types benefit most from DL augmentation. For instance, highly uncertain environments requiring rapid information synthesis might benefit more than stable environments with structured data flows. This theoretical development is left for future research.* |

## 5.2 Missing Theoretical Lenses

- **Institutional Theory**: How do regulatory environments, professional norms, and legitimacy concerns shape DLADM adoption and use?
- **Political Economy**: Who gains and loses from DLADM? How do power dynamics within organisations shape implementation?
- **Labour Process Theory**: How does DLADM affect worker autonomy, skill requirements, and the meaning of work?
- **Trust and Human-AI Interaction**: The paper mentions trust but doesn't engage with the substantial literature on algorithm aversion/appreciation.

---

# 6. Critical Assessment and Limitations

## 6.1 What the Paper Gets Right

- Accessible technical explanation without oversimplification
- Reproducible methodology with public code availability
- Honest acknowledgment of economic and organisational challenges
- Appropriate positioning within information processing tradition
- Recognition that "managers must remain in the driver's seat"

## 6.2 Significant Limitations

| **🔴 Limitation 1: Lab vs Field Validity** |
|:----|
| *The case studies use benchmark datasets (Fashion-MNIST, Rotten Tomatoes) rather than actual organisational data. The gap between controlled experiments and messy organisational reality is substantial. Production systems face data quality issues, concept drift, adversarial inputs, and integration challenges absent from benchmarks.* |

| **🔴 Limitation 2: Optimistic Assumptions About Adoption** |
|:----|
| *The paper assumes organisations can and will rationally adopt DLADM when beneficial. It underestimates institutional barriers: legacy systems, change resistance, skills gaps, and the political dynamics of technology adoption in organisations. The challenges section acknowledges costs but not adoption barriers.* |

| **🔴 Limitation 3: Unexamined Augmentation Assumptions** |
|:----|
| *The "augmentation" framing assumes DL will complement rather than substitute for human decision-making. This assumption is not examined critically. Under what conditions does augmentation occur versus automation? How do organisations design for augmentation versus inadvertent automation?* |

| **🔴 Limitation 4: Limited Engagement with Failure Modes** |
|:----|
| *The organisational challenges section mentions errors, bias, and opacity but treats them as solvable problems rather than potentially endemic features. The possibility that DLADM might systematically fail in certain contexts is not explored.* |

| **🔴 Limitation 5: Missing Governance Framework** |
|:----|
| *While the paper calls for governance mechanisms, it provides no framework for what such governance should look like. How should organisations decide when to use DL? What oversight structures are appropriate? How should algorithmic decisions be audited?* |

---

# 7. Implications for AI Governance Research

## 7.1 Contribution to Research

This paper provides foundational context for understanding how DL is conceptualised in management literature. The DLADM framework captures a common assumption: that DL augments rather than replaces human decision-making, and that the appropriate governance response is human-in-the-loop oversight.

| **🔵 Pattern Confirmation** |
|:----|
| *This paper **CONFIRMS** the pattern that technical AI literature tends to assume organisational adoption will follow from demonstrated technical capability. The gap between "DL outperforms traditional ML on benchmarks" and "organisations should implement DLADM" is bridged through assumed rational adoption. This gap is precisely where governance research should focus.* |

## 7.2 Boundary Conditions

**Claims hold when:**
- Large, clean datasets are available
- Decision tasks involve pattern recognition in unstructured data
- Organisations have technical capability (or can acquire it)
- Error costs are manageable

**Claims likely break when:**
- Data is scarce, biased, or non-representative
- Decision contexts require explainability or legal justification
- Stakes are high and errors are irreversible
- Organisational culture resists algorithmic decision support
- Regulatory environments mandate human decision-making

*Acknowledged by authors: Partially (economic challenges yes; organisational barriers no)*

## 7.3 Future Research Directions

1. Field studies of DLADM implementation in diverse organisational contexts
2. Development of governance frameworks for algorithmic decision augmentation
3. Examination of human-AI interaction patterns in DLADM settings
4. Investigation of failure modes and unintended consequences
5. Comparative analysis across industries and organisational sizes

---

# 8. Glossary of Technical Terms

| Term | Definition |
|------|------------|
| **DLADM** | Deep Learning-Augmented Decision-Making: Decision processes that incorporate DL algorithm outputs |
| **CNN** | Convolutional Neural Network: DL architecture designed for image processing with translation invariance |
| **Transfer Learning** | Using pre-trained models as starting point for new tasks to reduce data/compute requirements |
| **BERT** | Bidirectional Encoder Representations from Transformers: Pre-trained language model for NLP tasks |
| **Feature Engineering** | Manual process of creating input features for ML models (not required for DL) |
| **Activation Function** | Non-linear function applied to neuron outputs (e.g., ReLU, sigmoid) |
| **Epoch** | One complete pass through the training dataset during model training |
| **tf-idf** | Term frequency-inverse document frequency: Text vectorisation method |
| **GPU/TPU** | Graphics Processing Unit / Tensor Processing Unit: Specialized hardware for DL computation |

---

# 9. Suggested Further Reading

## 9.1 Foundational Papers
- March, J.G. & Simon, H.A. (1958). *Organizations*. Wiley. — Carnegie School foundation
- Galbraith, J.R. (1974). Organization design: An information processing view. *Interfaces*. — Information processing theory
- Goodfellow, I., Bengio, Y., & Courville, A. (2016). *Deep Learning*. MIT Press. — Comprehensive DL textbook

## 9.2 AI in Organisations
- von Krogh, G. (2018). Artificial intelligence in organizations: New opportunities for phenomenon-based theorizing. *Academy of Management Discoveries*.
- Kaplan, A. & Haenlein, M. (2020). Rulers of the world, unite! The challenges and opportunities of artificial intelligence. *Journal of Business Ethics*.
- Tambe, P., Cappelli, P., & Yakubovich, V. (2019). Artificial intelligence in human resources management: Challenges and a path forward. *California Management Review*.

## 9.3 Human-AI Interaction
- Logg, J.M., Minson, J.A., & Moore, D.A. (2019). Algorithm appreciation: People prefer algorithmic to human judgment. *OBHDP*.
- Glikson, E. & Woolley, A.W. (2020). Human trust in artificial intelligence: Review of empirical research. *Academy of Management Annals*.

## 9.4 Critical Perspectives
- Zuboff, S. (2019). *The Age of Surveillance Capitalism*. Profile Books.
- Barocas, S. & Selbst, A.D. (2016). Big data's disparate impact. *SSRN Electronic Journal*.
- Samek, W. & Müller, K.-R. (2019). Towards explainable artificial intelligence.

---

# PART 2: TEMPLATED PARAMETER MAPPING

## Triage

| Criterion | Assessment |
|-----------|------------|
| **Paper Type** | Core - Foundational for understanding DLADM conceptualisation |
| **Relevance Score** | 4/5 |
| **Bucket** | AI Implementation / Organisational Technology |
| **Rationale** | Establishes baseline assumptions about how DL augments (vs replaces) decisions; useful for identifying gaps in governance thinking |

---

## 1. Paper Identity & Positioning

| Field | Value |
|-------|-------|
| **Title** | Augmenting organizational decision-making with deep learning algorithms: Principles, promises, and challenges |
| **Authors** | Yash Raj Shrestha, Vaibhav Krishna, Georg von Krogh |
| **Year / Venue** | 2021 / Journal of Business Research |
| **Domain** | Management & Organisation Studies / AI Applications |
| **DOI** | https://doi.org/10.1016/j.jbusres.2020.09.068 |

### Level of Operation

☐ Technical (algorithms, models, metrics)
☑ Organisational (processes, roles, workflows) ← PRIMARY
☐ Institutional (governance structures, accountability)
☐ Societal (norms, public discourse, collective action)
☐ Multi-level

**It exists because** the gap between technical AI capabilities and managerial understanding is currently under-specified, limiting organisational adoption.

---

## 2. Core Claim (Distilled)

> **The Core Conditional Claim**
>
> **If** organisations have access to sufficient data, computing resources, and data science expertise,
> **then** deep learning algorithms can augment decision-making across targeting, monitoring, and scheduling functions
> **by** extracting patterns from unstructured data that humans and traditional ML cannot efficiently process.

| Dimension | Assessment |
|-----------|------------|
| **Confidence in assumption** | Medium — Demonstrated on benchmarks but not in organisational field settings |
| **Mechanism specified** | Partial — Information processing enhancement but human-AI interaction unspecified |
| **Outcome measurable** | Yes for accuracy metrics; No for decision quality or organisational performance |

### Evidence Basis

| Dimension | Assessment |
|-----------|------------|
| **Evidence type** | Tutorial + Case Studies (Empirical benchmarking) |
| **Evidence strength** | Moderate for technical claims; Weak for organisational claims |
| **Sample/scope** | Two public benchmark datasets; No organisational data |
| **Generalisability concerns** | Lab vs field validity gap; Selection bias in examples toward large tech firms |

---

## 3. System Model

### Implicit System

**Pre-DLADM State:**
```
Unstructured Data → [Manual Analysis / Traditional ML] → Limited Insights → Human Decision
```

**Post-DLADM State:**
```
Unstructured Data → [DL Algorithm] → Patterns/Predictions → Human-Augmented Decision
```

| Element | Status |
|---------|--------|
| **The gap is filled by** | DL algorithms (CNN, BERT, etc.) processing unstructured data |
| **Accountability sits with** | Unspecified — Paper mentions "managers in driver's seat" but no accountability framework |
| **This is** | Implicit |

### Transformation Vector

☑ Tool substitution (DL replaces traditional ML for specific tasks)
☐ Process redesign (not addressed)
☐ Structural change (mentioned but not developed)
☐ Institutional evolution (not addressed)

---

## 4. Assumptions

### 4.1 Technical Assumptions

> The argument relies on technical stability around **DL model performance**,
> which is treated as: **Tested** (on benchmarks)

**Critical technical dependencies:**
1. Data quality and quantity sufficient for DL training
2. GPU/TPU computing infrastructure availability
3. Model performance generalises from benchmark to production

### 4.2 Organisational Assumptions ⭐ KEY SECTION

**Organisational behaviour assumed:** 🟡 Optimistic

| Actor | Assumption | Reality Check |
|-------|------------|---------------|
| **Leadership** | Will invest in DLADM when ROI demonstrated | Cost justification difficult; competing priorities |
| **Middle management** | Will adopt algorithmic inputs | Potential resistance; job security concerns |
| **Operators/Users** | Will use DL outputs appropriately | Automation bias / algorithm aversion unaddressed |
| **Data scientists** | Available and skilled | Labor market shortage acknowledged |

### Incentive Alignment Check

| Actor | Optimises for | Alignment |
|-------|---------------|-----------|
| Leadership | Efficiency, cost reduction | ✓ |
| Middle Management | Role preservation | ⚠ Potentially threatened |
| Operators/Workers | Task completion, job security | ? Unspecified |
| Data Scientists | Technical excellence | ✓ |

### Policy-Practice Gap

| Dimension | Assessment |
|-----------|------------|
| **Policy assumes** | Rational adoption following technical demonstration |
| **Organisation actually does** | Not examined |
| **Gap explained by** | Not addressed |
| **Who benefits from gap** | Not addressed |

### 4.3 Policy/Institutional Assumptions ⭐ KEY SECTION

This work assumes governance and accountability will:

☐ Function as designed
☐ Require adaptation (specifies how)
☐ Face systematic barriers (identifies them)
☑ Not addressed

| Mechanism | Status |
|-----------|--------|
| **Enforcement mechanism** | Not addressed |
| **Accountability mechanism** | Mentioned as needed; not specified |

---

## 5. Lens Checks

### 5.1 Human Behaviour Lens — Status: 🟡 IMPLICIT

| Dimension | Assessment |
|-----------|------------|
| **Human role** | On-the-loop (monitoring DL outputs) |
| **Attention/cognitive load** | Not addressed |
| **Trust calibration** | Mentioned in challenges but not developed |

**Failure modes considered:**

- ☐ Automation bias (over-reliance on AI)
- ☐ Algorithm aversion (under-reliance on AI)
- ☐ Deskilling (capability atrophy)
- ☑ Accountability diffusion (mentioned)
- ☐ Alert fatigue
- ☐ Expertise asymmetry

### 5.2 Incentives Lens — Status: 🔴 ABSENT

| Element | Assessment |
|---------|------------|
| **Gaming potential** | Not addressed |
| **Goodhart risk** | Not addressed |

### 5.3 Institutional Reality Lens — Status: 🔴 ABSENT

| Element | Assessment |
|---------|------------|
| **Cross-boundary coordination** | Not addressed |
| **Regulatory capacity** | Privacy mentioned; regulatory constraints not developed |

---

## 6. Comparative Context

| Dimension | This Paper |
|-----------|------------|
| **Stronger on** | Technical accessibility; Reproducible demonstrations; Honest challenge acknowledgment |
| **Weaker on** | Organisational field validity; Governance frameworks; Human-AI interaction |
| **Novel contribution** | DLADM conceptualisation; Targeting/Monitoring/Scheduling taxonomy |
| **Gap not addressed** | How organisations actually implement and govern algorithmic decision support |

### Literature Positioning

This paper sits: **At the intersection of information systems, strategic management, and AI/ML**, positioned as a bridge for management scholars to understand DL.

Gap in literature: **The translation from "technically possible" to "organisationally implemented and governed" remains undertheorised.**

---

## 7. Synthesis & Research Insight

### Pattern Recognition

> [!TIP]
> **🔵 Pattern Confirmation**
> 
> *This paper **CONFIRMS** the pattern that AI/ML management literature assumes rational adoption following technical demonstration, without engaging deeply with adoption barriers, political dynamics, or governance requirements. The gap between "technically possible" and "organisationally implemented" remains undertheorised.*

### Contribution to Thesis

| Dimension | Assessment |
|-----------|------------|
| **Supports argument** | Provides accessible baseline for understanding technical DLADM claims |
| **Challenges argument** | Does not challenge; reinforces augmentation optimism |
| **Provides evidence for** | DL technical superiority over traditional ML on benchmark tasks |

### Boundary Conditions

**Claims hold when:**
- Large, clean datasets are available
- Decision tasks involve pattern recognition in unstructured data
- Organisations have technical capability (or can acquire it)
- Error costs are manageable

**Claims break if:**
- Data is scarce, biased, or non-representative
- Decision contexts require explainability or legal justification
- Stakes are high and errors are irreversible
- Organisational culture resists algorithmic decision support
- Regulatory environments mandate human decision-making

*Acknowledged by authors: Partially*

---

## 8. Metadata & Linkages

| Field | Value |
|-------|-------|
| **Tags** | deep-learning, organisational-decision-making, AI-augmentation, information-processing, CNN, NLP, BERT, transfer-learning |
| **Collections** | AI-in-Organisations, Technical-Foundations |
| **Related Items** | vonKrogh2018, Kaplan2020, Tambe2019, MarchSimon1958 |

### Research Questions Relevance

| Research Question | Relevance | Score |
|-------------------|-----------|-------|
| How do organisations govern AI decision support? | Medium — Identifies need but no framework | 3/5 |
| What organisational conditions enable/constrain AI adoption? | Low — Assumed rather than examined | 2/5 |
| How do humans interact with algorithmic decision aids? | Low — Mentioned but not developed | 2/5 |

### Follow-ups

**Questions to revisit:**
- How do the authors' subsequent papers develop the DLADM concept?
- Has the targeting/monitoring/scheduling taxonomy been validated empirically?
- What field studies exist of actual DLADM implementation?

**Connections to other papers:**
- Links to von Krogh (2018) on AI in organisations
- Extends information processing view (Galbraith, 1974; Tushman & Nadler, 1978)
- Complements Tambe et al. (2019) on AI in HR

**Potential quotes for thesis:**
- Page 599: "there are no 'free lunches' with DL. Managers must remain in the driver's seat" — Useful for framing governance requirements
- Page 600: "managers become accountable and are required to set up a governance mechanism" — Identifies accountability gap

---

*— End of Annotation —*
