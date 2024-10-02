name: Bug Report
description: "Found a bug? We'd appreciate if you'd first search through our open issues and docs, to make sure the issue isn't already known."
labels: ["bug"]
title: "bug: " 
body:
  - type: checkboxes
    attributes:
      label: "Dupe Check"
      options:
        - label: "I have [searched ProxyPal bugs](https://github.com/ProxyPalAI/ProxyPal/issues?q=is%3Aissue+label%3Abug+) and there are no duplicates"
          required: true
  - type: textarea
    id: "describe-the-bug"
    attributes:
      label: "Describe the bug"
      description: "A clear and concise description of what the bug is."
      placeholder: Tell us what you see.
    validations:
      required: true
  - type: textarea
    id: "to-reproduce"
    attributes:
      label: "To reproduce"
      description: "Bug reports with clear reproduction will get prioritized higher and addressed more quickly."
      placeholder: "Steps to reproduce: 1. Go to '...' 2. Click on '...' 3. Scroll down to '...' 4. See error '...'"
    validations:
      required: true
  - type: textarea
    id: "expected-behavior"
    attributes:
      label: "Expected behavior"
      description: "A clear and concise description of what you expected to happen."
      placeholder: Tell us what you expect to see.
    validations:
      required: false
  - type: textarea
    id: "screenshots"
    attributes:
      label: "Screenshots"
      description: "If applicable, add screenshots/videos to help explain your problem. While optional, screenshots help expedite the time in which your bug is addressed."
    validations:
      required: false
  - type: dropdown
    id: "os"
    attributes:
      label: "Operating system"
      multiple: false
      options:
        - MacOS
        - Windows
        # - Linux
    validations:
      required: true
  - type: textarea
    id: "proxypal-version"
    attributes:
      label: "Current ProxyPal version"
      description: "Click on ProxyPal Menu->About ProxyPal->Copy"
      placeholder: |
        Version: 1.0.1
        Environment: prod
        Build: 1727892378
    validations:
      required: true
  - type: dropdown
    id: "regression"
    attributes:
      label: "Regression"
      description: "Is this a regression (used to work in a previous ProxyPal version)?"
      multiple: false
      options:
        - "No, this bug or issue has existed throughout my experience using ProxyPal"
        - "Yes, this bug started recently"
    validations:
      required: true
  - type: input
    id: "proxypal-version-regression-date"
    attributes:
      label: "Recent working ProxyPal date"
      description: "Most recent date that ProxyPal worked as expected"
    validations:
      required: false
  - type: textarea
    id: "additional-context"
    attributes:
      label: "Additional context"
      description: "Add any other context about the problem here"
    validations:
      required: false
  - type: dropdown
    id: "blocker"
    attributes:
      label: "Does this block you from using ProxyPal daily?"
      description: "All feedback will be reviewed, even if you select 'No'."
      multiple: false
      options:
        - "No"
        - "Yes, this issue prevents me from using ProxyPal daily."
    validations:
      required: true
