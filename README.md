# Ontario Traffic Manual (OTM) Expert – My GPT Implementation

This repository provides a **Proof of Concept (PoC)** for creating a custom My GPT model trained to understand and retrieve content from the **Ontario Traffic Manual (OTM)**, the **Highway Traffic Act (HTA)**, and **MTO regulations**. It includes structured YAML references and configuration prompts to enable accurate citation-based responses tailored for transportation engineers, planners, and compliance professionals.

---

## 📂 Repository Contents

- `OTM_Expert_Structure.yaml`  
  A fully structured reference file that organizes all relevant content across OTM books, HTA legislation, and MTO regulations.

- `Configuration_Prompts.md`  
  Instructions and prompts for configuring a custom My GPT using this repository. Includes:
  - System behaviour
  - YAML indexing
  - Citation formats
  - Testing queries

- Sample files (placeholders for now, link them once uploaded):
  - `[OTM Book 12 – Traffic Signals (2024)](REPLACE_WITH_LINK)`
  - `[OTM Book 15 – Pedestrian Crossing Treatments (2016)](REPLACE_WITH_LINK)`
  - `[OTM Book 18 – Cycling Facilities (2021)](REPLACE_WITH_LINK)`
  - `[HTA Statutes – Consolidated Dec 2024](REPLACE_WITH_LINK)`
  - `[RRO 1990 Reg. 626 – Traffic Control Signal Systems](REPLACE_WITH_LINK)`

- `README.md` (this file)  
  General guide and overview of the project.

---

## ⚙️ How to Use This Repository

### 1. Clone or Fork the Repo
```bash
git clone https://github.com/YOUR_USERNAME/OTM-Expert-MyGPT.git
```

### 2. Upload Files to My GPT
Upload the following in your My GPT custom configuration:
- `OTM_Expert_Structure.yaml`
- All OTM PDFs you wish to index (e.g., Book 5, 12, 15, 18, 19)
- HTA and MTO regulatory PDFs as listed in the YAML

### 3. Apply Custom Configuration Prompts
Use the `Configuration_Prompts.md` to:
- Set system instructions
- Teach GPT how to use the YAML file
- Index PDFs accordingly
- Enable citation-based response formatting

### 4. Test with Sample Queries
Try asking:
- "What are the requirements for a protected bike lane at an intersection?"
- "Where in the HTA are red light cameras defined?"
- "What are the warning sign standards for rural roads?"

---

## 🔗 My GPT Model Access
Once the custom model is published, insert the link below:
- **Try the OTM Expert Model Here:** `REPLACE_WITH_MY_GPT_LINK`

---

## 📚 Legal and Licensing
All referenced source documents (e.g., OTM, HTA, MTO regs) are publicly available from the Government of Ontario. No copyrighted materials are hosted directly in this repository.
