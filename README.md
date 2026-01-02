# RTHH: Robby The Hallucination Hunter
Evaluating and Reducing Medical Hallucinations in Large Language Models

**Project Summary**

RTHH explores how large language models hallucinate when answering medical questions and whether structured prompt design can reduce those errors.
The project evaluates two models — Gemini and ChatGPT, in two stages:
- Phase I: Baseline responses using simple prompts
- Phase II: Structured prompting using four tones to test whether tone reduces hallucinations

The full research study, results, and figures are included in the project's final paper.

**Tools & Tech**
- Language: Python
- Libraries: Pandas, NumPy, Matplotlib, SentenceTransformers
- Models: Gemini (API), ChatGPT (API)
- Embedding Model: MiniLM-L6
- Datasets:
    - CuraiHealth Medical Questions (used only for initial pipeline testing)
    - MedQuad Medical QA (primary dataset for both phases)

**What’s Inside the Repository**

**Documents Folder**

Contains all final written materials for RTHH:
- Tecnical Report - the full research paper (Abstract, Methods, Results, Conclusion, IEEE citations)
- Structural Prompts - the four structured prompts used in Phase II (Professional Doctor, Medical Specialist, Friendly/Respectful, Rude/Direct)

These allow anyone to fully understand and replicate the experiment.

**Phase I Folder**

Materials related to baseline testing:
- Code used to send raw questions with simple prompts
- Manual labels (correct, incorrect, hallucinated)
- Embedding similarity calculations
- CSVs used to generate the baseline diagram

This phase shows how the models behave without guidance.

**Phase II Folder**

Materials from the structured prompting experiments:
- Code for evaluating the four prompt tones
- Model outputs for each tone
- Embedding similarity CSVs
- Result files used for the ChatGPT and Gemini prompt tone diagrams

This phase measures how prompt tone affects hallucination rates.

**Presentation Folder**

Contains the final presentation used for the course:
- Slide Show - overview of the problem, methods, results, and key findings

**Repository Notes**

- Ollama (DeepSeek, Gemma) was removed due to hardware limitations
- Only Gemini and ChatGPT were used in the final study
- All citations appear inside the paper

**Thank You**

Thank you for taking the time to explore this project. I hope the findings and materials in this repository are helpful for anyone interested in medical AI safety or hallucination research.
