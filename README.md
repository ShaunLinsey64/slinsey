mkdir -p ~/github-essentials
cd $_

echo "# github-essentials-v2" >> README.md
git init
git add README.md
git commit -m "first commit"
git remote add origin git@github.com:<username>/<repository>.git
git push -u origin master

git checkout -b add_description

echo "\n## Description\n\nGitHub for dummies" >> README.md
git add README.md
git commit -m "Add second level header to README file"
git push origin add_description
