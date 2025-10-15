# Lab 01: Set up a Git repository with separate branches for frontend and backend, then merge them into the main branch.

## Objective
The objective of this lab is to demonstrate Git branching and merging workflows by:
1. Creating a Git repository with separate branches for frontend and backend development
2. Developing code in isolated branches
3. Merging the branches into the main branch to create a complete full-stack application
4. Understanding Git workflow best practices for collaborative development

## Tools / Technologies
- **Git**: Version control system for tracking changes
- **GitHub**: Remote repository hosting platform
- **Command Line Interface**: For executing Git commands
- **Text Editor**: For creating and editing code files
- **Python**: Backend development language
- **HTML/CSS**: Frontend development technologies

## Prerequisites
- Git installed and configured on the local machine
- GitHub account with repository access
- Basic understanding of command line operations
- Text editor or IDE for code development
- Python installed (for backend development)

## Steps / Commands

### Step 1: Initialize Git Repository
```bash
git init
git remote add origin <repository-url>
```

### Step 2: Create and Switch to Frontend Branch
```bash
git checkout -b frontend
```

### Step 3: Develop Frontend Code
Create frontend files and commit changes:
```bash
# Create frontend/index.html
git add frontend/
git commit -m "Add frontend HTML structure"
```

### Step 4: Create and Switch to Backend Branch
```bash
git checkout -b backend
```

### Step 5: Develop Backend Code
Create backend files and commit changes:
```bash
# Create backend/app.py
git add backend/
git commit -m "Add backend Python application"
```

### Step 6: Switch to Main Branch
```bash
git checkout master
```

### Step 7: Merge Frontend Branch
```bash
git merge frontend
```

### Step 8: Merge Backend Branch
```bash
git merge backend
```

### Step 9: Push to Remote Repository
```bash
git push origin master
```

## Expected Output / Result
- A complete Git repository with three branches: `master`, `frontend`, and `backend`
- Frontend branch containing HTML/CSS files
- Backend branch containing Python application files
- Main branch containing merged code from both frontend and backend branches
- Clean merge history showing the integration of both development streams

## Deliverables (what to push)
- `Labs/Lab01_Set_up_a_Git_repository_with_separate_br.md` (this file, completed)
- `Lab01_files/` directory containing:
  - `git_workflow_diagram.png` - Visual representation of the branching strategy
  - `merge_conflict_resolution.md` - Documentation of merge conflict handling
  - `branch_comparison.txt` - Output of git log showing branch history
  - `final_project_structure.txt` - Directory structure of the completed project

## Notes / Tips
- Always create feature branches from the main branch to maintain clean history
- Use descriptive commit messages to track changes effectively
- Test code in individual branches before merging to main
- Resolve merge conflicts carefully to maintain code integrity
- Keep branches focused on specific features or components
- Use `git log --oneline --graph` to visualize branch history
- Consider using pull requests for code review in collaborative environments
