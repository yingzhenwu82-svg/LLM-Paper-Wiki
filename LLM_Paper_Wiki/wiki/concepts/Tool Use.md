# Tool Use
Tool use allows an LLM Agent to invoke external functions or interfaces such as search, code execution, APIs, or software tools.

## Design considerations
- Define tool names, schemas, and usage boundaries.
- Validate inputs and outputs.
- Handle errors and retries.
- Observe results before selecting follow-up actions.
- Prefer least privilege and require confirmation for consequential actions.

## Related
- [[Reasoning and Acting]]
- [[LLM Agent]]
- [[../papers/Toolformer]]
- [[../papers/SWE-agent]]
- [[../papers/ReAct]]
