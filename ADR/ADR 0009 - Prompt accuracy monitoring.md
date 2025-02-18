# 0009 Prompt accuracy monitoring

## Context

We use multiple prompts to increase the accuracy of AI-assisted assessment of each test question answer. Since a poorly defined prompt may significantly affect our results, it is crucial to monitor them as well. If a given prompt frequently gives low confidence, it should be rephrased.

## Decision

We will implement a monitoring system for prompt accuracy. This system will track the confidence levels of AI responses for each prompt version. If the average confidence for a prompt falls below a certain threshold, the prompt will be flagged for review by moderators and administrators. 

## Justification

This will ensure that prompts are continuously optimized to maintain high accuracy in AI-assisted assessments.

## Consequences

1. **Improved Accuracy**: Ensures that AI-assisted assessments are based on well-defined and effective prompts.
2. **Resource Allocation**: Moderators and administrators will need to allocate time to review and rephrase flagged prompts.
3. **Data-Driven Decisions**: Provides data-driven insights into prompt performance, helping to make informed decisions about prompt modifications.
4. **Scalability**: The monitoring system can handle a large number of prompts, making it scalable as the number of test questions and prompts increases.

By implementing this feature, we aim to enhance the accuracy and reliability of our AI-assisted assessments through continuous monitoring and optimization of prompts.
