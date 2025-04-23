# Prompt‑Engineering Playbook

A curated **library of prompts, agent blueprints, and practical notebooks** that demonstrate modern prompt‑engineering patterns for large language models (LLMs).

---

## ✨ Why this repo?

* **Ready‑to‑use prompt templates** for customer‑service agents, strategic AI advisers, and more.  
* **Conversational‑agent role cards** in Spanish & English, showing how to scope instructions, interaction rules, and closing phrases.  
* **Notebooks that dissect advanced tactics** such as inner‑monologue, meta‑prompting, and multi‑round RAG.  
* **Reference txt guides** pulled from the OpenAI Cookbook and other public repos to complement hands‑on experimentation.

---

## 📂 Repository layout

```
prompt-engineering/
├── Agentic_Prompts/
│   └── CUSTOMER_SERVICE_AGENT.txt
├── Conversational_Agents/
│   ├── 🤖 AGENTE Agente de Inteligencia Artificial.txt
│   └── 🧩 AGENTE Ingeniero en IA Avanzada.txt
├── Prompts_from_other_repos/
│   ├── Enhance_your_prompts_with_meta_prompting.ipynb
│   ├── gpt4-1_prompting_guide.ipynb
│   └── prompt-engineering.txt
└── README.md   ← you are here
```

### Folder overview

| Folder | What’s inside | Highlights |
|--------|---------------|------------|
| `Agentic_Prompts` | Self‑contained **system prompts** that wire up tool calling & response formats. | Shows function‑calling schemas per OpenAI API guidelines. |
| `Conversational_Agents` | Spanish “role cards” for domain‑expert agents (AI strategy, advanced ML engineering). | Demonstrates layered instructions + closing triggers (“Cierro …”). |
| `Prompts_from_other_repos` | Educational notebooks & text excerpts sourced from OpenAI and community repos. | Covers inner‑monologue, meta‑prompting, eval strategies. |

---

## 🔨 How to use

1. **Clone the repo**

   ```bash
   git clone https://github.com/felipeortizh/prompt-engineering.git
   cd prompt-engineering
   ```

2. **Browse text assets**  
   Open any `.txt` file to copy the prompt into ChatGPT, your LangChain script, or the OpenAI Playground.

3. **Run the notebooks**  
   Launch Jupyter or VS Code to step through meta‑prompting and RAG demos. The notebooks require only `openai`, `langchain`, and `faiss‑cpu`/`chromadb` to run locally.

4. **Adapt & extend**  
   - Swap the *company name*, *tone*, or *tool schema* in `CUSTOMER_SERVICE_AGENT.txt`.  
   - Translate role cards to another language or domain.  
   - Plug the prompts into your code using LangChain Hub: `prompt = hub.pull("<your-prompt-id>")`.

---

## 🧠 Prompt‑engineering best practices

* Put clear **system instructions** first, separated by delimiters (e.g., `"""`).  
* Be specific about **formatting requirements** and closing behaviour.  
* Use **step‑by‑step reasoning or hidden inner‑monologue** when the chain of thought should not be exposed to users.  
* Iterate with **meta‑prompting**—let a stronger model rewrite prompts for a smaller model.  
* Couple prompts with **function calling** to ground factual answers in real data or APIs.  
* When building RAG systems, embed & retrieve external knowledge rather than stuffing long context blocks.  

For a deeper dive, check the OpenAI Cookbook prompt‑engineering guide and the latest research on goal‑oriented prompts.

---

## 🤝 Contributing

Issues & PRs are welcome!  
Add new prompt patterns, translate existing ones, or share notebooks exploring advanced evaluation strategies. Please follow the `CONTRIBUTING.md` guide (coming soon).

---

## 📜 License

This repository is distributed under the **MIT License**—see `LICENSE` for details.

---

## 📚 Further reading

* OpenAI Help Center – Best practices for prompt design  
* Hugging Face blog – *Make your own RAG from scratch*  
* arXiv – IM‑RAG: Multi‑round Retrieval‑Augmented Generation  
* OpenAI docs – Function calling  
* Medium – Meta‑prompting practical guide  

---

*Last updated: 23 Apr 2025*
