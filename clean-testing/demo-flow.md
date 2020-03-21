# Clean testing demo

## Intro - slides

How it often looks, how it should look like, micro-contribution, the defining moment,

## The unit under test

- What is it about
- It's not perfect intentionally

## Test structure patterns

- Show title "The test structure"

### Naming

- Problem: A test fails, I'm about to deploy, what is it about? now have to read the code 📹
- Guideline: Write for the visitor, speak at the requirement level, show requirement document 🖼
- Advice: include 3 parts, from Osherove book 📓
- BP: 3 parts in each test name ✅
- First try: code 3 parts in one line, report looks bad 🖼
- Linter: eslint-plugin-test-names ️️⚙️

### Hirearchy

- Problem: Long textual list, any relation between the failing test?
- Making this better: organized report 🖼, can run only one category 🆒
- Applying categorization: Group by common
- Method 1: Group by scenario, great when there are few scenarios and many tests, like, the source of "it", Mocha context
- Method 2: Group by custom category, create describe, put tests
- Tagging: sometime we want to run custom
- BP: Categorize your tests ✅
- Linter: ⚙️
- Here's a list with useful linters 🎁

### The test parts

- Problem: Bulk of test, why does it fail?
- Literature: GOOS about structure 📓
- Explain: Our brains stay on system1 when recognize patterns (pattern), zero cpu cycles
- BP: AAA ✅
- Do it: move to AAA
- My test snippet ⚙️

## Test assertion patterns

### No IF

- Problem: I see here code, something to dive into, something to test?
- Recommendation: Flat, no loops, no if, simple set of instructions
- Why we don't need it: If you did, you're probably doing something wrong
- Literature: Entry point & exit point 📓
- Remove from code
- Linter ⚙️

### Declarative assertions

- Problem: Additional imperative code, buggy, test the tests
- Literature: X-patterns about... 📓
- Anti-example: how errors look now
- Better-example: now the error is clearer
- Take it further: Cocumber, custom message
- BP: AAA & IF ✅

## Test setup patterns
