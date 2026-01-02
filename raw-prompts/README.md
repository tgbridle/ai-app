# 🧠 AI Prompt Library (Prompt Engineering)

This folder contains the "Intelligence Assets" of the project. These prompts define the personas, logic, and output constraints for the LLMs used in the discovery and application phases.

## 🛠️ Engineering Standards
Every prompt in this library follows the **RTC (Role-Task-Constraint)** framework:
* **Role:** Defines the expert persona (e.g., "AI PM Specialist").
* **Task:** Clear, actionable objective.
* **Constraints:** Specific limitations (e.g., "German/English only," "JSON output only").

## 📂 Library Structure
* **[/discovery](./discovery/):** High-temperature prompts for market synthesis and persona ideation.
* **[/app-v1](./app-v1/):** Low-temperature, highly structured prompts for the production "Search-to-Dive" engine.
