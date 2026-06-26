# PHYSIQUEIQ System Architecture

## Vision

PHYSIQUEIQ is an evidence-based AI coaching platform.

The platform is divided into independent systems that communicate with one another through well-defined interfaces.

This separation allows the application to scale without redesigning the platform.

---

# Layer 1 — User Layer

Responsible for:

- Authentication
- Onboarding
- Dashboard
- Progress Tracking
- User Settings

This layer only collects and displays information.

It never makes coaching decisions.

---

# Layer 2 — Decision Engine

Responsible for:

- Reading user information
- Reading knowledge
- Applying evidence rules
- Generating recommendations

This is the coaching intelligence.

---

# Layer 3 — Knowledge Engine

Responsible for storing structured information about:

- Exercises
- Nutrition
- Supplements
- Recovery
- Periodization
- Powerlifting
- Bodybuilding
- ICN Prep
- Fat Loss
- Behaviour Change

This layer contains facts, not decisions.

---

# Layer 4 — Research Vault

Responsible for:

- Scientific papers
- Position stands
- Textbooks
- Competition rulebooks
- Clinical guidelines

Every knowledge entry should be traceable to one or more trusted sources.

---

# Layer 5 — Evidence Engine

Responsible for:

- Ranking evidence quality
- Resolving conflicting evidence
- Calculating confidence scores
- Updating recommendations when evidence changes

---

# Layer 6 — Generator Engine

Responsible for generating:

- Workout Plans
- Nutrition Plans
- Cardio Plans
- Recovery Plans
- Deloads
- Competition Peaks

Generation must always use the Decision Engine and Knowledge Engine.

---

# Layer 7 — Analytics Engine

Responsible for:

- Progress monitoring
- Plateau detection
- Compliance analysis
- Prediction models
- Weekly adjustments

---

# Core Principle

User data, scientific knowledge, and coaching logic must remain independent.

Changing one layer must not require redesigning the others.
