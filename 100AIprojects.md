# 100 Artificial Intelligence Projects for Students and Developers

> A curated collection of 100 hands-on AI project ideas spanning 10 core domains, designed to guide students from fundamentals to production-grade systems. Each project includes a reference link to relevant repositories, papers, or frameworks.

---

## Table of Contents

- [Domain 1: Retrieval-Augmented Generation (RAG)](#domain-1-retrieval-augmented-generation-rag)
- [Domain 2: AI Agents and Autonomous Systems](#domain-2-ai-agents-and-autonomous-systems)
- [Domain 3: Natural Language Processing (NLP)](#domain-3-natural-language-processing-nlp)
- [Domain 4: Computer Vision](#domain-4-computer-vision)
- [Domain 5: Generative AI and Large Language Models](#domain-5-generative-ai-and-large-language-models)
- [Domain 6: Speech and Audio AI](#domain-6-speech-and-audio-ai)
- [Domain 7: Reinforcement Learning](#domain-7-reinforcement-learning)
- [Domain 8: MLOps and AI Infrastructure](#domain-8-mlops-and-ai-infrastructure)
- [Domain 9: AI for Healthcare and Science](#domain-9-ai-for-healthcare-and-science)
- [Domain 10: Multimodal AI Systems](#domain-10-multimodal-ai-systems)

---

## Recommended Prerequisites

Before starting any project, ensure familiarity with the following:

- Python 3.9 or higher
- Basic machine learning concepts (supervised, unsupervised learning)
- Familiarity with at least one deep learning framework (PyTorch or TensorFlow)
- Understanding of REST APIs and JSON data formats
- Version control with Git

---

## Domain 1: Retrieval-Augmented Generation (RAG)

RAG systems combine the generative power of large language models with external knowledge retrieval, enabling AI to answer questions grounded in real, up-to-date documents.

**Core Resources**

- LangChain RAG Documentation: https://python.langchain.com/docs/use_cases/question_answering/
- LlamaIndex (formerly GPT Index): https://github.com/run-llama/llama_index
- FAISS Vector Search by Facebook AI: https://github.com/facebookresearch/faiss
- ChromaDB Open-Source Vector Store: https://github.com/chroma-core/chroma

---

**Project 1: PDF Question-Answering System**

Build a pipeline that ingests PDF documents, splits them into chunks, embeds them using a sentence transformer, stores them in a vector database, and answers natural language questions using an LLM.

Reference: https://github.com/run-llama/llama_index/tree/main/docs/examples/query_engine

---

**Project 2: Multi-Document Research Assistant**

Extend the basic RAG pipeline to handle multiple documents simultaneously. Implement source attribution so the model cites which document each answer comes from.

Reference: https://github.com/langchain-ai/langchain/tree/master/cookbook

---

**Project 3: RAG with Re-Ranking**

Implement a two-stage retrieval system: initial BM25 keyword retrieval followed by a cross-encoder re-ranker to improve answer relevance before passing context to the LLM.

Reference: https://github.com/UKPLab/sentence-transformers/tree/master/examples/applications/retrieve_rerank

---

**Project 4: Conversational RAG Chatbot with Memory**

Build a RAG chatbot that maintains conversation history across turns. The system should reformulate follow-up questions using prior context before issuing retrieval queries.

Reference: https://python.langchain.com/docs/use_cases/question_answering/chat_history

---

**Project 5: RAG over a SQL Database**

Implement a text-to-SQL RAG system that translates natural language questions into SQL queries, executes them against a relational database, and returns synthesized answers.

Reference: https://github.com/run-llama/llama_index/blob/main/docs/examples/index_structs/struct_indices/SQLIndexDemo.ipynb

---

**Project 6: Graph RAG System**

Build a knowledge graph from a document corpus using entity extraction and relation detection. Use graph traversal to retrieve contextually connected entities before generation.

Reference: https://github.com/microsoft/graphrag

---

**Project 7: Hybrid Search RAG (Dense + Sparse)**

Combine dense vector similarity search (semantic) with sparse BM25 keyword search using a weighted fusion strategy such as Reciprocal Rank Fusion (RRF).

Reference: https://github.com/weaviate/weaviate/tree/main/examples

---

**Project 8: RAG Evaluation Framework**

Build an automated evaluation system for RAG pipelines using metrics such as faithfulness, answer relevancy, and context precision.

Reference: https://github.com/explodinggradients/ragas

---

**Project 9: Streaming RAG API with FastAPI**

Wrap a RAG pipeline in a production-ready FastAPI server that streams responses token-by-token to the client using server-sent events.

Reference: https://github.com/tiangolo/fastapi

---

**Project 10: Adaptive RAG with Query Routing**

Build a RAG system that classifies user queries and dynamically routes them to the appropriate retrieval strategy: vector search, SQL lookup, or web search.

Reference: https://github.com/langchain-ai/langgraph/tree/main/examples

---

## Domain 2: AI Agents and Autonomous Systems

AI agents use LLMs as a reasoning engine to plan, use tools, and execute multi-step tasks autonomously with minimal human intervention.

**Core Resources**

- LangGraph Framework: https://github.com/langchain-ai/langgraph
- AutoGen by Microsoft: https://github.com/microsoft/autogen
- CrewAI Multi-Agent Framework: https://github.com/crewAIInc/crewAI
- OpenAI Swarm (experimental): https://github.com/openai/swarm

---

**Project 11: ReAct Agent with Custom Tools**

Implement the ReAct (Reasoning + Acting) agent pattern from scratch. Equip the agent with tools such as web search, a calculator, and a code executor.

Reference: https://arxiv.org/abs/2210.03629

---

**Project 12: Autonomous Code Review Agent**

Build an agent that reads a GitHub repository, identifies potential bugs and code smells, writes a structured review report, and optionally opens pull request comments.

Reference: https://github.com/microsoft/autogen/tree/main/samples/apps

---

**Project 13: Multi-Agent Research Pipeline**

Architect a crew of specialized agents: a Researcher, a Writer, and an Editor. Each agent has a defined role and passes outputs to the next in sequence.

Reference: https://github.com/crewAIInc/crewAI/tree/main/examples

---

**Project 14: Browser Automation Agent**

Build an agent that can navigate the web, fill forms, extract information, and report results using browser automation tools combined with an LLM planner.

Reference: https://github.com/browser-use/browser-use

---

**Project 15: Data Analysis Agent**

Create an agent that accepts a raw CSV file, autonomously runs exploratory data analysis, generates charts, identifies correlations, and produces a written summary report.

Reference: https://github.com/langchain-ai/langchain/blob/master/cookbook/pandas_dataframe_agent.ipynb

---

**Project 16: Email Triage and Response Agent**

Build an agent connected to a Gmail or Outlook inbox that classifies incoming emails by urgency, drafts suggested replies, and routes action items to a task manager.

Reference: https://github.com/microsoft/autogen/tree/main/samples

---

**Project 17: Agentic DevOps Pipeline**

Design an agent that monitors application logs, detects anomalies, searches a knowledge base for known issues, and drafts a runbook entry or incident report automatically.

Reference: https://github.com/langchain-ai/langgraph/blob/main/examples/agent_supervisor.ipynb

---

**Project 18: Self-Correcting Agent with Reflection**

Implement an agent that critiques its own outputs, identifies errors in reasoning or code, and revises its answer through a structured self-reflection loop.

Reference: https://arxiv.org/abs/2303.11366

---

**Project 19: Financial Research Agent**

Build an agent that retrieves company filings, earnings transcripts, and financial news, synthesizes the information, and produces an investment thesis with risk factors.

Reference: https://github.com/crewAIInc/crewAI/blob/main/examples/stock_analysis.py

---

**Project 20: Long-Horizon Task Planning Agent**

Implement a hierarchical planning agent (using frameworks such as HuggingGPT or Plan-and-Execute) that decomposes complex, multi-day tasks into subtasks and executes them sequentially.

Reference: https://github.com/langchain-ai/langchain/blob/master/cookbook/plan_and_execute_agent.ipynb

---

## Domain 3: Natural Language Processing (NLP)

NLP encompasses a wide range of text understanding and generation tasks, from sentiment analysis to machine translation.

**Core Resources**

- Hugging Face Transformers: https://github.com/huggingface/transformers
- spaCy Industrial NLP: https://github.com/explosion/spaCy
- NLTK Toolkit: https://github.com/nltk/nltk
- AllenNLP Research Library: https://github.com/allenai/allennlp

---

**Project 21: Fine-Tuned Sentiment Classifier**

Fine-tune a BERT-based model on a domain-specific review dataset (e.g., product reviews, clinical notes) to perform multi-class sentiment classification.

Reference: https://github.com/huggingface/transformers/tree/main/examples/pytorch/text-classification

---

**Project 22: Named Entity Recognition (NER) System**

Train a custom NER model to extract domain-specific entities such as medical terms, legal clauses, or financial instruments from unstructured text.

Reference: https://spacy.io/usage/training

---

**Project 23: Abstractive Text Summarization**

Fine-tune a sequence-to-sequence model (BART or T5) on a news dataset to generate concise, human-quality summaries of long-form articles.

Reference: https://github.com/huggingface/transformers/tree/main/examples/pytorch/summarization

---

**Project 24: Machine Translation System**

Train a transformer-based translation model on a parallel corpus for a low-resource language pair and evaluate it using BLEU and chrF metrics.

Reference: https://github.com/huggingface/transformers/tree/main/examples/pytorch/translation

---

**Project 25: Question Generation from Text**

Build a system that reads a passage and automatically generates high-quality comprehension questions, useful for educational platforms and automated quiz creation.

Reference: https://github.com/patil-suraj/question_generation

---

**Project 26: Text Classification with Few-Shot Learning**

Implement a few-shot text classifier using a pre-trained LLM and prompt engineering. Compare its accuracy against a fully supervised fine-tuned model.

Reference: https://github.com/huggingface/setfit

---

**Project 27: Coreference Resolution Pipeline**

Build a system that identifies all mentions of the same entity in a document and links them, enabling downstream tasks like information extraction and document summarization.

Reference: https://github.com/huggingface/neuralcoref

---

**Project 28: Automatic Essay Grading System**

Build a model that evaluates student essays along dimensions such as coherence, grammar, and argument strength, providing a score and written feedback.

Reference: https://github.com/BNUDPCC/AES

---

**Project 29: Legal Document Clause Extraction**

Build an NLP pipeline that identifies and classifies specific clauses in contracts (e.g., indemnification, governing law, termination) using a fine-tuned transformer.

Reference: https://github.com/TheAtticusProject/cuad

---

**Project 30: Multilingual Intent Classification**

Train an intent classifier using XLM-RoBERTa that handles customer service queries across five or more languages without language-specific fine-tuning.

Reference: https://github.com/huggingface/transformers/tree/main/examples/pytorch/text-classification

---

## Domain 4: Computer Vision

Computer vision enables machines to interpret and understand visual information from images and video.

**Core Resources**

- Ultralytics YOLOv8: https://github.com/ultralytics/ultralytics
- OpenCV: https://github.com/opencv/opencv
- torchvision: https://github.com/pytorch/vision
- Detectron2 by Facebook AI: https://github.com/facebookresearch/detectron2

---

**Project 31: Real-Time Object Detection System**

Deploy a YOLOv8 model to detect and track objects in a live video feed. Add a dashboard that displays object counts and confidence scores in real time.

Reference: https://github.com/ultralytics/ultralytics/tree/main/examples

---

**Project 32: Medical Image Segmentation**

Train a U-Net model to segment tumors or organs from medical imaging data (e.g., CT or MRI scans) using the Medical Segmentation Decathlon dataset.

Reference: https://github.com/MIC-DKFZ/nnUNet

---

**Project 33: Facial Expression Recognition**

Build a convolutional neural network that classifies facial expressions into categories (happy, sad, angry, surprised, etc.) and deploy it as a browser-based demo.

Reference: https://github.com/HSE-asavchenko/face-emotion-recognition

---

**Project 34: Document Layout Analysis**

Build a system that detects tables, figures, headings, and paragraphs in scanned documents using a layout detection model, enabling structured data extraction from PDFs.

Reference: https://github.com/microsoft/unilm/tree/master/layoutlm

---

**Project 35: Optical Character Recognition (OCR) Pipeline**

Build an end-to-end OCR pipeline using a text detection model combined with a recognition model, capable of handling curved or low-quality text in natural scene images.

Reference: https://github.com/PaddlePaddle/PaddleOCR

---

**Project 36: Anomaly Detection in Manufacturing Images**

Train a model to identify defects on product surfaces using an industrial inspection dataset. Implement a one-class classification approach for detecting unseen defect types.

Reference: https://github.com/openvinotoolkit/anomalib

---

**Project 37: Pose Estimation for Exercise Tracking**

Use a human pose estimation model to analyze exercise form in video, count repetitions, and flag incorrect posture in real time.

Reference: https://github.com/CMU-Perceptual-Computing-Lab/openpose

---

**Project 38: Satellite Image Land Cover Classification**

Train a semantic segmentation model on satellite imagery to classify land cover types (urban, forest, water, farmland) using the EuroSAT or DeepGlobe dataset.

Reference: https://github.com/phelber/EuroSAT

---

**Project 39: 3D Object Detection from Point Clouds**

Implement a 3D object detection system using LiDAR point cloud data from the KITTI benchmark to detect vehicles and pedestrians for autonomous driving research.

Reference: https://github.com/open-mmlab/mmdetection3d

---

**Project 40: Visual Question Answering (VQA) System**

Build a VQA model that takes an image and a natural language question as input and produces a free-form text answer. Fine-tune on the VQA v2 dataset.

Reference: https://github.com/LAVIS-LM/LAVIS

---

## Domain 5: Generative AI and Large Language Models

Generative AI covers the development, fine-tuning, and evaluation of models that create text, code, and structured outputs.

**Core Resources**

- Hugging Face PEFT (Parameter-Efficient Fine-Tuning): https://github.com/huggingface/peft
- Axolotl Fine-Tuning Framework: https://github.com/OpenAccess-AI-Collective/axolotl
- LM Evaluation Harness: https://github.com/EleutherAI/lm-evaluation-harness
- Ollama Local LLM Runner: https://github.com/ollama/ollama

---

**Project 41: Domain-Specific LLM Fine-Tuning with LoRA**

Fine-tune an open-source LLM (Mistral, LLaMA 3, or Phi-3) on a domain-specific instruction dataset using LoRA adapters to reduce computational cost.

Reference: https://github.com/huggingface/peft/tree/main/examples/sequence_classification

---

**Project 42: Code Generation and Explanation Tool**

Build a developer assistant that generates boilerplate code from natural language specifications and explains existing code in plain English, using a code-specialized LLM.

Reference: https://github.com/bigcode-project/starcoder

---

**Project 43: LLM Benchmark Evaluation Suite**

Create an evaluation pipeline that tests an LLM across multiple benchmarks (MMLU, HellaSwag, TruthfulQA) and produces a comparative leaderboard.

Reference: https://github.com/EleutherAI/lm-evaluation-harness

---

**Project 44: Structured Output Generation with JSON Mode**

Build a pipeline that uses an LLM to reliably extract structured JSON data from unstructured text, using guided decoding or tool-calling to enforce schema constraints.

Reference: https://github.com/outlines-dev/outlines

---

**Project 45: Instruction Dataset Curation Pipeline**

Build an automated pipeline to generate, filter, and deduplicate instruction-tuning data from raw text corpora using Self-Instruct or Evol-Instruct methodologies.

Reference: https://github.com/tatsu-lab/stanford_alpaca

---

**Project 46: LLM-Powered Code Debugging Assistant**

Build a tool that takes buggy code as input, identifies the root cause of the error, suggests a fix, and explains the reasoning step by step using chain-of-thought prompting.

Reference: https://github.com/microsoft/PyDebugger

---

**Project 47: Retrieval-Augmented Code Generation**

Extend standard code generation with retrieval: the system searches a codebase index to find relevant function signatures and documentation before generating new code.

Reference: https://github.com/BerriAI/litellm

---

**Project 48: Prompt Injection Detection System**

Build a classifier that identifies adversarial prompt injection attempts in user inputs to an LLM-powered application and filters or flags malicious queries.

Reference: https://github.com/protectai/rebuff

---

**Project 49: Automated Report Generation System**

Build a system that accepts structured data (e.g., financial metrics, survey results) and uses an LLM to generate a polished narrative report with sections, headings, and insights.

Reference: https://github.com/langchain-ai/langchain/blob/master/cookbook/report_writing.ipynb

---

**Project 50: Continual Learning for LLMs**

Investigate and implement strategies for continually updating an LLM with new knowledge without catastrophic forgetting, using techniques such as elastic weight consolidation or replay buffers.

Reference: https://github.com/joeljang/continual-learning-for-language-models

---

## Domain 6: Speech and Audio AI

Speech AI enables machines to understand, generate, and analyze spoken language and sound.

**Core Resources**

- OpenAI Whisper: https://github.com/openai/whisper
- Coqui TTS: https://github.com/coqui-ai/TTS
- SpeechBrain Toolkit: https://github.com/speechbrain/speechbrain
- Kaldi ASR Framework: https://github.com/kaldi-asr/kaldi

---

**Project 51: Multilingual Speech Transcription Service**

Build a transcription API using OpenAI Whisper that automatically detects language, transcribes audio, adds punctuation, and outputs SRT subtitle files.

Reference: https://github.com/openai/whisper

---

**Project 52: Speaker Diarization System**

Build a pipeline that identifies and separates different speakers in a multi-speaker audio recording, outputting a timestamped transcript labelled by speaker.

Reference: https://github.com/pyannote/pyannote-audio

---

**Project 53: Custom Voice Cloning System**

Implement a voice cloning system that takes a short audio sample of a target speaker and synthesizes new speech in their voice from text input.

Reference: https://github.com/coqui-ai/TTS/tree/dev/recipes/ljspeech

---

**Project 54: Real-Time Speech Emotion Recognition**

Build a model that classifies the emotional tone of speech (anger, happiness, sadness, neutral) from audio features in real time using a streaming audio pipeline.

Reference: https://github.com/speechbrain/speechbrain/tree/develop/recipes/IEMOCAP

---

**Project 55: Keyword Spotting for Edge Devices**

Train a lightweight keyword spotting model (using the Google Speech Commands dataset) optimized for deployment on microcontrollers or embedded devices with TFLite.

Reference: https://github.com/ARM-software/ML-KWS-for-MCU

---

**Project 56: Audio Deepfake Detection**

Build a classifier that distinguishes between genuine human speech and synthetic or manipulated audio generated by TTS models, using the ASVspoof dataset.

Reference: https://github.com/asvspoof-challenge/2021

---

**Project 57: Meeting Transcription and Summarization Pipeline**

Build an end-to-end pipeline that transcribes a meeting recording, diarizes speakers, and produces an action-item summary using an LLM.

Reference: https://github.com/openai/whisper/discussions

---

**Project 58: Music Genre Classification**

Train a convolutional neural network on mel-spectrograms extracted from audio clips to classify music into genres, using the GTZAN dataset.

Reference: https://github.com/Hguimaraes/gtzan.keras

---

**Project 59: Audio Source Separation**

Build a system that separates vocals, drums, bass, and other instruments from a mixed music track using a deep learning source separation model.

Reference: https://github.com/facebookresearch/demucs

---

**Project 60: Spoken Language Understanding (SLU) System**

Build an end-to-end SLU system that combines ASR and NLU to directly classify the intent and extract entities from spoken utterances without intermediate text.

Reference: https://github.com/speechbrain/speechbrain/tree/develop/recipes/SLURP

---

## Domain 7: Reinforcement Learning

Reinforcement learning trains agents to make sequential decisions by maximizing cumulative reward through environment interaction.

**Core Resources**

- Stable-Baselines3: https://github.com/DLR-RM/stable-baselines3
- RLlib by Ray: https://github.com/ray-project/ray/tree/master/rllib
- OpenAI Gymnasium: https://github.com/Farama-Foundation/Gymnasium
- CleanRL: https://github.com/vwxyzjn/cleanrl

---

**Project 61: Deep Q-Network (DQN) for Atari Games**

Implement DQN from scratch and train it on classic Atari games (Pong, Breakout). Reproduce key results from the original DeepMind paper and analyze learning curves.

Reference: https://github.com/vwxyzjn/cleanrl/blob/master/cleanrl/dqn_atari.py

---

**Project 62: Proximal Policy Optimization (PPO) for Continuous Control**

Implement PPO and train it on a continuous control benchmark (MuJoCo HalfCheetah or Ant) to learn smooth locomotion policies.

Reference: https://github.com/vwxyzjn/cleanrl/blob/master/cleanrl/ppo_continuous_action.py

---

**Project 63: Multi-Agent Competitive Environment**

Build a multi-agent competitive game (e.g., a simplified soccer or capture-the-flag environment) and train agents using self-play to produce emergent competitive strategies.

Reference: https://github.com/Farama-Foundation/PettingZoo

---

**Project 64: RL for Stock Trading**

Train an RL agent to make buy, sell, and hold decisions in a simulated stock market environment. Benchmark it against baseline strategies such as buy-and-hold.

Reference: https://github.com/AI4Finance-Foundation/FinRL

---

**Project 65: Curriculum Learning for RL Agents**

Implement curriculum learning by progressively increasing task difficulty during training. Compare sample efficiency and final performance against standard uniform training.

Reference: https://github.com/DLR-RM/stable-baselines3/blob/master/docs/guide/examples.rst

---

**Project 66: Offline Reinforcement Learning**

Train an RL agent from a static logged dataset without any environment interaction, using offline RL algorithms such as Conservative Q-Learning (CQL) or IQL.

Reference: https://github.com/takuseno/d3rlpy

---

**Project 67: Reward Shaping and Intrinsic Motivation**

Implement curiosity-driven exploration by adding an intrinsic reward signal based on prediction error of a world model, applied to a sparse-reward navigation task.

Reference: https://github.com/pathak22/noreward-rl

---

**Project 68: Robotic Arm Manipulation with Sim-to-Real Transfer**

Train a robotic manipulation policy in simulation (using Isaac Gym or MuJoCo) and implement domain randomization techniques to enable transfer to a physical robot.

Reference: https://github.com/NVIDIA-Omniverse/IsaacGymEnvs

---

**Project 69: RLHF Pipeline for LLM Alignment**

Implement a simplified Reinforcement Learning from Human Feedback (RLHF) pipeline: train a reward model from preference data, then fine-tune an LLM using PPO.

Reference: https://github.com/CarperAI/trlx

---

**Project 70: Hierarchical Reinforcement Learning**

Implement a two-level hierarchical RL architecture: a high-level manager sets subgoals while a low-level worker executes primitive actions to achieve them.

Reference: https://github.com/tensorflow/agents/tree/master/tf_agents/agents/ddpg

---

## Domain 8: MLOps and AI Infrastructure

MLOps covers the practices, tools, and systems required to deploy, monitor, and maintain machine learning models in production.

**Core Resources**

- MLflow Experiment Tracking: https://github.com/mlflow/mlflow
- Weights and Biases: https://github.com/wandb/wandb
- BentoML Model Serving: https://github.com/bentoml/BentoML
- Kubeflow Pipelines: https://github.com/kubeflow/pipelines

---

**Project 71: Automated ML Pipeline with MLflow**

Build an end-to-end ML pipeline that tracks experiments, logs metrics and artifacts, compares model versions, and registers the best-performing model to the MLflow Model Registry.

Reference: https://github.com/mlflow/mlflow/tree/master/examples

---

**Project 72: Model Serving API with BentoML**

Package a trained machine learning model as a production-ready REST API using BentoML, including input validation, batching support, and Docker containerization.

Reference: https://github.com/bentoml/BentoML/tree/main/examples

---

**Project 73: Data and Model Versioning with DVC**

Set up a data version control system using DVC that tracks dataset changes alongside model checkpoints, enabling reproducible experiment reproduction.

Reference: https://github.com/iterative/dvc

---

**Project 74: Real-Time Model Monitoring Dashboard**

Build a monitoring system that detects data drift and model performance degradation in production using statistical tests and alerts, visualized in a Grafana dashboard.

Reference: https://github.com/evidentlyai/evidently

---

**Project 75: Feature Store Implementation**

Design and implement a lightweight feature store that computes, stores, and serves ML features consistently between training and inference to eliminate training-serving skew.

Reference: https://github.com/feast-dev/feast

---

**Project 76: Automated Hyperparameter Optimization**

Implement a hyperparameter optimization service using Optuna or Ray Tune that automatically searches for optimal model configurations using Bayesian optimization.

Reference: https://github.com/optuna/optuna

---

**Project 77: CI/CD Pipeline for Machine Learning**

Build a complete CI/CD pipeline for an ML project using GitHub Actions: automated testing, model training, evaluation gating, and deployment to a staging environment.

Reference: https://github.com/iterative/cml

---

**Project 78: Model Compression and Quantization**

Apply post-training quantization (INT8) and pruning techniques to a large vision or language model to reduce inference latency by 2-4x with minimal accuracy loss.

Reference: https://github.com/intel/neural-compressor

---

**Project 79: Distributed Training with PyTorch DDP**

Implement distributed data-parallel training across multiple GPUs for a large image classification model and measure linear scaling efficiency.

Reference: https://github.com/pytorch/examples/tree/main/distributed/ddp-tutorial-series

---

**Project 80: LLM Inference Optimization with vLLM**

Deploy a large language model with vLLM's PagedAttention-based serving system and benchmark throughput and latency improvements over naive Hugging Face inference.

Reference: https://github.com/vllm-project/vllm

---

## Domain 9: AI for Healthcare and Science

AI is transforming scientific discovery and healthcare by accelerating drug discovery, diagnosing disease, and modeling complex natural phenomena.

**Core Resources**

- DeepMind AlphaFold: https://github.com/google-deepmind/alphafold
- MONAI Medical Imaging Framework: https://github.com/Project-MONAI/MONAI
- RDKit Cheminformatics: https://github.com/rdkit/rdkit
- BioNeMo by NVIDIA: https://github.com/NVIDIA/BioNeMo

---

**Project 81: Chest X-Ray Disease Classification**

Train a convolutional neural network on the NIH ChestX-ray14 dataset to classify 14 thoracic pathologies from frontal chest radiographs and generate Grad-CAM visualizations.

Reference: https://github.com/jrzech/reproduce-chexnet

---

**Project 82: Protein Structure Prediction**

Use AlphaFold2 or ESMFold to predict the 3D structure of a custom protein sequence and analyze the predicted structure against experimentally determined structures in the PDB.

Reference: https://github.com/google-deepmind/alphafold

---

**Project 83: Drug-Target Interaction Prediction**

Build a graph neural network that predicts the binding affinity between drug molecules and protein targets, using the BindingDB or KIBA benchmark dataset.

Reference: https://github.com/thinng/GraphDTA

---

**Project 84: Clinical Note Summarization**

Fine-tune a biomedical language model (BioGPT or ClinicalBERT) on clinical notes to generate concise, accurate discharge summaries for electronic health record systems.

Reference: https://github.com/EmilyAlsentzer/clinicalBERT

---

**Project 85: Genomic Sequence Classification**

Train a transformer model on DNA sequences to classify functional genomic elements (promoters, enhancers, splice sites) using the ENCODE or GENCODE dataset.

Reference: https://github.com/lucidrains/enformer-pytorch

---

**Project 86: Epidemic Spread Forecasting**

Build a hybrid model combining epidemiological compartmental models (SIR/SEIR) with neural networks to forecast disease spread from real-world case data.

Reference: https://github.com/CSSEGISandData/COVID-19

---

**Project 87: Pathology Slide Tumor Detection**

Train a multiple-instance learning model to classify whole-slide pathology images for cancer detection, handling the gigapixel resolution challenge through patch-based processing.

Reference: https://github.com/mahmoodlab/CLAM

---

**Project 88: Molecular Generation with Graph Neural Networks**

Build a generative model (using a variational autoencoder or flow model) that designs novel drug-like molecules with targeted chemical properties using the ZINC dataset.

Reference: https://github.com/bowenliu16/rl_graph_generation

---

**Project 89: Medical Report Generation from Images**

Train a multimodal model that generates structured radiology reports from chest X-ray images, combining a vision encoder with a language decoder.

Reference: https://github.com/cuhksz-nlp/R2Gen

---

**Project 90: Mental Health Signal Detection in Social Media**

Build an NLP classifier that identifies signals of depression, anxiety, or crisis in social media posts, with careful attention to ethical considerations and bias mitigation.

Reference: https://github.com/kharrigian/mental-health-datasets

---

## Domain 10: Multimodal AI Systems

Multimodal systems combine information from multiple modalities (text, image, audio, video) to perform tasks that require cross-modal understanding.

**Core Resources**

- OpenAI CLIP: https://github.com/openai/CLIP
- LLaVA Visual Instruction Tuning: https://github.com/haotian-liu/LLaVA
- BLIP-2 by Salesforce: https://github.com/salesforce/LAVIS
- ImageBind by Meta AI: https://github.com/facebookresearch/ImageBind

---

**Project 91: Zero-Shot Image Classification with CLIP**

Use OpenAI CLIP to build a zero-shot image classification system that classifies images into arbitrary categories defined by natural language descriptions, with no task-specific training.

Reference: https://github.com/openai/CLIP

---

**Project 92: Multimodal Retrieval System**

Build a cross-modal search engine where users can query using an image to retrieve semantically similar text passages, or query with text to retrieve matching images.

Reference: https://github.com/rom1504/clip-retrieval

---

**Project 93: Visual Instruction Following Agent**

Fine-tune LLaVA or a similar vision-language model on a custom visual instruction dataset to follow complex commands involving image understanding and reasoning.

Reference: https://github.com/haotian-liu/LLaVA

---

**Project 94: Video Question Answering System**

Build a system that answers natural language questions about video content by extracting key frames, captioning them, and using an LLM to reason over the temporal narrative.

Reference: https://github.com/MILVLG/singularity

---

**Project 95: Multimodal Fake News Detection**

Build a classifier that identifies fake news by jointly modeling the credibility of the textual claim and the consistency of accompanying images, using the FakeNewsNet dataset.

Reference: https://github.com/KaiDMML/FakeNewsNet

---

**Project 96: Text-Guided Image Editing**

Build an application that edits specific regions of an image based on natural language instructions, using diffusion-based inpainting models combined with CLIP guidance.

Reference: https://github.com/timothybrooks/instruct-pix2pix

---

**Project 97: Multimodal Sentiment Analysis**

Build a sentiment classifier that fuses acoustic features from speech, facial expressions from video, and transcribed text to predict the overall sentiment of a spoken utterance.

Reference: https://github.com/declare-lab/multimodal-sentiment-analysis

---

**Project 98: Audio-Visual Speech Recognition**

Build an automatic speech recognition system that incorporates lip movement video as an additional input signal to improve accuracy in noisy acoustic environments.

Reference: https://github.com/mpc001/auto_avsr

---

**Project 99: Image Captioning with Transformer Architecture**

Build an end-to-end image captioning system using a CNN image encoder and a transformer decoder. Fine-tune and evaluate on the COCO Captions benchmark.

Reference: https://github.com/ruotianluo/ImageCaptioning.pytorch

---

**Project 100: Multimodal AI Tutoring System**

Design an intelligent tutoring assistant that accepts diagrams, handwritten equations, and natural language questions from students, provides step-by-step explanations, and adapts to the learner's level.

Reference: https://github.com/microsoft/guidance

---

## General Learning Resources

The following curated resources are recommended regardless of domain:

- Papers With Code (State-of-the-Art Benchmarks): https://paperswithcode.com
- Hugging Face Hub (Models and Datasets): https://huggingface.co
- ArXiv AI Preprints: https://arxiv.org/list/cs.AI/recent
- Deep Learning Textbook (Goodfellow et al.): https://www.deeplearningbook.org
- fast.ai Practical Deep Learning: https://course.fast.ai
- Stanford CS229 Machine Learning: https://cs229.stanford.edu
- Full Stack Deep Learning: https://fullstackdeeplearning.com
- Andrej Karpathy's Neural Networks from Scratch: https://github.com/karpathy/nn-zero-to-hero

---

## Contribution Guidelines

If you would like to contribute a new project idea or update an existing reference link, please open a pull request with the following information:

1. Domain assignment and project title
2. A clear two-to-three sentence description
3. A valid, publicly accessible reference link
4. Estimated difficulty level: Beginner, Intermediate, or Advanced

---

## License

This repository is released under the MIT License. All referenced external repositories and papers are subject to their own respective licenses. Please review each license before use in commercial applications.

---

*Maintained by a community of AI researchers and educators. Last reviewed: 2025.*

---

## Author

Created by **Sriram Sowmithri**
