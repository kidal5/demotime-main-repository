# demotime-main-repository

bash scripts to hand-test everything
```
# Initial state if repository
tree

# Currently no submodules are initialized, initialize all of them and check out `not-opt-in` submodules  
git submodule update --init
tree


# Changing to different branch do not updates submodules, can be verified by git status
git checkout differentBranch 
git status
tree

# Update submodules to sync them
git submodule update
git status
tree

# Checkout opt-in submodules
git submodule update --checkout
tree

# Switch branch, notice submodules not updated
git checkout main
git status
tree

# By using submodule update only `not-opt-in` submodules are updated
git submodule update
git status
tree

# By using --checkout, all submodules are updated
git submodule update --checkout
git status
tree
```
 


