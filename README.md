# supliCheck

A decoupled, full-stack mobile reminder system designed to optimize daily supplement schedules and validate timing conflicts for safe absorption.

---

## 📌 Project Overview
The idea for `supliCheck` was born directly out of a personal friction point. Managing daily supplement intake like iron is challenging amid a busy schedule. Furthermore, standard tracking applications operate merely as passive digital text logs. They fail to account for critical timing conflicts, such as how caffeine or calcium consumption can severely inhibit iron absorption. 

`supliCheck` addresses this gap. Instead of acting as a passive alarm, it serves as an active assistant. The system evaluates user inputted intake schedules against a validation engine to help ensure supplement routines are safe and structurally optimized before any data is saved. 

### 🤖 The Engineering Approach: Why Build From Scratch?
While modern AI models can easily provide supplement advice or generic reminders, this project takes a step back to foundational computer science principles. The objective is to strengthen core algorithmic thinking and architectural design by building the logical rules manually. AI is leveraged strictly as an external technical mentor and debugging aid rather than outsourcing the core processing engine.

---

## 🛠️ Technical Architecture & Stack
To replicate industry standard enterprise patterns, the application is split into a completely decoupled two tier design:

* **Frontend:** A cross platform mobile user interface engineered using **Dart & Flutter SDK** to handle interactive user intake logs and notifications.
* **Backend API:** A distributed client server application managed via **Java** to parse data payloads and handle system logic.
* **Storage Layer:** Relational data tracking and schema enforcement powered by **PostgreSQL**, connected natively via self taught **JDBC** frameworks.
* **Verification Layer:** A rigid validation core using **NuSMV formal methods** to mathematically evaluate state loops against temporal timing rules.

---

## 📁 Repository Structure
```text
supliCheck/
├── backend/          # Java API source code & server logic
├── database/         # PostgreSQL schema files, tables, and JDBC scripts
├── frontend/         # Flutter/Dart mobile application files
├── verification/     # NuSMV state machine files and LTL/CTL logic rules
└── README.md         # Project documentation
```

---

## 📈 Learning Roadmap & Milestones
This project is an ongoing engineering exercise in public self directed learning, focusing on concepts outside the standard university curriculum:

- [ ] **Phase 1: Backend & Database Foundations** — Establish the local PostgreSQL relational schema and write the foundational Java JDBC connection scripts.
- [ ] **Phase 2: Logic Validation Core** — Build out the basic NuSMV state machine to test simple 24 hour routine parameters.
- [ ] **Phase 3: Decoupled API Integration** — Expose secure REST endpoints in the Java layer to accept data inputs.
- [ ] **Phase 4: Mobile Frontend Deployment** — Design the interface in Flutter and connect it asynchronously to the backend network engine.

---

## 👥 About the Developer
I am a Computer Science student at **SIM Global Education (University of London)**. I am utilizing this project as a practical playground to transition from theoretical programming concepts to active full stack systems engineering. 

Updates on this project, including technical breakthroughs and failures, are documented weekly as a transparent **"Build in Public" project series** on my LinkedIn network.

