# FLY_Katapult

    * 包含最新FLY全部主板的Katapult与BL


## Katapult固件更新Katapult速率方法

    * 请注意需要Katapult固件更新原来的Katapult固件需要使用developer目录下的Katapult固件
    * 此方法是直接通过CAN更新工具板原有的Katapult固件
        ```bash
        ~/klippy-env/bin/python ~/klipper/lib/canboot/flash_can.py -f <Update firmware path>  -u <Toolboard ID>
        ```

    * 需要将`<Update firmware path>`替换成固件路径比如 `~/FLY_Katapult/developer/SHT36/FLY_SHT36V2_103_1M.bin`
    * 需要将`<Toolboard ID>`替换成你的工具板ID比如说`72a773244776`

    * 下方是参考命令
        ```bash
        ~/klippy-env/bin/python ~/klipper/lib/canboot/flash_can.py -f ~/FLY_Katapult/developer/SHT36/FLY_SHT36V2_103_1M.bin  -u 72a773244776
        ```

