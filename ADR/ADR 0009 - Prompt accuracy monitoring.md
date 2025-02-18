# 0009 Prompt Accuracy Monitoring

## Context

We use multiple prompts to increase the accuracy of AI-assisted assessment of each test question answer. Since a poorly defined prompt may significantly affect our results, it is crucial to monitor them as well. If a given prompt frequently gives low confidence, it should be rephrased.

## Decision

We will implement a monitoring system for prompt accuracy. This system will track the confidence levels of AI responses for each prompt version. If the average confidence for a prompt falls below a certain threshold, the prompt will be flagged for review by moderators and administrators. This will ensure that prompts are continuously optimized to maintain high accuracy in AI-assisted assessments.

## Justification

1. **Accuracy**: Monitoring and optimizing prompts will help maintain high accuracy in AI-assisted assessments.
2. **Quality Control**: Regularly reviewing and rephrasing low-confidence prompts will ensure the quality and reliability of the AI assessments.
3. **Efficiency**: Automating the monitoring process will save time and resources, allowing human reviewers to focus on more complex tasks.
4. **Continuous Improvement**: By tracking and analyzing prompt performance, we can continuously improve the effectiveness of our AI-assisted assessments.

## Consequences

1. **Improved Accuracy**: Ensures that AI-assisted assessments are based on well-defined and effective prompts.
2. **Resource Allocation**: Moderators and administrators will need to allocate time to review and rephrase flagged prompts.
3. **Data-Driven Decisions**: Provides data-driven insights into prompt performance, helping to make informed decisions about prompt modifications.
4. **Scalability**: The monitoring system can handle a large number of prompts, making it scalable as the number of test questions and prompts increases.

By implementing this feature, we aim to enhance the accuracy and reliability of our AI-assisted assessments through continuous monitoring and optimization of prompts.
