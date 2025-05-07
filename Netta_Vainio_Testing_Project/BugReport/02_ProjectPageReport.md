## Summary (Summarize the bug encountered concisely)

Creating a new project with an existing name does not trigger any error, and the system allows duplicates.

## Steps to reproduce     

1. Log in to GitLab
2. Navigate to the Projects page
3. Create a new project with the name `Test Project`
4. After successful creation, click "New Project" again
5. Use the same name `Test Project`
6. Submit the form

## What is the current bug behavior?

GitLab accepts the second project with the same name without displaying a validation error.

## What is the expected correct behavior?

The system should block duplicate project names and display an error like "Project name already exists."

## Relevant logs and/or screenshots

_No visible error message on UI; both projects appear in the list with the same name._

## Possible fixes

- Add frontend and backend validation to check for existing project names before submission.
- Display a user-friendly error if the name is already taken.

## Whom do you report/ Assign To/ Tags

- Report to: GitLab Frontend or Project Management Team
- Tags: `bug`, `project-page`, `validation`, `TS-3-Project`

## Priority

**Medium**


      
