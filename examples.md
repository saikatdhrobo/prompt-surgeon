# Prompt Surgeon — Examples

---

# Example 1 — Vague Research Prompt

## Before

```txt
Analyze the market and give me insights.
```

## After

```txt
Analyze the global electric vehicle (EV) market for 2024-2025.

Provide:
1. Market size and YoY growth
2. Top manufacturers by market share
3. Key growth drivers
4. Regional breakdowns
5. Major risks and headwinds

Output format:
Structured report with bullet points.

Mark projections as [ESTIMATED].
If data is unavailable, state "Data not available."
```

## Why It Works

* Defines scope
* Specifies output structure
* Adds hallucination guardrails
* Improves controllability

---

# Example 2 — Conflicting Instructions

## Before

```txt
Write a detailed but brief summary of quantum computing. Make it simple but comprehensive.
```

## After

```txt
Write a 300-word introduction to quantum computing for computer science students familiar with classical computing but not quantum mechanics.

Structure:
1. Core concept
2. 3 key principles
3. Main use cases
4. Current limitations

Use analogies where useful.
Avoid equations.
```

## Why It Works

* Removes contradictory instructions
* Defines audience precisely
* Specifies structure and depth
* Improves clarity

---

# Example 3 — Coding Prompt

## Before

```txt
Write a Python function to validate email addresses.
```

## After

```txt
Write a Python function:

validate_email(email: str) -> dict

Requirements:
- Validate standard email formatting
- Return:
{
  "valid": bool,
  "error": str | null
}

Handle:
- empty strings
- missing @
- multiple @
- invalid domains

Include 5 test cases.
```

## Why It Works

* Defines return structure
* Adds explicit constraints
* Specifies edge cases
* Improves reliability

---

# Example 4 — Agentic Workflow

## Before

```txt
Research Tesla and write a report.
```

## After

```txt
OBJECTIVE:
Produce a 1-page investor brief on Tesla.

RESEARCH MODULES:
1. Financial performance
2. Business segments
3. Competitive advantages
4. Risks
5. Recent developments

CONSTRAINTS:
- Distinguish facts from projections
- Flag uncertainty
- Specify reporting periods

OUTPUT:
Structured executive brief under 400 words.
```

## Why It Works

* Converts vague task into workflow
* Adds modular structure
* Improves reasoning quality
* Reduces hallucination risk

---

# Example 5 — Simple Prompt Optimization

## Before

```txt
Make this email sound better.
```

## After

```txt
Rewrite this email to sound more professional while keeping the tone concise and friendly.
```

## Why It Works

* Adds clear optimization goal
* Preserves simplicity
* Avoids unnecessary complexity
