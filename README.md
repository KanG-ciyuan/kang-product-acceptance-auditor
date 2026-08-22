# kang-product-acceptance-auditor

[![status](https://img.shields.io/badge/status-public%20release-2ea44f)](https://github.com/KanG-ciyuan/kang-product-acceptance-auditor/releases)
[![version](https://img.shields.io/github/v/release/KanG-ciyuan/kang-product-acceptance-auditor?label=version)](https://github.com/KanG-ciyuan/kang-product-acceptance-auditor/releases)
[![tests](https://img.shields.io/badge/contract%20tests-3-2ea44f)](tests/)
[![license](https://img.shields.io/badge/license-MIT-6f42c1)](LICENSE)

Kang 的独立产品验收数字员工 Skill。适用于 SaaS、内部工具、工作流和数字服务，从干净入口按已批准的真实用户场景验收任务、权限、交接、恢复和发布阻塞。

调用：`$kang-product-acceptance-auditor`

输入：已批准的产品契约、目标用户、关键场景、权限和可运行环境。输出：可复现场景记录、运行证据、严重度、阻塞项和 `pass` / `conditional_pass` / `fail` / `not_testable`。它不在验收时修改代码。

## 你可以直接这样说

“使用 `$kang-product-acceptance-auditor` 从干净入口验收作者、编辑、法务从投稿到发布的路径，不要在验收中修代码。”

## 安装与验证

```bash
npx skills add KanG-ciyuan/kang-product-acceptance-auditor
python3 ~/.codex/skills/.system/skill-creator/scripts/quick_validate.py ~/.codex/skills/kang-product-acceptance-auditor
python3 ~/.codex/skills/kang-meta-skill/scripts/validate_skill.py ~/.codex/skills/kang-product-acceptance-auditor
```

## 前置条件

- [ ] 已准备已批准的产品契约和关键场景
- [ ] 已准备干净入口、身份和可观察运行环境
- [ ] 已确认验收只读且独立

## Troubleshooting

如果没有契约、干净入口或真实运行证据，标记 `not_testable` / `missing evidence`，不要用 API 200、按钮可见或单测通过冒充产品通过。

## License

MIT. See [LICENSE](LICENSE). This is a reusable product-development agent Skill, separate from any private enterprise product.

<!-- kang-author:start -->
## About Kang

Maintained by Kang. GitHub: https://github.com/KanG-ciyuan/

<!-- kang-author:end -->
