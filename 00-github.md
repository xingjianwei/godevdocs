# github

## create a new repository on the command line
```
echo "# godevdocs" >> README.md
git init
git add README.md
git commit -m "first commit"
git remote add origin https://github.com/xingjianwei/godevdocs.git
git push -u origin master
```

## push an existing repository from the command line
```
git remote add origin https://github.com/xingjianwei/godevdocs.git
git push -u origin master
```

## syncing a fork
```
git remote -v
git remote add upstream https://github.com/ORIGINAL_OWNER/ORIGINAL_REPOSITORY.git
git fetch upstream
git checkout master
git merge upstream/master
```