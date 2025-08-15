<h1 id="esp32c3">关于使用esp32c3</h1>
<br/>
<p>在 <strong>Arduino|文件|首选项|其他开发板管理器地址</strong> 中填入</p>
<blockquote>
<p class="text-info">
https://espressif.github.io/arduino-esp32/package_esp32_index.json
https://espressif.github.io/arduino-esp32/package_esp32_dev_index_cn.json
</p>
</blockquote>

烧录时一定要把flash模式改成dio，合宙esp32c3仅支持dio，
如果是选择qio模式烧录了程序，板子是无限重启，串口会不断打印系统重启信息

# tft
[学习文档](https://www.cnblogs.com/jzcn/p/16687980.html)  
[csdn esp32c3开发tft屏幕](https://blog.csdn.net/qq_44715428/article/details/129537267?ops_request_misc=%257B%2522request%255Fid%2522%253A%2522f70ab1af5703f921ee4cec59687a06b9%2522%252C%2522scm%2522%253A%252220140713.130102334..%2522%257D&request_id=f70ab1af5703f921ee4cec59687a06b9&biz_id=0&utm_medium=distribute.pc_search_result.none-task-blog-2~all~sobaiduend~default-1-129537267-null-null.142^v102^control&utm_term=esp32c3%20tft%E5%B1%8F%E5%B9%95&spm=1018.2226.3001.4187)  
`tft.invertDisplay(true);`反转颜色
或者在User_Setup.h里用`#define TFT_INVERSION_ON`反转颜色  
`  tft.setRotation(x); #0~3`顺时针旋转90*X