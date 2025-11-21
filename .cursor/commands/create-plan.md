# Create Plan

# Implementation Planning Checklist

## Overview
This checklist outlines how to produce a clear, concise, and thorough implementation plan for a given problem or feature request.

Your goal is to:
- Understand the context of the work  
- Review and map the relevant areas of the codebase  
- Propose detailed, step-by-step implementation changes  
- Ensure all required tests and conventions are accounted for  
- Deliver a plan that a junior engineer could follow start-to-finish  

Ensure all rules in `./cursor/rules/` are followed.

---

## Inputs Required
Before starting, confirm you have:

- [ ] Problem statement or specification  
- [ ] Links to relevant code sections (services, modules, endpoints, etc.)  
- [ ] Any related tickets or historical discussions  
- [ ] Logs, metrics, or error reports (if applicable)

IF not, ask the user for more guidance

---

## Deliverables

Your final output should be a single markdown planning document containing:

### 1. Summary
- [ ] 2–4 sentence description of the problem  
- [ ] Clear articulation of the intended behavior or outcome  

### 2. Current Behavior & Code Map
- [ ] Explanation of the current flow or behavior  
- [ ] List of relevant files and modules, each with a short note on why it matters  
- [ ] Identification of dependencies, flags, shared components, or external services  

### 3. Proposed Changes (Step-by-Step)
- [ ] Ordered list of implementation steps  
- [ ] For each step:
  - [ ] What will change (functions, classes, handlers, endpoints, schemas, etc.)  
  - [ ] Why the change is needed  
  - [ ] Notes on assumptions, constraints, or tradeoffs  

### 4. Testing Plan
- [ ] List of test cases to cover  
- [ ] Identification of existing tests to update  
- [ ] New tests to add (unit, integration, E2E)  
- [ ] Clear list of edge cases and failure scenarios  

### 5. Risk & Impact
- [ ] Potential breaking changes  
- [ ] Sensitive areas touched (auth, billing, async jobs, data integrity, etc.)  
- [ ] Rollout ideas (feature flags, canary strategy, monitoring)  

### 6. Open Questions
- [ ] List of items needing clarification or external input  
- [ ] Any decisions still pending  

---

## Process

### 1. Understand the Context
- [ ] Read the problem statement thoroughly  
- [ ] Restate the goal in your own words in the **Summary**  
- [ ] Identify constraints (performance, security, backward compatibility)  

### 2. Explore the Codebase
- [ ] Search relevant keywords and imports  
- [ ] Trace the end-to-end flow to find all touchpoints  
- [ ] Document everything in **Current Behavior & Code Map**  
- [ ] Call out any unexpected behavior or technical debt  

### 3. Design the Change
- [ ] Identify where new logic will live  
- [ ] Identify what should be refactored vs. extended  
- [ ] Break work into small, reviewable steps  
- [ ] Document these steps clearly in **Proposed Changes**  

### 4. Plan the Tests
- [ ] Define happy path scenarios  
- [ ] Define error scenarios  
- [ ] Define boundary/edge cases  
- [ ] Map each case to test type (unit, integration, etc.)  

### 5. Ensure Readability & Conventions
- [ ] Use existing naming and architectural patterns  
- [ ] Ensure plan is sequential, readable, and unambiguous  
- [ ] Confirm a junior engineer could implement it end-to-end  

# IMPORTANT 
## Coding Conventions & Quality Expectations
All planned changes should:

- [ ] Follow project architectural boundaries  
- [ ] Respect naming conventions  
- [ ] Avoid unnecessary complexity  
- [ ] Target smaller, incremental PRs where appropriate