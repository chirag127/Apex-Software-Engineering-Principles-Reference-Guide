name: "🐛 Bug Report: Content or Formatting Issue"
about: "Report an inaccuracy, broken link, formatting error, or any other content-related bug."
labels: ["bug", "content-error", "help-wanted"]
body:
  - type: markdown
    attributes:
      value: |
        Thanks for taking the time to report a bug in **Apex-Software-Engineering-Principles-Reference-Guide**!
        Your detailed report helps us maintain a high-quality, accurate, and up-to-date resource for the community.

        Please fill out the following sections completely. Providing as much detail as possible will help us address the issue quickly.
  - type: input
    id: short-summary
    attributes:
      label: "1. Short Summary of the Bug"
      description: "Provide a concise, one-sentence summary of the problem."
      placeholder: "e.g., Typo in 'SOLID Principles' section or Broken link to 'Hexagonal Architecture'."
    validations:
      required: true
  - type: textarea
    id: problem-description
    attributes:
      label: "2. Detailed Description of the Problem"
      description: "Elaborate on the issue. What specifically is incorrect, broken, or missing?
                    Include the exact section, heading, or line number if applicable.
                    If it's an external link, provide the URL and what it should link to."
      placeholder: "e.g., In the 'DRY Principle' section under 'Best Practices', the explanation for 'Don't Repeat Yourself' incorrectly states..."
    validations:
      required: true
  - type: input
    id: location
    attributes:
      label: "3. Location of the Bug (File/Section)"
      description: "Specify the exact file path (e.g., `principles/SOLID.md`), section heading, or URL where the bug is found."
      placeholder: "e.g., `README.md`, Section: 'Architectural Patterns', Sub-section: 'Microservices Overview'"
    validations:
      required: true
  - type: textarea
    id: steps-to-reproduce
    attributes:
      label: "4. Steps to Reproduce (if applicable)"
      description: "If the bug requires specific actions (e.g., clicking a link, viewing on a certain browser), list them here.
                    (For content errors, simply pointing to the location is usually sufficient)."
      placeholder: "1. Navigate to `/docs/architecture/clean-architecture.md`\n2. Scroll down to 'Key Components'.\n3. Observe the bullet point 'Interactors' is missing a description."
    validations:
      required: false
  - type: textarea
    id: expected-behavior
    attributes:
      label: "5. Expected Behavior"
      description: "What should happen instead? How should the content appear or function correctly?"
      placeholder: "e.g., The explanation should accurately define 'Don't Repeat Yourself' as..." or "The link should point to `https://example.com/correct-resource`."
    validations:
      required: true
  - type: textarea
    id: actual-behavior
    attributes:
      label: "6. Actual Behavior"
      description: "What is currently happening or being displayed incorrectly?"
      placeholder: "e.g., The explanation incorrectly states that 'DRY' refers to..." or "The link is broken and returns a 404 error."
    validations:
      required: true
  - type: dropdown
    id: severity
    attributes:
      label: "7. Severity"
      options:
        - Critical (Breaks core understanding, major error)
        - High (Significant inaccuracy, important broken link)
        - Medium (Minor inaccuracy, formatting issue, small typo)
        - Low (Grammatical error, stylistic suggestion)
    validations:
      required: true
  - type: textarea
    id: screenshots
    attributes:
      label: "8. Screenshots or Videos (Optional)"
      description: "If applicable, add screenshots or a short video to help explain your problem."
      placeholder: "Attach images directly or provide links."
    validations:
      required: false
  - type: input
    id: environment
    attributes:
      label: "9. Environment (Browser/OS - if viewing on GitHub/web)"
      description: "What browser and operating system are you using to view the guide? (e.g., Chrome 120, macOS Sonoma 14.2)"
      placeholder: "e.g., Firefox 121.0.1 on Windows 11"
    validations:
      required: false
  - type: textarea
    id: additional-context
    attributes:
      label: "10. Additional Context (Optional)"
      description: "Add any other context about the problem here."
    validations:
      required: false
  - type: markdown
    attributes:
      value: |
        ---
        Thank you for contributing to the improvement of the **Apex-Software-Engineering-Principles-Reference-Guide**!
        Your efforts help ensure it remains a high-quality resource for everyone.
        [View the project on GitHub](https://github.com/chirag127/Apex-Software-Engineering-Principles-Reference-Guide)