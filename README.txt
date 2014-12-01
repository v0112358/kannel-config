kannel config for Huawei e173
=============

1. List USB device
# lsusb
Bus 002 Device 021: ID 12d1:14a7 Huawei Technologies Co., Ltd. 

2. Switch USB to GSM modem
# usb_modeswitch -v 12d1 -p 14a7 -M '55534243123456780000000000000011062000000100000000000000000000' 
# modprobe option
# lsusb
# echo "12d1 14a8" > /sys/bus/usb-serial/drivers/option1/new_id
