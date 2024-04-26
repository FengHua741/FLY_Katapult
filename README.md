# FLY_Katapult

包含最新FLY工具板最新的Katapult与普通主板的BL，使用要求如下:

* 可以搜索到CANID
* CAN缓存为1024
* 建议安装好FLY_Tools,方便切换速率
* 请不要使用红米,WIFI棒子与魔改的上位机，可能会导致失败！！！

## 1. 拉取固件包

```
cd && git clone https://github.com/FengHua741/FLY_Katapult.git
```

* 如果是固件可能随时更新建议使用前先执行下方命令

```
cd ~/FLY_Katapult && git pull && cd
```

## 2. 更新工具板Katapult固件

* 请注意需要Katapult固件更新原来的Katapult固件需要使用developer目录下的Katapult固件

* 此方法是直接通过CAN更新工具板原有的Katapult固件

```
 ~/klippy-env/bin/python ~/klipper/lib/canboot/flash_can.py -f <Update firmware path>  -u <Toolboard ID>
```

* 需要将`<Update firmware path>`替换成固件路径比如 `~/FLY_Katapult/developer/SHT36/FLY_SHT36V2_103_1M.bin`
* 需要将`<Toolboard ID>`替换成你的工具板ID比如说`72a773244776`

* 下方是参考命令

```
 ~/klippy-env/bin/python ~/klipper/lib/canboot/flash_can.py -f ~/FLY_Katapult/developer/SHT36/FLY_SHT36V2_103_1M.bin  -u 72a773244776
```

