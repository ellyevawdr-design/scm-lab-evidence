# Session 2 Reflection

##Q1: How do Issues and Pull Requests Together Support Change Control?
Issues define what change is needed, why it matters, and the acceptance criteria before work begins, establishing clear requirements traceability. Pull requests then provide a controlled mechanism to propose, inspect, and discuss the actual code or documentartion changes before they enter 'main'. Linking a pull request to an issue (such as using 'Closes #1) connects the planned requirement to the verified implementation abd automatically tracks completion. Together, they prevent untracked edits and clear audit trail of every approved change.

##Q2: Why Did The Conflict in Part 4 Happen, and How Could a Team Reduce Such Conflicts?
The conflict in Part 4 happened because two branches modified the same lines in 'session2/conflict-demo.md' with incompatible values (staging versus production), so Git could not automatically decide which edit to keep. Teams can reduce conflicts by keeping feature branches short-lived and focused on small, well-scoped tasks. Regularly pulling or rebasing updates from 'main' into active branches also surface overlaping edits early. Clear communication and dividing work across seperate files or sections further minimise collisions.

##Q3: What Would Be Lost if People Merged Straight into 'Main' Without a Pull Request?
Merging directly into 'main' without a pull request removes the peer-review gate that catches typos, logic errors, and missing requirements before they affect the main branch. It also makes it harder to see the contect behind why a change was made, because discussions and review feedback are not tied to the change set. Over time, 'main' becomes noisier and riskier to deploy or build upon. Without pull requests, team lose both early quality checks and clear-history accountability.
