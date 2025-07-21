### **Theme 1: The Project Lacked a Clear and Stable Strategy**

A project needs a clear, consistent target to hit. The Ki Development project's target was blurry and kept moving, which caused confusion and led directly to downstream technical and process problems.

**Observation: The Project Had Three Competing Goals**

From the start, it wasn't clear what the most important goal was. The project was trying to be three things at once:
1.  A high-quality, maintainable tool for Philips.
2.  A quick, low-budget delivery.
3.  A training opportunity for a junior developer.

Because these goals were never officially ranked, the team had to guess which one mattered most on any given day. This conflict made it difficult to make good technical decisions. When "quality" and "speed" are both priority #1, "speed" usually wins.

**Observation: The Budget and Timeline Were Unstable**

The project's constraints changed abruptly, which forced a short-term mindset.
*   On April 23rd, the project was suddenly put on a tight 24-man-day budget, with the direction to build only the "bare minimum." This sent a clear message that code quality was not a priority.
*   A few weeks later, this budget constraint was removed.
*   Finally, on June 2nd, the release was abruptly moved up to June 16th. This rush directly led to the abandonment of the final refactoring branches (`refactor-report-generators` and `exe-bundling`).

While the constraint was temporary, the "quick and dirty" approach it encouraged was not. It's hard to build a solid foundation when the project's timeline and budget are unpredictable. This instability was a key factor in the accumulation of technical debt.

**Observation: Project Management Was Not Proactive**

The project would have benefited from more proactive management in key areas:
*   **Scope:** Feature requests from Philips were added to the workload without a clear process for prioritization or technical review.
*   **Process:** The Azure board was intended to track progress, but it wasn't kept up-to-date with the actual work being done, making it an unreliable tool for understanding project status.
*   **Technical Direction:** When the team had different views on important technical decisions (like whether to refactor or add new features), there was an opportunity for management to step in and provide a clear decision, which didn't happen.

Without this active guidance, the project drifted. The lack of a firm, consistent direction allowed an unstructured development workflow to take over, resulting in the maintainability issues the project now faces.

---
[**< Previous: Executive Summary**](00_executive_summary.md) | [**Next: Gaps in Collaboration >**](02_collaboration_gaps.md)