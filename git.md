---
Index: "[[Linux Commands]]"
---

how to push a existing Dir to git repo 
~~~ bash
git remote add origin https://github.com/HeavyShadow18/Mr_Robot.git
git branch -M main
git push -u origin main
~~~

Creat a repo from the Cli
~~~bash 
echo "# Mr_Robot" >> README.md
git init
git add README.md
git commit -m "first commit"
git branch -M main
git remote add origin git@github.com:HeavyShadow18/Mr_Robot.git
git push -u origin main
~~~
