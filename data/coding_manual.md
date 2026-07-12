# Coding Manual

## Multi-Agent LLM Systems for Psychology, Behavior, and Education

**Version:** Rebuttal-stage audit  
**Unit of analysis:** One distinct study or formally published paper.

---

## 1. Purpose

This manual defines the coding rules used to classify studies in the review of
multi-agent LLM systems for psychology, behavior, and education.

The coding framework distinguishes five layers:

1. application domains;
2. architectural mechanisms;
3. process-level system components;
4. evaluation targets;
5. human-validation status.

Application domains, architectural mechanisms, process components, and
evaluation targets are **non-exclusive multi-label dimensions**. A study may
receive more than one label in each dimension.

---

## 2. General Coding Principles

### 2.1 Evidence levels

Each binary or multi-label code should be recorded as:

- **Yes**: the feature is explicitly described or centrally implemented;
- **Partial**: the feature is present indirectly, weakly, or only in a limited
  part of the system;
- **No**: the feature is absent or not reported.

A code should not be assigned solely because a related term appears in the
introduction or literature review.

### 2.2 Publication unit

- Use the formal published version when available.
- Use an arXiv version when it is the version included in the review or when no
  formal version was available at the corpus cut-off date.
- Treat an arXiv paper and its later formal publication as one study unless the
  versions report substantively different systems or experiments.
- Record the retained version and any superseded version in the notes field.

### 2.3 Multi-label logic

A system can combine multiple mechanisms. For example, a system may use:

- a functional pipeline for task decomposition;
- deliberative debate for critique;
- persona-based roles for perspective diversity;
- a game-like attack-defense structure;
- external grounding through retrieval or knowledge graphs.

Such a study should receive all applicable architecture labels.

---

## 3. Application Domains

### 3.1 Psy — Psychological Assessment and Mental Health

Code **Psy = Yes** when the study primarily addresses one or more of:

- psychological assessment or measurement;
- mental-health support;
- cognitive distortion;
- psychological safety;
- clinical or counseling reasoning;
- psychological traits, states, symptoms, or diagnoses.

Do not assign Psy solely because the paper uses the word “behavior” in a
technical or robotic sense.

### 3.2 Beh — Behavioral and Social Simulation

Code **Beh = Yes** when the study primarily models or evaluates:

- social behavior;
- opinion dynamics;
- conformity;
- negotiation;
- cooperation or competition;
- deception;
- collective behavior;
- group identity or social influence.

Do not assign Beh to purely mechanical multi-agent coordination without a
human, social, or psychologically meaningful behavior construct.

### 3.3 Edu — Education, Learning, and Assessment

Code **Edu = Yes** when the study primarily supports:

- teaching or tutoring;
- learning or learner modeling;
- feedback;
- educational assessment or scoring;
- question or item generation;
- curriculum alignment;
- instructional design;
- classroom interaction.

### 3.4 H-A — Human-Agent Collaboration and Cognitive Modeling

Code **H-A = Yes** when the study primarily concerns:

- human-agent collaboration;
- theory of mind;
- trust in or oversight of agents;
- human-AI teaming;
- persona evaluation;
- cognitive modeling relevant to human-agent interaction.

---

## 4. Architectural Mechanisms

The five architecture codes are non-exclusive.

### 4.1 Pipe — Functional Pipeline

Code **Pipe = Yes** when:

- agents are organized as sequential specialist modules;
- outputs are explicitly routed from one role or stage to another;
- the system contains a recognizable planning, retrieval, generation, review,
  or revision chain.

Do not assign Pipe merely because several agents have different roles; there
must be explicit task routing or stage-wise dependency.

### 4.2 Deb — Deliberative or Debate-Based Collaboration

Code **Deb = Yes** when agents:

- exchange critiques or arguments;
- deliberate over alternatives;
- vote, judge, or synthesize competing views;
- engage in structured discussion to revise or select an output.

Assign **Partial** when multiple agents produce separate views but do not
meaningfully interact.

### 4.3 Soc — Persona-Based Social Simulation

Code **Soc = Yes** when agents are initialized with:

- personality traits;
- demographic identities;
- beliefs, values, goals, or social roles;
- persistent persona profiles used to shape interaction.

Do not assign Soc when “role” refers only to a functional software module
without a social, psychological, or identity-based profile.

### 4.4 Game — Game-Theoretic or Self-Play Mechanism

Code **Game = Yes** when the system includes:

- explicit game rules;
- rewards, utilities, or strategic incentives;
- hidden roles;
- self-play;
- attack-defense interaction;
- repeated strategic choices.

### 4.5 GrdW — Grounded Workflow

Code **GrdW = Yes** when external evidence is structurally integrated into the
workflow through:

- retrieval-augmented generation;
- knowledge graphs;
- rubrics or validated scales;
- curricula or standards;
- domain theories;
- datasets or learner profiles used as reasoning evidence.

Do not assign GrdW when external knowledge is mentioned but not integrated
into agent reasoning or validation.

---

## 5. Process-Level Components

### 5.1 Role — Role or Persona Initialization

Code when the system explicitly defines agent roles, personas, expertise, task
responsibilities, or behavioral profiles.

### 5.2 Mem — Memory and Context Management

Code when the system uses interaction history, local or global memory,
short-term or long-term state, learner profiles, or cross-step context.

### 5.3 Grd — External Grounding

Code when agent reasoning draws on external evidence, theory, rubrics,
retrieval, curricula, datasets, or knowledge graphs.

**Distinction:** `Grd` is a component; `GrdW` is an architectural mechanism in
which grounding is structurally integrated into the broader workflow.

### 5.4 Ref — Critique, Reflection, Review, or Adjudication

Code when the system includes a critic, reviewer, evaluator, judge,
reflection loop, revision step, or explicit quality-control mechanism.

### 5.5 Con — Consensus or Synthesis

Code when the system includes consensus formation, synthesis, voting,
arbitration, aggregation, conflict resolution, or a final decision agent.

---

## 6. Evaluation Targets

### 6.1 CV — Construct Validity

Code when the study evaluates whether the system represents or measures the
intended psychological or educational construct.

Evidence may include:

- theory mapping;
- expert annotation;
- convergent validity;
- manipulation checks;
- construct-specific ablations.

### 6.2 Rel — Reliability and Robustness

Code when the study evaluates stability or consistency across:

- repeated runs;
- prompts;
- model versions;
- agent order;
- decoding settings;
- perturbations or ablations.

### 6.3 BR — Behavioral Realism

Code when the study evaluates agent behavior against:

- human behavioral data;
- known psychological or social effects;
- empirical distributions;
- human transcripts;
- experimentally established patterns.

### 6.4 Ped — Pedagogical Impact

Code when the study evaluates:

- learning outcomes;
- feedback quality;
- assessment quality;
- classroom relevance;
- learner experience;
- teacher usability;
- fairness across learner groups.

### 6.5 Safe — Safety and Fairness

Code when the study evaluates:

- harmful advice;
- bias or discrimination;
- manipulation;
- privacy risk;
- overconfident diagnosis;
- safety policy or escalation behavior.

---

## 7. Human Validation

Human validation is a separate status variable.

- **Yes**: human experts, users, annotators, teachers, clinicians, or domain
  professionals directly validate system outputs or evaluation results.
- **Partial**: limited human review, small-scale preference checking, or
  indirect comparison with human-created materials.
- **No**: no human validation is reported.

---

## 8. Coding Workflow

1. Read the full paper or the sections describing system design and evaluation.
2. Record bibliographic metadata and publication status.
3. Assign all applicable application-domain labels.
4. Assign all applicable architectural-mechanism labels.
5. Code process components and evaluation targets.
6. Record human-validation status.
7. Add a short evidence note for every `Yes` or `Partial` code.
8. Mark ambiguous cases for adjudication.
9. Resolve disagreements using this manual and retain a boundary-case note.

---

## 9. Reliability Assessment

Because the application and architecture dimensions are multi-label, agreement
should be calculated separately for each label.

Recommended reporting:

- number and proportion of independently double-coded studies;
- percent agreement for each label;
- binary Cohen's kappa or Krippendorff's alpha for each label;
- macro-average agreement across labels;
- disagreement-resolution procedure.

No reliability statistic should be reported until an independent coding check
has actually been completed.

---

## 10. Boundary-Case Guidance

### Hybrid architectures

A study combining a sequential workflow and agent debate should receive both
`Pipe` and `Deb`.

### Functional role versus persona

- “Retriever,” “generator,” and “reviewer” normally indicate functional roles
  and support `Role`, but not necessarily `Soc`.
- A profile defined by personality, identity, beliefs, or social attributes
  supports `Soc`.

### Grounding component versus grounded workflow

- Assign `Grd` when any agent accesses external evidence.
- Assign `GrdW` when grounding determines the structure of multiple workflow
  stages or is central to generation, critique, or validation.

### Human-generated benchmark only

Using a human-created dataset does not automatically count as human
validation. Code `HV = Yes` only when humans directly validate system outputs
or evaluation results in the reported study.
