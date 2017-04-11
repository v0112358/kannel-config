kannel configure for Huawei e173 - 3G Viettel
=============

1. List USB device
# lsusb
Bus 002 Device 021: ID 12d1:14a7 Huawei Technologies Co., Ltd. 
(Vendor ID:12d1; Product ID:14a7)

2. Switch USB to GSM modem
# usb_modeswitch -v 12d1 -p 14a7 -M '55534243123456780000000000000011062000000100000000000000000000' 
# modprobe option
# lsusb
# echo "12d1 14a8" > /sys/bus/usb-serial/drivers/option1/new_id

Kannel configure for ZTE WCDMA MF627 - 3G Viettel
==============
1. List USB device
# lsusb
Bus 001 Device 003: ID 19d2:2000 ZTE WCDMA Technologies MSM MF627/MF628/MF628+/MF636+ HSDPA/HSUPA
(Vendor ID: 19d2; Product ID: 2000)

2. Switch USB to GSM modem:
# usb_modeswitch -v 19d2 -p 2000 -M '5553424312345678000000000000061e000000000000000000000000000000' 
# modprobe option
# lsusb
# echo "19d2 2002" > /sys/bus/usb-serial/drivers/option1/new_id
