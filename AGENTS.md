# AGENTS.md - CMPLX-Formalization

Guidance for working with the Layer 4 Formalization repository.

---

## Repository Purpose

**Layer 4: Formalization** - Scientific papers and formal specifications that present CMPLX systems to academic peers. This is NOT implementation code, but rigorous mathematical and theoretical documentation.

---

## Key Conventions

### Paper Structure
All papers MUST follow this structure:
```
papers/AREA-XXX-title.md
├── Abstract
├── Introduction
├── Preliminaries
├── Core Theory
├── Applications to CMPLX
├── Related Work
├── Conclusion
├── References (bibtex format)
└── Appendix (proofs)
```

### Formal Specifications
Specifications use:
- **LaTeX math** for equations ($...$ or $$...$$)
- **Agda/Coq-style** for type theory judgments
- **BNF grammar** for syntax definitions
- **Inference rules** for operational semantics

### Document Status Tags
- 🔴 **Planning** - Outline/idea stage
- 🟡 **Drafting** - Content being written
- 🟢 **Review** - Ready for peer feedback
- 🔵 **Submitted** - At venue
- ✅ **Published** - Accepted/published

---

## Three Core Areas

### 1. Mathematical Framework
Focus: Type theory, category theory, lambda calculus

Key Concepts:
- Morphonic lambda calculus
- E8-embedded type systems
- Categorical semantics

### 2. Geometric Design Principles
Focus: E8 lattice, Leech lattice, geometric embeddings

Key Concepts:
- 240 roots of E8
- 196560 minimal vectors of Leech
- Geometric closure operations

### 3. Semantic Reasoning Theory
Focus: Meaning, truth, inference

Key Concepts:
- W5H semantic frames
- Causal truth maintenance
- Receipt semantics

---

## Source Material Processing

Documents in `source-docs/` are ORIGINALS (scanned/processed):
- Keep original filenames
- Extract to markdown in `source-materials/`
- Cite properly in papers

---

## Bibliography Format

```bibtex
@article{key,
  author = {Name},
  title = {Title},
  journal = {Venue},
  year = {2026},
  url = {https://...}
}
```

---

## Cross-References

Link to other CMPLX repositories:
- Implementation: `repos/cmplx-baseline/`
- Dev tools: `repos/cmplx-devkit/`
- MCP: `repos/cmplx-mcp/`
- Services: `repos/cmplx-monorepo/`
- Families: `repos/cmplx-uni/`
