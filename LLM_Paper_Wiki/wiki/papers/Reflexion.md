# Reflexion: Language Agents with Verbal Reinforcement Learning
- Authors: Noah Shinn et al.
- Year: 2023
- Source: https://arxiv.org/abs/2303.11366

## Problem
Agent outcomes may improve if experience and feedback are used to guide subsequent attempts, without updating model weights each time.

## Approach
Reflexion uses feedback and verbal self-reflection, storing reflections in an episodic memory buffer that can inform future trials.

## Key idea
`Attempt → Feedback → Reflection → Memory → Next attempt` is a loop for learning from trial outcomes at inference time.

## Limitations / cautions
Reflection quality depends on feedback and memory context. Reflection text alone does not guarantee better outcomes; inspect experimental conditions in the full paper.

## Links
- [[../concepts/Reflection]]
- [[../concepts/LLM Agent]]
