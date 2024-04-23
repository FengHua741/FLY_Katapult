# FLY_Katapult
FLY工具板最新的katapult固件，目前只使用与CAN连接，请保证在普通用户下使用此固件包

## 1. 拉取固件包

```
cd && git clone https://github.com/FengHua741/FLY_Katapult.git
```

* 如果是固件可能随时更新建议使用前先执行下方命令

```
cd && cd ~/FLY_Katapult && git pull
```

## 2. 更新工具板固件

```
 ~/klippy-env/bin/python ~/klipper/lib/canboot/flash_can.py -f <Update firmware path>  -u <Toolboard ID>
```

* 需要将`<Update firmware path>`替换成固件路径比如 `~/FLY_Katapult/SHT36/FLY_SHT36V2_103_CANBOOT_1M.BIN`
* 需要将`<Toolboard ID>`替换成你的工具板ID比如说`72a773244776`

* 下方是参考命令

```
 ~/klippy-env/bin/python ~/klipper/lib/canboot/flash_can.py -f ~/FLY_Katapult/SHT36/FLY_SHT36V2_103_CANBOOT_1M.BIN  -u 72a773244776
```

