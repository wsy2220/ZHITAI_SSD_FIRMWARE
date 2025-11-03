Firmware filse dumped from ZHITAI_UNIMASTER_SSD.exe. 

Use at your own risk.

Linux firmware upgrade command:

```
nvme fw-download --fw=TiPro9000/SMI/4TB.bin /dev/nvme1
nvme fw-commit -v --action=3 /dev/nvme1
echo 1 > /sys/class/nvme/nvme1/reset_controller
nvme fw-log /dev/nvme1
reboot
```
