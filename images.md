# Image Asset Register

**Project:** Hardware, Network & Behaviourist AI
**Last updated:** 2026-10-27
**Maintained by:** Thirishanth Veerasingam

This file logs every image used across the deck. Update it the moment an image is added, replaced, or removed. If an image breaks or a source vanishes, this file is how you find the replacement.

---

## Status legend

| Status | Meaning |
| :--- | :--- |
| ✅ **Local** | Downloaded, stored in `/images`, referenced by relative path. Safe. |
| ⚠️ **Hotlinked** | Loaded from an external URL. Renders today; may break without warning. |
| 🔍 **Unverified** | Caption or content not yet checked against the actual image. |
| 🚩 **Flagged** | Known problem — AI-generated, garbled labels, expiring URL, or wrong figure. |
| ⬜ **Planned** | Needed but not yet sourced or created. |

---

### Master table

| Fig | Chapter | Subject | Status | Local file |
| :---: | :---: | :--- | :---: | :--- |
| 1 | 1 | Von Neumann Bottleneck | ✅ Local | [Hand-drawn](https://github.com/user-attachments/assets/35a5d384-d54d-4053-b084-52139bf8277b) |
| 2 | 1 | Training vs. Inference | ✅ Local | [techwith.ram](https://www.instagram.com/p/DcTY23NJT5O/) |
| 3 | 1 | Explanation of GPU / TPU / NPU / FPGA / ASIC | ✅ Local | [ChatGPT](https://private-user-images.githubusercontent.com/161692024/685915662-86f73a16-9bb2-4d37-8eab-b43346c8e95a.png) |

### Figure 1 — Von Neumann Bottleneck

- **Chapter / section:** Ch 1 → Von Neumann Bottleneck
- **URL:** `https://github.com/user-attachments/assets/35a5d384-d54d-4053-b084-52139bf8277b`
- **Caption:** The performance limitation caused by the physical separation of the CPU (compute) and memory (storage) in traditional computers, forcing data to shuttle back and forth.
- **Attribution:** Hand-drawn by Thirishanth Veerasingam

### Figure 2 — Training vs. Inference

- **Chapter / section:** Ch 1 → Training vs. Inference
- **URL:** `https://www.instagram.com/p/DcTY23NJT5O/`
- **Attribution:** techwith.ram — "Training vs. Inference"
- **Reference number:** 7

### Figure 3 — Positional Encoding

- **Chapter / section:** Ch 3 → How LLMs Operate → 2. The Transformer and Self-Attention
- **URL:** `https://media.geeksforgeeks.org/wp-content/uploads/20250818131508982635/positional_encoding_in_transformer.webp`
- **Alt text:** Positional encoding adds a position signal to each token embedding
- **Caption:** Positional encoding injects a position signal into each token's embedding, so the model can tell "dog bites man" from "man bites dog".
- **Attribution:** GeeksforGeeks — "Positional Encoding in Transformers"
- **Reference number:** 11
- **Notes:**
  - Placement sits before the concept is fully used. Consider adding one bridging clause to the preceding paragraph: *"Without this signal, 'dog bites man' and 'man bites dog' would produce identical attention scores."*
- **Action:** Download locally; confirm it shows the position signal (heat-map or vector diagram), not the full transformer block.
