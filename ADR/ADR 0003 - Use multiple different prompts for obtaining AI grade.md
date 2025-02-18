# 0003 Use multiple prompts for obtaining AI grade

# Context

The current LLM's suffer from hallucinations, which means that the responses we get from them cannot be treated as 100% correct.
In order to preserve credibility of our certificates, we need to develop strategies that will help to mitigate that risk. 

# Decision

We will send multiple prompts to the same LLM and verify that the response is coherent despite the prompt being different.
The final result will be an average of all results.

# Consequences

By sending multiple prompts to the LLM, we're increasing the cost of the service. This increase may either be visible
by literally a bigger amount on the invoice, or by reaching the monthly token limit faster.

# Technique Description

1. **Multiple Prompt Generation**: For each question, generate multiple variations of the prompt to be sent to the LLM.
2. **Response Collection**: Send each prompt variation to the LLM and collect the responses.
3. **Coherence Verification**: Compare the responses to ensure they are coherent and consistent. If the responses are not consistent, flag the question for human review.
4. **Final Grading**: Use the consistent responses to determine the final grade for the question.
