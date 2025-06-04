# Version Control Reflection

The goal of this project was to practice using Git for version control by creating and managing multiple branches, making changes in isolated environments, and resolving a merge conflict. The steps below summarize the process I followed:

- Initialized the repository and started on the `main` branch.
- Created a new branch `feature/header` from `main`.
- In the `feature/header` branch, created an `index.html` file and added a header section.
- Switched back to the `main` branch and merged in the changes from `feature/header`.
- Created a new branch `feature/footer` from `main`.
- In the `feature/footer` branch, added a footer section to the existing `index.html` file.
- Switched back to the `main` branch and merged in the changes from `feature/footer`.
- Switched back to the `feature/header` branch and modified the content of the footer section.
- Returned to the `main` branch and attempted to merge in `feature/header` again.
- Git reported a **merge conflict** in `index.html` because both `feature/footer` and `feature/header` modified the same footer section.
- Opened the conflicted file, reviewed both versions of the code, and resolved the conflict by **accepting the incoming change** from `feature/header`.
- Staged the resolved file and completed the merge with a new commit.

This exercise demonstrated how Git enables structured collaboration through branches and merges, and how to manually resolve conflicts when different branches modify the same parts of a file.