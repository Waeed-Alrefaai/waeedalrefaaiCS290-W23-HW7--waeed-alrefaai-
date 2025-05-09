# waeedalrefaai
greet

git clone <https://github.com/Waeed-Alrefaai/waeedalrefaaiCS290-W23-HW7--waeed-alrefaai-/commit/56f595da9e2379b670921e36f2106495d6cd18ff>
```
git add fileA.txt
```
git commit -m "commit (A): fileA.txt content"
```
Replace `"commit (A): fileA.txt content"` with your own commit message.
git push origin master

git branch master
```
git checkout master
```
git add fileA.txt
```
git commit -m "commit (B): add fileA.txt" -p A
```
Replace `"commit (B): add fileA.txt"` with your own commit message.

The `-p A` flag specifies that the new commit has a parent commit `A`.
git push origin master
```
Enter your GitHub username and password when prompted to complete the push.

git branch feature1 master
```
git checkout feature1
git add fileA.txt
git commit -m "commit (C): add feature 1" -p B
git push origin feature1

git checkout feature1
```
git add fileA.txt
```
git commit -m "commit (D): feature 1 enhancement" -p C
```
Replace `"commit (D): feature 1 enhancement"` with your own commit message.

The `-p C` flag specifies that the new commit has a parent commit `C`.
git push origin feature1
```
Enter your GitHub username and password when prompted to complete the push.
git checkout master
```
git merge --no-ff feature1
```
This will create a merge commit that combines the changes from the `feature1` branch into the `master` branch. The `--no-ff` flag ensures that a merge commit is created even if it's not a fast-forward merge.
git add fileA.txt
```
git commit -m "Merge branch 'feature1'" -p B -p D
```
Replace `"Merge branch 'feature1'"` with your own commit message.
The `-p B -p D` flag specifies that the new commit has two parent commits, `B` and `D`, representing the commits from the `master` and `feature1` branches respectively.
git tag v1.0
```
This will create a tag named `v1.0` for the commit.
git push origin master --tags
```
Enter your GitHub username and password when prompted to complete the push.
git branch -d feature1
git push origin --delete feature1

git checkout master
```
git branch feature2
```
git checkout feature2
```
git add fileA.txt
```
git commit -m "commit (F): add feature 2" -p E
```
Replace `"commit (F): add feature 2"` with your own commit message.

The `-p E` flag specifies that the new commit has a parent commit `E`.
git push origin feature2
```
Enter your GitHub username and password when prompted to complete the push.

git checkout master
```
git branch Bugfix
git checkout Bugfix
git add fileA.txt
git commit -m "commit (G): fix feature 1 bug" -p E
git push origin Bugfix

git checkout master
````
git merge --no-ff Bugfix
````
This will create a merge commit that combines the changes from the `Bugfix` branch into the `master` branch. The `--no-ff` flag ensures that a merge commit is created even if it's not a fast-forward merge.
git add fileA.txt
````
git commit -m "Merge branch 'Bugfix'" -p E -p G
````
Replace `"Merge branch 'Bugfix'"` with your own commit message.
The `-p E -p G` flag specifies that the new commit has two parent commits, `E` and `G`, representing the commits from the `master` and `Bugfix` branches respectively.
git tag v1.01
````
This will create a tag named `v1.01` for the commit.
git push origin master --tags
````
Enter your GitHub username and password when prompted to complete the push.
git branch -d Bugfix
git push origin --delete Bugfix
git checkout master
```
git merge feature2
```
This will create a merge commit that combines the changes from the `feature2` branch into the `master` branch.
Note: This step may result in a merge conflict since both `F` and `H` modify the `fileA.txt` in different ways. You will need to resolve the conflict before proceeding.
git add fileA.txt
```
git commit -m "Merge branch 'feature2'" -p F -p H
```
Replace `"Merge branch 'feature2'"` with your own commit message.
The `-p F -p H` flag specifies that the new commit has two parent commits, `F` and `H`, representing the commits from the `feature1` and `Bugfix` branches respectively.
git push origin master
```
Enter your GitHub username and password when prompted to complete the push.


git clone <https://github.com/Waeed-Alrefaai/waeedalrefaaiCS290-W23-HW7--waeed-alrefaai-/commit/56f595da9e2379b670921e36f2106495d6cd18ff>
```

git checkout master


git merge feature2

git add fileA.txt


git commit -m "Merge branch 'feature2'" -p F -p H


git push origin master


git branch -d feature2


git push origin --delete feature2





