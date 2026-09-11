# 一个关于git以及github使用的学习记录~~（也许不只是git 也有markdown）~~  

## 准备一个github账户  
github账户的注册相当简单没有繁复的各种验证，我们只需要准备一个干净的邮箱就可以了  
当初注册github账户还是为了在上边下些有趣程序（~~不得不说这可比某盘好用，什么都搜得到~~ **赞美伟大的开源社区！！！**
  
## 关于github仓库
GitHub是相当好用的开源平台，限制其使用的或许只有我的英语水平இдஇ~~这英语是非学不可吗~~  
无论是吧编程语言还是学习工具或是软件大多是英文的（什么？你说可以用自然语言vibe coding 那可需要不少钱，先生

## 关于git使用
就像和chat对话debug时最常用的是CTRL+C和CTRL+V，对我而言git毋庸置疑git clone，git pull，git push。（汗
### 一些尝试
#### 我如果改了平台上的仓库名字，那么我在push的时候会自动更新本地仓库名吗？
更改仓库名对于push应该是没有影响的，clone拉取的是那个网址（根据查的资料说会重定向，也就是按照之前的网址，之后自动跳转到新网址，都是同一个仓库，前提是之前的仓库名没有被再次使用）  
但是**本地仓库名不会变化。**
```PS C:\Users\86199\Desktop\QD-LEARNING\Jotang-2026-recruit> git push
To https://github.com/KPK5432154/Jotang-2026-recruit.git
 ! [rejected]        main -> main (non-fast-forward)
error: failed to push some refs to 'https://github.com/KPK5432154/Jotang-2026-recruit.git'
hint: Updates were rejected because the tip of your current branch is behind
hint: its remote counterpart. If you want to integrate the remote changes,
hint: use 'git pull' before pushing again.
hint: See the 'Note about fast-forwards' in 'git push --help' for details.
```
噢噢噢，试图push但是忘记在网页改过一点readme.md
现在需要先pull再push 
但是**本地仓库名都没有变化。**
#### 那么怎么才能同步仓库名字呢？
根据资料和ai，我需要重新设置远程仓库地址
```
git remote -v//查看当前的远程地址
origin  https://github.com/KPK5432154/Jotang-2026-recruit.git (fetch)
origin  https://github.com/KPK5432154/Jotang-2026-recruit.git (push)
```
说明这是之前的地址，现在是Jotang-2026-recruit-git
```
git remote set-url [类][地址]//重新设置远程仓库地址

git remote set-url origin https://github.com/KPK5432154/Jotang-2026-recruit-git.git
git remote -v
origin  https://github.com/KPK5432154/Jotang-2026-recruit-git.git (fetch)
origin  https://github.com/KPK5432154/Jotang-2026-recruit-git.git (push)
 
```
但是**本地仓库名字还是没有变化**  
我检索了一些资料，最简单的方法应该就是直接改文件名就好了...

## *未完待续......*