# COMP3104_Group5_Assignment

![CI](https://github.com/7harlot/COMP3104_Group5_Assignment/actions/workflows/ci.yml/badge.svg)

## Group Members
- **Leader:** Ben Morrison (101572409) - [GitHub](https://github.com/7harlot)
- **Member 2:** FULL NAME (STUDENTID) - [GitHub](https://github.com/USERNAME)
- **Member 3:** FULL NAME (STUDENTID) - [GitHub](https://github.com/USERNAME)
- **Member 4:** FULL NAME (STUDENTID) - [GitHub](https://github.com/USERNAME)
<!-- Each member adds/edits THEIR OWN line, from their own branch, so it shows in their commit log. -->

## Project Description
This repository hosts the group assignment for the COMP3104 DevOps course at George Brown
College. It practices a collaborative Git workflow: per-developer branches, pull requests into
`main`, merge-conflict resolution, and continuous integration with GitHub Actions.

Each member contributes three files in the repository root:

| File | Topic |
|------|-------|
| `STUDENTID_gb.txt` | George Brown College |
| `STUDENTID_devops.txt` | The COMP3104 DevOps course |
| `STUDENTID_sdlc.txt` | Why DevOps matters in the software development lifecycle |

## Setup Instructions
1. Clone the repository:
   ```bash
   git clone https://github.com/7harlot/COMP3104_Group5_Assignment.git
   cd COMP3104_Group5_Assignment
   ```
2. Create and switch to your branch: `git checkout -b STUDENTID-Name` (e.g. `101572409-Ben`)
3. Push it: `git push -u origin STUDENTID-Name`
4. No dependencies to install. All work is plain text files.

## CI/CD Pipeline
The project uses GitHub Actions for continuous integration. The workflow is defined in
`.github/workflows/ci.yml` and runs on every push to any branch and on every pull request into
`main`. Besides the sample echo steps, it checks that every `.txt` file sits in the repository
root and is named `STUDENTID_gb.txt`, `STUDENTID_devops.txt` or `STUDENTID_sdlc.txt`.

## Branch Strategy
Each member has their own branch named `STUDENTID-Name` (per-developer branching). Members
commit locally, push to their branch, and open a pull request into `main` using the template in
`.github/PULL_REQUEST_TEMPLATE.md`. Before opening a PR, members merge the latest `main` into
their branch and resolve any conflicts locally. `main` is only changed through pull requests.

## Commit Message Conventions
- Start with a verb: Add, Update, Fix, Remove
- Say what changed and where, e.g. "Add campuses section to gb.txt"
- One logical change per commit