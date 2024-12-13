---
name: NewBugReport
description: File a bug report
title: "[Bug]: "
labels: ["bug", "triage"]
projects: ["octo-org/1", "octo-org/44"]
assignees:
  - octocat
body:
  - type: markdown
    attributes:
      value:
        thanks for taking the time to fill out this bug report !
  - type: input
    id: contact
    attributes:
      label: contact details
      description: How can we get in touch with you if we need more info?
      placeholder: ex. email@example.com
    validations:
      required: false
  - type: textarea
    id: what-happen
    attributes:
      label: what happend?
      description: Also tell us, what did you expect to happend?
      placeholder: Tell us what you see !
      vaule: "a bug happend!"
    validations:
      required: true
  - type: dropdown
    id: version
    attributes:
      label: version
      description: What version of our software are you running?
      options:
        - 1.0.2 (Defult)
        - 1.0.3 (Edge)
      defult: 0
    validations:
      required: true
  - type: dropdown
    id: browsers
    attributes:
      label: What browsers are you seeing the problem on?
      multiple: true
      options:
        - firefox
        - chrome
        - safari
        - microsoft edge
  - type: textarea
    id: logs
    attributes:
      labels: Relevent log output
      decriptions: please copy and paste any relevent log output. This will be automatically formated into code, so no need for backticks.
  - type: checkboxes
    id: terms
    attributes:
      label: code of conduct
      description: by submitting this issue, you agree to follow out [code of conduct] (https://example.com)
      options:
        - label: I agree to follow this projects code of conduct
        required: true
    
---
