# Voyager: An Open-Ended Embodied Agent with Large Language Models
- Authors: Guanzhi Wang et al.
- Year: 2023
- Source: https://arxiv.org/abs/2305.16291

## Problem
An embodied agent in an open-ended environment needs to explore, acquire skills, and use them across tasks over time.

## Approach
Voyager uses an automatic curriculum, an execution feedback loop, and a skill library in the Minecraft environment, with LLM-driven planning and code generation.

## Key idea
Skills can be accumulated as reusable programs; exploration and feedback can drive progressively more complex behavior in an open-ended environment.

## Limitations / cautions
The demonstrated environment is Minecraft; results should not be assumed to transfer directly to other environments. Verify implementation details in the paper.

## Links
- [[../concepts/Agent Environment]]
- [[../concepts/Reflection]]
- [[../concepts/LLM Agent]]
