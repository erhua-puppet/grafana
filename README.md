# grafana监控整套
# 使用docker-compose部署，已调试通过，运行前需给映射目录赋予可读写权限
# config按需添加配置
  chmod  777 data/grafana
  chmod  777 data/prometheus

# 目录结构如下：
grafana
├── config
│   ├── alertmanager.yml          #邮件配置
│   └── prometheus
│       ├── alert-node.yml        #告警监控项
│       ├── alert-rules.yml       #告警监控项
│       ├── cadvisor.yml          #监控容器
│       ├── node.yml              #监控主机
│       └── prometheus.yml        #
├── data
│   ├── grafana
│   │   ├── csv
│   │   ├── grafana.db
│   │   ├── plugins
│   │   │   └── camptocamp-prometheus-alertmanager-datasource
│   │   │       ├── CHANGELOG.md
│   │   │       ├── img
│   │   │       │   ├── json-logo.svg
│   │   │       │   ├── overview.png
│   │   │       │   └── table.png
│   │   │       ├── LICENSE
│   │   │       ├── MANIFEST.txt
│   │   │       ├── module.js
│   │   │       ├── module.js.map
│   │   │       ├── plugin.json
│   │   │       └── README.md
│   │   └── png
│   └── prometheus
│       ├── chunks_head
│       ├── queries.active
│       └── wal
│           ├── 00000000
│           ├── 00000001
│           ├── 00000002
│           ├── 00000003
│           ├── 00000004
│           └── 00000005
├── docker-compose_node.yml
└── docker-compose.yml





