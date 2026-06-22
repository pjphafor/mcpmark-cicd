---
name: Feature Request
description: Suggest a new feature for the project
labels: ["enhancement", "needs-triage"]
body:
  - type: markdown
    attributes:
      value: |
        Thanks for suggesting a feature!
  - type: textarea
    id: description
    attributes:
      label: Feature Description
      description: Describe the feature you'd like to see
      placeholder: Describe the feature in detail
    validations:
      required: true
  - type: textarea
    id: problem
    attributes:
      label: Problem Statement
      description: What problem does this feature solve?
    validations:
      required: true
  - type: textarea
    id: solution
    attributes:
      label: Proposed Solution
      description: How would you implement this feature?
      placeholder: Describe your proposed implementation
  - type: input
    id: usecase
    attributes:
      label: Use Case
      description: Who would benefit from this feature?
    validations:
      required: true
  - type: dropdown
    id: priority
    attributes:
      label: Priority
      description: How important is this feature?
      options:
        - Critical (production blocker)
        - High (important)
        - Medium (nice to have)
        - Low (low priority)
  - type: textarea
    id: additional
    attributes:
      label: Additional Context
      description: Any other information that might help
      placeholder: Screenshots, mockups, etc.