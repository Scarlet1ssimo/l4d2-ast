======================================================
！本插件包与本人的服务器的内容基本相同，
！但不保证内容与细节完全相同，
！同时不保证此插件包完全稳定，
！因此建议使用下方注明的服务器环境。

！若出现服务端崩溃等情况联系我也没有用，完全随缘更新。
！群号：819906811。
！QQ：448174863。

！此版本基于 Acemod 和 ZoneMod 制作。

！感谢所有在服务器和插件上帮助过我的人，
！感谢我所有的 Steam 好友：https://steamcommunity.com/id/larkspur2017/friends/

！不定期更新链接：https://dl.hykq.cc/?dir=L4D2/AstMod
！不定期更新链接：https://crowley.lanzous.com/b05mk1wub
======================================================



一、安装步骤：
    请参考 Zonemod：
        https://github.com/SirPlease/L4D2-Competitive-Rework/tree/master/Dedicated%20Server%20Install%20Guide
    以及六花的 Linux 服务端架设建教程（不完整，有些楼层被百度吞了，推荐看上面的）：
        https://tieba.baidu.com/p/4783601071?see_lz=1
        
    从旧版本更新：
        1. 备份 addons/sourcemod/configs/ 下的 Admin 配置、服务器名称、投票面板、公告，以及所有自行修改过的内容；
        2. 将此压缩包的文件覆盖到服务端；
        3. 恢复第一步备份的文件。



二、更换模式方法：
    /vote，更换模式；



三、其他说明：
    这套插件已经是我对 L4D2 和插件的理解的上限了，
    但是很多地方也没有仔细打磨，
    希望有能力的玩家可以自行修改。

    若出现服务器崩溃等情况联系我也没有用。

    1. 本人的服务器环境：
        Debian 10.4 64位。

    2. SteamCMD 无法运行，提示：“./steamcmd.sh： line 37： /root/steamcmd/linux32/steamcmd： No such file or directory.”：
        执行 apt install lib32gcc1

    3. 启动服务端方法：
        执行 ./run.sh，可自行编辑启动项。

    4. 关于启动项：
        +hostport                       端口；
        -nomaster                       完全隐藏服务器。

    5. 隐藏服务器两种方法：
        1) 启动项 -nomaster，完全隐藏，只能通过 connect ip:端口 连接；
        2) server.cfg 添加 sv_tags hidden，半隐藏，可通过 openserverbroswer 刷出。

    6. 常用配置文件：
        服务器名称：addons/configs/hostname/hostname.txt
        投票面板：addons/configs/cfgs.txt
        聊天公告：addons/configs/advertisements.txt
        不同人数方案：cfg/sourcemod/difficulty_adjustment_system/
        模式配置文件：cfg/confogl/模式名

    7. 关闭服务端：exit。
    
    8. 使用 ./run.sh 后打字不显示了，需要打开输入回显：stty echo。
