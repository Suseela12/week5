# Experiment 5: Zero-Shot vs Few-Shot Prompting

## Aim
To compare zero-shot and few-shot prompting techniques for sentiment classification of customer reviews.

## Problem Statement
Classify five customer reviews into Positive, Neutral, or Negative categories using zero-shot and few-shot prompts. Compare their predictions with the known labels.

## Technologies Used
- Python
- Google Gemini AI
- Google Gen AI SDK
- Pandas

## Prompting Techniques

### Zero-Shot Prompting
The model classifies a review without being given classification examples.

### Few-Shot Prompting
The model receives three labelled examples before classifying each test review.

## Algorithm
1. Define five test reviews and their ground-truth labels.
2. Create a zero-shot prompt.
3. Create a few-shot prompt with three examples.
4. Use the same model and temperature for both methods.
5. Generate predictions for every review.
6. Compare predictions with ground-truth labels.
7. Calculate accuracy and agreement between the methods.
8. Save the comparison table as a CSV file.

## Installation

```bash
pip install -r requirements.txt
```

## Configuration
Set the `GEMINI_API_KEY` environment variable before running the program. Never upload API keys to GitHub.

## Execution

```bash
python src/main.py
```

## Expected Output
- Review and ground-truth labels.
- Zero-shot and few-shot predictions.
- Correctness of each prediction.
- Accuracy of both methods.
- Agreement percentage.
- CSV results saved to `output/sentiment_results.csv`.

## Result
The experiment compares the classification performance of zero-shot and few-shot prompting on the same test dataset.

## Conclusion
Zero-shot prompting relies on instructions alone, while few-shot prompting provides labelled examples to guide classification. Few-shot prompting may improve consistency and accuracy, but its effectiveness must be verified using the actual results.


