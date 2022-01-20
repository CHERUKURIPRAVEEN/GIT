# Get All Branches in Local repo

### First clone the repo
```sh
   git clone <repo url> 
```

### Create a below getAllBranches.sh
```sh 
   for branch in `git branch -a | grep remotes | grep -v HEAD | grep -v master `; do
     git branch --track ${branch#remotes/origin/} $branch
   done
```

### Run below commands
```sh 
   chmod +x getAllBranches.sh    
   sh getAllBranches.sh 
   
   git branche
```
