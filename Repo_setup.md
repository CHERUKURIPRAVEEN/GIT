##Git global setup
```sh
   git config --global user.name "user"
   git config --global user.email "user@gmail.com"
```

###Create a new repository
```sh
  git clone <repo url>
  cd lg-multishop-category-service
  git switch -c main
  touch README.md
  git add README.md
  git commit -m "add README"
  git push -u origin main
```

###Push an existing folder
```sh 
  cd existing_folder
  git init --initial-branch=main
  git remote add origin http://gitlab-ce.lgcomus.lge.com/multishop/lg-multishop-category-service.git
  git add .
  git commit -m "Initial commit"
  git push -u origin main
```

####Push an existing Git repository
```sh
  cd existing_repo
  git remote rename origin old-origin
  git remote add origin http://gitlab-ce.lgcomus.lge.com/multishop/lg-multishop-category-service.git
  git push -u origin --all
  git push -u origin --tags
```
