# Toolformer: Language Models Can Teach Themselves to Use Tools
- Authors: Timo Schick et al.
- Year: 2023
- Source: https://arxiv.org/abs/2302.04761

## Problem
A language model may benefit from external tools (e.g., calculator, search, translation), but tool calls need to be learned and selectively used.

## Approach
Toolformer describes a self-supervised process for teaching a model to insert API calls into text and retain calls that improve prediction outcomes, using a small number of demonstrations to specify APIs.

## Key idea
Tool-use decisions can be learned from data and utility signals rather than relying solely on manually written tool-call examples.

## Limitations / cautions
Results and applicability depend on the available APIs and training setup. Do not generalize beyond evaluated tasks without checking the paper.

## Links
- [[../concepts/Tool Use]]
- [[../concepts/LLM Agent]]
