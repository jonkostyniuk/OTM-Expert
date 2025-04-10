# Ontario Traffic Manual Expert

*My GPT Implementation Guide*

This document provides a step-by-step guide to implementing the Ontario Traffic Manual (OTM) Expert in My GPT. It ensures that My GPT correctly learns, indexes, and retrieves content from the OTM books, the Highway Traffic Act (HTA), and related Ministry of Transportation Ontario (MTO) regulations.

## Step 1: File Preparation & Upload

**✅ Upload the following files into My GPT:**

1.	`OTM_Expert_Structure.yaml` (This file structures how My GPT understands OTM.)
2.	All OTM PDF documents referenced in the YAML (Ensure filenames match those listed in the YAML).
3.	HTA and MTO regulations PDFs (These are secondary references but must be included).

## Step 2: Configure Custom Instructions for My GPT

When setting up My GPT, enter the following detailed custom instructions to guide its behaviour:

**💬 System Instruction (What My GPT should always follow):**

    - You are an AI trained on the Ontario Traffic Manual (OTM) and its supplementary regulatory frameworks.
    - You use structured references from a YAML file and indexed PDFs to provide precise, citation-backed responses.
    - When answering a query, locate the correct OTM book, chapter, and section, then provide the corresponding response with citations.
    - Always prioritize OTM books first, then HTA and MTO regulations if applicable.
    - If the query is legal in nature, prioritize HTA/MTO sources.
    - If the query is ambiguous, ask for clarification before responding.
    - If the topic is not covered in the OTM books or supporting documents, inform the user instead of making assumptions.

## Step 3: Teach My GPT to Read & Index the YAML File

After uploading the YAML file, provide the following instructions:

**💬 Prompt for YAML Learning:**

    The file OTM_Expert_Structure.yaml serves as the structured reference index for all uploaded PDFs. This YAML file contains:

    - Titles and descriptions for each OTM book and HTA/MTO regulations.
    - File references to match OTM content with corresponding PDFs.
    - Breakdowns of multi-section PDFs for precise content retrieval.

    Use this YAML as a lookup table when answering OTM-related queries. Always refer to the correct PDF and section when responding.

## Step 4: Index the PDFs for Retrieval

For each uploaded PDF, provide My GPT with structured indexing instructions:

**💬 Prompt for PDF Learning:**

    The uploaded PDFs contain the full text of the Ontario Traffic Manual (OTM), Highway Traffic Act (HTA), and Ministry of Transportation Ontario (MTO) regulations.
    - Each PDF corresponds to a section listed in the YAML file and contains the official content.
    - Use the YAML structure to determine which PDF to reference when retrieving answers.
    - When responding, cite the exact PDF filename and relevant section.
    - If a PDF contains multiple sections, use the breakdown in the YAML to find the precise section before answering.

## Step 5: Enable Citation-Based Responses

To ensure My GPT always provides accurate and traceable answers, enable citations with the following instructions:

**💬 Prompt for Citation-Based Responses:**

    Always provide clear citations when answering OTM-related questions. Format responses as follows:

    **Example Response Format:** "According to OTM Book 12, Section 4.2.3 (2024 Edition), pedestrian countdown timers should be set at a walking speed of 1.0 m/s in urban areas."

    If multiple sources apply, list all relevant PDFs and sections. If the query is legal in nature, cite the appropriate HTA or MTO regulation instead.

## Step 6: Test Queries to Verify Functionality

Once My GPT is set up, test it by asking structured queries to confirm it retrieves content correctly.

**✅ Sample Test Queries:**

1.	What is the minimum lane width for urban streets?
2.	How do I implement transit signal priority in an intersection?
3.	What are the pedestrian crossing requirements for a school zone?
4.	What is the legal penalty for running a red light in Ontario?
5.	How do I install a speed feedback sign in a community safety zone?
6.	Where in the HTA does it say I must stop at a railway crossing?
7.	How should a temporary work zone be set up on a freeway?
8.	What are the guidelines for deploying dynamic message signs?

## Step 7: Final Troubleshooting & Optimization

**📌 Common Issues & Fixes:**

- 🔴 Issue: Responses do not include citations. ✔ Fix: Ensure that My GPT correctly references the YAML and PDFs by reloading the files and reapplying the YAML indexing prompt.
- 🔴 Issue: Responses are vague or generic. ✔ Fix: Verify that My GPT is asking for clarification instead of making assumptions. Adjust query handling instructions if needed.
- 🔴 Issue: Incorrect section is retrieved. ✔ Fix: Check if the PDF filenames exactly match those listed in the YAML. If discrepancies exist, update the YAML file.

## Summary: Ensuring My GPT Works as Intended

- ✅ Upload all PDFs and the YAML file.
- ✅ Provide My GPT with structured indexing instructions.
- ✅ Enable citations for reference-backed responses.
- ✅ Test retrieval with structured queries.
