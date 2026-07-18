# Experiment Summary

## Main reproduction result

The SST-2 LoRA experiment with RoBERTa-base achieved 95.07% validation
accuracy, compared with 95.1% reported in the LoRA paper.

## Additional GLUE results

| Task | Metric | Result | Best epoch |
|---|---:|---:|---:|
| CoLA | MCC | 0.6132 | 7 |
| MRPC | Accuracy | 0.8676 | 10 |
| MRPC | F1 | 0.9046 | 10 |
| RTE | Accuracy | 0.7437 | 9 |
| STS-B | Pearson | 0.9088 | 7 |

## WebNLG extension

Qwen2.5-7B-Instruct was adapted using 4-bit NF4 QLoRA.

- Training steps: 1,000
- Training loss: 0.5375
- Validation loss: 0.4986
- BLEU: 46.66
- chrF: 75.37

## Iterative process

The project included model-size testing, environment debugging,
forward and backward validation, a pilot experiment, final training,
learning-curve analysis, and task-specific evaluation.

## Limitations

DART was not completed and is listed as future work. A complete
hyperparameter grid search was not performed.
