# 版本说明

- 规则参考：[语义化版本2.0.0](https://semver.org/lang/zh-CN/)
- 本项目规则：
  - 以 X.Y.Z 的形式定义版本号；
  - 初始版本号为：0.1.0；
  - 当进行任一版本值变更时，需进行文档记录；

| 版本格式 |           X            |           Y            |                       Z                        |
| :------: | :--------------------: | :--------------------: | :--------------------------------------------: |
|   版本   |         主版本         |        次版本号        |                     修订号                     |
|  值限定  |          >= 0          |          >= 0          |                      >= 0                      |
|  值递增  | 当次版本号累计10时 + 1 | 当进行功能性新增时 + 1 | 当进行 Bug 修复、<br/>引入插件等问题修正时 + 1 |
|   清0    |           /            |  当主版本号递增时 = 0  |         当主版本号或次版本号递增时 = 0         |

# 分支命名规范

- 格式：type/branch_version_function@name

  - type：类型
  - version：版本号
  - function：功能开发命名
  - name：开发者的名称
  
  ### 类型描述  Type：
  
  |  类型   |   描述   |
  | :-----: | :------: |
  | feature | 功能开发 |
  | hotfix  | 功能修复 |
  
  ### 分支简写 branch:
  
  | 命名 |  描述   |
  | :--: | :-----: |
  | dev  | develop |
  | rel  | release |

# Git 提交规范

- 格式：<类型> 说明内容 
- 示例：<feature> 框架功能上传； 

|  类型   |   使用情景   |                 提交资源格式                 |
| :-----: | :----------: | :------------------------------------------: |
| feature |    新功能    |               cs、txt、prefab                |
|   fix   |   Bug修复    |                   cs、txt                    |
|  style  | 代码规范修改 |                   cs、txt                    |
|  test   |   测试代码   |                   cs、txt                    |
|   ui    |   ui 资源    |           prefab、png、spriteatlas           |
|  anim   |   动画资源   | prefab、anim、controller、overrideController |
|   doc   |   文档更新   |           xlsx、pdf、docx、md、txt           |
|  scene  |   场景资源   |             prefab、scene、asset             |
| plugin  |     插件     |                      *                       |
|  misc   |   工程杂项   |                      *                       |
