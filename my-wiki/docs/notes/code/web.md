localStorage 是一种 Web 存储机制，
允许网站在用户的浏览器中存储数据，即使浏览器关闭后数据仍然保留。  
`localStorage.setItem('hideDevSitePopup', 'true');`
这行代码的作用是将键 'hideDevSitePopup' 和值 'true' 存储到
浏览器的 localStorage 中。这样，即使用户关闭了浏览器，再次访问网站时，
这个键值对仍然存在。  
- 关联：`localStorage.getItem(hideDevSitePopup)`获取已保存键的值


---
[关于edge开启远程调试](https://learn.microsoft.com/zh-cn/microsoft-edge/devtools/remote-debugging/windows#install-and-configure-microsoft-edge) 
[csdn教程](https://blog.csdn.net/tjb132/article/details/136655986)  
edge输入edge://flags  
找到`Enable remote debugging through Windows Device Portal`将该标志设置为 `Enabled`

在完全关闭浏览器情况下，命令行输入`msedge.exe --remote-debugging-port=9222`  
然后访问 `http://127.0.0.1:9222/json` 如果看到一个包含当前打开的标签页信息的 JSON 列表，说明远程调试已成功启用。  
- 可以在“目标”字段中，添加 --remote-debugging-port=9222 参数。例如：
`"C:\Program Files (x86)\Microsoft\Edge\Application\msedge.exe" --remote-debugging-port=9222`