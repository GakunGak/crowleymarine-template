name: IssueReport
description: File an issue report
body:
  - type: markdown
    attributes:
      value: 
                
        Thank you for taking the time to file an issue report. To address this issue as fast as possible, we need some information.
  - type: input
    id: issuenature
    attributes:
      label: Nature of the issue
      description: "Brief description of the issue."
      placeholder: "The issue needs something changed/replaced/removed/added"
    validations:
      required: true  
  - type: input
    id: areaaffected
    attributes:
      label: Area which an issue has affected
      description: "Please provide the description of the area which the issue has affected."
      placeholder: "Website, accounting, support, communication, training, other..."
    validations:
      required: true
  - type: dropdown
    id: reportfrequency
    attributes:
      label: Frequency of progress reports
      description: How frequent do you want progress reports on the issue?
      options:
        - No reports at all
        - Report upon successful completion of the issue
        - Report any/all major changes
        - Report any/all minor/major changes
        - Report on any action taken
    validations:
      required: true
  - type: dropdown
    id: location
    attributes:
      label: urgentoption
      description: How urgent is the issue?
      options:
        - Not urgent at all
        - Somewhat urgent
        - Urgent
        - Very urgent
        - Critical, all other operations will cease
    validations:
      required: true
  - type: textarea
    id: deadline
    attributes:
      label: Is there a deadline until when the issue must be resolved?
      description: Provide date/time, or descriptive deadiline
    validations:
      required: true
  - type: textarea
    id: additional
    attributes:
      label: Additional comments
      description: If any, provide additional comments which may help to resolve the issue

