# Take-Home Final Exam for CENG442: Text Summarization Using Seq2Seq Models

## Topic:
Developing a Text Summarization System for News Articles Using Seq2Seq Models with TensorFlow

---

## Objective:
Students will implement a Seq2Seq model with attention for summarizing news articles. The project will involve dataset preparation, model development, evaluation, and submission of a report, code, and a short video presentation.
The dataset: https://drive.google.com/file/d/1SgsCORTz5seRiuBLQefmr-MNeH9SuN7s/view?usp=sharing

---

## Instructions:

### Dataset:
- You will be provided with a dataset in Parquet format containing news articles and their summaries.
- **Reading the Dataset:** Use the following code snippet to load the dataset:
    ```python
    import pandas as pd

    # Read the Parquet file
    df = pd.read_parquet('file_path.parquet')

    # Display the DataFrame
    print(df)
    ```
- Split the dataset into training, validation, and testing sets. Suggested split: 80% training, 10% validation, 10% testing.

---

### Tasks:

#### 1. Preprocessing:
- Tokenize the text data and convert it to sequences using TensorFlow/Keras Tokenizer.
- Pad or truncate sequences to ensure uniform input length.
- Handle special tokens (e.g., start-of-sequence `<sos>` and end-of-sequence `<eos>`).

#### 2. Model Development:
- Build a Seq2Seq model in TensorFlow with the following components:
  - Encoder (RNN/LSTM/GRU).
  - Decoder with attention mechanism.
  - Attention layer to enhance summary quality.

#### 3. Training:
- Train the model on the training set, monitor performance using the validation set, and adjust hyperparameters as necessary.

#### 4. Evaluation:
- Use the test set to generate summaries.
- Evaluate the generated summaries using the ROUGE metric.

#### 5. Analysis:
- Compare generated summaries to reference summaries and discuss performance.
- Suggest potential improvements or extensions for better results.

---

### Deliverables:

#### README File:
A text file containing:
- The names of the group members (maximum 2 students per group).
- Links to:
  1. The project report.
  2. The project files (Python code).
  3. The YouTube video presentation (uploaded as unlisted).

#### Project Report:
- Detailed documentation of the dataset, methodology, experiments, evaluation, and analysis of results.

#### Python Code:
- Include well-documented Python code for preprocessing, model development, and evaluation.

#### Video Presentation:
- A short video (5–10 minutes) explaining the project approach, implementation, and findings, uploaded to YouTube as unlisted.

---

### Submission Guidelines:
- Submit a zipped folder containing the README file, project report, and code.
- Ensure all links are working and accessible before submission.

---

### Group Policy:
- Students may work in groups of up to 2 members.
- All group members must contribute equally and include their names in the README file.

---

## Grading Criteria:
1. **Model Implementation (40%)**
   - Proper use of Seq2Seq architecture and attention mechanism.
2. **Evaluation and Analysis (30%)**
   - Quality of summaries and interpretation of results using ROUGE metrics.
3. **Code Quality and Documentation (20%)**
   - Clean, well-documented, and organized code.
4. **Presentation (10%)**
   - Clarity and quality of the video presentation.
   - If a YouTube presentation is not submitted, it will result in a grade of 0.

---

## Learning Outcomes:
- Implement Seq2Seq models in TensorFlow for text summarization.
- Understand attention mechanisms and their role in improving performance.
- Evaluate summarization models using established metrics.
- Develop teamwork and communication skills through collaborative project work.
