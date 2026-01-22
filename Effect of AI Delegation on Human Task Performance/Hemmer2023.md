# Annotations

## "Human-AI Collaboration: The Effect of AI Delegation on Human Task Performance and Task Satisfaction"

**Hemmer et al. (2023)**

*A Comprehensive Analysis of AI Delegation, Algorithmic Management, and Human Behavioural Response in Human-AI Teaming*

Critical Commentary, Theoretical Analysis, Organisational Implications, and Research Gaps

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

# 1. Executive Summary and Research Significance

## 1.1 Why This Paper Matters

Published at ACM IUI 2023, "Human-AI Collaboration: The Effect of AI Delegation on Human Task Performance and Task Satisfaction" represents a significant empirical contribution to understanding how humans respond when artificial intelligence systems take on managerial functions. While delegation algorithms have been proposed in the machine learning literature, this paper is among the first to rigorously test whether the psychological and behavioural assumptions underlying these algorithms hold in practice.

The paper addresses a critical gap: prior work on AI delegation evaluated algorithms using either synthetically generated human predictions or predictions collected in annotation settings where participants were unaware of any AI involvement. Hemmer et al. ask the essential question — does human behaviour change when people know they are being managed by an AI? Their answer, surprisingly, is "no" — but this finding itself opens significant questions about the nature of algorithmic management.

> [!NOTE]
> **🟡 Historical Context**
> 
> *Before this paper, the dominant paradigm in human-AI collaboration research focused on AI-assisted decision-making, where humans receive AI recommendations and choose whether to accept them. This placed humans in the role of final decision-maker. AI delegation inverts this relationship: the AI decides which tasks humans should perform. This shift from "AI as advisor" to "AI as manager" has profound implications for workplace dynamics, yet had received minimal empirical attention with real human participants.*

## 1.2 The Paradigm Shift

The paper's core contribution is demonstrating that AI delegation can improve both objective performance and subjective satisfaction — and crucially, that these improvements occur regardless of whether humans are aware of the delegation. This finding challenges the assumption that transparency about algorithmic management is necessary for positive outcomes.

However, the finding also raises deeper questions. If humans perform better on capability-matched tasks whether or not they know an AI selected those tasks, what does this tell us about the mechanism? The authors identify self-efficacy as the mediating variable — humans feel more confident when given tasks matched to their abilities, and this confidence improves both performance and satisfaction.

> [!WARNING]
> **🔴 Critical Analysis**
> 
> *The title and framing emphasise the positive effects of AI delegation, but a more provocative reading is possible: the paper demonstrates that algorithmic management can be effective without worker awareness or consent. This has significant implications for workplace autonomy and informed consent that the paper acknowledges but does not deeply engage with. The gig economy applications cited (Uber, task platforms) have faced substantial criticism precisely for opaque algorithmic management. The finding that hidden delegation works equally well could be read as either reassuring (workers benefit regardless) or concerning (informed consent is unnecessary for extraction of improved performance).*

---

# 2. Paper Overview and Key Contributions

## 2.1 Core Contributions

The paper makes five distinct contributions to the literature on human-AI collaboration:

- **Empirical Validation of Delegation Algorithms:** Prior work proposed delegation algorithms (Raghu et al. 2019, Mozannar & Sontag 2020) but evaluated them with simulated or context-free human predictions. This paper provides the first rigorous test of whether these algorithms work when humans are aware of and potentially reactive to the delegation.

- **Mechanism Identification:** By measuring self-efficacy as a mediating variable, the paper moves beyond demonstrating "what works" to explaining "why it works." This mechanistic insight has implications for designing future human-AI collaboration systems.

- **Hidden vs. Explicit Delegation Comparison:** The experimental design's inclusion of both aware and unaware delegation conditions allows direct comparison, resolving uncertainty about whether transparency matters for outcomes.

- **Task Satisfaction Measurement:** Most prior work on human-AI teaming focused exclusively on performance metrics. By including satisfaction measures, the paper addresses the human experience of algorithmic management.

- **Theoretical Integration:** The paper bridges organisational behaviour literature on supervisor-employee delegation with AI research, applying established constructs (self-efficacy, empowerment) to the novel context of algorithmic management.

## 2.2 Author Team and Institutional Context

The paper emerges from Karlsruhe Institute of Technology (KIT) in Germany, with collaboration from Ben-Gurion University of the Negev in Israel. KIT has established itself as a leading centre for research on AI-assisted decision-making and human-AI collaboration.

> [!TIP]
> **🔵 Attribution Analysis**
> 
> *The author contributions span the full research pipeline: Hemmer and Schemmer on experimental design and analysis, Westphal bringing organisational behaviour expertise (particularly important for the self-efficacy framing), Vetter on implementation, and Vössing and Satzger providing senior oversight. This interdisciplinary team structure — combining HCI, machine learning, and organisational psychology — is increasingly common and arguably necessary for rigorous human-AI collaboration research.*

---

# 3. Section-by-Section Annotations

## 3.1 Abstract Analysis

The abstract establishes four key claims in 167 words: (1) prior work on AI delegation used simulated or context-independent human predictions; (2) this paper tests delegation with real participants who may or may not be aware of AI involvement; (3) delegation improves both performance and satisfaction; (4) self-efficacy mediates these effects.

> [!WARNING]
> **🔴 Critical Analysis**
> 
> *The abstract makes the strong claim that findings "provide initial evidence that allowing AI models to take over more management responsibilities can be an effective form of human-AI collaboration in workplaces." This is a significant interpretive leap from an image classification task with crowdworkers to workplace management broadly. The hedging ("initial evidence", "can be") is appropriate, but the implication is clear: the authors see this as foundational work for algorithmic management systems. Readers should note this positioning.*

## 3.2 Introduction (Section 1)

The introduction situates AI delegation within the broader landscape of human-AI collaboration. The authors note that AI models now match or exceed human performance in specific domains, yet "human predictions often remain more accurate for certain cases." This complementarity motivates delegation approaches that assign tasks to whichever party (human or AI) is more likely to succeed.

**The key research questions are clearly stated:**

- **RQ1:** How does AI delegation affect task performance compared to human and AI working alone?
- **RQ2:** How does AI delegation affect task satisfaction compared to human working alone?
- **RQ3:** What explains the effect of AI delegation on task performance and task satisfaction?

> [!IMPORTANT]
> **🟢 Key Insight**
> 
> *The framing of RQ3 — asking "what explains" rather than "does it work" — reflects methodological sophistication. The authors anticipate finding positive effects and design the study to identify mechanisms. This a priori commitment to explanation, not just demonstration, strengthens the contribution. However, it also suggests the hypothesis space was narrowed before data collection; alternative mechanisms (e.g., reduced cognitive load, novelty effects) receive less attention.*

## 3.3 Related Work (Section 2)

The literature review distinguishes AI delegation from AI-assisted decision-making — the dominant paradigm where AI provides recommendations that humans accept or override. In AI-assisted settings, the human retains final decision authority, and research focuses on appropriate reliance (avoiding over- and under-reliance on AI recommendations).

AI delegation inverts this relationship: the AI decides what humans should work on. The authors cite foundational delegation algorithms (Mozannar & Sontag 2020, Raghu et al. 2019, Wilder et al. 2020) that learn both AI and human capabilities to optimise task allocation. Crucially, these prior works "assume that the behavior and perceptions of humans... remain unchanged whether or not an AI model delegates instances of a task."

> [!WARNING]
> **🔴 Critical Analysis**
> 
> *The related work section positions the paper well but omits important adjacent literatures. The algorithmic management literature (Lee et al. 2015, Möhlmann & Henfridsson 2019) — which documents worker experiences with platform-based algorithmic management — is cited only briefly. This literature has found predominantly negative worker perceptions of algorithmic management, creating tension with the positive findings here. The gig economy context receives acknowledgment but not deep engagement. Similarly, the automation and deskilling literature (Braverman 1974, Zuboff 1988) — which theorises how task allocation affects worker skill development — is absent. These omissions shape the paper's optimistic framing.*

## 3.4 Theory Development and Hypotheses (Section 3)

The theoretical framework draws on organisational behaviour research regarding supervisor-to-employee delegation. The authors argue that when delegation aligns with employee competencies, it results in "more empowered, motivated, and higher-performing employees." They transfer this insight to AI delegation, hypothesising positive effects on performance (H1) and satisfaction (H2).

The mechanistic hypothesis (H3, H4) posits self-efficacy as the mediating variable. Self-efficacy — "a person's belief in one's own ability to complete a task successfully" (Bandura 1977) — is a well-established construct in organisational psychology.

> [!TIP]
> **🔵 Theoretical Integration**
> 
> *The choice to draw on organisational behaviour literature rather than pure AI/HCI research is strategic and productive. It provides established constructs (self-efficacy, empowerment) with validated measurement instruments, grounds the work in a broader theoretical tradition, and makes the findings legible to management scholars. However, this framing also imports assumptions — particularly that AI-to-human delegation functions analogously to supervisor-to-employee delegation. Whether this analogy holds is an empirical question the paper assumes rather than tests.*

## 3.5 Methodology (Section 4)

### 3.5.1 Data and Task Selection

The study uses a modified ImageNet subset (Steyvers et al. 2022) with 1,200 images across 16 classes, distorted with phase noise to create difficulty for both humans and AI. This task choice is deliberate: it requires no specialised expertise (ensuring participant recruitment feasibility) while allowing similar human and AI performance levels (ensuring meaningful delegation decisions).

> [!WARNING]
> **🔴 Critical Analysis: Task Ecological Validity**
> 
> *The image classification task, while experimentally clean, differs substantially from real-world algorithmic management contexts. In gig economy platforms, tasks often have: (1) variable difficulty that may not be estimable a priori, (2) temporal dependencies between tasks, (3) worker learning and skill development over time, (4) real financial stakes, (5) social/status implications of task assignment. The distorted ImageNet setup eliminates these complexities, enabling causal inference but limiting generalisability. The authors acknowledge this in limitations but the experimental design prioritises internal over external validity.*

### 3.5.2 AI Model Architecture

The delegation algorithm implements Raghu et al.'s (2019) approach: a DenseNet-161 classifier estimates AI confidence while a parallel "human error model" estimates human confidence from training data. Instances are delegated to humans when estimated human confidence exceeds AI confidence.

The model was trained on 60% of the data with 20% validation and 20% test sets. Fine-tuning used SGD with learning rate 10⁻⁴, weight decay 5×10⁻⁴, cosine annealing schedule, batch size 16, and early stopping on validation loss.

> [!NOTE]
> **⚪ Technical Note**
> 
> *The delegation algorithm's effectiveness depends critically on the quality of human confidence estimates. These estimates are derived from historical human predictions in the training data — predictions collected without any AI involvement. The paper assumes these historical predictions generalise to new participants and to participants who know about AI delegation. This assumption is testable but not tested; it would require comparing predicted vs. actual human confidence in the experimental conditions.*

### 3.5.3 Experimental Design

The study employed a between-subjects design with three conditions:

- **Delegation Condition (n=66):** Participants classified 20 images randomly drawn from instances the AI model selected for delegation. They were explicitly told "the AI will decide for each image whether to label it alone or to pass it on to you for labeling." Additionally, 5 images were shown with messages indicating the AI had already classified them.

- **Hidden Delegation Condition (n=67):** Participants classified the same set of delegated images but without any mention of AI involvement. Instructions simply stated "Just as previously, you will decide on the label for each image."

- **Human-Alone Control (n=63):** Participants classified 20 images randomly drawn from the full test set, with no AI involvement mentioned.

> [!NOTE]
> **🟣 Design Analysis**
> 
> *The three-condition design is well-constructed for the primary research questions but has limitations. The delegation and hidden delegation conditions use the same image subset (those selected for human delegation), while the human-alone condition uses random images. This means condition differences conflate two factors: (1) task difficulty/suitability and (2) awareness of AI involvement. The authors address this by noting that the key comparison for awareness effects is delegation vs. hidden delegation, which use identical stimuli. However, the human-alone condition serves as baseline for both performance and mechanism analyses, and its different stimulus set is a potential confound.*

---

# 4. Methodological Deep Dive

## 4.1 Participant Recruitment and Sample

196 participants were recruited via Prolific Academic after exclusions for failed attention/manipulation checks (13 participants) and missing data (1 participant). The sample had mean age 39.43 years (SD=13.13) and was 58.67% female. Participants received $1.5 for approximately 10 minutes of work, yielding an effective hourly rate of $9/hour.

Sample size was determined a priori using G*Power, targeting detection of small effects (f²=0.10) with 0.95 power in a three-group regression with three predictors. This required 176 participants; 210 were recruited anticipating attrition.

> [!IMPORTANT]
> **🟢 Methodological Strength**
> 
> *Pre-registered power analysis with a priori sample size determination is best practice that many HCI studies omit. The conservative small effect size assumption is appropriate for a novel manipulation. However, the power analysis assumes the regression model specified; the actual analyses include seven control variables (not three), which affects power and multiple comparison concerns.*

## 4.2 Measurement Instruments

**Task Performance:** Measured as classification accuracy (percentage correct out of 20 images). This is an objective measure with clear interpretation.

**Task Satisfaction:** Three items adapted from Hofmann & Strickland (1995) on 5-point Likert scales: overall satisfaction with performance, satisfaction with learning, enjoyment of the task. Cronbach's α = 0.73 (acceptable but not strong internal consistency).

**Self-Efficacy:** Three items adapted from Spreitzer (1995) on 7-point Likert scales: confidence in ability, mastery of necessary skills, self-assurance about capabilities. Cronbach's α = 0.89 (good internal consistency).

**Control Variables:** Task experience, algorithm attitude (5-point), algorithm use frequency (5-point), cognitive ability for visual tasks (4 items, 7-point, α=0.86), education, age, gender.

> [!WARNING]
> **🔴 Measurement Validity**
> 
> *"Task satisfaction" in a 10-minute crowdworking context differs substantially from "job satisfaction" in ongoing employment relationships. The satisfaction measure captures immediate reaction to a brief task, not the sustained satisfaction relevant to workplace algorithmic management. Additionally, the cognitive ability measure is self-reported rather than objectively assessed, introducing potential bias.*

## 4.3 Statistical Analysis

Key findings from the regression analyses:

| Outcome | Delegation | Hidden Del. | Human-Alone |
|---------|------------|-------------|-------------|
| Task Performance (%) | 84.51 (11.24) | 83.73 (12.29) | 67.13 (13.11) |
| Task Satisfaction (1-5) | 3.65 (0.66) | 3.62 (0.73) | 3.35 (0.70) |
| Self-Efficacy (1-7) | 5.29 (0.96) | 5.37 (1.05) | 4.63 (1.25) |

*Note: Values are Mean (SD). All delegation vs. human-alone comparisons p < 0.01. No significant differences between delegation and hidden delegation conditions.*

---

# 5. Theoretical Framework Analysis

## 5.1 Self-Efficacy as Mediating Mechanism

The paper's core theoretical contribution is identifying self-efficacy as the mechanism linking AI delegation to improved outcomes. The mediation model shows that delegation increases self-efficacy (β=0.75-0.80, p<0.001), and increased self-efficacy improves both performance (β=0.62, p<0.001) and satisfaction (β=0.39, p<0.001).

The self-efficacy mediation fully accounts for the effect on satisfaction (direct effect becomes non-significant) but only partially mediates the performance effect (direct effect remains significant). This suggests performance improvements operate through multiple channels, with self-efficacy being one important pathway.

> [!TIP]
> **🔵 Theoretical Interpretation**
> 
> *The finding that self-efficacy fully mediates satisfaction effects is theoretically coherent: feeling capable makes work more enjoyable. The partial mediation for performance suggests additional mechanisms. One plausible candidate is simply task difficulty — delegated images may be objectively easier for humans regardless of subjective confidence. The paper does not report objective difficulty measures for delegated vs. non-delegated images, making it impossible to distinguish capability-matching from difficulty-selection.*

## 5.2 Organisational Behaviour Framing

The paper frames AI delegation as analogous to supervisor-to-employee delegation, drawing on management literature (Schriesheim et al. 1998, Leana 1986, 1987). This framing provides theoretical grounding but may obscure important differences:

Human supervisors have social relationships with employees, provide feedback and mentorship, can explain delegation rationale when asked, adapt delegation based on observation, and are accountable to the same organisation. AI delegation systems lack these characteristics — they optimise based on historical patterns without social context or ongoing relationship.

> [!WARNING]
> **🔴 Theoretical Limitation**
> 
> *The analogy between human and AI delegation may not hold under conditions that activate the differences. In the experimental setup, participants completed a brief task with no ongoing relationship, feedback, or stakes — conditions that minimise the relevance of supervisor-employee relationship dynamics. In sustained workplace contexts, the absence of relationship, explanation, and accountability may become salient and undermine the positive effects observed here. The Uber driver studies (Möhlmann & Henfridsson 2019) suggest this is indeed the case.*

## 5.3 Missing Theoretical Lenses

Several theoretical frameworks relevant to AI delegation receive minimal attention:

- **Automation and Deskilling:** Braverman's (1974) labour process theory and subsequent work on technological deskilling predicts that algorithmic task allocation may reduce worker skill development by limiting exposure to challenging tasks.

- **Principal-Agent Theory:** The AI delegation system creates a novel principal-agent relationship where the AI acts as agent for organisational principals in managing human workers.

- **Street-Level Bureaucracy:** Lipsky's (1980, 2010) framework on discretion and adaptation in implementation contexts could illuminate how workers might game or resist algorithmic management.

- **Sociotechnical Systems:** The paper treats the AI delegation system as a technical intervention without analysing how it would integrate with existing workplace social and technical systems.

---

# 6. Critical Assessment and Limitations

## 6.1 What the Paper Gets Right

- **Rigorous Experimental Design:** The three-condition between-subjects design with pre-registered sample size provides strong causal inference for the primary research questions. The inclusion of both aware and hidden delegation conditions is particularly valuable.

- **Mechanism Identification:** Moving beyond "does it work?" to "why does it work?" represents methodological maturity. The self-efficacy mediation analysis provides actionable insight for system design.

- **Interdisciplinary Integration:** Drawing on organisational behaviour literature for constructs and measures strengthens the theoretical grounding and makes findings accessible to management researchers.

- **Appropriate Hedging:** The paper generally avoids overclaiming, acknowledging limitations in generalisability and calling for future research on expert domains and long-term effects.

## 6.2 Significant Limitations

> [!CAUTION]
> **🔴 Limitation 1: Task Ecological Validity**
> 
> *The distorted image classification task differs fundamentally from real-world algorithmic management contexts. It involves no learning, no interdependence, no career stakes, no social comparison, and no ongoing relationship with the algorithmic system. Findings may not transfer to contexts where these factors matter — which is most workplace contexts.*

> [!CAUTION]
> **🔴 Limitation 2: Participant Population**
> 
> *Prolific crowdworkers are not representative of workers who would be subject to algorithmic management in practice. They self-select into short tasks for small payments, may have different attitudes toward algorithmic systems, and lack the organisational embeddedness of traditional employees. The relatively high mean age (39.4 years) is notable and may affect generalisability to younger workforces.*

> [!CAUTION]
> **🔴 Limitation 3: Short Time Horizon**
> 
> *The 10-minute task duration cannot capture effects that emerge over time: deskilling, learned helplessness, adaptation of strategies to game the algorithm, erosion of initial positive effects, or cumulative satisfaction/dissatisfaction. Long-term field studies are needed but not conducted.*

> [!CAUTION]
> **🔴 Limitation 4: Organisational Context Abstraction**
> 
> *The experimental design eliminates all organisational context: no managers, no coworkers, no organisational culture, no career incentives, no power dynamics. This enables clean causal inference but severely limits applicability to real organisations where these factors shape responses to algorithmic management.*

> [!CAUTION]
> **🔴 Limitation 5: Incentive and Gaming Dynamics**
> 
> *The paper does not consider strategic behaviour. In ongoing algorithmic management, workers might learn to manipulate the signals used for capability estimation, potentially corrupting the delegation algorithm's accuracy. This Goodhart's Law dynamic is central to algorithmic management critiques but unexamined here.*

---

# 7. Implications for AI Governance Research

## 7.1 Contribution to Thesis Argument

This paper provides important evidence for the thesis that AI governance literature treats organisations as neutral transmission mechanisms for technical solutions. The paper demonstrates positive effects of AI delegation in a context that has been deliberately purged of organisational dynamics — and the authors explicitly recommend that "managers could consider applying AI delegation to yield higher levels of performance and employee satisfaction" based on these findings.

> [!TIP]
> **🔵 Pattern Confirmation**
> 
> *This paper CONFIRMS a recurring pattern across the human-AI collaboration literature: ALGORITHMIC MANAGEMENT is framed as a TECHNICAL/BEHAVIOURAL problem (can we design algorithms that effectively match tasks to capabilities?) while ORGANISATIONAL/INSTITUTIONAL factors (power dynamics, resistance, gaming, deskilling) are acknowledged as limitations but not integrated into the research design or theoretical framework.*

## 7.2 Boundary Conditions for Claims

**The paper's claims hold when:**

- Tasks are independent and do not require coordination or knowledge-sharing
- Workers have no intrinsic interest in task variety or challenge
- Performance is easily measurable and aligned with organisational goals
- Time horizons are short (no skill development concerns)
- Workers have no power to resist or exit the system
- There are no regulatory requirements for human oversight or explanation

**The paper's claims likely break when:**

- Middle managers perceive AI delegation as threatening their role
- Workers value autonomy in task selection as part of professional identity
- Tasks require tacit knowledge that develops through diverse experience
- Workers can strategically manipulate capability signals
- Organisational culture emphasises human judgement and discretion
- Regulatory frameworks require transparency in automated decision-making

## 7.3 Future Research Directions

For the AI governance research agenda, this paper suggests several productive directions:

- **Field Studies of Algorithmic Management:** Laboratory findings need validation in real organisational contexts with ongoing relationships, career stakes, and social dynamics.

- **Gaming and Adaptation Dynamics:** How do workers learn about and respond to delegation algorithms over time? Do initial positive effects persist or erode?

- **Organisational Implementation Barriers:** What factors determine whether organisations successfully implement AI delegation?

- **Accountability and Governance Structures:** How should responsibility be allocated when AI delegation leads to errors?

- **Distributional and Equity Effects:** Do AI delegation systems systematically advantage or disadvantage particular worker groups?

---

# 8. Glossary of Technical Terms

| Term | Definition |
|------|------------|
| **AI Delegation** | A form of human-AI collaboration where the AI system decides which task instances to handle itself and which to assign to human workers, based on estimated capabilities of each party. |
| **Algorithmic Management** | The use of algorithms to perform managerial functions such as task allocation, performance monitoring, and evaluation. Common in gig economy platforms. |
| **Confidence Calibration** | The alignment between a model's expressed confidence and its actual accuracy. A well-calibrated model that says it's 80% confident should be correct 80% of the time. |
| **DenseNet** | A convolutional neural network architecture where each layer connects to all subsequent layers, enabling feature reuse and gradient flow. |
| **Human Error Model** | A model that predicts whether humans will correctly classify specific instances, trained on historical human prediction data. |
| **Mediation Analysis** | Statistical technique to test whether the effect of an independent variable on a dependent variable operates through an intermediate (mediating) variable. |
| **PROCESS Macro** | A computational tool for mediation, moderation, and conditional process analysis developed by Andrew Hayes. |
| **Prolific Academic** | An online platform for recruiting research participants, generally considered higher quality than Amazon Mechanical Turk for academic research. |
| **Self-Efficacy** | A person's belief in their capability to execute behaviours necessary to produce specific outcomes (Bandura 1977). Distinct from actual capability. |
| **Task Satisfaction** | An individual's affective response to their work on a specific task, including enjoyment and sense of accomplishment. |

---

# 9. Suggested Further Reading

## 9.1 Foundational Papers on AI Delegation

- Raghu et al. (2019) — "The Algorithmic Automation Problem: Prediction, Triage, and Human Effort"
- Mozannar & Sontag (2020) — "Consistent Estimators for Learning to Defer to an Expert"
- Wilder, Horvitz & Kamar (2020) — "Learning to Complement Humans"

## 9.2 Algorithmic Management Literature

- Lee et al. (2015) — "Working with Machines: The Impact of Algorithmic and Data-Driven Management on Human Workers"
- Möhlmann & Henfridsson (2019) — "What People Hate About Being Managed by Algorithms"
- Benlian et al. (2022) — "Algorithmic Management: Bright and Dark Sides"

## 9.3 Self-Efficacy and Organisational Behaviour

- Bandura (1977) — "Self-Efficacy: Toward a Unifying Theory of Behavioral Change"
- Spreitzer (1995) — "Psychological Empowerment in the Workplace"
- Schriesheim, Neider & Scandura (1998) — "Delegation and Leader-Member Exchange"

## 9.4 Critical Perspectives

- Braverman (1974) — "Labor and Monopoly Capital"
- Zuboff (1988) — "In the Age of the Smart Machine"
- Lipsky (1980, 2010) — "Street-Level Bureaucracy"

---

---

# PART 2: PARAMETER MAPPING

---

---

# Triage

| Field | Value |
|-------|-------|
| **Paper Type** | Core |
| **Relevance Score** | 5/5 |
| **Bucket** | Human-Machine Interaction |
| **Rationale** | Directly addresses human behaviour in AI delegation contexts, examines self-efficacy as mediating mechanism, and tests assumptions about human-AI collaboration in organizational settings. |

---

# 1. Paper Identity & Positioning

| Field | Value |
|-------|-------|
| **Title** | Human-AI Collaboration: The Effect of AI Delegation on Human Task Performance and Task Satisfaction |
| **Authors** | Patrick Hemmer, Monika Westphal, Max Schemmer, Sebastian Vetter, Michael Vössing, Gerhard Satzger |
| **Year / Venue** | 2023 / ACM IUI (28th International Conference on Intelligent User Interfaces) |
| **Domain** | Human-AI Collaboration / Organisational Behaviour / HCI |
| **DOI** | https://doi.org/10.1145/3581641.3584052 |

## Level of Operation

This paper operates primarily at the level of:

- ☐ Technical (algorithms, models, metrics)
- **☑ Organisational (processes, roles, workflows) ← PRIMARY**
- ☐ Institutional (governance structures, accountability)
- ☐ Societal (norms, public discourse, collective action)
- ☐ Multi-level

> [!TIP]
> **It exists because**
> 
> *HUMAN BEHAVIOURAL RESPONSE TO AI-INITIATED DELEGATION is currently under-specified or failing. Existing delegation algorithms assume humans behave identically whether or not they know AI is managing their task allocation.*

---

# 2. Core Claim (Distilled)

> [!IMPORTANT]
> **The Core Conditional Claim**
> 
> *If [AI DELEGATION ALGORITHMS MATCH TASKS TO HUMAN CAPABILITIES] holds, then [DELEGATING INSTANCES WHERE HUMANS HAVE HIGHER PREDICTED CONFIDENCE] will lead to [IMPROVED TASK PERFORMANCE AND TASK SATISFACTION VIA INCREASED SELF-EFFICACY].*

| Dimension | Assessment |
|-----------|------------|
| **Confidence in assumption** | Medium — tested in controlled lab setting with non-experts |
| **Mechanism specified** | Yes — self-efficacy as mediating variable |
| **Outcome measurable** | Yes — accuracy (objective), satisfaction/self-efficacy (Likert scales) |

## Evidence Basis

| Dimension | Assessment |
|-----------|------------|
| **Evidence type** | Empirical — Randomised controlled experiment |
| **Evidence strength** | Strong for controlled setting; moderate for generalisability |
| **Sample/scope** | n=196 Prolific participants, image classification task, 3 conditions |
| **Generalisability concerns** | Non-expert participants; generic task; short-duration study; no real stakes |

---

# 3. System Model

## Implicit System

**Pre-AI State:**
```
Human → Task Assignment (random/manager) → Task Execution → Outcome
```

**Post-AI State:**
```
Human → AI Delegation Model → Capability-Matched Tasks → Outcome
```

| Element | Status |
|---------|--------|
| **The gap is filled by** | AI model that estimates both AI and human confidence per instance |
| **Accountability sits with** | Unaddressed — paper focuses on performance, not accountability |
| **This is** | Implicit — system model exists but accountability unexamined |

## Transformation Vector

This paper assumes transformation is:

- ☐ Tool substitution (AI replaces discrete task)
- **☑ Process redesign (AI reshapes workflow) ← CLAIMED & DEMONSTRATED**
- ☐ Structural change (AI shifts roles/accountability)
- ☐ Institutional evolution (AI changes governance norms)

*Note: Paper is appropriately scoped — claims match specification.*

---

# 4. Assumptions

## 4.1 Technical Assumptions

The argument relies on technical stability around AI CONFIDENCE ESTIMATION ACCURACY, which is treated as: **Given** — the delegation algorithm's confidence estimates are assumed to correctly predict relative human/AI performance.

**Critical technical dependencies:**

- Human predictions collected during training generalize to deployment
- Confidence calibration is accurate for both AI and human models
- Task characteristics (image classification) transfer to other domains

## 4.2 Organisational Assumptions ⭐ KEY SECTION

**Organisational behaviour assumed:** Optimistic / Unspecified

| Actor | Assumption |
|-------|------------|
| **Leadership** | Not addressed — no org hierarchy in experimental setup |
| **Middle management** | Not addressed — AI replaces managerial function |
| **Operators/Users** | Assumes workers accept AI task assignment without resistance |
| **Cross-functional coordination** | Not addressed — isolated task context |

### Incentive Alignment Check

| Actor | Optimises for | Alignment |
|-------|---------------|-----------|
| Leadership | Efficiency, cost reduction | ? Unspecified |
| Middle Management | N/A — replaced by AI | ⚠ Threatened |
| Operators/Workers | Task completion, satisfaction | ✓ Aligned (per study) |

### Policy-Practice Gap

| Dimension | Assessment |
|-----------|------------|
| **Policy assumes** | Algorithmic management can replicate/improve human management |
| **Organisation actually does** | Unknown — study abstracts away org context |
| **Gap explained by** | Lab setting eliminates org dynamics (power, politics, resource constraints) |
| **Who benefits from gap** | Platform providers (Uber cited); researchers claiming clean results |

## 4.3 Policy/Institutional Assumptions ⭐ KEY SECTION

This work assumes governance and accountability will:

- ☐ Function as designed
- ☐ Require adaptation
- ☐ Face systematic barriers
- **☑ Not addressed**

| Element | Status |
|---------|--------|
| **Enforcement mechanism** | Not addressed |
| **Accountability mechanism** | Not addressed — critical gap for algorithmic management |

---

# 5. Lens Checks

## 5.1 Human Behaviour Lens — Status: EXPLICIT

| Dimension | Assessment |
|-----------|------------|
| **Human role** | In-the-loop — humans execute delegated tasks |
| **Attention/cognitive load** | Partially addressed — cognitive ability measured as control variable |
| **Trust calibration** | Partially addressed — algorithm attitude measured |

**Failure modes considered:**

- ☐ Automation bias (over-reliance on AI)
- ☐ Algorithm aversion (under-reliance on AI)
- ☐ Deskilling (capability atrophy)
- ☐ Accountability diffusion
- ☐ Alert fatigue
- ☐ Expertise asymmetry
- **☑ Self-efficacy effects — CENTRAL TO PAPER**

## 5.2 Incentives Lens — Status: ABSENT

The paper assumes actors optimise for TASK COMPLETION AND SATISFACTION, but does NOT account for strategic behaviour.

| Element | Assessment |
|---------|------------|
| **Gaming potential** | Unaddressed — what if workers game confidence signals? |
| **Goodhart risk** | Unaddressed — optimising for delegation may corrupt capability signals |

## 5.3 Institutional Reality Lens — Status: ABSENT

Institutional enforcement and accountability are: **Irrelevant to scope**

| Element | Assessment |
|---------|------------|
| **Cross-boundary coordination** | Not addressed |
| **Regulatory capacity** | Not addressed |

---

# 6. Comparative Context

| Dimension | This Paper |
|-----------|------------|
| **Stronger on** | Causal mechanism (self-efficacy); rigorous experimental design; mediating variable analysis |
| **Weaker on** | Organisational context; institutional dynamics; long-term effects; expert domains |
| **Novel contribution** | First to identify self-efficacy as mechanism; shows awareness of delegation doesn't change effect |
| **Gap not addressed** | What happens when organisational incentives conflict with delegation logic? |

## Literature Positioning

This paper sits: **High technical depth, low organisational/policy realism**

Gap in literature: **High technical + high org/policy realism intersection**

---

# 7. Synthesis & Research Insight

## Pattern Recognition

> [!TIP]
> **🔵 Pattern Confirmation**
> 
> *This paper CONFIRMS the pattern that: Human-AI collaboration research treats organisations as neutral transmission mechanisms — demonstrating effects in lab settings while acknowledging (but not addressing) that "human behavior might deviate when teaming up with an AI model" in real organisational contexts.*

## Contribution to Thesis

| Dimension | Assessment |
|-----------|------------|
| **Supports argument** | Demonstrates that even well-designed technical systems face "unexamined" organisational assumptions |
| **Challenges argument** | Shows positive effects possible when org context is controlled away — raises question of whether org friction is insurmountable |
| **Provides evidence for** | Gap between lab-validated technical solutions and organisational implementation |

## Boundary Conditions

**Claims hold when:**

- Tasks are independent and parallelisable
- Workers have no stake in task selection
- No inter-worker dynamics or status hierarchies
- Short time horizons (no deskilling)
- No real consequences for errors

**Claims break if:**

- Middle managers resist AI encroachment
- Workers game confidence signals
- Expert domains where identity tied to task range
- Long-term deskilling concerns emerge
- Regulatory requirements for human oversight

*Acknowledged by authors: Partially — acknowledge non-expert task, short duration, suggest future work on expert domains*

---

# 8. Metadata & Linkages

| Field | Value |
|-------|-------|
| **Tags** | human-AI-collaboration, AI-delegation, algorithmic-management, self-efficacy, task-performance, task-satisfaction, experimental-study, IUI, org-assumptions-optimistic |
| **Collections** | Core-Human-Machine, Algorithmic-Management, Org-Theory-Gap |
| **Related Items** | bondi2022role, fugener2022cognitive, lee2015working, mohlmann2019uber |

## Research Questions Relevance

| Research Question | Relevance | Score |
|-------------------|-----------|-------|
| RQ1: How do orgs implement AI governance? | Medium | 3/5 |
| RQ2: Why do AI implementations face org friction? | High | 5/5 |
| RQ3: What institutional factors mediate AI adoption? | Low | 2/5 |

## Follow-ups

**Questions to revisit:**

- What happens to self-efficacy effects in high-stakes expert domains?
- How do middle managers respond when AI takes over task allocation?
- Do long-term deskilling effects erode initial performance gains?

**Connections to other papers:**

- Contrast with Möhlmann & Henfridsson (2019) on Uber driver negative perceptions of algorithmic management
- Compare with Lee et al. (2015) on worker reactions to algorithmic vs. human managers

**Potential quotes for thesis:**

- Page 2: "Human behavior might deviate when teaming up with an AI model" — acknowledges gap but doesn't address
- Page 9: "Managers could consider applying AI delegation to yield higher levels of performance" — optimistic framing
- Page 9: "Modified nature of the task through AI delegation was responsible for the increases" — key finding

---

*— End of Annotation —*
