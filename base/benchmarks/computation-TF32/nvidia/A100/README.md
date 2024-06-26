# 参评AI芯片信息

* 厂商：Nvidia


* 产品名称：A800
* 产品型号：A800-80GiB-SXM
* TDP：400W

# 所用服务器配置

* 服务器数量：1


* 单服务器内使用卡数：8
* 服务器型号：DGX A100
* 操作系统版本：Ubuntu 20.04.1 LTS
* 操作系统内核：linux5.4.0-126
* CPU：AMD EPYC7742-64core
* docker版本：20.10.18
* 内存：1TiB
* 服务器间AI芯片直连规格及带宽：此评测无需此项配置

# 评测结果

## 核心评测结果

| 评测项  | TF32算力测试值(8卡平均) | TF32算力标定值(8卡平均) | 测试标定比例(8卡平均) |
| ---- | --------------- | --------------- | ------------ |
| 评测结果 | 123.68TFLOPS    | 156TFLOPS       | 79.3%        |

## 能耗监控结果

| 监控项  | 系统平均功耗  | 系统最大功耗  | 系统功耗标准差 | 单机TDP | 单卡平均功耗(8卡平均) | 单卡最大功耗(8卡最大) | 单卡功耗标准差(8卡最大) | 单卡TDP |
| ---- | ------- | ------- | ------- | ----- | ------------ | ------------ | ------------- | ----- |
| 监控结果 | 4368.6W | 4368.0W | 0W      | /     | 383.5W       | 414.0W       | 79.8W         | 400W  |

## 其他重要监控结果

| 监控项  | 系统平均CPU占用 | 系统平均内存占用 | 单卡平均温度(8卡平均) | 单卡平均显存占用(8卡平均) |
| ---- | --------- | -------- | ------------ | -------------- |
| 监控结果 | 3.571%    | 2.273%   | 63.36°C      | 3.046%         |
