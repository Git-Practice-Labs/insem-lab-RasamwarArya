# Merge Conflict Resolution Guide

## What are Merge Conflicts?
Merge conflicts occur when Git cannot automatically merge changes from different branches because the same lines of code have been modified in different ways.

## Common Scenarios
1. **Same file, different changes**: Two branches modify the same lines in a file
2. **File deletion**: One branch deletes a file while another modifies it
3. **Different file additions**: Both branches add files with the same name

## Resolution Steps

### 1. Identify the Conflict
```bash
git status
# Shows files with conflicts marked as "both modified"
```

### 2. Open Conflicted Files
Look for conflict markers:
```
<<<<<<< HEAD
Code from current branch
=======
Code from incoming branch
>>>>>>> branch-name
```

### 3. Resolve Conflicts
- Choose which version to keep
- Combine both versions if needed
- Remove conflict markers (`<<<<<<<`, `=======`, `>>>>>>>`)

### 4. Stage Resolved Files
```bash
git add <resolved-file>
```

### 5. Complete the Merge
```bash
git commit
```

## Best Practices
- Always test code after resolving conflicts
- Use merge tools for complex conflicts
- Communicate with team members about conflicting changes
- Keep commits small to minimize conflicts
