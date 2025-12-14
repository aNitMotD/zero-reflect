# Example MCP Pipeline with ZR Gate

1. User submits input
2. Trigger check (T1–T5)
3. If triggered → invoke ZR
4. Apply gates (G1–G5)
5. If allowed → execute downstream tools
6. Otherwise → return ZR output and stop

Note:
Downstream execution MUST NOT be interpreted
as automated decision-making.
All triggers and execution contexts
remain under explicit user responsibility.