# 0002 Selected models for AI-assisted grading

## Context

Following the decision to use AI in ADR 0001, we need to select which models/services to use. The requirements we have are:
1. The AI needs to be able to grade answers as correct/incorrect, as well as give points in the range of 1-10.
2. The AI needs to be able to respond to a question "on a scale of 1 to 100, how certain are you that your grade is correct?".

## Decision

For the initial release, we will use ChatGPT 4, Gemini 1.5 Pro and Claude 3.5 Sonnet.

## Consequences

The selected models fulfill the requirements and as a bonus, they are considered as the leading LLMs in the market.
All of them have a subscription service and are widely available.
