# 参评AI芯片信息

* 厂商：Nvidia


* 产品名称：A100
* 产品型号：A100-40GiB-SXM
* TDP：400W

# 所用服务器配置

* 服务器数量：1


* 单服务器内使用卡数：1
* 服务器型号：DGX A100
* 操作系统版本：Ubuntu 20.04.4 LTS
* 操作系统内核：linux5.4.0-113
* CPU：AMD EPYC7742-64core
* docker版本：20.10.16
* 内存：1TiB
* 服务器间AI芯片直连规格及带宽：此评测项不涉及服务期间AI芯片直连

# 算子库版本

https://github.com/FlagOpen/FlagGems. Commit ID:9168f2d031ecc1b31a9f658fb66dd6735b7306b3

# 评测结果

## 核心评测结果

| 评测项  | 平均相对误差(with FP64-CPU) | TFLOPS(cpu wall clock) | TFLOPS(kernel clock) | FU(FLOPS Utilization)-cputime | FU-kerneltime |
| ---- | -------------- | -------------- | ------------ | ------ | ----- |
| flaggems | 0.00E+00    | /  | /        | / | / |
| nativetorch | 0.00E+00    | /  | /      | /      | /    |

## 其他评测结果

| 评测项  | 相对误差(with FP64-CPU)标准差 | cputime | kerneltime | cputime吞吐 | kerneltime吞吐 | 无预热时延 | 预热后时延 |
| ---- | -------------- | -------------- | ------------ | ------------ | -------------- | -------------- | ------------ |
| flaggems | 0.00E+00    | 108940.43us       | 106414.08us        | 9.18op/s | 9.4op/s | 279049.06us | 98172.16us |
| nativetorch | 0.00E+00    | 100299.41us       | 96353.28us        | 9.97op/s | 10.38op/s | 270552.12us | 96428.79us |

## 能耗监控结果

| 监控项  | 系统平均功耗  | 系统最大功耗  | 系统功耗标准差 | 单机TDP | 单卡平均功耗 | 单卡最大功耗 | 单卡功耗标准差 | 单卡TDP |
| ---- | ------- | ------- | ------- | ----- | ------------ | ------------ | ------------- | ----- |
| nativetorch监控结果 | 1560.0W | 1560.0W | 0.0W   | /     | 59.96W       | 62.0W      | 1.89W        | 1560.0  |
| flaggems监控结果 | 1560.0W | 1560.0W | 0.0W   | /     | 60.33W       | 62.0W      | 1.55W        | 1560.0  |

## 其他重要监控结果

| 监控项  | 系统平均CPU占用 | 系统平均内存占用 | 单卡平均温度 | 单卡最大显存占用 |
| ---- | --------- | -------- | ------------ | -------------- |
| nativetorch监控结果 | 19.861%    | 1.719%   | 32.85°C       | 1.828%        |
| flaggems监控结果 | 19.185%    | 1.73%   | 33.29°C       | 1.034%        |