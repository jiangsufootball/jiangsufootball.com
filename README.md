# 江苏城市足球联赛赛事网（jiangsufootball.com）

> 本项目是面向江苏地区的城市足球联赛赛事信息展示与管理平台，基于 Python/Django + PostgreSQL 技术栈开发，致力于服务本地足球爱好者和赛事组织者。

## 项目简介

本系统为江苏各地足球联赛提供全面的信息展示，包括赛程发布、比分查询、球队与球员管理、成绩统计等功能，支持多城市、多赛季协同，助力江苏足球事业发展。

## 功能特色

- **赛事信息展示**：实时发布与查询城市足球联赛赛程、比分和结果
- **球队与球员管理**：球队注册、球员信息维护、阵容展示
- **成绩统计与排行榜**：自动统计比赛数据，生成积分榜、射手榜等
- **后台管理系统**：赛事组织者可维护比赛、球队、球员等数据
- **多城市多赛季支持**：适应江苏省多地赛事需求
- **数据导出分享**：支持赛程和成绩数据导出，便于分享和媒体报道

## 技术栈

- **后端**：Python 3.x, Django 4.x
- **数据库**：PostgreSQL
- **前端**：Django 模板 / Bootstrap / Vue.js（如有单独前端项目可补充说明）
- **环境与部署**：Docker, GitHub Actions (CI/CD)

## 环境搭建与运行

### 1. 克隆代码仓库

```bash
git clone https://github.com/xincanzhecom/jiangsufootball.git
cd jiangsufootball
```

### 2. 创建虚拟环境并安装依赖

```bash
python3 -m venv venv
source venv/bin/activate  # Mac/Linux
venv\Scripts\activate     # Windows

pip install -r requirements.txt
```

### 3. 配置环境变量

- 复制 `.env.example` 文件为 `.env`，并根据实际情况填写 PostgreSQL 数据库连接信息及 Django 配置。

### 4. 初始化数据库

确保 PostgreSQL 服务已运行，并已创建数据库和用户。

```bash
python manage.py migrate
```

### 5. 创建超级管理员账号

```bash
python manage.py createsuperuser
```

### 6. 启动开发服务器

```bash
python manage.py runserver
```

浏览器访问：[http://localhost:8000](http://localhost:8000)

---

## Docker 一键部署（可选）

如需快速部署，可使用 Docker：

```bash
docker-compose up -d
```

详见仓库中的 `docker-compose.yml` 文件。

---

## 参与贡献

欢迎开发者、足球爱好者参与到本项目建设：

- Bug反馈和建议：请通过 [Issues](https://github.com/xincanzhecom/jiangsufootball/issues) 提交
- 代码贡献：Fork 仓库并提交 Pull Request
- 其他贡献：文档、UI 设计、测试、翻译等

贡献流程参考 [CONTRIBUTING.md](./CONTRIBUTING.md)。

---

## 开源协议

本项目采用 MIT 许可证，详见 [LICENSE](./LICENSE)。

---

## 联系方式

- 官方网站：[JIANGSUFOOTBALL.COM](https://jiangsufootball.com)
- 邮箱：info@jiangsufootball.com
- 微信/QQ群：请在 Issues 留言获取最新交流群信息

---

感谢每一位为江苏足球和开源社区做出贡献的朋友！
