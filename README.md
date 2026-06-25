# 智汇知识库 Vue 前端原型

基于 Vue 3、TypeScript、Pinia 和 Vue Router 构建的企业知识库高保真前端原型，包含 Web 端与小程序端。视觉参考用户提供的“智慧园区”样式，采用深海军蓝框架、白色内容区、企业蓝与青绿色状态色，不使用大面积渐变或玻璃拟态。

## 启动

```bash
npm install
npm run dev
```

生产构建：

```bash
npm run build
npm run preview
```

## 主要入口

- Web 端：`/web/workbench`
- 企业空间：`/web/enterprise`
- 个人空间：`/web/personal`
- 协作空间：`/web/collaboration`
- 与我相关：`/web/related`
- 安全外链：`/web/links`
- 误删恢复：`/web/recycle`
- 部门管理：`/web/admin/dept`
- 成员管理：`/web/admin/member`
- 管理员设置：`/web/admin/subadmin`
- 小程序端：`/mini`

## Iconify 在线图标

项目通过以下在线 Web Component 加载 Iconify 图标：

```html
<script src="https://code.iconify.design/iconify-icon/2.3.0/iconify-icon.min.js"></script>
```

通用操作图标统一采用 `solar` 图标集；Word、Excel、PowerPoint、PDF 等文件类型采用 `vscode-icons` 图标集。项目没有堆叠本地手写 SVG。

## 已实现原型交互

- 工作台空间入口、最近文件、待办和统计
- 企业/个人空间：上传、拖拽上传、新建文件夹、搜索、排序、列表/网格、预览、重命名、收藏、外链、软删除、详情抽屉
- 个人文件转入企业空间的组织资产确认
- 协作空间：新建、归档、群组文件、成员、动态与内部邀请
- 与我相关：共享给我、权限审批、文件收集
- 安全外链：创建、复制、公开访问预览、启停和删除
- 误删恢复：还原、还原到、批量还原和彻底删除确认
- 部门管理：组织树、新建/编辑/停用、资料库联动、默认权限、裁撤检查
- 成员管理：部门筛选、MDM 同步、添加、停用、查看与个人空间交接
- 管理员设置：范围授权、权限配置、启停、移交和删除
- 小程序：首页、文件、协作、消息、我的、搜索和快速新建底部弹层

原型数据保存在 Pinia 内存状态中，刷新页面后恢复初始演示数据。
