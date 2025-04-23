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

│   brew_poison.py
│   defaults.sh
│   defaults_distributed.sh
│   dist_brew_poison.py
│   main.py
│   README.md
│   test_poisons.py
│   training_loop.py
│   __init__.py
│
├───data
│   │   cifar-10-python.tar.gz
│   │
│   └───cifar-10-batches-py
│           batches.meta
│           data_batch_1
│           data_batch_2
│           data_batch_3
│           data_batch_4
│           data_batch_5
│           readme.html
│           test_batch
│
├───forest
│   │   angular-expanse-455003-v7-cc6a622f8eaa.json
│   │   consts.py
│   │   cpoutput.txt
│   │   filtering_defenses.py
│   │   gcloud.py
│   │   hyperparameters.py
│   │   options.py
│   │   utils.py
│   │   __init__.py
│   │
│   ├───data
│   │   │   cached_dataset.py
│   │   │   datasets.py
│   │   │   diff_data_augmentation.py
│   │   │   kettle_base.py
│   │   │   kettle_benchmark_experiment.py
│   │   │   kettle_det_experiment.py
│   │   │   kettle_external.py
│   │   │   kettle_random_experiment.py
│   │   │   lmdb_datasets.py
│   │   │   mixing_data_augmentations.py
│   │   │   README.md
│   │   │   __init__.py
│   │   │
│   │   └───__pycache__
│   │           cached_dataset.cpython-312.pyc
│   │           datasets.cpython-312.pyc
│   │           diff_data_augmentation.cpython-312.pyc
│   │           kettle_base.cpython-312.pyc
│   │           kettle_benchmark_experiment.cpython-312.pyc
│   │           kettle_det_experiment.cpython-312.pyc
│   │           kettle_external.cpython-312.pyc
│   │           kettle_random_experiment.cpython-312.pyc
│   │           mixing_data_augmentations.cpython-312.pyc
│   │           __init__.cpython-312.pyc
│   │
│   ├───victims
│   │   │   batched_attacks.py
│   │   │   context.py
│   │   │   mobilenet.py
│   │   │   models.py
│   │   │   README.md
│   │   │   training.py
│   │   │   utils.py
│   │   │   vgg.py
│   │   │   victim_base.py
│   │   │   victim_distributed.py
│   │   │   victim_ensemble.py
│   │   │   victim_single.py
│   │   │   __init__.py
│   │   │
│   │   └───__pycache__
│   │           batched_attacks.cpython-312.pyc
│   │           context.cpython-312.pyc
│   │           mobilenet.cpython-312.pyc
│   │           models.cpython-312.pyc
│   │           training.cpython-312.pyc
│   │           utils.cpython-312.pyc
│   │           vgg.cpython-312.pyc
│   │           victim_base.cpython-312.pyc
│   │           victim_distributed.cpython-312.pyc
│   │           victim_ensemble.cpython-312.pyc
│   │           victim_single.cpython-312.pyc
│   │           __init__.cpython-312.pyc
│   │
│   ├───visualizations
│   │       gcp_activity.png
│   │       pca_detection.png
│   │       poison_output.py
│   │       xai_analysis.py
│   │
│   ├───witchcoven
│   │   │   gcp_activity.png
│   │   │   modules.py
│   │   │   output.py
│   │   │   pca_detection.png
│   │   │   README.md
│   │   │   witch_base.py
│   │   │   witch_bullseye.py
│   │   │   witch_convex_polytope.py
│   │   │   witch_htbd.py
│   │   │   witch_matching.py
│   │   │   witch_metapoison.py
│   │   │   witch_patch.py
│   │   │   witch_poison_frogs.py
│   │   │   witch_watermark.py
│   │   │   __init__.py
│   │   │
│   │   └───__pycache__
│   │           modules.cpython-312.pyc
│   │           witch_base.cpython-312.pyc
│   │           witch_bullseye.cpython-312.pyc
│   │           witch_convex_polytope.cpython-312.pyc
│   │           witch_htbd.cpython-312.pyc
│   │           witch_matching.cpython-312.pyc
│   │           witch_metapoison.cpython-312.pyc
│   │           witch_patch.cpython-312.pyc
│   │           witch_poison_frogs.cpython-312.pyc
│   │           witch_watermark.cpython-312.pyc
│   │           __init__.cpython-312.pyc
│   │
│   └───__pycache__
│           consts.cpython-312.pyc
│           filtering_defenses.cpython-312.pyc
│           hyperparameters.cpython-312.pyc
│           options.cpython-312.pyc
│           utils.cpython-312.pyc
│           __init__.cpython-312.pyc
│
├───log
│       README.md
│
├───patches
│       firefox.jpg
│       trigger_10.png
│
├───poisons
│       README.md
│
└───scripts
        benchmark_gen.py

