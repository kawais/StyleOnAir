作为一个没有mac，没有iphone，使用google play版微信的开发，每次要调试微信浏览器里面页面样式的时候，感觉就像吃了狗屎一样难受，简直不能忍。于是写了这个可以在不同设备同步css的工具。可以一边在pc上调样式，一边在手机上看效果。

支持内联样式、style标签、同源css文件的样式修改同步。

## 使用
1. 克隆
2. 安装依赖 npm i
3. 启动服务 npm run run
4. 在html页面中加入client js <script src="http://ip:port/client.js"></script>
5. 在各设备打开页面，点击右下角SOA文字弹出设置项目
6. 点击Start开始同步

## 注意
1. SOA黄色为暂停状态，绿色为同步状态。绿色时才能发送、接受样式修改。
2. 勾选Sync Click Event可以在设备间同步click事件。
3. 在chrome调试工具中就行的修改才能同步。
4. 修改跨域css文件内的样式无法同步。