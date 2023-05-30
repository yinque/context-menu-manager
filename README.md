# context-menu-manager
便捷的windows右键菜单管理系统（待初始化）
# 介绍
管理windows右键菜单内容，禁用或者启用已有的菜单项。
# 开发计划
- [ ] 启用、禁用管理
- [ ] 筛选单个应用注册的菜单项
## 添加自定义功能
- [ ] 图片的快速压缩功能。右键图片文件，弹出压缩图片选项，展开选择压缩率，开始压缩图片
# 信息收集
https://learn.microsoft.com/en-us/windows/win32/shell/context-menu-handlers
## 菜单空间注册表映射
| 右键菜单项   | 注册表位置                                                   |
| ------------ | ------------------------------------------------------------ |
| 所有后缀文件 | HKEY_CLASSES_ROOT\*\shell                                  |
| 特定后缀文件 | HKEY_CLASSES_ROOT\\<.file_extension>\shell                  |
| 目录         | HKEY_CLASSES_ROOT\Directory\shell                          |
| 目录背景     | HKEY_CLASSES_ROOT\Directory\Background\shell               |
| 库文件夹背景 | HKEY_CLASSES_ROOT\LibraryFolder\Background\shell           |
| 文件夹       | HKEY_CLASSES_ROOT\Folder\shell                             |
| 压缩文件夹   | HKEY_CLASSES_ROOT\CompressedFolder\shell                   |
| 驱动器       | HKEY_CLASSES_ROOT\Drive\shell                              |
| 桌面         | HKEY_CLASSES_ROOT\DesktopBackground\shell                  |
| 发送到       | HKEY_CLASSES_ROOT\AllFilesystemObjects\shellex\ContextMenuHandlers\SendTo |
| 新建         | HKEY_CLASSES_ROOT\Directory\Background\shellex\ContextMenuHandlers\New |
| IE浏览器     | HKEY_CLASSES_ROOT\IE.AssocFile.<file_extension>\shell      |
| 此电脑       | HKEY_CLASSES_ROOT\CLSID\{20D04FE0-3AEA-1069-A2D8-08002B30309D}\shell |
| 快捷方式     | HKEY_CLASSES_ROOT\lnkfile\shell                            |
