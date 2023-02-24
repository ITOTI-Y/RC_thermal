# 🌤️基于 Numpy 的天空辐射制冷量计算

这个项目旨在使用 Numpy 实现天空辐射制冷量的计算，数据采用实测数据。可以单独计算平衡方程中的各个值。

## 📋 功能

- 针对实测数据计算天空辐射制冷量
- 单独计算平衡方程中的各个值

## 💻 系统要求

- Python 3.9+
- Numpy 1.24+

## 🚀 快速开始

### 安装

```shell
https://github.com/ITOTI-Y/RC_thermal.git
pip install -r requirements.txt
```

### 使用

```python
import pandas as pd
import numpy as np

# 读取实测数据
df_T = pd.read_csv('data/T_amb.csv', header=None)       # 辐射体温度/环境温度
df_e = pd.read_csv('data/cooler.csv', header=None)        # 辐射体发射率
df_a = pd.read_csv('data/cooler.csv', header=None)        # 辐射体吸收率
df_cc = pd.read_csv('data/cc.csv', header=None)        # 云层覆盖率
df_trans = pd.read_csv('data/trans.csv', header=None)  # 太阳辐射透过率
df_g = pd.read_csv('data/G.csv', header=None)       # 太阳辐射
df_v = pd.read_csv('data/V_wind.csv', header=None)  # 大气风速

# 单独计算平衡方程中的各个值
P_rad(),P_atm(),P_bld(),P_solar(),P_loss()

E_rad(),E_atm(),E_bld(),E_solar(),E_loss()
```
## 📜 License

[MIT](https://opensource.org/licenses/MIT)
