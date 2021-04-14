# Microsoft SQL Server安装和使用

## 一、安装

0. 准备安装文件;
1. 进入安装中心：可以参考硬件和软件要求、可以看到一些说明文档；
2. 选择全新安装模式继续安装；
3. 输入产品秘钥：这里使用演示秘钥进行；
4. 在协议中，点击同意，并点击下一步按钮，继续安装；
5. 进入全局规则检查项，这里可能要花费几秒钟，试具体情况而定；
6. 配置更新项，推荐检查更新；
7. 选择安装更新的具体内容；
8. 安装程序文件；
9. 安装规则检查；
10. 安装功能选择（可全选）；
11. 实例配置，使用默认即可（如果之前安装过，这里需要特别注意下）；
12. PolyBase配置选择--默认即可；
13. 服务器配置--默认即可；
14. 引擎配置--建议使用混合模式，并记住密码；
15. Analysis Service配置--推荐使用使用默认；
16. Reporting Services配置--推荐使用使用默认；
17. Distributed Replay控制器配置---推荐使用使用默认（添加当前用户）；
18. Distributed Replay 客户端配置--推荐使用使用默认；
19. 协议授权，接受协议；
20. 最后安装确认页面，会显示所有的安装配置信息；
21. 等待安装进度--这一步会消耗比较长的时间，在虚拟机里面耗时15分钟左右；
22. 继续等待--较耗时；
23. 安装完毕，退出安装程序。


## 二、导入数据库文件

1. 登陆SQL Server Management Studio，选择：数据库引擎、windows身份验证、服务器类型(local)；
2. 右击“对象资源管理器”中的数据库文件夹，新建一个数据库，并命名；
3. 右击新建的数据库，选择：任务 -> 还原 -> 数据库；
4. 点击“源设备”，选择本地的待还原数据库文件；
5. 在出现的选项栏中点击左侧的选项，勾选“覆盖现有的数据库”；
6. 点击确定，开始还原。