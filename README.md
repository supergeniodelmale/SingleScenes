# 🎬 SingleScenes: A Simple Benchmark for LLM Film Script Understanding and Generation

Welcome to the **SingleScenes** repository! This dataset is designed to serve as a simple benchmark for evaluating the capabilities of Large Language Models (LLMs) in film script generation and understanding. **SingleScenes** consists of a collection of **film script scenes** partitioned from film scripts from The Internet Movie Script Database paired with their corresponding **summaries**, offering a structured framework for training and testing LLMs on both script comprehension and generative tasks.

## 🏆 Leaderboard

We encourage you to participate in the **SingleScenes** benchmarking challenge! To help the community track progress, we have created a **leaderboard** where the results of different LLMs will be displayed based on their performance in **single scene generation** task.

1. **Run the Benchmark**: Evaluate your model using the dataset according to the provided evaluation metrics.
2. **Submit Your Results**: Share your model/approach and results by posting a comment in the [Leaderboard Issues](https://github.com/yourusername/SingleScenes/issues).
3. **Confirmation & Pubblication**: Wait for our independent test with your model/method and check the leaderboard for updates!

### **Eternal Sunshine of the Spotless Mind** Leaderboard:

| Rank | Model/TMethod      | Single Scene Generation (Mistral Instruct) |
|------|--------------------|--------------------------------------------|
| 1    | Mistral Instruct   | TBA                                        |
| 2    | GPT-4o             | TBA                                        |

### **Inception** Leaderboard:

| Rank | Model/TMethod      | Single Scene Generation (Mistral Instruct) |
|------|--------------------|--------------------------------------------|
| 1    | Mistral Instruct   | TBA                                        |
| 2    | GPT-4o             | TBA                                        |

### **The Shawshank Redemption** Leaderboard:

| Rank | Model/TMethod      | Single Scene Generation (Mistral Instruct) |
|------|--------------------|--------------------------------------------|
| 1    | Mistral Instruct   | TBA                                        |
| 2    | GPT-4o             | TBA                                        |

## 📏 Metrics

### 🎭 Single Scene Generation: Pairwise Comparison Scoring

To evaluate the quality of model-generated scenes, we use a **pairwise comparison system** where the generated scene competes directly against the **original film scene**. Here’s how it works:

1. **Pairwise Comparison**:
   - For each scene summary in the dataset:
     - The model generates a corresponding scene script.
     - The generated script is compared against the **original film scene script** (considered the gold standard).
   - An external critic—either a human evaluator or an LLM—decides which script is **better**.

2. **Evaluation Criteria**:
   - The external critic evaluates the scripts based on:
     - **Narrative Coherence** 🧩: Does the scene flow as a cohesive and logical story?
     - **Fidelity to the Summary** 🎯: Does the scene align with the key elements of the provided summary?
     - **Dialogue and Action Realism** 🗨️: Are the characters' interactions and actions believable?
     - **Cinematic Quality** 🎥: Does the scene feel polished and professional?
   - The decision is holistic: The critic chooses the script that best balances these aspects without assigning individual scores.

3. **Scoring**:
   - **1 Point** is awarded to the method (original or generated) deemed **better** in each pairwise comparison.
   - No points are awarded for ties.

4. **Dataset-Wide Evaluation**:
   - This process is repeated for all scene summaries in the dataset.
   - The total points accumulated by the generated scenes are summed up and compared against the total points for the original scenes.
   - This results in a **percentage score** for the model, representing the proportion of comparisons where the generated scenes were preferred.

5. **Performance Interpretation**:
   - **Higher Scores**: Indicate that the generated scenes are frequently preferred over the original film scenes.
   - **Lower Scores**: Suggest that the generated scenes rarely match the quality of the original film scenes.


## 📚 Features

- **Film Script Scenes**: Each entry includes a detailed scene from a film script, featuring dialogue, action descriptions, and other narrative elements.
- **Summaries**: Every scene is paired with a concise summary, capturing the key points and thematic essence of the scene.

## ⚙️ Usage

This dataset can be used for:

- **Benchmarking**: Evaluate the performance of LLMs in script comprehension, scene generation, and summarization tasks 📊.
- **Research**: Conduct studies into how LLMs understand and generate narratives in a screenplay context 🔬.

## 🚫 Disclaimer

Please note that the **SingleScenes** dataset **cannot** be used for **fine-tuning** Large Language Models as it contains copyrighted material. The dataset is provided strictly for **benchmarking**, **evaluation**, and **research purposes**. Any usage beyond these purposes, including training or fine-tuning models, is prohibited.



