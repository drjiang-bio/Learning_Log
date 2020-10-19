1. 安装git, 然后在Rstudio中设定git.exe所在目录
2. 在Rstudio中Create RSA Key或者用现有的
3. 将上述Key复制到github(Settings)
4. shell命令：
```
  git config --global user.email "youremail@gmail.com"
  git config --global user.name "yourname"
  ssh -T git@github.com
  使用GitHub上的名字
```
5. github上新建repository, 按照第一个方法复制代码在shell中运行（本地--远程）
6. 在Rstuido中新建项目--使用现有目录


…or create a new repository on the command line
```
echo "# project_methy_new" >> README.md
git init
git add README.md
git commit -m "first commit"
git branch -M main
git remote add origin git@github.com:drjiang-bio/project_methy_new.git
git push -u origin main
```

…or push an existing repository from the command line
```
git remote add origin git@github.com:drjiang-bio/project_methy_new.git
git branch -M main
git push -u origin main
```

…or import code from another repository
You can initialize this repository with code from a Subversion, Mercurial, or TFS project.
