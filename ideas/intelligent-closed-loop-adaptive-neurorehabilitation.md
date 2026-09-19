# RESEARCH KNOWLEDGE BASE

## Intelligent Closed-Loop Adaptive Neurorehabilitation

### AI + Virtual Reality + Gamification + Behavioural Analytics

**Knowledge-base status:** Research concept / interdisciplinary pilot research
**Evidence window:** Primarily 2024–September 2026
**Primary objective:** Develop a publishable interdisciplinary research study and potential grant proposal; not currently intended as a PhD topic.

---

## 1. Core Research Concept

The proposed research investigates an AI-driven neurorehabilitation framework in which Virtual Reality (VR), gamification, multimodal movement sensing and behavioural analytics are integrated into a continuous closed-loop system.

The central proposition is:

> Rehabilitation should adapt not only to what a patient can physically perform, but also to how the patient behaves, engages and responds during rehabilitation.

The proposed system continuously estimates a patient's functional and behavioural state and uses this estimate to personalise VR rehabilitation tasks, difficulty, feedback and gamification.

Conceptual loop:

PATIENT
→ sensing / interaction
→ movement analysis
→ behavioural analysis
→ patient-state estimation
→ personalised intervention
→ VR/gamified rehabilitation
→ new patient response
→ state re-estimation
→ adaptation

---

## 2. Research Domain

The project sits at the intersection of:

* Artificial Intelligence
* Machine Learning
* Computer Vision
* Virtual Reality
* Gamification
* Behavioural Analytics
* Human-Computer Interaction
* Neurorehabilitation
* Physiotherapy
* Digital Health
* Explainable AI
* Adaptive Systems
* Human-in-the-loop AI

The initial clinical use case should preferably be post-stroke upper-limb rehabilitation because it has substantial literature, measurable motor outcomes, established clinical scales and a large body of VR/gamification research.

Other populations such as Parkinson's disease, multiple sclerosis and spinal cord injury may be considered later.

---

## 3. Established Knowledge

The following are NOT sufficient novelty claims on their own:

1. VR can be used for rehabilitation.
2. Gamification can increase motivation or engagement.
3. AI/ML can analyse rehabilitation movements.
4. AI can provide automated feedback.
5. VR difficulty can be adjusted dynamically.
6. Machine learning can personalise rehabilitation.
7. Closed-loop adaptive VR rehabilitation exists.

The research landscape by 2026 already contains studies and reviews covering these areas.

Therefore, the project should not position itself merely as another AI-VR rehabilitation system.

---

## 4. Current Research Landscape

Recent literature indicates:

* VR has demonstrated potential as an adjunct to conventional stroke rehabilitation.
* Gamified rehabilitation has been extensively studied, including VR, robotics and other technologies.
* AI + gamification is emerging but remains fragmented.
* ML-based adaptive VR rehabilitation is becoming a defined research area.
* Reinforcement learning and deep learning are being used for adaptive rehabilitation.
* Real-time closed-loop adaptation has already been demonstrated in multiple systems.
* However, many studies remain small, heterogeneous and short-term.
* Clinical validation, standardised outcomes, explainability, safety, equity and real-world deployment remain important challenges.
* Automatic adaptation remains relatively immature across gamified VR systems.
* Personalisation of gamification according to patient characteristics, cognitive status, recovery stage and motivational state remains insufficiently understood.

---

## 5. Primary Research Gap

The strongest proposed gap is not simply adaptive rehabilitation.

The proposed gap is:

> Existing systems tend to model rehabilitation performance primarily through physical/motor measures, while comparatively less mature work integrates functional movement state with behavioural interaction state to drive personalised gamification and adaptive rehabilitation.

The proposed research therefore treats the patient as a multimodal state rather than a movement-performance score.

---

## 6. Proposed Patient-State Model

Represent patient state as:

P(t) = {F(t), B(t), E(t), C(t)}

Where:

F(t) = functional/motor state
B(t) = behavioural interaction state
E(t) = engagement state
C(t) = contextual/session state

This notation is conceptual and should not be presented as a validated clinical model until empirically evaluated.

---

## 7. Functional State Variables

Candidate variables include:

* movement accuracy
* trajectory deviation
* movement smoothness
* velocity
* acceleration
* reaction time
* range of motion
* task completion
* repetition count
* coordination
* movement asymmetry
* error rate
* temporal consistency
* task-specific motor performance

Potential sensing modalities:

* RGB camera
* depth camera
* markerless pose estimation
* VR controllers
* IMUs
* wearable sensors
* EMG, if resources permit

The initial MVP should avoid unnecessary hardware complexity.

---

## 8. Behavioural Analytics

Behavioural analytics is a central differentiating component.

Candidate behavioural features:

* task persistence
* hesitation
* retry frequency
* task abandonment
* voluntary repetition
* time-on-task
* interaction frequency
* preferred difficulty
* response to failure
* response to reward
* exploration behaviour
* consistency across sessions
* adherence
* progression choices
* interaction latency
* challenge acceptance/rejection

These should be treated initially as candidate behavioural indicators rather than automatically valid clinical biomarkers.

Validation against established behavioural/clinical measures is required.

---

## 9. Engagement Model

Engagement should not be treated as a single observable variable.

Potential dimensions:

### Behavioural engagement

What the patient actually does.

### Cognitive engagement

Attention, task persistence, decision-making and challenge response.

### Emotional/affective engagement

Enjoyment, frustration, confidence and perceived difficulty.

### Longitudinal engagement

Whether participation is sustained across sessions.

The system should preferably estimate engagement from multiple observable signals rather than relying only on self-report.

---

## 10. Personalised Gamification

A major research opportunity is moving from:

"gamification for rehabilitation"

to:

"patient-specific gamification."

Potential adaptive parameters:

* reward frequency
* reward type
* challenge intensity
* visual complexity
* task duration
* competition/cooperation elements
* progression speed
* feedback frequency
* positive reinforcement
* achievement structure
* goal setting
* game theme
* difficulty progression

The system should not assume that one gamification strategy suits every patient.

The research question is whether behavioural and functional state can be used to select or modify gamification mechanisms.

---

## 11. Adaptive Rehabilitation

The system may adapt:

* task difficulty
* target size
* target distance
* movement speed
* required precision
* repetition count
* cognitive load
* visual complexity
* assistance level
* feedback intensity
* reward structure

Adaptation should be constrained by therapist-defined safety and clinical boundaries.

AI should preferably generate recommendations within predefined safe ranges rather than operate without constraints.

---

## 12. Closed-Loop Architecture

Recommended architecture:

INPUT
→ sensing
→ feature extraction
→ functional-state estimation
→ behavioural-state estimation
→ multimodal patient-state fusion
→ personalisation engine
→ intervention adaptation
→ VR/gamified exercise
→ new patient response
→ continuous feedback

The system should maintain a distinction between:

1. Observation
2. State estimation
3. Prediction
4. Recommendation
5. Intervention
6. Outcome measurement

This distinction is important for scientific validity and explainability.

---

## 13. Explainable Adaptation

Every significant adaptation should ideally have an interpretable rationale.

Example:

"Difficulty increased because task accuracy remained above 85%, completion time decreased, and performance was stable over the previous three sessions."

Example:

"Difficulty was maintained because accuracy improved but movement variability and hesitation increased."

The research should investigate whether interpretable adaptation decisions improve clinician trust and system usability.

---

## 14. Clinician-in-the-Loop Principle

The system should not be positioned as an autonomous clinical decision-maker.

Recommended architecture:

AI assessment
→ AI recommendation
→ therapist review
→ approved/modified intervention
→ patient

The therapist remains responsible for clinical decisions.

This architecture improves clinical acceptability and reduces the risk of overclaiming AI capability.

---

## 15. Candidate AI Methods

Potential methods should be selected according to the research question rather than complexity.

### Functional-state estimation

* Random Forest
* XGBoost
* SVM
* temporal neural networks
* LSTM/GRU
* transformer-based temporal models

### Behaviour classification

* clustering
* hidden Markov models
* supervised classification
* sequence models

### Patient profiling

* clustering
* latent-state models
* trajectory modelling

### Adaptation

* rule-based baseline
* contextual bandits
* reinforcement learning
* constrained reinforcement learning

A rule-based system should preferably be retained as a baseline so that AI adaptation can be evaluated objectively.

Do not use reinforcement learning merely because it appears sophisticated. It should be justified by the sequential decision-making problem.

---

## 16. Recommended Experimental Logic

### Baseline condition

Fixed or therapist-defined rehabilitation progression.

### Experimental condition

AI-adaptive rehabilitation.

Compare:

* movement performance
* task completion
* engagement
* adherence
* perceived workload
* usability
* progression rate
* behavioural response

If clinically feasible, include established clinical measures.

---

## 17. Research Questions

### Primary RQ

Can multimodal AI combining functional movement and behavioural interaction data continuously estimate patient state and personalise gamified VR neurorehabilitation?

### Secondary RQs

RQ1. Can movement data reliably estimate task-level rehabilitation performance?

RQ2. Does behavioural interaction data provide information beyond movement performance?

RQ3. Can multimodal models identify meaningful patient states or behavioural profiles?

RQ4. Can adaptive difficulty maintain an appropriate challenge level?

RQ5. Can personalised gamification improve engagement or adherence compared with fixed gamification?

RQ6. Can digital performance indicators correlate with established clinical measures?

RQ7. Can adaptation decisions be made interpretable to therapists?

RQ8. Does adaptive rehabilitation demonstrate measurable advantages over fixed-progression rehabilitation in a controlled pilot?

---

## 18. Hypothesis Structure

H1: Multimodal movement + behavioural features provide better patient-state estimation than movement features alone.

H2: Behaviour-aware adaptation produces different and potentially more appropriate intervention trajectories than fixed-difficulty rehabilitation.

H3: Personalised gamification improves engagement-related outcomes compared with fixed gamification.

H4: Digital performance indicators show measurable associations with established clinical/functional outcomes.

These are research hypotheses, not assumptions that the study has already established.

---

## 19. Most Important Novelty Claim

Do NOT claim:

"First AI-based VR rehabilitation system."

"First adaptive VR rehabilitation system."

"First gamified rehabilitation system."

These claims are unlikely to be defensible.

Preferred novelty framing:

> The study investigates a behaviour-aware multimodal closed-loop architecture in which functional movement state and behavioural interaction state are jointly used to personalise both rehabilitation difficulty and gamification.

The contribution should be demonstrated empirically rather than asserted.

---

## 20. Candidate Contribution Types

### Technical contribution

Multimodal patient-state estimation.

### AI contribution

Behaviour-aware adaptation/personalisation.

### HCI contribution

Adaptive gamification based on user state.

### Rehabilitation contribution

Data-informed personalised intervention.

### Clinical contribution

Correlation between digital interaction measures and clinical outcomes.

### System contribution

Closed-loop therapist-in-the-loop architecture.

---

## 21. MVP Recommendation

Do not initially build:

* BCI
* robotic exoskeleton
* EMG + EEG + IMU simultaneously
* full clinical-grade medical device
* highly complex metaverse environment

Start with:

VR or desktop-based immersive rehabilitation task
+
camera/pose or VR-controller movement tracking
+
behavioural interaction logging
+
AI patient-state model
+
adaptive difficulty
+
basic personalised gamification.

The first objective is to establish the intelligence layer.

---

## 22. Suggested Initial Use Case

Post-stroke upper-limb rehabilitation.

Example task:

Patient reaches toward virtual objects using a tracked hand/controller.

Capture:

* trajectory
* speed
* accuracy
* reaction time
* target success
* hesitation
* retries
* voluntary repetitions
* session duration
* difficulty selection
* progression

AI estimates:

* functional performance
* behavioural engagement
* challenge tolerance

System adapts:

* target distance
* target size
* movement speed
* repetition requirement
* reward frequency
* visual complexity

---

## 23. Candidate Study Phases

### Phase 0 — Literature + framework

Establish taxonomy and research gap.

### Phase 1 — Healthy participants

Validate sensing, feature extraction and behavioural analytics.

### Phase 2 — Patient pilot

Evaluate feasibility and safety with a small clinical sample.

### Phase 3 — Adaptive vs fixed comparison

Evaluate whether adaptive intervention changes engagement/performance.

### Phase 4 — Clinical validation

Evaluate associations with established clinical outcomes.

This phased strategy avoids attempting a full clinical trial before technical feasibility has been demonstrated.

---

## 24. Potential Papers

### Paper 1

Behaviour-aware AI framework for adaptive gamified VR neurorehabilitation.

### Paper 2

Multimodal functional and behavioural state estimation for rehabilitation.

### Paper 3

Adaptive versus fixed gamification/difficulty in VR rehabilitation.

### Paper 4

Association between digital rehabilitation metrics and clinical motor outcomes.

These should be treated as potential publication pathways, not guaranteed outputs.

---

## 25. Potential Grant Proposition

Proposed grant title:

"ICAR: Intelligent Closed-loop Adaptive Rehabilitation Using AI, Virtual Reality and Behavioural Analytics"

Core objective:

Develop and pilot-test an AI-enabled rehabilitation platform that continuously estimates functional and behavioural patient state and adapts VR-based rehabilitation tasks and gamification under therapist supervision.

Expected outputs:

* AI patient-state model
* VR rehabilitation prototype
* behavioural analytics framework
* adaptive personalisation engine
* explainable adaptation mechanism
* pilot dataset
* research publications
* prototype/IP potential
* basis for larger clinical grant

---

## 26. Risk Management

### Risk: AI model overclaims clinical meaning

Mitigation: distinguish digital indicators from validated clinical biomarkers.

### Risk: small sample

Mitigation: position early work as feasibility/pilot research.

### Risk: VR causes cybersickness

Mitigation: monitor usability and simulator-sickness measures and provide non-immersive fallback.

### Risk: adaptation becomes unsafe

Mitigation: therapist-defined safety boundaries.

### Risk: model overfits individuals

Mitigation: subject-independent validation and leave-one-subject-out/cross-validation strategies.

### Risk: behavioural signals are ambiguous

Mitigation: triangulate behavioural features with self-report and therapist assessment.

### Risk: excessive system complexity

Mitigation: MVP-first architecture.

---

## 27. Scientific Positioning

The central scientific transition should be:

FROM:

Technology-assisted rehabilitation

TO:

Data-driven personalised rehabilitation

AND ultimately:

Continuous closed-loop rehabilitation intelligence.

The research should focus on whether multimodal patient-state estimation can improve personalisation rather than simply demonstrating that VR is engaging.

---

## 28. Important Evidence Caveats

The literature currently supports the feasibility and promise of VR, gamification and AI-assisted rehabilitation but remains heterogeneous.

Many studies have small samples, short interventions, heterogeneous protocols and inconsistent outcome measures.

Clinical efficacy should therefore not be assumed from technical feasibility.

The project should explicitly distinguish:

* feasibility
* usability
* engagement
* task-level performance
* digital biomarkers
* clinical outcomes
* long-term recovery

These are different claims and require different evidence.

---

## 29. Working Research Thesis

The project can be built around the following proposition:

> A rehabilitation system that continuously models both what a patient does and how the patient interacts with the rehabilitation environment may enable more responsive and individualised intervention than systems relying solely on fixed progression or motor performance.

The research must experimentally determine whether this proposition holds.

---

## 30. Guidance for Any LLM Assisting With This Research

When assisting with this project:

1. Treat VR rehabilitation as an established field, not the novelty.
2. Treat gamification as established, not the novelty.
3. Treat AI-based movement analysis as an established/emerging field.
4. Treat closed-loop adaptive rehabilitation as an emerging field with substantial 2026 literature.
5. Do not claim novelty merely because AI dynamically adjusts difficulty.
6. Focus on the intersection of functional state, behavioural state, engagement and personalised gamification.
7. Prefer multimodal patient-state estimation over single-score performance models.
8. Maintain therapist-in-the-loop principles.
9. Distinguish candidate digital behavioural indicators from clinically validated biomarkers.
10. Avoid unsupported claims about neuroplasticity or clinical recovery.
11. Use established clinical measures whenever patient studies are conducted.
12. Prioritise explainability and safety constraints.
13. Use fixed/rule-based adaptation as an appropriate baseline.
14. Do not introduce reinforcement learning unless sequential adaptation is genuinely required.
15. Prefer MVP-first development.
16. Separate technical feasibility from clinical efficacy.
17. Treat small samples as appropriate for pilot/feasibility work but insufficient for broad clinical claims.
18. Search the 2024–2026 literature before making novelty claims.
19. Explicitly compare proposed contributions against recent 2026 systematic reviews.
20. The objective is a credible interdisciplinary research contribution, not a technology demonstration alone.

---

## 31. Current Research Direction

The strongest working direction is:

**Behaviour-Aware Intelligent Closed-Loop Neurorehabilitation**

with the following core pipeline:

MOVEMENT
+
BEHAVIOUR
+
ENGAGEMENT
↓
MULTIMODAL PATIENT-STATE ESTIMATION
↓
PERSONALISATION ENGINE
↓
ADAPTIVE VR REHABILITATION
+
ADAPTIVE GAMIFICATION
↓
PATIENT RESPONSE
↓
CONTINUOUS RE-ESTIMATION

The proposed research should test whether this architecture provides measurable advantages over fixed or non-personalised rehabilitation approaches.
