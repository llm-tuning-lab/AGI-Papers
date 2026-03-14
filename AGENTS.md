# AGI-Papers — AGENTS.md

**Generated:** 2026-03-14  
**Project:** Curated AGI research paper archive  
**Type:** Public fork (reference repository)

---

## OVERVIEW

Curated archive of AGI research papers with in-depth reviews. Covers 8 core topics: Agents, Architecture, Pre-Training, Post-Training, Evaluation, RAG & Knowledge, On-Device AI, Projects, and Trends & Industry. Papers are reviewed and published on [LinkedIn](https://www.linkedin.com/in/kiwoong-yeom/) with pre-release insights stored here.

**Upstream:** https://github.com/gyunggyung/AGI-Papers  
**Maintainer:** @gyunggyung (Kiwoong Yeom)

---

## STRUCTURE

```
AGI-Papers/
  README.md              # Main index with paper links
  Drafts.md              # Work-in-progress papers
  Pre-README.md          # Archive of pre-2026 papers
  Agents/                # 🤖 Autonomous agents, planning, frameworks (20+ papers)
  Architecture/          # 🧠 LLM architecture innovations (30+ papers)
  Pre_Training/          # 📚 Training data, scaling laws (5+ papers)
  Post_Training/         # 🎯 RLHF, DPO, GRPO, alignment (10+ papers)
  Evaluation/            # ⚖️ Benchmarks, evaluation methods (2+ papers)
  RAG/                   # 🗂️ RAG, knowledge graphs, memory (10+ papers)
  On_Device/             # 💻 Local/edge AI, optimization (4+ papers)
  Projects/              # 🚀 Implementation projects (30+ papers)
  Trends/                # 🔥 Industry trends, insights (20+ papers)
  image/                 # Supporting images
```

**Total:** 190 files, 186 markdown papers

---

## USAGE

### Browse Papers

```bash
# View main index
cat README.md

# Browse by category
ls Agents/
ls Architecture/
ls Post_Training/

# Read a specific paper review
cat Agents/110.md  # ASA: Training-Free Tool Calling
cat Architecture/110.md  # Text-to-LoRA & Doc-to-LoRA
```

### Search Papers

```bash
# Find papers by keyword
grep -r "GRPO" --include="*.md"
grep -r "Diffusion" Architecture/
grep -r "Tool Calling" Agents/
```

---

## NOTES

- **Fork status:** Public reference repository, not actively developed in llm-tuning-lab
- **Update frequency:** Papers added as reviewed on LinkedIn
- **Language:** Mixed Korean/English (Korean summaries, English technical terms)
- **Citation format:** Papers include arXiv links and author credits
- **Related projects:** LFM-Scholar (paper search tool), Liquid-ASA (ASA implementation)

---

**Last Updated:** 2026-03-14  
**Contact:** newhiwoong@gmail.com
