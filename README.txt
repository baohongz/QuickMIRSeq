# Check out empty repository (created in github account)
git clone https://github.com/username/ProjectName.git
cd ProjectName
git checkout --orphan gh-pages
cp -R path2result/Results/* .

# add all files at the current directory
git add .

# check file status
git status

# commit
git commit -a -m "Mouse miRNA Data Set"

# push (real uploading files)
git push origin gh-pages

git add README.txt 
git -a -m "Added README.txt"
git push origin gh-pages

# Added Rat Data Set
git add GSE60900_rat/.
git status
git commit -a -m "Added Rat Data Set"
git push origin gh-pages

# Added Human Data Set
git add GSE64977_human/.
git status
git commit -a -m "Added Human Data Set"
git push origin gh-pages
