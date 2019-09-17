# FreeSwitch-Train-doc
···
目录
一、 通信发展历程	7
  1.  电话的发明者	7
  2.  第一代结构	7
  3. 第二代	8
  4. 第三代	8
  5. 第四代	9
二、 呼叫中心和IPPBX的区别	10
  IPPBX的说明	10
  呼叫中心的说明	10
三、 FreeSWITCH的安装	10
  A. Windows下安装	10
  B. CentOS下安装	11
  C. Debian安装	13
四、 FreeSWITCH的音频通话	16
  A. FreeSWITCH启动及查看	16
  查看启动与否	19
  fs_cli 连接不了本机的freeswitch	21
  查看本机freeswitch的运行状态	21
  查看sip相关的状态	21
  添加一个新的用户	22
  FreeSWITCH中的路由配置	22
  B. linphone配置	23
  C. linphone通话及FreeSWITCH日志查看	24
五、 使用FreeSWITCH作为视频通话服务器	26
  A. 配置视频相关	26
  B. Linphone配置视频通话	28
  C．FreeSWITCH视频会议相关	29
六、 FreeSWITCH与外线连接	29
  A. 与sangoma板卡相连	29
  B. 与网关或Voip外线连接	29
七、 FreeSWITCH与WEBRTC	30
  A. 什么是WEBRTC	30
  B.  让FreeSWITCH支持WEBRTC	30
  C. 使用Jssip来实现webrtc通话	31
  D. Sip.js与Odoo与FreeSWITCH结合	31
八、 FreeSWITCH的彩铃和IVR	32
  A. 来去电回应	32
  B. Ring的格式及转码	32
  C. IVR配置	32
九、 FreeSWITCH的API与 APP	33
十、 FreeSWITCH Inbound连接	33
十一、 FreeSWITCH Outbound连接	34
十二、 FreeSWITCH与LUA	35
  A.什么是 Lua	35
  B. 在FreeSWITCH中如何调用Lua	36
  C. 使用lua与数据库协助FreeSWITCH管理用户	36
十三、 其它与FreeSWITCH相关的开发语言	36
十四、智能客服、外呼	37
十五、语音实时识别	37
十六、FSGui介绍	38
十七、 如何使用开发语言来实现自己对FS ESL的调用	39
  ESL消息类型	39
  ESL通信类型	39
  ESL数据结构	40
附录一：	41
安装问题	41
源码快速git地址	41
到底如何选择一个版本	42
如何去编译某个模块	42
如何选择一个操作系统	43
如何在centos上安装libyuv,vpx,opus,libpng,libav	43
如何在centos上快速源码编译一套freeswitch	44
如何让freeswitch支持h264	44
如何让freeswitch支持postgresql	45
使用问题	45
如何增加一个分机帐号	45
如何动态增加一个分机帐号	45
FreeSWITCH 使用域名注册	46
有关透传号码及由平台发起呼叫或回拨	46
如何采用esl inbound处理路由	46
如何采用esl outbound处理路由	46
如何向一个正在通话的通道中送dtmf	47
如何配置mrcp	47
Freeswitch配置外呼并录音	47
ESL中获取是呼入fs还是由fs 呼出的	48
ESL中如何收DTMF	48
代码重启fs	49
允许或限制多终端注册	49
如何设置一个FS服务器支持的并发数？	49
如何设置一个FS服务器每秒呼叫数	49
如何设置一个FS服务器的rtp端口范围	49
如何修改一个编码的ptime	49
如何一直保持某个呼入不被挂断	49
将接通的电话转至conference	50
从fs_cli查看相关具体的事件	50
中止当前某个通道上的操作	50
查看fs中相关sip profile信息	50
开启sip包跟踪	50
变更日志级别	50
发送（180 RINGING）的效果	50
重新注册网关	50
fs监听某个通话	51
使用esl监听	51
Fs同步系统时间	51
优化一、采用内存数据库	52
优化二、使用jemalloc	52
FreeSWITCH与线路网关对接(IP认证)	53
FreeSWITCH与线路采用密码验证	53
如何设置最长通话时间	54
FreeSwitch中用户不经过认证即可注册成功	54
如何设置不听远程的彩铃，按自己的设置放彩铃	54
设置呼转的号码是多个且同时振铃，当有一个接听后，其它就不再振铃	54
设置呼转的号码是多个且顺序振铃，当有一个接听后，其它就不再振铃	54
某个路由必须走某种编码	54
如何在外呼时，让其送出的号码不是’0000000’	55
控制通话的音量	55
fs转发客户端的自定义头	55
如何使用postgresql记录freeswitch话单	55
修改sdp中的fs名称	56
如何做一个fs的级联	56
Fs中如果放公网需要开放的端口（默认）	57
由平台先呼a再呼b时，先放彩铃再听回铃再接通	57
平台外呼后放音再转座席	57
如何调整 jitterbuffer	57
FreeSwitch网关轮询模块mod_distributor	57
遇到本机8021fs_cli连fs不上	61
使用webrtc时没声音或提示Remote Address Error!	61
遇到总是提示domain 被acl拒绝	61
刚安装好，使用时总是延时十秒才呼叫	61
修改默认密码	62
Webrtc中candidate 多个ip地址	62
fs在内网，但要处理公网上的请求	62
关闭rtp自动调整	63
修改默认的sip端口	63
ULIMIT 配置	63
在哪里去检查语音通话的质量	63
如何查看已注册的相关分机	64
在dialplan xml中检查文件是否存在	64
如何调整fs_cli中日志显示的级别	64
呼叫保持和恢复	65
expand的使用	65
limit_execute的使用	65
控制呼叫频率	65
控制呼出总数	65
重新加载external配的网关	66
呼叫保持和恢复	66
让通话接通后放音	66
如何让fs回复一个值，如486	66
放在内网的goip注册到公网中的fs如何呼叫	66
如何判断是由先挂机	66
如何快速查看fs使用中的通道变量	66
Freeswitch通道变量	67
选择G711还是G729？	83
添加sip头，用于非标的一些sip server	83
强行注销一个sip分机或重启	84
让fs内核使用postgresql数据库	84
录音最短时间	84
当b路挂机后继续走路由	84
freeswitch将sip日志写入文件	84
如何设置P-Asserted-Identity	85
让freeswitch通话进行变声	85
限制5080送入需要认证才能呼叫	85
让客户端定时发送注册包	85
让fs转发info	85
fs1.6.7以后默认不转码处理	85
调试xml_curl	85
用于控制originate的一些参数	86
示倒，用pocketsphinx实现的说省会城市就放音	86
Auto Changing audio port 是什么设置导致的？	94
有的移动ims没有彩铃	94
无法二次拨号，DTMF不能用	94
接通后报工号	94
fs 的 invite中的几个头参数	94
FreeSwitch模块mod_unimrcp配置数据库化初探	95
如果是移动运营商开启了volte的ims，因为100rel而没有回铃如何处理	97
附录二、上海宁卫产品列表	98
通信运营平台	98
呼叫中心中间件FSGUI	98
智能外呼、智能客服	99
语音实时质检	99
宁卫SBC	100
···
