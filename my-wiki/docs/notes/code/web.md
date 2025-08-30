localStorage 是一种 Web 存储机制，
允许网站在用户的浏览器中存储数据，即使浏览器关闭后数据仍然保留。  
`localStorage.setItem('hideDevSitePopup', 'true');`
这行代码的作用是将键 'hideDevSitePopup' 和值 'true' 存储到
浏览器的 localStorage 中。这样，即使用户关闭了浏览器，再次访问网站时，
这个键值对仍然存在。  
- 关联：`localStorage.getItem(hideDevSitePopup)`获取已保存键的值
