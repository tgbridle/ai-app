# Product Requirements Document (PRD): German "Search-to-Dive" MVP

**Version:** 1 (Unified AI Stack)  
**Status:** Ready for Design/Build  
**Platform:** Mobile-Responsive Web (Lovable + Supabase)

---

## 1. Executive Summary
**Project Name:** German Vocab Deep-Dive  
**Objective:** Eliminate the "Two-Step Friction Loop" for English speakers learning German by providing a single, seamless path from partial word lookup to full grammatical understanding.

## 2. Problem Statement
Existing tools (Google Translate, DeepL) are optimized for speed but lack **educational depth**. Learners currently face two friction points:
1. **The Search Gap:** Users encounter inflected forms (e.g., "Hunden") but struggle to find the base "Lemma" and its associated article.
2. **The Context Gap:** Knowing a word means "Dog" is insufficient; the learner needs the **Article** and **Plural** to use it correctly in a sentence.

## 3. Target Audience: "The Intentional Learner"
* **Persona:** Alex (32), an English speaker living in/working with Germany.
* **Goal:** High accuracy and grammatical correctness over gamified streaks.
* **Pain Point:** Context-switching between translators, dictionaries, and grammar tables.

## 4. Functional Requirements (MVP Scope)

### P0: Smart Type-Ahead (The "Search")
* **Requirement:** As the user types (e.g., "Hu"), the app suggests `Article + Lemma + English Translation`.
* **Logic:** Must handle partial strings and resolve inflected forms back to the root Lemma.

### P0: The Deep-Dive (The "Learn")
* **Requirement:** Selecting a suggestion reveals a structured deep-dive view.
* **Core Data:** * Full 4-case table (Nominative, Accusative, Dative, Genitive) for Singular and Plural.
    * 1-sentence "Grammar Insight" explaining the noun's pattern (e.g., "Strong Masculine").

### P1: Clean Utility UI
* **Requirement:** Minimalist, fast, text-focused interface optimized for mobile browser input.

## 5. Technical Requirements (Unified Stack)

| Component | Tooling | Role |
| :--- | :--- | :--- |
| **Frontend** | Lovable (React/Tailwind) | UI/UX and client-side search logic. |
| **Backend/DB** | Supabase (Postgres) | Storage for word data and search history. |
| **AI Engine** | Claude 3.5 Sonnet | Integrated directly via Lovable for grammar generation. |
| **Version Control** | GitHub Two-Way Sync | Direct commit history to `ai-learning-journey/ai-app/`. |

## 6. User Stories
1. **As Alex**, I want to type "Hu" and see "der Hund — dog" so I don't have to finish typing the word to know its gender.
2. **As Alex**, I want to see a table of cases for "Hund" so I know whether to write "den Hund" or "dem Hund" in my email.
3. **As Alex**, I want the app to recognize "Hunden" and map it to "der Hund" so I don't need to know the base form to start my search.

## 7. Future Scope (V2+)
* Verb conjugation deep-dives.
* Personal "Saved Vocab" lists and SRS (Spaced Repetition) integration.
* Audio pronunciation.

---
