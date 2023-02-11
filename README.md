CUPS的Web界面v2.4.1汉化包 \
CUPS 2.4.1 Chinese Language Patch \
 \
从[TubroDog/CUPSChinesePatch](https://github.com/TubroDog/CUPSChinesePatch)复制过来，稍微改了一点。 \
2.2.10到2.4.1的菜单差异并没有比较，只是把影响我使用的一些改了。所以有可能不全。 \
 \
使用方法: \
直接用本项目的文件替换以下两目录下的对应的文件，直接刷新页面即可生效。 \
/usr/share/cups/doc-root/index.html \
/usr/share/cups/templates/*.tmpl



原因是我在配置文件下增加了DefaultLanguage zh_CN,发现并不起作用。官方有人提这个issue[#5763](https://github.com/apple/cups/issues/5763)，说浏览器的Request Header中的语言和这个匹配才会生效。 \
 \
强烈建议先备份原来的英文翻译，在doc-root和templates文件夹下建一个default.en文件夹(备份文件夹名称不要叫en，要不翻译还是不生效)，把doc-root/index.html和template/*.tmpl复制进去。 \
 \
注意：web管理界面的首页模板文件是放在/usr/share/cups/doc-root目录下 \
其他菜单的翻译在/usr/share/cups/doc-root/template目录下
