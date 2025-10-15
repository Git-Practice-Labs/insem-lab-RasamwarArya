# Git Workflow Diagram

## Branching Strategy Used in Lab 01

```
Initial Commit (6f619b7)
    |
    ├── frontend branch (f1ffffe)
    │   └── Frontend HTML files
    │
    ├── backend branch (84aeb49)
    │   └── Backend Python files
    │
    └── master branch
        ├── Lab documentation (2e0043c)
        └── Merged backend (86257fe) ← HEAD
```

## Workflow Steps Demonstrated

1. **Repository Initialization**
   - Created initial commit with project structure
   - Set up frontend and backend directories

2. **Feature Branch Development**
   - `frontend` branch: Developed HTML interface
   - `backend` branch: Developed Python application

3. **Integration**
   - Merged `frontend` branch into `master`
   - Merged `backend` branch into `master`
   - Added comprehensive documentation

4. **Final State**
   - `master` branch contains complete full-stack application
   - Clean merge history with no conflicts
   - All deliverables properly organized

## Key Git Commands Used

```bash
# Branch Management
git checkout -b frontend
git checkout -b backend
git checkout master

# Merging
git merge frontend
git merge backend

# History Visualization
git log --oneline --graph --all
```

## Benefits of This Workflow

- **Isolation**: Frontend and backend development can proceed independently
- **Collaboration**: Multiple developers can work on different components
- **Integration**: Clean merging process maintains code quality
- **History**: Clear audit trail of all changes and merges
