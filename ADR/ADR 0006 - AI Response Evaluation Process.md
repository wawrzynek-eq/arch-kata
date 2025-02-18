# 0006 AI response evaluation process

## Context

To ensure the accuracy and reliability of AI-assisted grading, it is essential to have a robust process for evaluating AI responses. This process should include mechanisms for assessing the confidence levels of AI responses and incorporating human confirmation when necessary.

## Decision

We will establish a comprehensive AI response evaluation process that includes the following steps:

## Technique Description

1. **Confidence Level Assessment**: Each AI response will be accompanied by a confidence level indicating the AI's certainty in its answer.
2. **Threshold Determination**: A confidence threshold will be set to determine when human confirmation is required. Responses below this threshold will be flagged for human review.
3. **Human Confirmation**: For responses that fall below the confidence threshold, a human evaluator will review and confirm the AI's grading. This step ensures that low-confidence responses are accurately assessed and at the same time reduces the amount of work required from a human.
4. **Feedback Loop**: The results of human confirmation will be fed into the AI statistic db (see [ADR 0005](ADR%200005%20-%20Use%20RAG.md)) to improve its future performance. This feedback loop will help the AI to increase its accuracy over time.

By following this process, we can ensure that AI-assisted grading is both accurate and reliable, with a mechanism in place to handle low-confidence responses effectively.

## Consequences

Implementing this AI response evaluation process will enhance the reliability and accuracy of AI-aided grading. By incorporating confidence levels and human confirmation, we can reduce the likelihood of incorrect grades and ensure that low-confidence responses are properly evaluated.
