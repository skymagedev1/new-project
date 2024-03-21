echo "# new-project" >> README.md

git init

git add README.md

git commit -m "init"

git remote add origin git@github.com:account/new-project.git

git push -u origin main

git checkout -b development

echo "# some changes" >> README.md

git add README.md

git commit -m "changed README file"

git push origin development

git checkout main

git merge development

git push origin main