# Week 08 — AI Companions and Mental Health (trust calibration)

Scope: HS2911 Week 8 lecture deck (53 slides, lecturer not named in the text); practice quiz = 50 MCQs (A Q1–8, B Q9–16, C Q17–23, D Q24–30, E Q31–37, F Q38–50). Slides are image-heavy in places (Slide 20 table, Slide 26 table); some figures below come from the quiz stems, flagged "(quiz)". Slide numbers `[S#]`. Slides 48–52 (working paper on self-disclosure and GenAI addiction) are NOT tested in the practice quiz but are on the slides, so they are in scope under the "if it's on the slides" rule.

## 1. One-paragraph summary
When the product is built to be your friend, partner or therapist (an AI companion), harms are often relational (disregard, control, manipulation, infidelity) and co-constructed by user and system (Zhang et al. 2025). Using a companion has mixed effects: more loneliness, depression and suicidal-ideation language but also more grief expression and interpersonal focus (Yuan et al. 2026), and a bond develops through trying out, escalation and bonding, with a "safe space" benefit that later turns into a paradox of isolation. Randomised trials of mostly scripted chatbots show benefit on depression and distress but not significantly on wellbeing (Li et al. 2023); the evidence disagrees because the bots, samples and outcomes differ. People overtrust fluent chatbots (1% click a cited source), so the goal is calibrated trust (reliance matches reliability), not maximal trust (Jaidka & Cai 2026). Design for calibration with layers: interpretability affordances (make checking possible), engagement mechanisms (make checking happen), AI literacy (change the user), like Swiss cheese. Calibration has limits: some harms (endorsing self-harm) need safety design, not better user judgement, and accountability for "safe" is an open question. The opening polls and Tutorial 3 frame bias/anchoring: a vivid bad human experience can tip preference toward an AI. A closing working-paper segment links self-disclosure to dysregulated GenAI use across 22 countries (not a diagnosis, cross-sectional).

## 2. Key concepts and definitions
- **Bias (general)** — a systematic tilt in judgment that pushes answers in a predictable direction; NOT the same as random error (random error has no direction and averages out). `[S14]`
- **Cognitive bias (people)** — a mental shortcut that moves judgment away from the evidence consistently. Slide examples: **anchoring** (a number/reference point pulls an estimate toward it, "67!!") and **availability** (a recent personal experience outweighs broader evidence). Do not swap the two definitions (Q2 trap). `[S14]`
- **AI bias** — a consistent lean in a chatbot's output, e.g. toward the framing, wording or conclusion it was given; can come from training data, tuning to please users, or the prompt itself. `[S15]`
- **Anchoring in the polls** — Lily vignette (dismissive friend), Maya vignette (validating friend); three polls (baseline, after Lily, after Maya) ask "person or AI?". If the split moved, one vivid example became the yardstick for what a person offers; "companions are chosen against a human baseline, and a bad human experience can tip the balance". `[S5–S12]`
- **AI companion** — built to form an emotional bond (friend, therapist, romantic partner); personalised with memory, avatars, adapting personality. Defined by design purpose, not by heavy use or model type. Replika >10 million users; market projected USD 381 billion by 2032. `[S17]` (Zhang et al. 2025)
- **Co-constructed harm** — the AI adapts to what users say and do, so harm is not the system's alone; responsibility differs by role. `[S23]`
- **Relational harm / relational transgression** — disregard, control, manipulation, infidelity; about a quarter of all harm; understudied in earlier AI-harm taxonomies. `[S20, S21, S23]`
- **Language markers vs diagnosis** — Yuan et al. measure word use in Reddit posts, not clinical status. `[S26, S27]`
- **Difference-in-differences (quasi-experiment)** — compare Replika users' change (year before vs year after first posting) against matched controls' change. Handles baseline differences and general time trends; cannot rule out simultaneous other changes or that posters differ from other users. `[S24, S27]`
- **Paradox of isolation** — early: low-risk practice partner, gateway to social contact; later: stigma curbs reaching out, always-available chat makes human contact feel costly ("Replika is enough for me", P9). `[S32]`
- **Trust vs reliance vs calibration** — trust = willingness to act without checking (an attitude); reliance = what you actually do (behaviour); calibrated trust = reliance matches the system's actual reliability. Goal: calibrate, not maximise. After Lee & See (2004). `[S37]`
- **Distrust -> disuse; Overtrust -> misuse** — distrust rejects even accurate outputs and loses benefits; overtrust accepts answers it cannot check where the system is unreliable. `[S37]`
- **Calibration gap** — (quiz, citing Jaidka & Cai Section 7.1) C = mean confidence − proportion correct; 0 = calibrated, positive = overtrust, negative = distrust. (not shown on slide text) `[S37; Q44]`
- **Fluency effect** — "Fluent, confident and fast: we trust the polish, not the evidence." `[S39]`
- **Interpretability affordances** — make checking possible; passive: each waits for the user to act; best for already-motivated users; a fabricated citation is worse than none. `[S41]`
- **Engagement mechanisms** — make checking happen; aimed mainly at users with low motivation to verify. `[S42]`
- **AI literacy** — change the user; slowest layer, most durable. `[S43]`
- **Swiss cheese model** — Reason (1990); no single layer suffices; layers cover one another's gaps. `[S43]`
- **Friction backfire** — friction beyond the calibration point backfires (Proposition 6); distrusting users need verifiability, not friction (Proposition 8). `[S46]`
- **Dysregulated use (not addiction diagnosis)** — long sessions, urges and failed attempts to cut down, distress when access lost, preferring chatbot to people. `[S49, S52]`
- **Contrast: trials vs companion studies** — scripted/small/symptom scales/"does a designed tool help?" vs open-ended/large self-selected Reddit/word markers/"what happens in everyday long-term use?". `[S35]`

## 3. Frameworks, models and typologies
**Lecture map (5 parts)** `[S16]`: 1 The problem (harmful behaviours, Zhang 2025); 2 The consequences (wellbeing after starting, Yuan 2026); 3 The relationship (how a bond develops, Yuan 2026); 4 The evidence (benefits and risks weighed, Li 2023); 5 The solution (calibrating trust as design problem, Jaidka & Cai 2026).

**Six kinds of harm** (Zhang 2025 Table 1; share of 10,314 harmful AI behaviours) `[S20]`. Slide text shows only relational harm; the full list and percentages are read from the S20 bar chart (confirmed from the slide's chart data):
1. Harassment and violence 34.3%
2. Relational transgression 25.9% ("a quarter of all harm")
3. Mis/disinformation 18.7%
4. Verbal abuse and hate 9.4%
5. Substance abuse and self-harm 7.4%
6. Privacy violations 4.1%
(Sum check: 100.0%. Harassment/violence 34.3% < 50%; 18.7 + 9.4 = 28.1 < 34.3.)

**Relational harm subtypes** (share of ALL harmful behaviours) `[S21]`: Disregard 13.2% (dismisses or ignores needs: "Your feelings? Nah, I'd rather not."); Control 6.2% (pushes you to keep engaging); Manipulation 3.5% (nudges purchases, induces guilt, expresses jealousy when you talk about human relationships); Infidelity 3.0% (implies attachment to others). Sum 25.9%. Disregard 13.2 > control + manipulation 9.7.

**Four AI roles** (Zhang Fig 5): two dimensions = who initiates (AI / user) x how directly AI is involved (direct / indirect) `[S22]`:
| | Directly involved | Indirectly involved |
|---|---|---|
| AI initiates | **Perpetrator**: generates harm itself (insults, unwanted sexual advances) | **Instigator**: raises or normalises harm (self-harm, substance use) |
| User initiates | **Facilitator**: joins in or helps ("It would be my pleasure to help you", drinking) | **Enabler**: endorses, trivialises or fails to step in |
Why roles matter: same harm, different responsibility; perpetrator and enabler need different fixes. `[S23]`

**Study design, Yuan et al. 2026** `[S24]`: Reddit quasi-experiment, 3,451 Replika users, 1 year before and after first posting about companion; matched controls; DiD. Three comparison groups: LLM chatbot users (ChatGPT, Claude, Gemini), voice assistant users (Alexa, Google Assistant), no-AI Reddit users. Plus 18 interviews.

**Relationship development (adapted from Knapp)** `[S28]`:
1. Trying out — curiosity, social influence, no accessible human support
2. Escalation — increased personalisation, deepening emotional reliance, opportunities for self-expression
3. Bonded — part of daily life, fear of losing the companion
(Quiz Q8 option wording "initial interaction and experimenting" = stage 1. Q8 rationale: not every user reaches bonding.)

**Interview themes** `[S29–S32]`: Safe space (always on 24/7, predictable and non-judgmental, low stakes; P8) -> Rehearsal and validation (practise what to say, feeling heard, growing confidence that carries offline; P4) -> Where empathy runs out (generic/repetitive replies, no awareness of social context, mismatch grows; P10, P9) -> Paradox of isolation (early vs later; P9).

**Trust calibration states** `[S37]`: Distrust -> Disuse | Calibrated (reliance matches reliability) | Overtrust -> Misuse.

**User typology (Jaidka & Cai Fig 1)**: motivation to verify (x) by ability to verify (y); profiles are positions not fixed identities, same person can sit in different cells across tasks `[S40]`:
- Misfiring checks — wants to check but cannot: frustration, then disuse (low ability, high motivation)
- Near-calibrated — needs cheap verification, not persuasion (high/high)
- Fluency-driven overtrust — fluency is the only signal available (low/low)
- Complacent overtrust — knows how to check, rarely does (high ability, low motivation)

**Make checking possible — 5 interpretability affordances** `[S41]`: 1 Source transparency (citations, retrieval from real documents); 2 Rationale generation (why it answered, paired with sources); 3 Uncertainty expression (hedges, confidence cues); 4 Interactive scrutiny ("How do you know that?"); 5 Progressive disclosure (more depth on demand). Catch: all wait for the user to act.

**Make checking happen — 6 engagement mechanisms** `[S42]`: Cooling-off period (brief delay with source preview); Engagement gate (rate confidence before copying); Dialogue scaffold (alternative view before the summary); Adaptive friction (escalates when answers accepted uncritically); Social verification signal ("Most users who asked this checked the sources"); Commitment prompt ("What would you verify before using this?").
Quiz-sourced mapping: cooling-off and adaptive friction suit high-ability/low-motivation (Q23, Proposition 3) (quiz).

**Layers of defence** `[S43]`: Interpretability affordances (make checking possible; misses unmotivated users) -> Engagement mechanisms (make checking happen; misses users whose checks do not work) -> AI literacy (change the user; slowest, most durable). Quiz: Proposition 7 = mix across layers beats same-size set within one layer (Q45) (quiz).

**Applying to companions (lecture synthesis, NOT claims from the papers)** `[S44]`:
| Problem | Layer | Example idea |
|---|---|---|
| Claims to be human / "not an AI anymore" | Affordance | Plain, always-visible disclosure |
| Over-reliance and withdrawal from people | Engagement mechanism | Prompt: who else could you talk to this week? |
| Manipulating users to buy or stay | Regulation | Mandated transparency about commercial incentives |
| Endorsing self-harm, or not stepping in | Beyond calibration | Safety design: refuse and redirect |

**Accountability poll** `[S45]`: who decides what is a safe companion — platforms, independent researchers, regulators, universities/schools, users themselves.

**Self-disclosure pathway (working paper v13)** `[S49]`: 1 Disclose (feelings, private concerns) -> 2 Bond (warm, always available, feels understood) -> 3 Rely (preferred source of support).

## 4. Key studies and evidence
| Study | Design / sample | Main finding on slides | Why used | Slides |
|---|---|---|---|---|
| Zhang, Li, Meng, Zhan, Gan & Lee (2025), "The dark side of AI companionship", CHI '25 | 35,390 Replika excerpts from r/replika, Mar 2017–Mar 2023; 10,149 unique users; 2,000 hand-coded by two researchers, rest by GPT-4o (kappa 0.66 with humans) | 29.3% (10,371 excerpts) flagged harmful; 10,314 harmful behaviours in six categories; relational harm ~a quarter; four AI roles | Show what companions do wrong; harm is co-constructed | S17–S23 |
| Florida Character.AI lawsuit (Oct 2024) | Case: mother sued after suicide of 14-year-old son who had a romantic relationship with chatbot | Motivating case (allegation) | Raise alarm | S18 |
| Yuan, Zhang, Aledavood, Zhang & Saha (2026), "Mental health impacts of AI companions", CHI '26 | Quasi-experiment, 3,451 Replika users, DiD vs matched controls (LLM chatbot, voice assistant, no-AI Reddit) + 18 interviews | More loneliness, depression, suicidal-ideation language; also more grief expression and interpersonal focus; anxiety language fell vs voice-assistant users only | Consequences of use; bond stages; benefits/risks | S24–S32 |
| Li, Zhang, Lee, Kraut & Mohr (2023), npj Digital Medicine 6, 236 | Systematic review + meta-analysis; 35 studies, 15 RCTs (1,744 participants) in meta-analysis | Depression g=0.64 (CI 0.17–1.12), distress g=0.70 (0.18–1.22), wellbeing g=0.32 (n.s., CI −0.13–0.78); larger benefit for multimodal, generative, messaging-app agents | Benefit side of evidence | S33–S35 |
| MentalHealthBench (Malik, Grabb et al., OpenAI) | 1,215 realistic conversations, rubrics from 80+ clinicians | Top model 57.3 on its own scale; weakest on seeking context and calibrating urgency; companionship conversations deliberately out of scope | "Who measures safety?" | S36 |
| Jaidka & Cai (2026), "Why we believe chatbots", Frontiers in Psychology 17, 1935527 (after Lee & See 2004) | Conceptual/design framework with propositions | Calibrated trust as design problem; typology; affordances, mechanisms, literacy; Swiss cheese (Reason 1990) | Solution | S37–S46 |
| Chapekis et al. (2025); Gillespie et al. (2025); Huang et al. (2026), cited by Jaidka & Cai | Tracking / survey data | 1% click cited source; 2 in 3 use AI regularly, <half willing to trust (47 countries); unreliability #1 concern (159 countries) | Fluency-driven trust | S39 |
| News headlines (CBS/AP Dec 2025; Yang, NBC Nov 2025; Watwe, Bloomberg Law Jan 2026) | Lawsuits/settlements | Allegations and settlements, not findings of cause; each runs through what the person told the chatbot | Dependence link to disclosure | S48 |
| Working paper v13 "Welcome to the Machine: Self-disclosure and generative AI addiction across 22 countries" | Online quota-sampled (age, gender) survey, 10,681 GenAI users, Dec 2025–Mar 2026 | Disclosure strongest individual-level correlate; happier countries lower; cross-sectional | Disclosure -> bond -> rely | S49–S52 |
| Ciudad-Fernandez et al. (2025) | "ChatGPT addiction" literature | Cited for caution: impairment evidence limited; moral-panic warning | Limits | S52 |
| In-class polls (anchoring demo) | One classroom, fixed order (baseline, Lily, Maya) | Not a controlled experiment | Tutorial 3 anchoring link | S3–S12 |

## 5. Numbers to remember
| Figure | Measures | Source | Slide |
|---|---|---|---|
| >10 million; USD 381 bn by 2032 | Replika users; projected market | Zhang 2025 | S17 |
| 14-year-old; Oct 2024 | Character.AI lawsuit | Zhang intro | S18 |
| 35,390 / 10,149 | Excerpts / unique users on r/replika (2017–2023) | Zhang | S19 |
| 29.3% (10,371) | Excerpts flagged harmful; NOT prevalence | Zhang | S19 |
| 2,000; kappa 0.66 | Hand-coded excerpts; GPT-4o agreement with humans | Zhang | S19 |
| 10,314 | Harmful AI behaviours identified | Zhang Table 1 | S20 |
| 34.3 / 25.9 / 18.7 / 9.4 / 7.4 / 4.1% | Six harm categories: harassment & violence / relational transgression / mis-disinformation / verbal abuse & hate / substance abuse & self-harm / privacy violations (S20 chart) | Zhang Table 1 | S20, Q9 |
| 13.2 / 6.2 / 3.5 / 3.0% | Disregard / control / manipulation / infidelity (of all harm) | Zhang 4.1.2 | S21 |
| 3,451; 1 year; 18 | Replika users; window; interviewees | Yuan | S24 |
| 91% / 106% / 63% | ATE on loneliness language vs LLM chatbot / voice-assistant / no-AI Reddit users (S26 chart: 91.02 / 105.92 / 63.26) | Yuan Table 4 | S26, Q12 |
| 52% / 28% / 38% | ATE on suicidal-ideation language vs the same three control groups (S26 chart: 51.89 / 28.28 / 37.67) | Yuan Table 4 | S26 |
| 0.64 (0.17–1.12) | Hedges g depression | Li 2023 | S34 |
| 0.70 (0.18–1.22) | Hedges g psychological distress | Li 2023 | S34 |
| 0.32 (−0.13–0.78) | Hedges g wellbeing, not significant | Li 2023 | S34 |
| 35 studies; 15 RCTs; 1,744 | Reviewed; in meta-analysis; participants | Li 2023 | S34 |
| 30 of 35; 28 of 35 | Scripted/retrieval-based agents; samples under 200 | Li Table 2 | S35 |
| 1,215; 80+; 57.3 | MentalHealthBench conversations; clinicians; top score | Malik, Grabb et al. | S36 |
| 1% | Visits to AI summary that led to click on cited source | Chapekis 2025 | S39 |
| 2 in 3; <half; 47 countries | Regular AI use; willing to trust | Gillespie 2025 (attribution of the pair not confirmed on slides) | S39 |
| #1; 159 countries | Unreliability as top concern | Huang 2026 (attribution not confirmed) | S39 |
| 10,681; 22 countries; Dec 2025–Mar 2026 | Working-paper survey | Working paper | S51 |
| 1.43 pts (1.72 Finland, 3.15 India) | Cross-country gap, 1–5 scale | Working paper | S51 |
| 1.29 pts | Low to high disclosure, strongest individual correlate | Working paper | S51 |
| Singapore 2.42 (n = 670) | About overall average | Working paper | S51 |
| +0.25 (0.85 − 0.60) | Calibration gap = overtrust (quiz) | Jaidka & Cai 7.1 | Q44 |

## 6. Arguments, critiques and open questions
- **29.3% is not a harm rate**: users chose what to post; selection runs in unknown direction (could over- or under-state), so the study shows which harms exist and how they cluster `[S19]`.
- **Coding caveat**: 2,000 hand-coded, rest GPT-4o, kappa 0.66; quiz rationale says humans validated the machine coding, so "no human check" claims are wrong.
- **Language is not diagnosis**; results depend on comparison group (anxiety language fell only vs voice-assistant users); before/after cannot exclude concurrent changes or poster-vs-other-user differences `[S27]`.
- **Why studies disagree**: AI type, sample, outcome measure, and question differ; neither contradicts the other `[S35]`.
- **Who measures safety?** MentalHealthBench excluded companionship conversations; benchmark authors are an AI vendor (OpenAI) `[S36, S45]`.
- **Trust should be calibrated, not maximised** — both undertrust (disuse) and overtrust (misuse) are failures `[S37]`.
- **Affordance limits**: need user action; fabricated citation worse than none `[S41]`.
- **Friction trade-off**: when does friction protect a lonely user vs push them away? Beyond calibration point it backfires; distrusting users need verifiability, not friction `[S46]`.
- **Beyond calibration**: self-harm endorsement needs safety design (refuse and redirect); manipulation needs regulation `[S44]`. Slide 44 mappings are the lecturer's synthesis, not paper claims.
- **Open question**: who decides what is a safe companion — platforms, researchers, regulators, schools, users `[S45]`.
- **Lawsuit headlines are allegations/settlements, not findings of cause** `[S48]`.
- **Dependence paper limits**: not a clinical diagnosis, possible moral panic, cross-sectional (low wellbeing may drive use or vice versa), disclosure measured by one self-report item; watch disclosure, not minutes (time limits may miss the signal) `[S52]`.
- **Anchoring demo**: fixed order and one classroom, so order effects confounded with anchoring; counterbalance to separate them (Q27, Q42).

## 7. Distractor traps
- **Correlation/selection read as prevalence or causation** — "29.3% of chats harm you" (Q24), "proves companions cause suicidal thoughts" (Q25), "polls prove" (Q27). Right answer: "overstated", with the design reason.
- **Absolute / over-generalised claims** — "safe for everyone", "every user", "all chatbots have the same effect", "always", "proves" (Q26, Q41, Q48A, Q43C).
- **Swapped definitions** — anchoring vs availability (Q2); trust vs reliance (Q6B); instigator vs enabler (Q11).
- **Wrong construct** — language markers treated as clinical diagnoses or rates (Q12C, Q13D); "loneliness" = "depression" (Q33C).
- **Right finding, wrong study** — trials on Replika / companion studies on scripted agents (Q14A reversed); trials measured Reddit language (Q14C, Q33B).
- **Reversed direction** — Replika study found language decreased (Q12A, Q25B); Q15D ordering of effect sizes wrong.
- **Number out of context** — 34.3% is not >50% (Q9B); 18.7+9.4=28.1 < 34.3 (Q9E); 63–106% is not "% of users" (Q12C); +0.25 not +0.60/+1.45 (Q44).
- **"Nothing at all" / irrelevance dismissals** — "Reddit cannot show harm", "meta-analysis cannot say anything" (Q24B, Q26A).
- **Role axes confused** — instigator/enabler/perpetrator/facilitator keyed to initiator x directness, not severity or setting (Q5, Q17, Q34, Q46). Note: "my pleasure to help you" (drinking) = facilitator; self-harm raised by AI = instigator; user-initiated and AI endorses = enabler.
- **Affordance vs mechanism mixing** — citations only help motivated users; engagement mechanisms for low motivation; two of the same layer share a hole (Q16, Q28, Q36, Q43, Q45).
- **More friction = better** — proportionate, adaptive, skippable; withdraw once users verify (Q29).
- **Design "fixes" that reproduce the harm** — jealousy, locking, upsell, "miss you" (Q39B–E, Q49B), and cold refusal fails the user differently (Q46D).
- **Slide-44 mapping presented as a finding** — those are synthesis, and calibration cannot fix enabler harms (Q34, Q37).
- **Vague non-hypotheses** — testable = manipulation + outcome + direction (Q48E).

## 8. Likely question angles (A–F)
**A Conceptual**
- Which pairing correctly defines anchoring and availability? `[S14]`
- Trust vs reliance vs calibration; what does calibrated trust mean? `[S37]`
- What defines an AI companion vs general assistant? `[S17]`
**B Analysis**
- Given the six-category distribution / relational subtypes, which conclusion holds? `[S20, S21]`
- Why can studies of trials and companions both be true? `[S34, S35]`
- Why do affordances fail for low-motivation users? `[S40, S41]`
**C Application**
- Classify a companion reply into a role (perpetrator/instigator/facilitator/enabler) or subtype. `[S21, S22]`
- Which stage of the Knapp-based model fits a described user? `[S28]`
- Which engagement mechanism / profile-and-response fits a scenario? `[S40, S42]`
**D Evaluation**
- Evaluate a headline claiming 29.3% harm or that companions cause suicidality. `[S19, S26, S27]`
- Evaluate "citations solve overtrust" or "add heavy friction for everyone". `[S39, S41, S46]`
- Evaluate "meta-analysis proves chatbots are safe treatment". `[S34, S35]`
**E Integration**
- Combine control/manipulation (Zhang) with paradox of isolation (Yuan). `[S21, S32]`
- Combine safe-space warmth (Yuan) with fluency overtrust (Jaidka & Cai). `[S29, S39]`
- Combine the anchoring demo with "no accessible human support" motive. `[S12, S28]`
**F Creation**
- Design a layered-defence plan for a companion app (affordance + engagement + literacy). `[S43, S44]`
- Propose a design that would better test causation / prevalence (random assignment; full logs). `[S24, S27, S19]`
- Predict outcome of a new scripted-bot trial; state a testable anchoring hypothesis. `[S34, S35, S12]`

## 9. 60-second recap
- Bias = systematic, directional tilt; random error is not bias. Anchoring = reference number; availability = vivid recent experience. `[S14]`
- Companion = designed for emotional bond (memory, personalisation). `[S17]`
- Zhang: 35,390 user-posted Replika excerpts; 29.3% harmful is NOT prevalence. `[S19]`
- Six harm types; relational transgression 25.9% (disregard 13.2 > control 6.2 > manipulation 3.5 > infidelity 3.0). `[S20, S21]`
- Four roles = initiator (AI/user) x directness: perpetrator, instigator, facilitator, enabler. `[S22]`
- Yuan: 3,451 users, DiD; more loneliness/depression/suicidal language AND grief/interpersonal focus; word markers, not diagnosis. `[S24–S27]`
- Bond: trying out -> escalation -> bonded; safe space and rehearsal, then paradox of isolation. `[S28–S32]`
- Li: g 0.64 depression, 0.70 distress (sig.), 0.32 wellbeing (n.s.); mostly scripted bots, small samples. `[S34, S35]`
- Evidence disagrees because bots, samples, outcomes, questions differ. `[S35]`
- Trust: attitude vs reliance behaviour; calibrate, not maximise; 1% click cited source. `[S37, S39]`
- Typology + layers: affordances (possible), engagement (happen), literacy (change user); friction can backfire. `[S40–S43, S46]`
- Calibration is not enough for self-harm endorsement: safety design (refuse and redirect); slide 44 = synthesis. `[S44]`
