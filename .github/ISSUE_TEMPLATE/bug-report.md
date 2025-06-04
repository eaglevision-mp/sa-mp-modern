name: Bug Report (Android or PC)
description: Report bugs on Android or PC platforms, including crash logs or dump files if available.
labels: ["bug"]
body:
  - type: markdown
    attributes:
      value: |
        Before opening a new issue, please search existing issues:  
        https://github.com/eaglevision-mp/sa-mp-modern/issues

  - type: dropdown
    id: platform
    attributes:
      label: Platform
      description: Select the platform where the issue occurred.
      options:
        - Android
        - PC
    validations:
      required: true

  - type: textarea
    id: expected
    attributes:
      label: Expected and current behavior
      description: Concise description of the behavior you expect and what actually occurs.
    validations:
      required: true

  - type: textarea
    id: steps
    attributes:
      label: Steps to reproduce
      description: Provide clear and concise steps for us to reliably reproduce this issue.
    validations:
      required: true

  - type: textarea
    id: additional
    attributes:
      label: Additional information
      description: Any other useful info you want to add (e.g. system specs, Android version, PC OS, hardware).
    validations:
      required: false

  - type: textarea
    id: screenshots
    attributes:
      label: Screenshots / Videos
      description: Provide a screenshot and/or video demonstrating the issue.
    validations:
      required: false

  - type: textarea
    id: crash_log
    attributes:
      label: Crash Log / Dump (if any)
      description: |
        Please paste the content of your crash log here.  
        On Android, it is usually located at: `SAMP/crash_log.txt` inside the game data folder.  
        On PC, it is usually located at: `logs/crash_log.txt`.  
        Including this helps greatly in diagnosing crashes.
    validations:
      required: false
