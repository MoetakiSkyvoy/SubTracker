# SubTracker - 个人订阅服务追踪器

**一个简洁、高效的个人订阅服务管理工具，帮助您掌控每一笔订阅开销，告别意外扣费。**

`SubTracker` 是一个基于 JavaEE + MyBatis 技术栈开发的Web应用，旨在解决现代数字生活中订阅服务繁多、难以管理的问题。通过一个直观的仪表盘和清晰的记录列表，您可以轻松追踪所有订阅服务的价格、付款周期和到期日。

## ✨ 主要功能

- **📊 仪表盘信息汇总**: 登录即可访问可视化仪表盘，快速概览每月总支出、即将到期的订阅等关键信息。
- **📝 订阅记录管理**: 对您的所有订阅服务进行完整的操作。
- **⏰ 到期预警**: 高亮显示在“预警时间”内即将到期的订阅，让您从容决定续费或取消。
- **📈 订阅时间轴**: 以类似甘特图的时间轴直观展示各项订阅的持续周期，财务状况一目了然。
- **🔍 分页与检索**: 高效地分页浏览和检索您的订阅记录。
- **🔐 安全的用户认证**: 提供独立、安全的用户注册和登录功能。
- **⚙️ 个性化设置**: 允许用户自定义分页大小、预警时间等参数。

## 📸 应用截图

| **仪表盘 (Dashboard)**       | **记录管理 (Records Management)** |
| ---------------------------- | --------------------------------- |
| *[此处放置仪表盘页面的截图]* | *[此处放置记录管理页面的截图]*    |

| **添加新订阅 (Add New Record)**       | **用户设置 (User Settings)**   |
| ------------------------------------- | ------------------------------ |
| *[此处放置添加/编辑弹窗或页面的截图]* | *[此处放置用户管理页面的截图]* |

## 🛠️ 技术栈

- **后端**:
  - JavaEE
  - MyBatis 3
  - Jackson (JSON处理)
- **数据库**:
  - MySQL 8.0
- **前端**:
  - HTML5, CSS3, JavaScript
  - AJAX
- **构建工具**:
  - Gradle (Groovy DSL)
- **服务器**:
  - Apache Tomcat

## 🚀 快速开始

请按照以下步骤在您的本地环境中部署和运行本项目。

### 1. 先决条件

- JDK 8 或更高版本
- Gradle 7.0 或更高版本
- MySQL 8.0 或更高版本

### 2. 安装步骤 (Installation)

1. **克隆仓库**

   ```
   git clone https://github.com/MoetakiSkyvoy/SubTracker.git
   cd SubTracker
   ```

2. **数据库设置**

   - 在您的MySQL服务器中创建一个新的数据库，例如 `subtracker_db`。
   - 执行 `/docs/sql/` 目录下的SQL脚本来创建数据表和初始化数据。

3. **配置项目**

   - 打开 `src/main/resources/mybatis-config.xml` 文件。
   - 修改 `<dataSource>` 部分的数据库连接信息，包括 `url`, `username`, 和 `password`。

4. **构建并运行**

   - 使用Gradle构建项目：

     ```
     gradle build
     ```

   - 将构建生成的 `build/libs/SubTracker-1.0.war` 文件部署到您的Tomcat服务器。

   - 启动Tomcat服务器。

   - 在浏览器中访问 `http://localhost:8080/SubTracker/` (路径可能因您的部署配置而异)。

## 📁 项目结构 (Project Structure)

```
SubTracker/
├── build.gradle        # Gradle构建脚本
├── LICENSE             # 开源协议
├── README.md           # 您正在阅读的文件
├── src/
│   ├── main/
│   │   ├── java/       # Java源代码
│   │   └── resources/  # 资源文件 (MyBatis配置, SQL映射等)
│   └── test/           # 测试代码
└── docs/
    └── sql/            # 数据库脚本
```

## 🤝 贡献指南

欢迎对本项目做出贡献！如果您有任何改进建议或发现了Bug，请随时提交 Pull Request 或创建 Issue。

1. Fork 本仓库
2. 创建您的功能分支 (`git checkout -b feature/AmazingFeature`)
3. 提交您的更改 (`git commit -m 'Add some AmazingFeature'`)
4. 推送到分支 (`git push origin feature/AmazingFeature`)
5. 打开一个 Pull Request

## 📄 开源协议

本项目采用 **MIT License** 开源协议。详情请见 LICENSE 文件。

## 📧 联系方式

MoetakiSkyvoy - [skyvoy@moetaki.com](mailto:skyvoy@moetaki.com)

项目链接: [https://github.com/MoetakiSkyvoy/SubTracker](https://github.com/MoetakiSkyvoy/SubTracker)
