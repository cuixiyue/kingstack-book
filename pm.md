# 4. 物理机服务 {#4}

物理机服务是指将物理裸机以服务的形式提供给云的租户使用，通常用来承载一些高性能应用或者不适合云化的应用（比如Oracle RAC）。KingStack支持基于Linux通用镜像启动物理机。如果租户要是Windows操作系统，需通过物理裸机的IPMI控制台自行安装操作系统。

操作权限说明如下：

| 角色名称 | 查看 | 创建/复制 | 编辑 | 删除 | 
| :--- | :--- | :--- | :--- | :--- |
| Admin | √ | √ | √ | √ |
| Serviceadmin | -- | -- | -- | -- |
| Maintenanceadmin | -- | -- | -- | -- |
| Owner | √ | √ | √ | √ |
| Member | √ | √ | √ | √ |

以下将以Admin权限举例描述。

## 4.1 查看物理机列表 {#4-1}

登录金山私有云平台，点击左侧导航条中的『物理机』。

右侧物理机管理主界面会以列表的方式列出在当前项目下的所有物理机。

列表的右上角列出对物理机的三项基本操作『开机』、『关机』和『创建』方便用户对物理机的快捷操作，『更多操作』收录了物理机相关的其他操作。
在物理机列表中每一行显示物理机的相关信息，包括名称，状态，IP地址，监控状态，操作系统，所属网络区域，所属资源池，创建时间（支持按创建时间对物理机进行正向或逆向排序），以及物理机的所属项目和用户。

## 4.2 创建物理机 {#4-2}

#### 创建物理机实例步骤

1. 登录金山私有云平台，点击左侧导航条中的『物理机』 -> 『物理机管理』，在右侧云主机管理页面，点击『创建物理机』。
2. 在弹出的『创建物理机』对话框中输入物理机名称、物理机所属资源池，同时选择登录方式。然后点击下一步。
3. 选择物理机的镜像，输入物理机名称、物理机所属资源池，同时选择选择物理机的镜像，然后点击创建即可。

#### 配置选项

- 通用配置

| 选项 | 描述 |
| :--- | :--- |
| 物理机名称 | 物理机的名字 |
| 资源池 | 此物理机所属的资源池 |
| 选择镜像 | 当前只支持通用Linux镜像<br/>Windows操作系统需要通过IPMI接口安装 |

- 可选配置

| 选项 | 描述 |
| :--- | :--- |
| 登录方式 | 默认为密码登录<br/>勾选后采用证书登录(SSH密钥) |

## 4.3 更多物理机操作 {#4-3}

| 操作 | 描述 |
| :--- | :--- |
| 迁移监控服务 |迁移监控数据到指定服务器|
| 创建监控 | 为物理机创建监控 |
| 修改监控 | 修改监控项 |
| 停止监控 | 停止对物理机进行监控 |
| 删除物理机 | 删除此物理机 |




































































































































































































































































































































































































































