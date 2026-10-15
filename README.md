# 南京工业大学开源软件仓库名录：政策正文

这是 [主站](https://github.com/He0xD4C0/njtech-oss-namelist) 使用的中英双语政策源。EULA 对应 terms.md，另外两份也是网站注册所需的政策正文。

```text
zh-CN/
  privacy.md
  terms.md
  inclusion.md
en-US/
  privacy.md
  terms.md
  inclusion.md
```

## 网站接入

将政策正文源设为 `https://github.com/He0xD4C0/njtech-oss-eula.git`，触发“同步政策正文”。网站匿名读取默认分支的普通文件，每种语言必须三份非空正文齐全；目录与文件名区分大小写。不要嵌套目录、使用符号链接或提交编译产物。正文为 UTF-8 CommonMark，避免 HTML、YAML front matter 和依赖插件的表格。

页面为 `/policies/privacy/`、`/policies/terms/`、`/policies/inclusion/`，以 `?language=zh-CN` 或 `?language=en-US` 选择语言。Git SHA 标识实际导入的正文来源；发布仓库不会自动配置或部署网站。

## 运营信息

正文普通文字中的 `{{ operator_name }}` 和 `{{ operator_contact_email }}` 由主站“运营主体名称”和“公开联系邮箱”可选设置代入。缺省显示“本站运营者 / Site operator”和“联系邮箱未设置 / Contact email not set”，不推断学校官方身份，不读取管理员私有邮箱或 SMTP 发件邮箱。需要主站具备这两项字段及代入功能；旧版本会原样显示占位符。

代入仅针对 Markdown 普通文字，不执行模板语法，不替换链接目标或代码。不要把变量写成 mailto 链接。两种语言共用后台填写值，只有缺省文字按正文语言切换。配置有独立审计记录，正文 SHA 和注册同意版本不包含配置值。

允许技术缺省不代表运营身份或隐私告知已完整。实际启用前，运营者应按部署补充真实主体和联系方式、邮件与存储服务商、地点、具体保存周期及适用的跨境处理安排；正文不编造这些信息。条款适用性应由实际运营者确认，本仓库不是法律审查完成的证明。

## 维护

同时审阅中英对应文件，保持含义一致。正文依据主站实际实现：个人直接归属的公开仓库、完整文本机审、无手动放行、归档不失格、移除/解绑/注销撤下展示、基于实际观测的封存榜单。行为变化时更新相应政策。发布新正文不等于已有用户已重新同意。

文档独立编写，参考 [个人信息保护法](https://www.cac.gov.cn/2021-08/20/c_1631050028355286.htm) 的告知与权利框架和 [Turnstile 隐私附录](https://www.cloudflare.com/turnstile-privacy-policy/)。[许可证策略仓库](https://github.com/He0xD4C0/njtech-oss-license-policy) 独立维护许可证正文和分类。

政策不替代主站或第三方项目的软件许可证，也不授予对大学名称、标识或第三方作品的额外权利。仓库 Issue 用于不含敏感信息的文字勘误；账号及隐私请求应使用网站配置的联系方式。
