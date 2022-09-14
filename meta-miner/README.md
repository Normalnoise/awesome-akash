# Algo switching CPU miner by MoneroOcean

## Check mm.js builtin help

```
Usage: mm.js [<config_file.json>] [options]
Adding algo switching support to *any* stratum miner
<config_file.json> is file name of config file to load before parsing options (mm.json by default)
Config file and options should define at least one pool and miner:
Options:
        --pool=<pool> (-p):             <pool> is in pool_address:pool_port format, where pool_port can be <port_number> or ssl<port_number>
        --host=<hostname>:              defines host that will be used for miner connections (localhost 127.0.0.1 by default)
        --port=<number>:                defines port that will be used for miner connections (3333 by default)
        --user=<wallet> (-u):           <wallet> to use as pool user login (will be taken from the first miner otherwise)
        --pass=<miner_id>:              <miner_id> to use as pool pass login (will be taken from the first miner otherwise)
        --perf_<algo>=<hashrate>        Sets hashrate for algo that is: rx/0, rx/wow, cn/r, cn-pico/trtl, cn-heavy/xhv, cn/gpu, argon2/chukwa, k12, c29s, c29v, c29b, kawpow, ethash, autolykos2, panthera, ghostrider
        --algo_min_time=<seconds>       Sets <seconds> minimum time pool should keep our miner on one algo (0 default, set higher for starting miners)
        --miner=<command_line> (-m):    <command_line> to start smart miner that can report algo itself
        --<algo>=<command_line>:        <command_line> to start miner for <algo> that can not report it itself
        --watchdog=<seconds> (-w):      restart miner if is does not submit work for <seconds> (600 by default, 0 to disable)
        --hashrate_watchdog=<percent>:  restart miner if is hashrate dropped below <percent> value of of its expected hashrate (0 by default to disable)
        --miner_stdin:                  enables stdin (input) in miner
        --quiet (-q):                   do not show miner output during configuration and also less messages
        --verbose (-v):                 show more messages
        --debug:                        show pool and miner messages
        --log=<file_name>:              <file_name> of output log
        --no-config-save:               Do not save config file
        --help (-help,-h,-?):           Prints this help text
```


## Developer Donations

If you'd like to make an one time donation, the addresses are as follows:

* XMR - ```89TxfrUmqJJcb1V124WsUzA78Xa3UYHt7Bg8RGMhXVeZYPN8cE5CZEk58Y1m23ZMLHN7wYeJ9da5n5MXharEjrm41hSnWHL```
* AEON - ```WmsEg3RuUKCcEvFBtXcqRnGYfiqGJLP1FGBYiNMgrcdUjZ8iMcUn2tdcz59T89inWr9Vae4APBNf7Bg2DReFP5jr23SQqaDMT```
* ETN - ```etnkQMp3Hmsay2p7uxokuHRKANrMDNASwQjDUgFb5L2sDM3jqUkYQPKBkooQFHVWBzEaZVzfzrXoETX6RbMEvg4R4csxfRHLo1```
* SUMO - ```Sumoo1DGS7c9LEKZNipsiDEqRzaUB3ws7YHfUiiZpx9SQDhdYGEEbZjRET26ewuYEWAZ8uKrz6vpUZkEVY7mDCZyGnQhkLpxKmy```
* GRFT - ```GACadqdXj5eNLnyNxvQ56wcmsmVCFLkHQKgtaQXNEE5zjMDJkWcMVju2aYtxbTnZgBboWYmHovuiH1Ahm4g2N5a7LuMQrpT```
* MSR - ```5hnMXUKArLDRue5tWsNpbmGLsLQibt23MEsV3VGwY6MGStYwfTqHkff4BgvziprTitbcDYYpFXw2rEgXeipsABTtEmcmnCK```
* LTHN - ```iz53aMEaKJ25zB8xku3FQK5VVvmu2v6DENnbGHRmn659jfrGWBH1beqAzEVYaKhTyMZcxLJAdaCW3Kof1DwTiTbp1DSqLae3e```
* WOW - ```Wo3yjV8UkwvbJDCB1Jy7vvXv3aaQu3K8YMG6tbY3Jo2KApfyf5RByZiBXy95bzmoR3AvPgNq6rHzm98LoHTkzjiA2dY7sqQMJ```
* XMV - ```XvyVfpAYp3zSuvdtoHgnDzMUf7GAeiumeUgVC7RTq6SfgtzGEzy4dUgfEEfD5adk1kN4dfVZdT3zZdgSD2xmVBs627Vwt2C3Ey```
* RYO - ```RYoLsi22qnoKYhnv1DwHBXcGe9QK6P9zmekwQnHdUAak7adFBK4i32wFTszivQ9wEPeugbXr2UD7tMd6ogf1dbHh76G5UszE7k1```
* XLA - ```SvkpUizij25ZGRHGb1c8ZTAHp3VyNFU3NQuQR1PtMyCqdpoZpaYAGMfG99z5guuoktY13nrhEerqYNKXvoxD7cUM1xA6Z5rRY```
* XHV - ```hvxyEmtbqs5TEk9U2tCxyfGx2dyGD1g8EBspdr3GivhPchkvnMHtpCR2fGLc5oEY42UGHVBMBANPge5QJ7BDXSMu1Ga2KFspQR```
* TUBE - ```TubedBNkgkTbd2CBmLQSwW58baJNghD9xdmctiRXjrW3dE8xpUcoXimY4J5UMrnUBrUDmfQrbxRYRX9s5tQe7pWYNF2QiAdH1Fh```
* LOKI - ```L6XqN6JDedz5Ub8KxpMYRCUoQCuyEA8EegEmeQsdP5FCNuXJavcrxPvLhpqY6emphGTYVrmAUVECsE9drafvY2hXUTJz6rW```
* TRTL - ```TRTLv2x2bac17cngo1r2wt3CaxN8ckoWHe2TX7dc8zW8Fc9dpmxAvhVX4u4zPjpv9WeALm2koBLF36REVvsLmeufZZ1Yx6uWkYG```
* XTNC - ```XtazhSxz1bbJLpT2JuiD2UWFUJYSFty5SVWuF6sy2w9v8pn69smkUxkTVCQc8NKCd6CBMNDGzgdPRYBKaHdbgZ5SNptVH1yPCTQ```
* IRD - ```ir3DHyB8Ub1aAHEewMeUxQ7b7tQdWa7VL8M5oXDPohS3Me4nhwvALXM4mym2kWg9VsceT75dm6XWiWF1K4zu8RVQ1HJD8Z3R9```
* ARQ - ```ar4Ha6ZQCkKRhkKQLfexv7VZQM2MhUmMmU9hmzswCPK4T3o2rbPKZM1GxEoYg4AFQsh57PsEets7sbpU958FAvxo2RkkTQ1gE```
* XWP - ```fh4MCJrakhWGoS6Meqp6UxGE1GNfAjKaRdPjW36rTffDiqvEq2HWEKZhrbYRw7XJb3CXxkjL3tcYGTT39m5qgjvk1ap4bVu1R```
* XEQ - ```Tvzp9tTmdGP9X8hCEw1Qzn18divQajJYTjR5HuUzHPKyLK5fzRt2X73FKBDzcnHMDJKdgsPhUDVrKHVcDJQVmLBg33NbkdjQb```
* XTA - ```ipN5cNhm7RXAGACP4ZXki4afT3iJ1A6Ka5U4cswE6fBPDcv8JpivurBj3vu1bXwPyb8KZEGsFUYMmToFG4N9V9G72X4WpAQ8L```
* DERO - ```dero1qygrgnz9gea2rqgwhdtpfpa3mvagt5uyq0g92nurwrpk6wnn7hdnzqgudsv6t```
* CCX - ```ccx7dmnBBoRPuVcpKJSAVZKdSDo9rc7HVijFbhG34jsXL3qiqfRwu7A5ecem44s2rngDd8y8N4QnYK6WR3mXAcAZ5iXun9BQBx```
* BLOC - ```abLoc5iUG4a6oAb2dqygxkS5M2uHWx16zHb9fUWMzpSEDwm6T7PSq2MLdHonWZ16CGfnJKRomq75aZyviTo6ZjHeYQMzNAEkjMg```
* RVN - ```RLVJv9rQNHzXS3Zn4JH8hfAHmm1LfECMxy```
* RTM - ```RUCyaEZxQu3Eure73XPQ57si813RYAMQKC```
* ERG - ```9fe533kUzAE57YfPP6o3nzsYMKN2W2uCxvg8KG8Vn5DDeJGetRw```
* BTC - ```3HRbMgcvbqHVW7P34MNGvF2Gh3DE26iHdw```
* BCH - ```18sKoDSjLCFW9kZrXuza1qzEERnKi7bx8S```
* ETH - ```0xfE23a61548FCCE159a541FAe9e16cEB92Da650ed```
* ETC - ```0x4480Ad73a113BEFf05B2079E38D90c9757Ecb063```
* LTC - ```MGj8PU1PpTNDDqRHmuEqfDpH3gxp6cJrUU```
