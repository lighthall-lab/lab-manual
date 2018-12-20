[Return to Table of Contents](readme.md#table-of-contents)

# Procedures

## GitHub Workflow

### Creating a new analysis branch
1. `git branch Analysis-Name`

### Modifying an ongoing analysis branch
1. `git checkout Analysis-Name`
3. `cp existing-analysis-file new-analysis-file`
    1. `cp existing-other-analysis-file new-other-analysis-file`
    - ~ make changes to your code ~
4. `git add new-analysis file`
    1. `git add new-other-analysis-file`
5. `git commit -m "made some changes like blah blah blah"`

### Send your changes to GitHub
5. `git push --set-upstream origin Analysis-Name`

### Open a Pull Request
Once your analysis branch is in a stable state, checked and tested:
1. Open a pull request
    1. Have the code reviewed by project head, discuss, etc.
2. Project head merge the completed analysis branch into master and delete branch
3. Finally: update the local repository with newly merged `origin master`
    1. `git checkout master`
    2. `git pull origin master`
    3. `git branch -d analysis-name`
