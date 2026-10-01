# DataSage research preview

DataSage is an evaluation-in-progress approach for improving the reliability and
efficiency of data-analysis agents. This document describes the research direction;
it does not report or claim a validated DataAgentBench score.

## Research hypothesis

We are studying a combination of three general mechanisms:

1. **Ontology constraints** to keep planning, entity selection, joins, metrics, and
   answer construction consistent with the structure and semantics of the available
   data.
2. **Deterministic function tools** for operations that can be executed and checked
   directly, reducing unnecessary model calls and making intermediate computations
   reproducible.
3. **Jev model-based classification** to route rows and subtasks between deterministic
   local processing and model-assisted semantic processing.

Our hypothesis is that this combination can improve both analysis accuracy and
runtime efficiency. The hypothesis remains under evaluation and is not presented as
an established benchmark result.

## Evaluation and submission plan

Before requesting leaderboard review, we plan to:

- freeze the evaluated agent and model configuration;
- run all DataAgentBench queries five times, for 270 independent trials in total;
- retain a matching execution trace for every submitted answer;
- use only the benchmark-sanctioned data sources and prompt inputs;
- disclose the backbone model version, hint usage, and relevant runtime settings; and
- submit the results JSON and execution traces required by the repository rubric.

## Current status

Evaluation is in progress. No leaderboard placement or Pass@1 score is requested in
this draft. We will provide the complete score-bearing artifacts after the evaluation
and trace review are complete.
