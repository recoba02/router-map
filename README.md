# 目录

* [路由器CPU性能排行榜](#路由器CPU性能排行榜)
* [路由器无线性能排行榜](#路由器无线性能排行榜)

# 路由器CPU性能排行榜

鉴于通常情况下小伙伴们使用一个主路由（硬路由）实现各种业务功能，此时路由器的CPU负责绝大部分工作，故以CPU跑分成绩作为主要的考量标准。

跑分成绩多来源于互联网及小伙伴们的热心贡献，数值并非完全精确，仅供参考。目前跑分多以 `aes-128-gcm` 为标准，部分数据可能为 `aes-128-cbc` 结果，如有出入过大，欢迎及时指正。

```bash
openssl speed -evp aes-128-gcm
```

```bash
openssl speed -multi $(cat /proc/cpuinfo |grep processor | wc -l) -evp aes-128-gcm
```

| 典型设备      | CPU     | 频率(GHz) | 架构       | 加速 | AES单线程 | AES多线程 | DMIPS |
|-------------|--------- |----------|---------- |-----|---------:|---------:|------:|
| 华硕RT-AX89X | IPQ8074  | 2.2 x 4  | A53 14nm  | Y   | 785498   | 3101794  | 18400 |
| 华硕AX88U    | BCM4908  | 1.8 x 4  | A53 28nm  | Y   | 695583   | 2684741  | 16560 |
| 华硕AX92U    | BCM4906  | 1.8 x 2  | A53 28nm  | Y   | 696541   | 1358529  | 8280  |
| 小米AX3600   | IPQ8071A | 1.4 x 4  | A53 14nm  | Y   |    |   |  |
| 网件R7800    | IPQ8065  | 1.7 x 2  | Krait 300 |    |    |   |  |
| 网件R7500V2  | IPQ8064  | 1.4 x 2  | Krait 300 |    |    |   |  |
| 小米AX1800   | IPQ6000  | 1.2 x 4  | A53 14nm  | Y   | 322654   | 1268751  | 11040 |
| 华为AX3 Pro  | Hi5651T  | 1.4 x 4  | A53 28nm  |    |    |   | 12880 |
| 华为AX3      | Hi5651L  | 1.2 x 4  | A53 28nm  |    |    |   | 5520 |
| 网件R9000    | AL314P   | 1.7 x 4  | A15 28nm  |    |    |   |  |
| 华硕AX56U    | BCM6755  | 1.5 x 4  | A7 28nm   | N   | 38805    | 111395   | 11400 |
| 华硕AX3000   | BCM6750  | 1.5 x 3  | A7 28nm   | N   | 37865    | 72714    | 8550  |
| 某讯K3       | BCM4709  | 1.4 x 2  | A9 40nm   | N   | 25771    | 49662    |       |
| 小米AX6000   | IPQ5018  | 1.0 x 2  | A53 14nm  |    |    |   | 4600  |
| 网件6300V2   | BCM4708  | 0.8 x 2  | A9 40nm   | N   | 14811    | 29145    |       |
| 某讯K2P      | MT7621   | 0.88 x 2 | MIPS      | N   | 7165     | 14623    | 2640  |
| 某讯K3C      | GRX350   | 0.8 x 2  | MIPS      | N   |      |     |   |
| 华硕ACRH17   | IPQ4019  | 0.72 x 4 | A7        |    |      |     |   |
| 华硕n66u     | BCM4706  | 0.6 x 1  | MIPS      | N   |      |     |   |


# 路由器无线性能排行榜

规划中

