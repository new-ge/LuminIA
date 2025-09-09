# Branch Standard
## Simplified Standard for Branch Names

Standardizing branch names is an important practice. In addition to helping with the understanding of the development flow, it also facilitates project organization and collaboration.

> Our branches are created from Jira, following the task code defined by our Scrum Master.

## Branch Format:
```<Branch_id>```

- `<Branch_id>`: Identifier of the task in the task management system: Jira

## Opening a Branch:
To open a branch, follow these steps:

- In the **Details** window, select **"Create branch"**.

### Details Window Example:

![alt text](../docs/Task_details_example.png)

- In the **"Create GitHub Branch"** window, select the correct **Repository**.  
  **Example**: `new-ge/API_6SEM_FRONT_END`.
  
- Remove the task description.  
  **Example**: `LMN-3`.

- Click **"Create Branch"**.

### Create GitHub Branch Window Example

![docs/Create_branch_example.png](../docs/Create_branch_example.png)

## Branch Strategy

We are using a branching strategy that follows the pattern below:

---

#### Main Branch
- Used for production-ready code.  
- The product is delivered at the end of every sprint.

---

#### Dev Branch
- Used as the integration branch for ongoing development.  
- At the end of the sprint, it is merged into the **main** branch.

---

#### LMN Branch
- Dedicated branch for the LMN feature.  
- Every time the LMN feature is completed, it is merged into the **dev** branch.
 

## Code Review Process

- All code must be reviewed by at least **one (1) developer** before the Pull Request can be merged into the `main` branch.

- **Responsibility:** The task owner is responsible for testing and fixing issues in their code. Pull Requests that break the API will hold both the task owner and the reviewer who approved the code accountable.


## Pull Request Process
- Pull request name must be the same name of the incoming changes branch.
- Pull Requests must include detailed information about the main features added, as well as any issues found in the code and how they were resolved or worked around.
- Include screenshots if the work involves frontend changes.

---

#### Mandatory Checklist Before Opening a PR:

-  Code has been reviewed.
- Tests have been executed.