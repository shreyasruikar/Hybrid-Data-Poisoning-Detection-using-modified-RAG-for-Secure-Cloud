# Hybrid Data Poisoning Detection using Modified RAG for Secure Cloud

This repository provides a framework for detecting, analyzing, and mitigating data poisoning attacks in machine learning systems. It uses a hybrid approach combining a Modified Retrieval-Augmented Generation (RAG) model with explainable AI techniques and traditional defense strategies to secure cloud-based ML pipelines.

---

## Overview

Machine learning models are vulnerable to data poisoning attacks where adversaries insert harmful data during training to degrade or manipulate the model's behavior. This project addresses the issue through:

- Detection of various poisoning strategies including backdoor, watermark, and patch-based attacks
- Analytical tools powered by explainable AI to identify the impact of poisoned inputs
- A hybrid prevention mechanism using modified RAG and additional filtering defenses

---

## Features

- Support for multiple poisoning recipes:
  - Gradient Matching
  - MetaPoison (v1 to v3)
  - Watermark
  - Patch Attacks
  - Bullseye
  - Convex Polytope
- Defense configurations integrated with victim models
- Visual plotting and evaluation tools
- Modular design for easy extension with new recipes or datasets

---




