# ReAct: Synergizing Reasoning and Acting in Language Models
- Authors: Shunyu Yao et al.
- Year: 2022 (arXiv preprint; later conference publication)
- Source: https://arxiv.org/abs/2210.03629

## Problem
Language models may reason in text but lack a grounded way to interact with external environments; action-only approaches can also lack explicit reasoning traces.

## Approach
ReAct interleaves reasoning traces and actions. The model generates thoughts that guide actions, receives observations from the environment, and continues the loop.

## Key idea
`Thought → Action → Observation → ...` provides a structured interaction pattern. The reasoning text helps guide action selection while observations ground subsequent steps.

## Limitations / cautions
Reasoning traces are not necessarily faithful explanations. Performance depends on task, tools, prompts, and environment. This note is a preliminary summary; verify details in the full paper.

## Links
- [[../concepts/Reasoning and Acting]]
- [[../concepts/Tool Use]]
- [[../concepts/LLM Agent]]
