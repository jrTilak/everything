# Linters

A **linter** analyzes your code and **points out problems**.

Think of it as a strict reviewer who says:

- “This variable is unused.”
- “This code might crash.”
- “This style breaks the rules.”
- “This could be a bug.”

Linters focus on **correctness, best practices, and consistency**.

### What linters catch

- Syntax errors
- Unused variables or imports
- Possible bugs and unsafe patterns
- Violations of coding standards
- Code that is hard to read or maintain

A linter usually **does not change your code** by default. It warns you and lets you decide.

---

## Formatters

A **formatter** automatically **rewrites your code’s appearance**.

It does not care much about logic. It cares about:

- Indentation
- Spacing
- Line length
- Braces and commas
- Quotes and semicolons

Think of it as a neat freak who silently fixes your messy desk.

### What formatters do

- Align indentation
- Normalize spacing
- Enforce consistent style
- Make code visually predictable

Formatters **always modify your code**, usually in a deterministic way.

---

## How They Work Together

1. **Formatter runs first**
   Makes the code look clean.
2. **Linter runs next**
   Checks if the code is safe, correct, and well-written.
