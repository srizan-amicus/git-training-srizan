# Git Branching strategy followed
for this project I used a feature based branching strategy
- `main` contains the stable production ready code, protected from direct commits

- `feature` branches were created for implementing new features such as navigation, footer, sidebar and rebase practices.

- `hotfix/*` branch was created to demonstrate an urgent producion fix using cherry-pick

- A seperate practice branch was also used for reset and recovery demonstrations

This strategy keeps the main branch stable while allowing independent development of new features


---
## Branch Diagram
main
|
|---feature/add-navigation
|
|----------------merge
|
|
|---feature/add-footer-------------|
                                   |
                                   |
|------------hotfix/urgent-fix---- |
|              (cherry-pick)
|
|
|---feature/add-sidebar
|
|
|---feature/rebase-dummy
|
|
|---feature/reset-branch

---

## Branching Rules
### When to create a branch
- Before starting any new feature
- Before working on an urgent bug fix
- Before experimenting with different changes that should not affect the main branch

### Which branch should be used as the base
- Feature branches are created from `main`
- Hotfix branches are also created from `main`
- Practice branches can be created from `main`

### Branch Naming Convention
 - Feature branches :
 feature/<feature-name>

Examples:
 feature/add-sidebar,
 feature/add-footer,
 feature/add-navigation,

- Hotfix branches
hotfix/urgent-fix

- Practice branches:-
practice/<task-name>

## Merge vs Rebase

### Merge
- Combines two branches together
- keeps in record, full branch history
- Best for collaborative development

### Rebase
- Replays commits on top of another branch
- It produces a cleaner history
- Rewrites commit history
- Best used on local branches before merging

