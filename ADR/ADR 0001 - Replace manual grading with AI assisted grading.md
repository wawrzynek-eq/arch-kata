# 0001 Replace manual grading with AI assisted grading

# Context

There is an expected raise in the demand for architect certification. The forcasted numbers show that our current capability will soon be exhausted.
This lead us to explore the possibilities of utilizing LLM services for the purpose of shortening the required time to grade an exam.

# Decision

We will extend the current manual grading step in both "Test 1" and "Test 2" scenarios. The system will still rely on human interaction to accept or review the score suggested by AI.
Because of the fact, that LLM's do not produce 100% accurate results, we will use strategies that will reduce the chance of a test being graded incorrectly.
The solution will work in the following manner:

![AI assisted grading](ADR001-ai-assisted-grading.png "AI assisted grading")

# Consequences

With the aid of AI, we are going to signifficantly limit the time needed to grade both tests.
We are purposely leaving human actions as required, because for the moment, the results of AI interaction have a significant uncertainty factor
and due to the nature of our business we want to make sure, that the decision about granting or denying a certificate will be just and adhere to any laws on the subject.  
