# 4. 物理机服务 {#4}

物理机服务是指将物理裸机以服务的形式提供给云的租户使用，通常用来承载一些高性能应用或者不适合云化的应用（比如Oracle RAC）。KingStack支持基于Linux通用镜像启动物理机。如果租户要是Windows操作系统，需通过物理裸机的IPMI控制台自行安装操作系统。

操作权限说明如下：

| 角色名称 | 查看 | 创建/复制 | 更新 | 删除 | 
| :--- | :--- | :--- | :--- | :--- |
| Admin | √（public/private） | √（public/private） | √（public/private） | √（public/private） |
| Serviceadmin | -- | -- | -- | -- |
| Maintenanceadmin | -- | -- | -- | -- |
| Owner | √（public/private） | √（public/private） | √（public/private） | √（public/private） |
| Member | √（private） | √（private） | √（private） | √（private） |

以下将以Admin权限举例描述。

## 4.1 创建物理机 {#4-1}

1. 登录金山私有云平台，点击左侧导航条中的『物理机』 -> 『物理机管理』，在右侧云主机管理页面，点击『创建物理机』。
2. 在弹出的『创建物理机』对话框中输入物理机名称、物理机所属资源池，同时选择登录方式。然后点击下一步即可。

























