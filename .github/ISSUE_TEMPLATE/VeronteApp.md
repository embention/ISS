---
name: Problem Report 
about: Describe a PR
title: ''
labels: ["VeronteApp", "PR","Software"]
assignees: 'jmt1'

---
body:
  -type: markdown
   attributes:
    value: | 
        # References
          * This issue is created for the knowledge of possible errors generated in our applications and with the fact of improving our quality product.
          * Enter a description of the error that occurred so that our engineers can begin to solve it.
          * You can also introduce an image and/or video to demonstrate the problem and make the understanding easier.
  -type: markdown
   attributes:
   value: |
        # Description of problem
  - type: markdown
    attributes:
      value: |
        Thanks for taking the time to fill out this bug report!
  - type: textarea
    id: what-happened
    attributes:
      label: What happened?
      description: Also tell us, what did you expect to happen?
      placeholder: Tell us what you see!
      value: "A bug happened!"
    validations:
      required: true
  - type: dropdown
    id: version
    attributes:
      label: Version
      description: What version of our software are you running?
      options:
        - 1.0.2 (Default)
        - 1.0.3 (Edge)
    validations:
      required: true
  - type: dropdown
    id: browsers
    attributes:
      label: What browsers are you seeing the problem on?
      multiple: true
      options:
        - Firefox
        - Chrome
        - Safari
        - Microsoft Edge
  - type: textarea
    id: logs
    attributes:
      label: Relevant log output
      description: Please copy and paste any relevant log output. This will be automatically formatted into code, so no need for backticks.
      render: shell
  - type: checkboxes
    id: terms
    attributes:
      label: Code of Conduct
      description: By submitting this issue, you agree to follow our [Code of Conduct](https://example.com)
      options:
        - label: I agree to follow this project's Code of Conduct
          required: true
