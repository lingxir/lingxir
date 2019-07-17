// Javascript code with syntax highlighting.
var fun = function lang(l) {
  dateformat.i18n = require('./lang/' + l)
  return true;
}

# Ruby code with syntax highlighting
GitHubPages::Dependencies.gems.each do |gem, version|
  s.add_dependency(gem, "= #{version}")
end

<html>
<body style="background-color:https://github.com/lingxir/lingxir.github.io/blob/lingxir-patch-2/%E8%90%BD%E9%9C%9C_109951163990747016.jpg">
</body>
</html>
#꧁凌؀希꧂博客
##adb方法
![ace](https://raw.githubusercontent.com/lingxir/lingxir.github.io/42cec4b115529cc3e0ef27ba465868bba87c0f0d/Screenshot_20190606_044708_com.tencent.qqlive.jpg)

⒈教你如何使用安卓手机给另一部安卓手机刷机相信大家都熟知如何使用电脑来为安卓手机进行刷机。
可大家有尝试过用手机给另一部手机刷机吗？
⒉（这里主要说明的是adb+fastboot方式）
前提准备：两部安卓手机（系统版本最好是安卓4.4.4及以上的，
至少有一台支持otg功能，host必须获取了root权限）          
⒊一条OTG数据线如何开始：我们将用来给另一部安卓机刷机的手机称之为（host），
将被用来刷机的手机称之为（target）首先host用的安卓系统版本如果是4.4.4及其以上的一般都自带adb这个客户端程序而却没有fastboot这个命令行程序所以我们得在host上部署fastboot及其他可能会使用到的工具。
下载群文件里的fastboot，然后把fastboot拷贝到/system/bin或/system/xbin（这个倒无所谓，不过需要root）再赋予可执行权限，再安装好终端模拟器。
注意：fastboot使用的是针对arm架构的交叉编译工具链静态编译得到的，
所以这两个命令行工具只能用于arm架构处理器的安卓机!
上述工具部署完毕后，
host便可以通过OTG数据线和标准数据线来连接target了，
后面host就可以在终端下通过使用这些命令行工具来给target进行刷机了。
本人使用魅蓝2（host）来为米4移动4G版（target）进行刷机测试完美通过，
理论上针对可以进fastboot模式的安卓机都可以(对于有bl锁的机器，部分机型可解锁)
