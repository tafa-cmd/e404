# How Robust Are LLM Watermarks? Evaluating Text Watermarking Under Paraphrase Attacks

**CSGS Hackathon 2026 — P4: AI Security: Threat Analysis and Defensive Strategies**

## Overview

This project investigates the robustness of LLM text watermarking against paraphrase-based removal attacks. We implement the KGW green-list watermarking scheme (Kirchenbauer et al., ICML 2023), systematically evaluate it under four types of attacks across six watermark configurations, and propose an ensemble detection defense.

## Threat Model

- **Defender:** LLM service provider embedding watermarks to trace AI-generated content
- **Adversary:** Black-box attacker using a separate LLM to paraphrase and remove watermarks
- **Goal:** Attacker wants to reduce detection z-score below threshold while preserving text quality
