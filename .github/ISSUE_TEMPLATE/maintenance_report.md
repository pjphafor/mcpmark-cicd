---
name: Maintenance Report
description: Report a maintenance or housekeeping task
labels: ["maintenance", "needs-triage"]
body:
  - type: markdown
    attributes:
      value: |
        Thanks for reporting a maintenance task!
  - type: dropdown
    id: type
    attributes:
      label: Maintenance Type
      description: What type of maintenance is this?
      options:
        - Code Refactoring
        - Dependency Update
        - Documentation Update
        - Performance Optimization
        - Security Update
        - Code Cleanup
        - Other
    validations:
      required: true
  - type: textarea
    id: description
    attributes:
      label: Description
      description: Describe the maintenance task
      placeholder: Describe the maintenance task in detail
    validations:
      required: true
  - type: textarea
    id: scope
    attributes:
      label: Scope
      description: What areas of the codebase are affected?
    validations:
      required: true
  - type: textarea
    id: benefits
    attributes:
      label: Expected Benefits
      description: What benefits will this maintenance provide?
    validations:
      required: true
  - type: textarea
    id: impact
    attributes:
      label: Potential Impact
      description: Any potential risks or considerations?