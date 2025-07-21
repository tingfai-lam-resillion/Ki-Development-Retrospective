### **Theme 3: An Undisciplined Development and Version Control Process**

The project's technical problems are a direct result of *how* it was built. The process lacked discipline, both in how version control was used and in how code was written. This led to wasted effort, overwritten work, and a codebase that is now difficult to manage.

**Observation: Version Control Was Not Consistently Used**

The team did not follow standard version control practices, which caused significant problems.
*   **The "Zip File Incident":** Instead of using a pull request, a major contribution was delivered as a 319MB zip file. This single, massive commit bypassed the standard review process and made it impossible to track changes effectively.
*   **Architectural Work Was Abandoned:** Because of the zip file incident, a branch containing carefully planned architectural improvements (`architecture-enhancements`) had to be thrown away. Later in the project, the same thing happened to the `refactor-report-generators` and `exe-bundling` branches. This represents a significant sunk cost of development effort.
*   **Code Reviews Were Not Enforced:** There was no consistent process for code review, which meant that code was often merged without a second pair of eyes, allowing quality issues to build up.

When version control is not used correctly, it stops being a tool for collaboration and becomes a source of chaos.

**Observation: The Workflow Was Dominated by "Vibe Coding"**

The primary development method was a form of "vibe coding": using an AI tool to generate code based on a general feeling or "vibe" of what was needed, without a structured process or rigorous review.
*   **Code Was Written in a Black Box:** The workflow involved uploading files to an external AI service and then downloading the results. This is a black box process, disconnected from the local development environment and version control.
*   **Changes Were Consistently Overwritten:** Because this workflow was disconnected, it frequently led to other team members' changes being overwritten. The AI was working from old code, and its output was committed without checking for conflicts.
*   **AI-Generated Code Was Not Vetted:** The code produced by this method was committed without a thorough review. This is why the codebase shows classic signs of unvetted AI generation: inconsistent style, the same logic repeated with minor variations across dozens of files, and even AI-generated comments left in the code.

"Vibe coding" is all fun and games until you have to debug the vibes. While AI is a useful assistant, using it without discipline, review, or proper version control was a primary cause of the project's current code quality problems.

---
[**< Previous: Collaboration Gaps**](02_collaboration_gaps.md) | [**Next: Business Cost of Tech Debt >**](04_business_cost_of_tech_debt.md)