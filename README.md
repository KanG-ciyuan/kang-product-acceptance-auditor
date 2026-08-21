# kang-product-acceptance-auditor

[![status](https://img.shields.io/badge/status-public%20release-2ea44f)](https://github.com/KanG-ciyuan/kang-product-acceptance-auditor/releases)
[![version](https://img.shields.io/github/v/release/KanG-ciyuan/kang-product-acceptance-auditor?label=version)](https://github.com/KanG-ciyuan/kang-product-acceptance-auditor/releases)
[![tests](https://img.shields.io/badge/local%20tests-1%20passed-2ea44f)](tests/)
[![license](https://img.shields.io/badge/license-Kang%20terms-6f42c1)](LICENSE)

Kang 的独立产品验收 Skill。用于从干净入口按真实用户场景验收外部改造方、员工、核验人员和企业负责人路径，并判断是否可以发布。

调用：`$kang-product-acceptance-auditor`

输入：已批准的产品契约和可观察运行证据。输出：场景、证据、严重度、阻塞项和 `pass` / `conditional_pass` / `fail`。它不在验收时修改代码。

## 你可以直接这样说

“使用 `$kang-product-acceptance-auditor` 从干净入口验收员工、核验人员和负责人路径，不要在验收中修代码。”

## 安装与验证

```bash
npx skills add KanG-ciyuan/kang-product-acceptance-auditor
python3 ~/.codex/skills/.system/skill-creator/scripts/quick_validate.py ~/.codex/skills/kang-product-acceptance-auditor
python3 ~/.codex/skills/kang-meta-skill/scripts/validate_skill.py ~/.codex/skills/kang-product-acceptance-auditor
```

## 前置条件

- [ ] 已准备已批准的产品契约
- [ ] 已准备可观察运行证据
- [ ] 已确认验收只读且独立

## Troubleshooting

如果没有干净入口或真实运行证据，标记 `missing evidence`，不要用 API 200 或按钮可见冒充通过。

## License

Copyright (c) Kang. See [LICENSE](LICENSE).

<!-- kang-author:start -->
## About Kang

Maintained by Kang. GitHub: https://github.com/KanG-ciyuan/

<!-- kang-author:end -->
