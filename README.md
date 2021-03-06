# 云存储管理客户端 v0.2.2
![](http://blog-res.mayday5.me/niu_128.png?imageView2/1/w/30/h/30/q/75|imageslim)
> 云存储管理客户端。支持七牛云、腾讯云、青云。仿文件夹式管理、图片预览、拖拽上传、文件夹上传、同步、批量导出URL等功能

## 效果图
【目前已支持 七牛云、腾讯云、青云】
![%E5%B1%8F%E5%B9%95%E5%BF%AB%E7%85%A7%202018-11-20%20%E4%B8%8B%E5%8D%883.50.48.png](http://blog-res.mayday5.me/img/%E5%B1%8F%E5%B9%95%E5%BF%AB%E7%85%A7%202018-11-20%20%E4%B8%8B%E5%8D%883.50.48.png)

【多选 按住 mac:command win:ctrl】
![qiniuClient-1.0.0截图1.png](http://blog-res.mayday5.me/img/%E5%B1%8F%E5%B9%95%E5%BF%AB%E7%85%A7%202018-10-24%20%E4%B8%8B%E5%8D%885.10.48.png)

【右键菜单&dark 配色】
![qiniuClient-1.0.0截图2.png](http://blog-res.mayday5.me/img/%E5%B1%8F%E5%B9%95%E5%BF%AB%E7%85%A7%202018-10-24%20%E4%B8%8B%E5%8D%885.05.42.png)

## 更新说明
2018.12.07
***
- 腾讯云支持自定义域名
- 设置页面添加https开关
- 新增支持**阿里云**对象存储
- fix:windwos 不显示通知
2018.11.19
***
- 支持资源URL批量导出
- 应用内直接浏览图片
- 新增支持**青云**对象存储

2018.11.06
***
- 支持同步功能啦 [规则说明](https://github.com/willnewii/qiniuClient/wiki/bucket%E5%90%8C%E6%AD%A5%E8%A7%84%E5%88%99)

2018.10.30
***
- 增加dark配色(mac会自动判断,您也可以在设置页手动设置)
- 支持**腾讯云**对象存储
- 支持搜索功能(默认会读取您COS的全部文件列表,这样就可以支持模糊查询,坏处就是bucket切换特别慢...)
- 优化了大空间(主要是文件个数多)的加载.
- 模拟目录显示,方便文件归类

old
***
- 文件的增、删,同时也支持文件夹的批量上传和删除啦
- 文件按日期/大小 排序和筛选
- URL上传,现在URL也支持批量上传了
    - 七牛提供了API,可以直接通过url抓取文件并保存到七牛.如果你经常有先从别的网站下载,然后在上传至七牛云的操作,这个功能应该对你有帮助
- 托盘上传
    - mac的特性,方便快捷,谁用谁知道.致敬一下[iPic](https://toolinbox.net/iPic/)
- 拖拽上传
    - O__O "… 本来是看别人有才做的...后来发现还挺好用
- 图片模式
    - 显示预览图,如果您有维护图片的需求,这个功能还算实用.
- 私有空间操作([说明](https://github.com/willnewii/qiniuClient/wiki/%E4%B8%83%E7%89%9B%E7%A7%81%E6%9C%89%E7%A9%BA%E9%97%B4%E5%92%8C%E6%8E%88%E6%9D%83%E7%A9%BA%E9%97%B4%E5%A4%84%E7%90%86)）

## 下载
- [mac v0.2.2](http://blog-res.mayday5.me/file/%E4%BA%91%E5%AD%98%E5%82%A8%E7%AE%A1%E7%90%86%E5%AE%A2%E6%88%B7%E7%AB%AF-0.2.2-1207-mac.dmg)
- [win v0.2.0](http://blog-res.mayday5.me/file/COS%E7%AE%A1%E7%90%86%E5%AE%A2%E6%88%B7%E7%AB%AF-0.2.0-win_2.exe)

## Build Setup
``` bash
# 安装依赖
npm i
# 运行开发模式
npm run dev

# 构建对应你的平台的安装包
npm run build:mac
npm run build:win32
```

## Technologies
- [electron](https://github.com/electron/electron)
- [electron-vue](https://github.com/SimulatedGREG/electron-vue)
- [vue2.0 + axios + router + vuex](https://github.com/vuejs/vue)
- [iview 3.0](https://github.com/iview/iview)
- [v-contextmenu '右键菜单'](https://github.com/snokier/v-contextmenu)
- [vue-virtual-scroll-list](https://github.com/tangbc/vue-virtual-scroll-list)

## 参考资料
- [图标来源：懒人图库](http://www.lanrentuku.com/vector/animal/lansexinxianniunaibiaoqian-shiliang.html)
- [electron 文档](https://github.com/electron/electron/tree/master/docs-translations/zh-CN)
- [electron-vue 文档](https://simulatedgreg.gitbooks.io/electron-vue/cn/)
- [七牛API](https://developer.qiniu.com/kodo/api/1731/api-overview)
- [webpack2 文档](https://doc.webpack-china.org)
- [Node.js 文档](http://nodejs.cn/api/)
- [electron.build cli 文档](https://www.electron.build/cli)
