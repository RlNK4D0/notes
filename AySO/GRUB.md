
### show boot messages

```
config path:
/etc/default/grub

deberia verse asi

GRUB_CMDLINE_LINUX_DEFAULT = 'nowatchdog nvme_load=YES zswap.enabled=0'

remove quiet, splash or loglevel=3
```
