git常用命令大全 

	1.初始化本地git仓库（创建新仓库）
		git init
	2.clone远程仓库
		git clone 地址
	3.添加地址原点
		git remote add origin 地址
	4.查看当前版本状态（是否修改）
		git status
	5.添加到本地缓存
		git add .           //添加所有常用
		git add 文件名       //添加单个文件
	6.提交
		git commit -m "添加备注"     //常用
		git commit --amend -m 'xxx'     //合并上一次提交（用于反复修改）不常用
	7.将add和commit合为一步 
		git commit -am 'xxx'  
	8.新建分支/推送到远程
		git checkout -b 分支名称    //在本地新建分支x，并自动切换到该本地分支x
		git push origin 本地分支名 : 远程分支名     //远程没有此分支的时候用此命令 推送到远程分支
	9、查看分支  
		git fetch    //查看新分支
		git branch   //查看本地分支
		git branch -a  //查看本地及远程分支
	10.设置默认push当前分支
		 git config --global push.default "current"
	11.合并分支两步
		git merge dev  合并指定分支到当前分支 dev为分支名称
		git push origin  分支名称
	12.删除分支及远程分支
		git branch -d dev 删除分支本地分支
		git branch -r -D origin/dev1 删除本地的远程分支
	13.查看日志
		git log
	14.查看差异
		git diff
	15.git命令大全
		https://mp.weixin.qq.com/s?__biz=MzAwNjI5MTYyMw==&mid=2651494437&idx=1&sn=d88dc74a24305c0e69365094ae1e4b1d&chksm=80f191edb78618fb86cfa5784d403f0774b1ac47a0c3b19280d16e5d954cd19b5e4e23af85d6&scene=0&key=8e7349a2eeff6e43903220471f96eb056446a05ed599c108938519b8134dff47ed6c39f3eb91aad978583d2cb114014de59113766d42ec38181dee163683deb57cbae97050cf77280a4dd9eea0b1f7e4&ascene=0&uin=MjAwODg0MjE2MA%3D%3D&devicetype=iMac+Macmini7%2C1+OSX+OSX+10.10+build(14A389)&version=12020110&nettype=WIFI&fontScale=100&pass_ticket=PE4FcNApWvZeuKq3cE%2BAAppkHf8iYq%2FZThJTgAeDGiRYHtVfJE5QPHBJht9Jwq6f