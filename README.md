# German Vocab Deep-Dive: Search-to-Dive MVP

A mobile-first utility designed for English speakers learning German. This app eliminates the friction between quick word lookup and grammatical mastery by providing instant articles, plurals, and case inflections in a single interaction.

---

## 🎯 The Problem (The "Two-Step Friction Loop")
Most translation tools (Google Translate/DeepL) are optimized for speed but fail on **grammatical depth**. Learners often find a translation but then have to open a second tool (dictionary or grammar table) to find the article or the correct case ending. 

**This project solves that by bridging the gap between "Search" and "Deep-Dive."**

## ✨ Key Features
* **Smart Type-Ahead:** Instant suggestions including Article + Lemma + Meaning as you type.
* **Inflection Resolution:** Type "Hunden" and the app resolves to "der Hund" while explaining the Dative plural context.
* **Case Deep-Dive:** A structured view of all 4 German cases (Nom, Akk, Dat, Gen) for every noun.
* **Grammar Insights:** Brief, AI-generated explanations of noun patterns (Strong/Weak/Mixed).

## 🛠️ Technical Stack (The Unified AI Stack)
This project leverages a modern, AI-native development workflow to move from concept to production at high velocity:

* **Platform:** [Lovable](https://lovable.dev/) (Full-stack AI App Generator)
* **Frontend:** React + Tailwind CSS
* **Backend/Database:** [Supabase](https://supabase.com/) (PostgreSQL)
* **LLM Engine:** Claude 3.5 Sonnet & GPT-4o
* **Automation:** n8n (Market Research & Discovery Phase)

## 📂 Repository Structure
* **[`/docs`](./docs):** Product Discovery, User Personas, Use Cases, and the PRD.
* **[`/raw-prompts`](./raw-prompts):** The "Source Code" for the AI logic, including system instructions for the suggestion engine and grammar generator.
* **[`/src`](./src):** The production application code (synced via Lovable).

## 🧠 Product Journey
This app was developed using a "Discovery-First" approach:
1.  **Market Research:** Analyzed 15+ competitors using automated n8n workflows.
2.  **Persona Mapping:** Defined "Alex," the intentional learner who prioritizes correctness over gamification.
3.  **Prompt Engineering:** Developed RTC (Role-Task-Constraint) prompts to ensure high-fidelity linguistic data.

---
*Created by Tom as part of an AI-Powered Product Management Journey.*
