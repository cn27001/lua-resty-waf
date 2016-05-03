# lua-resty-waf

lua-resty-waf 是一款开源的入侵检测系统。


##版权声明
    本软件、包含相应的过滤规则等文件遵从AGPL许可协议, 版权属于上海守茂网络科技有限公司。

###用途：
    	
	防止sql注入，本地包含，部分溢出，fuzzing测试，xss,SSRF等web攻击
	防止svn/备份之类文件泄漏
	防止ApacheBench之类压力测试工具的攻击
	屏蔽常见的扫描黑客工具，扫描器
	屏蔽异常的网络请求
	屏蔽图片附件类目录php执行权限
	防止webshell上传


###使用说明：

默认安装目录为:/usr/local/openresty/



###配置文件详细说明：
        
###检查规则是否生效

部署完毕可以尝试如下命令：        
  
        curl http://xxxx/test.php?id=../etc/passwd
        返回警报信息字样，说明规则生效。

注意:默认，本机在白名单不过滤，可自行调整config.lua配置



##安装

    curl -fsSL http://www.smnode.com/smstatic/script/install_openresty.sh | bash

##交流QQ群
    323865245


## 守茂网络科技 Copyright
