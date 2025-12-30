# 🔬 OOPR Tool v1.0-alpha

**Open Ontological Peer Review** — A Reproducible AI-Based Peer Review Protocol for Ontological Frameworks

---

## ⚠️ Alpha Release Notice

**This is the first functional version of OOPR.** While the core concept is proven and the tool is usable, there is still significant work to be done. Development is ongoing, but time-intensive due to the complexity of the project.

### Current Status

✅ **Working:** 7 review axes, queue system, exports, stop control  
⚠️ **Limitations:** Requires trusted environment, no backend, no retry logic  
🔨 **In Development:** Backend security, public deployment, rate limiting  

**This is a research tool and proof-of-concept.** Use it in trusted environments (Claude artifacts, local development) while we work toward a production-ready v2.0.

---

## 📋 What is OOPR?

OOPR (Open Ontological Peer Review) is an **interactive tool** that enables rigorous, reproducible peer review of ontological and foundational frameworks using AI reviewers. Unlike traditional peer review which relies on authority and anonymous human judgment, OOPR formalizes review as an **open, installable, and repeatable procedure**.

### The Problem It Solves

Classical peer review fails systematically when confronted with:
- Pre-physical or ontological models
- Cross-disciplinary frameworks  
- Paradigm-forming or paradigm-questioning work
- Concepts that redefine foundational terms (time, mass, information)

Such works are often rejected not because they are inconsistent, but because they are **evaluated with inappropriate criteria**.

### The OOPR Solution

OOPR separates *review methodology* from *disciplinary authority* by:
- Using AI as **formal reviewers**, not judges
- Evaluating models along explicit, predefined axes
- Making all prompts and processes **fully transparent**
- Enabling **anyone to reproduce** the same review

---

## 🎯 Core Features

### 7 Review Axes

The tool evaluates frameworks along seven brutal, rigorous dimensions:

1. **A. Axiomatic Clarity** - Are foundational assumptions explicit and non-circular?
2. **B. Internal Consistency** - Are there contradictions or undefined behaviors?
3. **C. Logical Derivation** - Do conclusions follow necessarily from premises?
4. **D. Conceptual Precision** - Are key terms unambiguous and operationalizable?
5. **E. Model Scope & Boundaries** - What does it explain? Where does it stop?
6. **F. Falsifiability & Kill-Test** - What experiment would prove it wrong?
7. **G. Terminological Economy (Occam's Razor)** - Are new terms necessary or just renamings?

### Professional Workflow (v1.0-alpha)

- **Queue-Based Reviews** - Run all 7 axes automatically in sequence
- **Stop Control** - Abort reviews mid-process if needed
- **Run Modes** - "Run Missing" (skip completed) or "Re-run All" (fresh start)
- **Dual Export** - JSON snapshots (scientific) + Markdown reports (human-readable)
- **Full Reproducibility** - Every review includes prompts, versions, and metadata

---

## 🚀 Quick Start

### Easiest Way: Use in Claude Artifacts

The simplest way to use OOPR right now:

1. Go to [claude.ai](https://claude.ai)
2. Ask Claude: "Create the OOPR Tool v1.0-alpha as an artifact"
3. Paste the React code from `src/oopr-tool.jsx`
4. Start reviewing immediately - no installation needed!

**This is the recommended method for v1.0-alpha.**

### Alternative: Local Development

```bash
# Clone the repository
git clone https://github.com/yourusername/oopr-tool.git
cd oopr-tool

# Install dependencies
npm install

# Run locally
npm start
```

**Note:** Local setup requires Anthropic API access and proper configuration.

---

## 📖 How to Use

### Step 1: Enter Your Framework

Paste your ontological model, theory, or framework into the text area. Include:
- Core axioms
- Key principles  
- Foundational definitions
- Main derivations

**Tip:** Click "Load Example (Frequenzgesetz)" to see proper formatting.

### Step 2: Choose Your Review Mode

Select from the dropdown:
- **Run Missing** - Reviews only axes that haven't been completed yet (default)
- **Re-run All** - Clears all previous reviews and starts completely fresh

### Step 3: Start the Review Process

Click the button to start:
- **"Run Missing (X)"** - Shows how many axes still need review
- **"Re-run All (7)"** - Will review all 7 axes from scratch

**What happens:**
1. Each axis expands automatically as it's reviewed
2. The AI analyzes your framework with brutal honesty
3. Results appear in real-time below each axis
4. Progress bar shows overall completion

**Need to stop?** Click the red **"Stop"** button that appears during reviews.

### Step 4: Export Your Results

When reviews are complete, two export options appear:

- **Download JSON** - Complete scientific snapshot with all prompts, metadata, and reviews. Perfect for reproducibility and archiving.
- **Copy Markdown** - Human-readable report you can paste into documents, wikis, or papers.

---

## 📊 Understanding the Output

### What the AI Reviews Actually Look For

Each axis uses a **merciless prompt** designed to find weaknesses:

- **"Be merciless: name any circularity immediately"**
- **"Point out every contradiction — no matter how small"**
- **"Identify 'magical jumps' and hand-wavy reasoning"**
- **"If not falsifiable, write: NOT FALSIFIABLE"**
- **"Strip away poetic noise"**

This isn't about being nice - it's about being **honest and precise**.

### JSON Snapshot Structure

```json
{
  "tool": "OOPR",
  "version": "1.0-alpha",
  "generatedAt": "2025-01-XX...",
  "provider": {
    "name": "Claude Sonnet 4",
    "model": "claude-sonnet-4-20250514"
  },
  "axes": [
    {
      "id": "axiomatic",
      "title": "A. Axiomatic Clarity",
      "questions": [
        "Are base axioms explicitly stated?",
        "Is there clean separation between primitives?"
      ],
      "prompt": "Act as a rigorous theoretical physicist..."
    }
  ],
  "reviews": {
    "axiomatic": {
      "provider": "Claude Sonnet 4",
      "text": "Analysis results...",
      "timestamp": "2025-01-XX...",
      "promptVersion": "2.2.1",
      "axisId": "axiomatic"
    }
  },
  "metadata": {
    "totalAxes": 7,
    "completedAxes": 5,
    "maxTokens": 2000
  }
}
```

This enables:
- **Reproducibility** - Re-run with exact same prompts
- **Comparison** - Track framework evolution over time
- **Citation** - Reference specific reviews in academic work
- **Audit** - See exactly what was asked and answered

---

## 🧠 The Philosophy Behind OOPR

### Core Principle

> **Do not ask whether a model is correct. Ask whether it is coherent, explicit, and inspectable.**

OOPR is not about declaring truth. It's about **making review transparent, reproducible, and honest**.

### Ethical Foundation: "∞ − 1 = you"

OOPR is grounded in the axiom of finiteness:
- AI reviewers are **finite agents** (∞ − 1), not omniscient judges
- They serve **understanding and dialogue**, not verdicts
- Their role is **cooperative presentation**, not falsification
- **Authority is replaced with transparent methodology**

This principle comes from the Frequenzgesetz ethics protocol and applies to all OOPR reviews.

### What OOPR Is

✅ A **formal, reproducible review procedure**  
✅ A tool for **evaluating internal consistency**  
✅ An **open protocol** anyone can use and modify  
✅ A way to **stress-test** ontological frameworks  

### What OOPR Is NOT

❌ A truth oracle or validation system  
❌ A replacement for empirical science  
❌ An authority claim or academic gatekeeping  
❌ A substitute for human peer review  

**Think of it as:** A microscope for ideas. It shows structure, not correctness.

---

## 🔧 Technical Details

### Current Architecture (v1.0-alpha)

- **Frontend:** React with Tailwind CSS
- **AI Provider:** Anthropic Claude Sonnet 4 (via direct API)
- **Deployment:** Claude Artifacts or local development
- **Storage:** In-memory only (no persistence between sessions)

### Known Limitations

⚠️ **Use in trusted environments only:**

- API calls made directly from frontend (no backend proxy)
- API keys would be exposed in production deployment
- No rate limit handling or automatic retry
- No authentication or user management
- Best for: Claude artifacts, local testing, research use

### Coming in Future Versions

**v2.0 (Planned):**
- Serverless backend (Vercel/Cloudflare Workers)
- Secure API key handling
- Rate limit detection and retry logic
- Public deployment support
- User-provided API key option

**v3.0 (Planned):**
- Meta-review synthesis (AI aggregates all 7 axes)
- Multi-AI comparison (Claude vs GPT vs Gemini)
- Review evolution tracking
- Collaborative review sessions

---

## 📚 Use Cases

### For Framework Developers
- **Stress-test** your ontological model before publication
- **Identify weaknesses** early in development
- **Generate reproducible** review documentation
- **Show critics** you've done rigorous self-evaluation

### For Academic Reviewers  
- **Systematically evaluate** submitted frameworks
- **Ensure consistent** review criteria across papers
- **Provide structured**, actionable feedback
- **Document** your review process transparently

### For Educators
- **Teach critical thinking** about foundational theories
- **Demonstrate** what rigorous ontological review looks like
- **Show students** how to evaluate paradigm-level claims
- **Practice** philosophical analysis with AI assistance

### For Research Groups
- **Benchmark** competing ontological frameworks
- **Compare** different versions of a theory over time
- **Archive** review snapshots for reproducibility
- **Collaborate** on framework refinement

---

## 🤝 Contributing

OOPR is an **open protocol**. The concept is proven, but there's much work ahead.

### Ways to Contribute

**Code:**
- Backend implementation (v2.0)
- UI/UX improvements
- New review axes or prompt refinements
- Rate limiting and error handling
- Testing and bug reports

**Documentation:**
- Example frameworks with full reviews
- Tutorial videos or walkthroughs
- Translations to other languages
- Academic papers using OOPR

**Research:**
- Test OOPR on diverse ontological models
- Compare OOPR results with human peer review
- Develop meta-review algorithms
- Explore multi-AI consensus methods

### Development Priorities

**High Priority:**
1. Backend API proxy for secure deployment
2. Rate limit handling and retry logic
3. Better error messages and UX feedback

**Medium Priority:**
4. Meta-review synthesis feature
5. Multi-AI provider support
6. Review comparison tools

**Low Priority (but cool):**
7. Visual graph of framework structure
8. Automated claim extraction
9. Integration with academic platforms

See `ROADMAP.md` for detailed plans.

---

## 🗺️ Development Roadmap

### v1.0-alpha (Current)
- ✅ 7 review axes implemented
- ✅ Queue system with stop control
- ✅ JSON + Markdown export
- ✅ Reproducible snapshots
- ⚠️ Trusted environment only

### v2.0 (Next Major Release)
- 🔨 Serverless backend (API security)
- 🔨 Rate limit handling
- 🔨 Public deployment ready
- 🔨 User API key input option

### v3.0 (Future)
- 💭 Meta-review synthesis
- 💭 Multi-AI comparison
- 💭 Review evolution tracking
- 💭 Collaborative sessions

### v4.0+ (Vision)
- 🌟 Integration with arXiv, Zenodo
- 🌟 Visual framework mapping
- 🌟 Automated claim extraction
- 🌟 Real-time collaborative review

---

## 📄 License

MIT License - See LICENSE file for details.

You are free to use, modify, and distribute this tool. Attribution appreciated but not required.

---

## 🎓 Citation

If you use OOPR in academic work, please cite:

```bibtex
@software{berrang2025oopr,
  author = {Berrang, Christian},
  title = {OOPR: Open Ontological Peer Review Protocol},
  year = {2025},
  version = {1.0-alpha},
  url = {https://github.com/yourusername/oopr-tool}
}
```

**Plain text:**
```
Berrang, C. (2025). OOPR: Open Ontological Peer Review Protocol (v1.0-alpha).
GitHub. https://github.com/yourusername/oopr-tool
```

---

## 🌟 Acknowledgments

OOPR was developed alongside the **Frequenzgesetz** (Frequency Law) ontological framework as a companion tool for rigorous self-evaluation. The "∞ − 1 = you" ethical principle comes from that work.

**Special thanks to:**
- The AI research community for formal reasoning advances
- Early testers who provided brutal but valuable feedback
- Grok (xAI) for independently validating the protocol
- Claude (Anthropic) for enabling the Artifacts platform

---

## 📞 Contact & Support

### Getting Help

- **Issues:** [Open an issue](https://github.com/yourusername/oopr-tool/issues) for bugs or problems
- **Discussions:** [GitHub Discussions](https://github.com/yourusername/oopr-tool/discussions) for questions and ideas
- **Updates:** Watch this repo for new releases

### Community Guidelines

**Be constructive.** OOPR is about honest evaluation, not destruction.  
**Be patient.** This is an alpha release under active development.  
**Be open.** Share your review results and help improve the protocol.

---

## ❓ FAQ

**Q: Can I use this for my PhD thesis?**  
A: Yes, but make clear it's an alpha tool. Include the JSON snapshot for reproducibility.

**Q: Why only Claude? Can I use GPT-4?**  
A: v1.0-alpha uses Claude because it's available in Artifacts. v2.0 will support multiple AI providers.

**Q: Is this scientifically valid?**  
A: OOPR evaluates internal consistency, not empirical truth. It's a tool for philosophical analysis, not experimental validation.

**Q: Can I modify the review axes?**  
A: Yes! Fork the repo and customize the prompts. That's the whole point of "open" review.

**Q: Will this replace human reviewers?**  
A: No. OOPR complements human review by providing systematic, reproducible analysis. Humans still interpret results and make final judgments.

**Q: How long does a full review take?**  
A: About 3-5 minutes for all 7 axes, depending on model complexity and API response time.

---

## 🔥 Final Words

OOPR is **not perfect**. It's an alpha release with limitations and rough edges. But the core idea works: **formalized, reproducible, transparent peer review for ontological frameworks**.

If you believe that paradigm-questioning work deserves fair evaluation, if you think review should be a procedure rather than a verdict, if you want to stress-test your ideas with brutal honesty—

**Then OOPR is for you.**

---

**"Be merciless: name any circularity, vagueness or sleight-of-hand immediately."**

*— OOPR Review Principle*

---

**Status:** Alpha • **Version:** 1.0-alpha • **Last Updated:** January 2025
