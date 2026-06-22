---
name: Bug Report
description: Report a bug or issue with the project
labels: ["bug", "needs-triage"]
body:
  - type: markdown
    attributes:
      value: |
        Thanks for taking the time to report this bug!
  - type: textarea
    id: description
    attributes:
      label: Bug Description
      description: Please describe the bug you encountered
      placeholder: Describe the bug in detail
    validations:
      required: true
  - type: textarea
    id: reproduction
    attributes:
      label: Steps to Reproduce
      description: "Please describe the steps needed to reproduce the issue"
      placeholder: |
        1. Go to '...'
        2. Click on '...'
        3. See error
    validations:
      required: true
  - type: input
    id: expected
    attributes:
      label: Expected Behavior
      description: What did you expect to happen?
    validations:
      required: true
  - type: input
    id: actual
    attributes:
      label: Actual Behavior
      description: What actually happened?
    validations:
      required: true
  - type: dropdown
    id: priority
    attributes:
      label: Priority
      description: How urgent is this issue?
      options:
        - Critical (production issue)
        - High (blocking)
        - Medium
        - Low (nice-to-have)
  - type: textarea
    id: environment
    attributes:
      label: Environment
      description: "Environment details (OS, Node version, etc.)"
      value: |
        - OS: [e.g., macOS, Windows 10]
        - Node version: [e.g., 18.0.0]
        - Browser (if applicable): [e.g., Chrome 100]