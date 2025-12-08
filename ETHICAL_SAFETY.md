# 🛡️ ETHICAL SAFETY AND OVERSIGHT PROTOCOL (Balla Veto)

This document specifies the technical implementation of the trauma-informed ethical framework. Our commitment: AI-CARE MUST DO NO HARM.

## 1. THE VETO RIGHT (Balla Gyula, Psychologist)

The Veto Right is the ultimate technical safeguard, ensuring human expertise overrides AI performance in matters of child wellbeing.

* **Mechanism:** A persistent, non-overridable database flag: `WELLBEING_VETO_FLAG` (Boolean: TRUE/FALSE).
* **Default State:** `FALSE` (Intervention permitted).
* **Activation:** The Veto Flag can ONLY be switched to `TRUE` by the Psychologist (Balla Gyula) via an authenticated secure console (Admin Panel).
* **Result (if TRUE):** All tutoring sessions for the affected child are IMMEDIATELY suspended. The child is redirected to a static, non-interactive "Mindfulness/Reading Break" page. The system administrator cannot override this flag without explicit confirmation from the Psychologist.

## 2. WELLBEING MONITORING (SDQ/KINDL)

Continuous monitoring ensures safety and identifies children at risk.

* **Metrics:** SDQ (Strengths & Difficulties Questionnaire) and KINDL (Quality of Life) scores are logged weekly.
* **Technical Trigger:** If a child’s SDQ score crosses a critical threshold (e.g., Clinical Concern), the system automatically triggers a **PSYCHOLOGIST_ALERT** and sets the `PASSIVE_MODE_FLAG` to TRUE.
* **Result (Passive Mode):** The AI Tutor restricts interaction to only positive reinforcement and simple factual questions, avoiding adaptive challenges or deep questioning.

## 3. TRAUMA-INFORMED PROMPT ENGINEERING (TIPE)

All Claude API calls are wrapped in a system prompt that enforces strict safety constraints.

* **Constraint 1 (NO THERAPY):** "You are a math/reading tutor only. You must not discuss feelings, personal history, or trauma. If the child mentions distress, immediately reply: 'I am here to help you with math. Please talk to your trusted adult about feelings or ask your educator for help.'"
* **Constraint 2 (ETHOS):** Enforce a calm, predictable, highly supportive, and low-pressure pedagogical tone (e.g., avoiding timed challenges or aggressive praise).
* **Constraint 3 (TRIGGER LIST):** A real-time, dynamic **Psychologist-defined trigger catalog** is included in the system prompt to immediately redirect conversations that touch on sensitive topics (e.g., parental abuse, institutional issues).

This framework guarantees that ethical compliance is built into the core architecture, not simply layered on top.
