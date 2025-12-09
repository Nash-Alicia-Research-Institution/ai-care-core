# AI TOOLING STACK FOR NARI R&D (The Builder Track)

This document lists the Generative AI platforms utilized by the Principal Investigator (PI) and the NARI team for high-velocity research, software development (TIPE Protocol), strategic planning, and documentation.

## Strategic Use of AI Platforms

The project utilizes a diversified AI stack to leverage the unique strengths of each model, ensuring robust cross-validation and efficiency in R&D.

| Tool / Platform | Strategic Role in AI-CARE R&D | Key Contribution |
| :--- | :--- | :--- |
| **Claude Pro** (Anthropic) | **Core Ethical Alignment & Prompt Engineering.** | Used exclusively for the **TIPE (Trauma-Informed Prompt Engineering)** protocol development due to its foundation in **Constitutional AI** and superior safety focus. Critical for VETO logic refinement. |
| **Gemini Pro** (Google) | **Strategic Planning & Multimodal Analysis.** | Used for complex **grant strategy analysis** (e.g., ERC, Horizon Europe), budget breakdown, competitor analysis, and generating complex documentation templates (like this one). Provides real-time information access. |
| **Google AI Studio** | **Model Prototyping & Workflow Integration.** | Used for rapid prototyping and testing of the TIPE protocol's prompt architecture before migrating to the Claude API. Essential for quick iteration on safety triggers. |
| **ChatGPT (OpenAI)** | **General R&D & Idea Generation.** | Used for broad literature reviews, initial code scaffolding (e.g., non-critical parts of the UI), and brainstorming complex technical solutions (e.g., Filecoin forking concepts). |
| **GitHub Copilot** | **Software Development Efficiency.** | Used directly within the IDE for code acceleration, debugging, and drafting documentation for the Open Source repository, significantly speeding up the delivery of the NARI core code. |
| **Deepseek** | **Code Optimization & Benchmarking.** | Utilized for specialized code review, benchmarking performance, and seeking alternative, highly efficient code solutions for the decentralized data management layer. |

## Ethical Note on Tool Usage

The PI ensures that no sensitive project data (especially any clinical data) is shared with any external LLM platform unless specifically required for API testing within a secure, controlled, and anonymized environment (e.g., Google AI Studio prototyping).

The **TIPE Protocol** is built on the belief that human oversight is paramount. Therefore, all AI output is subject to the **PI's final, non-delegable critical review** and validation before deployment. The tools serve as accelerators, not decision-makers.
