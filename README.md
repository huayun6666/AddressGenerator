# 随机地址生成器

## 预览地址
[随机地址生成器](https://addr.jiangnan24.com/)


## 简介

这是一个基于 Cloudflare Workers 的随机地址生成器，可以生成全球多个国家的真实地址、姓名和电话号码。
本项目基于[Real-Address-Generator](https://github.com/Adonis142857/Real-Address-Generator)做了一些样式和逻辑上的调整和优化。

## 主要功能

- 支持多个国家/地区的地址生成
- 根据不同国家生成符合当地特色的姓名
- 生成符合各国格式的电话号码
- 实时地图预览
- 地址保存和管理
- 一键复制信息

## 部署到 Cloudflare Workers

在Cloudflare创建一个worker项目，把[woker.js](https://raw.githubusercontent.com/jiangnan1224/AddressGenerator/refs/heads/main/worker.js) 代码内容复制到worker项目内部署即可。

## 技术栈

- Cloudflare Workers
- TailwindCSS
- OpenStreetMap API (用于地址验证)
- Google Maps (用于地图显示)

## 注意事项

- 地址生成基于 OpenStreetMap API，请遵守其使用条款
- 建议在生产环境中设置适当的 CORS 策略
- 如需自定义国家/地区数据，可以修改 `countryCoordinates`、`namesByCountry` 和 `phoneFormats` 对象

## 许可证

MIT License

## 贡献

欢迎提交 Issue 和 Pull Request！

## 致谢

- OpenStreetMap 提供地理数据支持
- Google Maps 提供地图显示服务
- Cloudflare 提供托管服务
- [Real-Address-Generator](https://github.com/Adonis142857/Real-Address-Generator)
