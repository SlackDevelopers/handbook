# Rocket.Chat Engineering Contribution Guideline

## Development workflow&#x20;

To ensure a collaborative and efficient environment, there are key practices Rocket.Chat core developers should follow when contributing to the project. These practices benefit the team as a whole and streamline the development process.

**Step 1: Squad Task Selection:** The first step is to grab tasks from the squad board. These tasks might be pre-assigned by managers, product managers, or tech leads, or they can be self-selected.

**Step 2: Clarify Task Requirements:** Before diving in, ensure you fully grasp the task's details. Don't hesitate to communicate with your manager or tech lead if anything seems unclear. They'll be happy to clarify or involve relevant parties in the discussion.

**Step 3: Maintain a Detailed Task Log:** Use comments within the task to document decisions, steps taken, and any other relevant information. This meticulous record-keeping creates a clear history for future reference and assists other developers working on the same project.

**Step 4: Update Task Status:** As you progress on the task, remember to update its status on the board. This could be "In Progress", "Waiting Review", "QA", or any other relevant stage. This keeps everyone informed about the task's workflow.

**Step 5: Committing Changes:** Write commit messages that clearly describe the change you made. Following a semantic commit style (like "fix: resolved image upload issue") improves code readability and future maintenance.

**Step 6: Submitting a Pull Request:** After committing your changes, create a well-defined pull request (PR). The title should adhere to conventional commits standards (e.g., "fix: resolved image upload issue"). Provide a detailed description of the changes, their rationale, and any addressed issues. Include a changeset for fixes or features, and update relevant documentation. Keep your PR focused on the original task. Avoid adding unrelated changes, even minor refactoring. If refactoring is necessary, create a separate PR.

**Step 7: Comprehensive Test Coverage:** Always include relevant tests (API, UI, or unit) within your PR to validate your code changes. This strengthens code quality and ensures functionalities work as intended. For fixes, tests are crucial to prevent regressions and ensure the issue is resolved. Exceptions exist for purely visual changes or those dependent on external tools lacking reliable automated testing methods. Step 8: Code Review: The development team will meticulously examine your code. This review ensures it meets coding standards, functions as intended, and addresses any potential problems. We highly encourage active participation from everyone on the team in code reviews. Be prepared for discussions and revisions based on their feedback, fostering a collaborative environment.

**Step 9: Review, Test, and Merge:** After a thorough team review, your PR enters QA for rigorous testing. Upon successful QA, it lands in the merge queue for final integration.

## Code review process

This process ensures your code adheres to established coding standards, functions as intended, and catches any potential problems you might have overlooked. The collaborative review fosters knowledge sharing within the team, leading to high-quality code, improved development practices, and a stronger overall codebase.

**Step 1: Title and description:** Look for a clear and concise title and description in the PR. The title should accurately reflect the changes and follow the conventional commits standard, and the description should explain the purpose and functionality of the code.

**Step 2: Verify Changeset (Fix/Feature PRs):** Confirm that a changeset has been added for pull requests categorized as fixes or features. This changeset helps track versioning and simplifies release management. Kindly refer to the official documentation to see our changeset guidelines.

**Step 3: Verify Labels and Milestones:** Look for appropriate labels and milestones assigned to the PR. Labels help categorize the changes, while milestones track progress toward specific release versions. Confirm these are correctly assigned to ensure clear organization and efficient project management.

**Step 4: Review Automated Checks:** Verify that all automated checks (linting, type checking, tests, etc.) have passed successfully. These checks help identify potential errors and ensure code quality is maintained.

**Step 5: Code Review for Quality:** Meticulously examine the code for adherence to project standards, architecture principles, security best practices, readability, and maintainability. Furthermore, the PR should focus on a single solution. If the changes involve multiple solutions, suggest splitting them into separate PRs for a clearer and more manageable review process.

**Step 6: Review Test Coverage:** Ensure the PR includes relevant tests covering the proposed solution thoroughly. For exceptional cases (layout changes, external integrations, etc) where testing might be impractical, a comment explaining the rationale is recommended after seeking approval from the manager or tech lead. This fosters a balance between comprehensive testing and acknowledging limitations. Step 7: Review, Test, and Merge: After a thorough team review, your PR enters QA for rigorous testing. Upon successful QA, a label must be added indicating completion. Once all changes have been addressed and necessary approvals are granted, the designated bot automatically merges the PR into the codebase.
