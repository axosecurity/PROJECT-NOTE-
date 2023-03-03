



@echo off

set datetime=%date% %time%
set datetime=%datetime:/=-%

rem change this ---------------------///////////

set notes_path=C:\Users\City Online Ltd\Pictures\note_test2

set github_username=axosecurity

set github_token=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

set repo_name=note_axo2

rem create the repository on GitHub

curl -H "Authorization: token %github_token%" -d "{\"name\":\"%repo_name%\"}" https://api.github.com/user/repos

rem push files to the repository

cd %notes_path%

git init
git remote add origin https://github.com/%github_username%/%repo_name%.git
git add .
git commit -m "Adding notes - %datetime%"


git push --set-upstream origin master

