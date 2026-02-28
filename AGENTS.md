```markdown
# AGENTS.md Guidelines

These guidelines are designed to ensure consistent, maintainable, and high-quality code for our AGENTS repository. Adherence to these principles will significantly improve the development process and reduce complexity.

## 1. DRY (Don't Repeat Yourself)

*   **Single Responsibility Principle:** Each agent function or module should have a single, well-defined purpose. Avoid creating overly complex functions with multiple responsibilities.
*   **Reusable Components:** Design components that can be easily reused across multiple agents.
*   **Abstraction:**  Provide abstractions for common patterns to reduce duplication.
*   **Parameterization:**  Use parameters to make components more flexible and adaptable.

## 2. KISS (Keep It Simple, Stupid)

*   **Minimal Code:**  Strive for the shortest possible solution that satisfies the requirements.
*   **Readability:**  Code should be easy to understand for other developers (including yourself in the future).
*   **Concise Logic:**  Avoid unnecessary complexity and convoluted logic.
*   **Clear Names:**  Use descriptive variable and function names.

## 3. SOLID Principles

*   **Single Responsibility:** As stated above, each component should have one focused reason to exist.
*   **Open/Closed Principle:**  New agents/components should be able to be added without modifying existing code.  Existing code should not require modification.
*   **Liskov Substitution Principle:**  Subclasses should be substitutable for their base classes without altering the correctness of the program.
*   **Interface Segregation Principle:**  Clients should not be forced to use interfaces they do not need.
*   **Dependency Inversion Principle:**  High-level modules (like agents) should be replaced by low-level modules (like interfaces).

## 4. YAGNI (You Aren't Gonna Need It)

*   **Avoid Unnecessary Code:** Do not introduce functionality that is not currently required.
*   **Future-Proofing:**  Don't write code that might be required later, even if it's currently not used.
*   **Focus on Requirements:** Prioritize the requirements and design accordingly.

## 5. Development Workflow & Code Style

*   **Coding Style:**  Follow a consistent coding style (e.g., PEP 8, Google Style) for all files.  Use a linter (e.g., flake8, pylint) to automatically enforce this style.
*   **Comments:**  Provide concise comments explaining complex logic or non-obvious decisions.  Comments should not over-explain.
*   **Error Handling:** Use clear and informative error messages and logging.
*   **Testing:** All development must be productive and includes unit tests.
*   **Code Reviews:**  All code should undergo peer review before merging into the main branch.  Reviews should focus on adherence to these guidelines.
*   **Version Control:** Use Git for version control and commit with clear commit messages.
*   **Branching Strategy:** Implement a well-defined branching strategy (e.g., Gitflow) to manage development and releases.

## 6. File Limit: 180 Lines

*   Each file must contain no more than 180 lines of code.  This is a strict limit.

## 7. Test Coverage: 80% Minimum

*   All development must achieve at least 80% test coverage. This will be determined through automated test suites.

## 8.  File Structure

*   **Agent.py:** Core agent logic.
*   **Agent.tests:** Unit tests for Agent.py.
*   **Data.py:** Data management and storage (if applicable).
*   **Utilities.py:** Utility functions and modules.
*   **Configuration.py:** Configuration and settings.
*   **ExampleAgents.py:**  Illustrative examples of agent behavior.

## 9.  Dependencies -  Only Tests**

*   All dependencies must be dependencies for *only* automated tests. No external dependencies should be included.

## 10.  Documentation (Optional)**

*   Keep a brief README file explaining the purpose of each agent and its dependencies.

These guidelines are subject to change as the project evolves.  Regular review and updates will be conducted to maintain the quality and consistency of the AGENTS repository.
```