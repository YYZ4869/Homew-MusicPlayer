# MusicPlayer
## APP简介
*****
**这是一个iOS端音乐播放器APP，使用网易云音乐的数据，可以登录登录账号，查看歌单，进入播放界面，显示账号详情**

登录页采用伪登录，点击“forget your password"便可以进入主页

个人中心页显示账号的ID、头像、以及各种数据

首页显示推荐的歌曲以及歌单，我的歌单页显示账号收藏的歌单。点击歌单都可以进入歌单详情页。

点击歌曲便可以进入播放页面（由于技术原因暂不能实现播放、但保留界面）


## 技术要点及心得
****
项目架构 UITabBarController+UINavigationController
*参考资料：https://www.cnblogs.com/xufengyuan/p/6440733.html*     
网络请求基于AFNetWorking进行简单的封装    
页面布局除了用frame之外，还用了Masonry进行一些稍微复杂的页面布局    
首页瀑布流布局用了UICollectionView来实现，其他列表library和专辑歌单用UITableView实现，列表在数据请求完后，把数据储存在数组，然后reloaddata完成列表渲染。    




