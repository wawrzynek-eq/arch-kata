# 0003 Use multiple prompts for obtaining AI grade

# Context

The current LLM's suffer from hallucinations, which means that the responses we get from them cannot be treated as 100% correct.
In order to preserve credibility of our certificates, we need to develop strategies that will help to mitigate that risk. 

# Decision

We will send multiple prompts to the same LLM and verify that the response is coherent despite the prompt being different.

# Consequences

By sending multiple prompts to the LLM, we're increasing the cost of the service. This increase may either be visible
by literally a bigger amount on the invoice, or by reaching the monthly token limit faster.
