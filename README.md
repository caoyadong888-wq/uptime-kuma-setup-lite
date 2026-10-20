# Uptime Kuma Setup Guide (Lite)

## English

A compose file for Uptime Kuma and three HTTP checks against `example.com`. The image tag is the variable `UPTIME_KUMA_IMAGE`. The container data path is `/app/data`. The host port is bound to `127.0.0.1`.

Not in this subset: the volume notes, the bilingual deploy checklist, the nginx examples, the v1-shaped JSON sample, and the summary script.

### Deliverables

- `deliverables/docker-compose.yml` — service with a variable image tag
- `deliverables/env.example` — marker tag; replace it before any pull
- `examples/monitors-http.csv` — GET and HEAD rows for `https://example.com`

Export `UPTIME_KUMA_IMAGE` from `env.example` before `docker compose config`. The marker tag is not a published tag. Check upstream docs. Do not start a container from this sample until the tag is one you confirmed.

## 中文

一份 Uptime Kuma 的 compose 文件，以及三条指向 `example.com` 的 HTTP 检查。镜像标签是变量 `UPTIME_KUMA_IMAGE`。容器数据路径是 `/app/data`。主机端口绑在 `127.0.0.1`。

精简版不含：数据卷说明、中英部署清单、nginx 示例、v1 形状的 JSON 样本，以及摘要脚本。

### 交付文件

- `deliverables/docker-compose.yml`
- `deliverables/env.example`
- `examples/monitors-http.csv`

执行 `docker compose config` 之前，先按 `env.example` 导出 `UPTIME_KUMA_IMAGE`。记号标签不是已发布的标签。以官方文档为准（check upstream docs）。确认标签之前不要启动容器。

Full version: GUMROAD_URL
