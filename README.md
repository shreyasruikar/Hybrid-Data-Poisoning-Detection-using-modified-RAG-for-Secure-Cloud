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

## Project Structure

Hybrid-Data-Poisoning-Detection/ │ ├── brew_poison.py ├── defaults.sh ├── defaults_distributed.sh ├── dist_brew_poison.py ├── main.py ├── README.md ├── test_poisons.py ├── training_loop.py ├── init.py │ ├── data/ │ ├── cifar-10-python.tar.gz │ └── cifar-10-batches-py/ │ ├── batches.meta │ ├── data_batch_1 to data_batch_5 │ ├── readme.html │ └── test_batch │ ├── forest/ │ ├── angular-expanse-455003-v7-cc6a622f8eaa.json │ ├── consts.py, cpoutput.txt, gcloud.py, ... │ ├── data/ │ │ ├── *.py │ │ └── pycache/ │ ├── victims/ │ │ ├── *.py │ │ └── pycache/ │ ├── visualizations/ │ │ ├── gcp_activity.png │ │ ├── pca_detection.png │ │ ├── poison_output.py │ │ └── xai_analysis.py │ ├── witchcoven/ │ │ ├── *.py │ │ ├── *.png │ │ └── pycache/ │ └── pycache/ │ ├── log/ │ └── README.md │ ├── patches/ │ ├── firefox.jpg │ └── trigger_10.png │ ├── poisons/ │ └── README.md │ └── scripts/ └── benchmark_gen.py




