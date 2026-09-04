# Collaborative code development

In this assignment you'll create a collaborative code base for some very basic mathematical functions. You will divide your group in three subteams. With each subteam you'll work on implementations, but you will also review the other subteams' code and extend their functions and documentation. During this process you'll draw a Git history graph by hand, including the commit messages. You can use this graph during the offline question session. Remember that you can use VS Code Source Control graph to monitor the history of your repository, but please note that it might look slightly different depending on on which machine you are working.

You will work in a repository that is created from scratch (no starter files), use Jupyter notebooks for code, and write documentation in a `README.md`. This repository is not graded.

## Task 1: Create a new empty repository on GitHub

1. One team member creates a new empty repository in their personal GitHub account.
2. Name your repository (for example: `GA1.1-teamX`).
3. Add all team members as collaborators. (On the repository homepage -> Settings -> Collaborators)

## Task 2: Create the initial project structure

1. Clone the repository locally using VS Code.
2. In your local repository, create:
   - a folder `notebooks/`
   - a file `README.md`
3. Commit and push this initial structure to `main`.

## Task 3: Create base functions on separate branches

Now, you will work in 3 subteams, each with their own function to implement:

- Subteam A: `add(a, b)`
- Subteam B: `subtract(a, b)`
- Subteam C: `multiply(a, b)`

Instructions:

1. Create a branch for your task: `feature/<subteam>-base-function`
2. Create your notebook in `notebooks/`:
   - `add.ipynb` or `subtract.ipynb` or `multiply.ipynb`
3. In your notebook:
   - define your function
   - add 2–3 simple example calls
4. **Before every commit:** clear notebook outputs.
5. Update `README.md` with a short subsection for your function. Describe what it does and when it might break. Add a short example of how to use it.
6. Commit and push your branch.
7. Open a Pull Request to `main` on GitHub.
8. Collectively as a team, start your hand-drawn Git history graph. Remember to include the commit messages.

## Task 4: Review both other subteams' Pull Requests

Each subteam must review PRs from both other subteams.

For each review:

1. Pull the PR branch locally.
2. Run the notebook/function locally and test it with 2–3 example calls.
3. Write a review comment in the PR that includes:
   - what you tested
   - result of the test
   - some screenshot as evidence
4. Approve or request changes with a clear reason.

## Task 5: Merge and resolve a README conflict

You'll now merge these PRs into main, which will highly likely create a merge conflict in `README.md`. You will resolve this conflict manually with the complete team.

1. Merge one PR first.
2. For the other PR(s), resolve the merge conflict manually in `README.md`.
3. Update your hand-drawn Git history graph including the merge commits.
4. Push the resolved branch and complete the PR merge.
5. Update your hand-drawn Git history graph including the merge commits.

## Task 6: Extend your function

Now implement an extension function to extend the codebase. Work on the work previously performed by another team:

- Subteam B: `sum_list(values)` and repeatedly call `add(...)`
- Subteam C: `distance_from_zero(x)` and call `subtract(...)`
- Subteam A: `square(x)` and call `multiply(...)`

Rules:

1. Create a branch based on the updated `main`: `feature/<subteam>-extension-function`. Make sure you've synced your local `main` with the remote `main` before creating this branch.
2. The new function must call the original base function.
3. Clear notebook outputs before commit.
4. Update `README.md` with a short explanation and example.
5. Open a PR to `main`.

## Task 7: Review and merge

As before, review the other subteams' PRs and merge them into `main`. Resolve any merge conflicts in `README.md` as a subteam. Update your hand-drawn Git history graph accordingly, remembering to include the commit messages.

If you've time left, you can continue with the [bonus assignment](./bonus.md).
