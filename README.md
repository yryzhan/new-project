## How to set up infrastructure

1. Create new repo folder:

    ```mkdir new-project```
2. Go to folder, init the repo and create README.md file

    ```
   cd new-project &&
   git init &&
   techo "# New Project" > README.md     
   ```
3. Commit changes
    ```
   git add README.md &&
   git commit -m "init" &&
   git branch development &&
   git checkout development
    ```
4. Add instruction to the README.md and commit changes
   
   ```
   git add README.md &&
   git commit -m "Add instructions"
   ```
5. Merge changes to the main branch
   ```
   git checkout main &&
   git merge development
   ```

6. Push changes to the remote
   ```
   git remote add origin https://github.com/yryzhan/new-project.git &&
   git push -u origin main
   ```