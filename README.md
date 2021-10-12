# http
/****************************************************************************
http服务器搭建:
----------------------------------------------------------------------------
    搭建这个服务器的原因是兴趣所在；
----------------------------------------------------------------------------
    服务器很简陋，以后将一步步优化，加油！！
****************************************************************************/

各目录介绍：
    js：   该文件夹存放--html所需JavaScript脚本文件
    css：  该文件夹存放--html所需的css文件
    src：  该文件夹存放--c语言web服务器文件
    icon： 该文件夹存放--服务器需加载的图片文件
    Makefile：   编译工具
    app.html：   app主页面
    http：       c语言web服务器--可执行文件
    
服务器怎么运行：
    1、make编译工程，将会生产一个http的可执行文件
    2、运行服务器：./http（默认端口号8080） 
        或者 ./http  8080（8080指服务器的端口号，可自行指定）
    3、ifconfig查看本地ip地址
    4、修改app.js文件中的function get_file_from_server()函数
        将 url: "http://192.168.13.132:8080/app.html/allfile" 中的IP地址和端口号改成你的主机地址
          或者把ip地址改为 localhost:8080, 但这样修改，将只能在Ubuntu的浏览器中访问服务器
    5、访问服务器：浏览器输入 http://192.168.13.132:8080/app.html 即可
        或者 http://localhost:8080/app.html
    6、服务器启动成功
