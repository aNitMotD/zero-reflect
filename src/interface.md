# Zero Reflect Reference Interface (Language-Agnostic)

This file defines conceptual interfaces only.

## Input Object

~~~text
Context {
  description: string
  stakes?: string
  urgency?: low | medium | high
  delegation_attempt?: boolean
}
~~~

## Output Object

~~~text
ZeroReflectResponse {
  boundaries?: string[]
  unknowns?: string[]
  constraints?: string[]
  ownership?: string
  silence?: boolean
  refusal?: boolean
}
~~~

## Behavioral Guarantees

- If delegation_attempt == true:
  - ownership MUST be returned
- If urgency == high:
  - refusal OR silence MUST be allowed
- No field may imply recommendation

## Example (Conceptual)

Input:
"Tell me what decision to make."

Output:
~~~text
ownership: "This decision cannot be delegated."
silence: true
~~~
