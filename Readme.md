1. Create directory baru 
mkdir Git_de
cd Git_de

2. Initialize git repository
git init

3. Set up GitHub username and email
git config user.name "dimas"
git config user.email "dzipras1@gmail.com"

4. Create a new branch named 'main' (if main branch doesn't exist)
git checkout -b main

## Project Operations

5. Create a new file and modify and existing one
touch test.txt
nano test.txt

6. Create a new branch for adding a file
git checkout -b add/file
<!-- as the brach add/file already created in session before, I just switched into branch -->
git checkout add/file

7. Add files to staging
git add .

8. Commit changes
git commit -m "adding redme file and test.txt"

0. Check the last 2 commits
git log -n2

10. Stash changes for later if it's a WIP(Work in Progress)
git stash

11. Switch back to main branch
<!-- if main branch already exists -->
git checkout main  

If main branch doesn't exist:
git checkout -b main

11. Adding new lines in test
nano test.txt

12. Adding test.txt to staging
git add test.txt

13. Commit changes in test.txt
git commit -m "manambahkan beberapa lines"

14. Adding Readme.md ke staging
<!-- as i had clicked publish the Readme.md file gone and con't be recvoer 
then adding new Readme.md file-->
touch Readme.md
git add Readme.md

15. Commit changes in Readme.md
<!-- commit changes in Readme.md -->
git commit -m "menambahkan Readme.md yg ditelan bumi"

16. Log in simpler form
git log --oneline

17. Create new bracnch 
git checkout -b add/features

18. add some lines to Readme.md
19. git add Readme.md then commit the changes
git add Readme.md
git commit -m "add failed line"

<!-- theres some folder should be deleted and commit the change -->
20. stage the deletion, and other file and commit the change
git rm belajar_git/test.txt
git add db_latihan-1.code-workspace
git commit -m "delete and staging other untracked working file"

21. Merge add/features branch ke add/file
git checkout add/file
git merge add/features

<!-- Conflicted -->
git add db_latihan-1.code-workspace
git commit -m "commit conflict"

22. Push branch baru ke remote
git remote -v  <!-- cek dulu ada remote atau engga -->
git remote add origin https://github.com/DimasPrsety/db_latihan_2.git <!-- add origin -->
git branch -M main <!-- rename branch ke main -->
git push -u origin main <!-- push local branch ke remote repo -->

23. Create Pull Request

32. Merge branch baru ke main
git merge add/file