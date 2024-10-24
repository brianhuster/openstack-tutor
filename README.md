# Openstack tutor
## Cài Openstack
```sh
sudo snap install openstack --channel 2024.1/beta
```
### Cài phụ thuộc
```sh
sunbeam prepare-node-script | bash -x && newgrp snap_daemon
```

### Khởi động cloud
```sh
sunbeam cluster bootstrap --accept-defaults
```
Nếu gặp lỗi, có thể bạn chưa khởi động một trình điều khiển (controller). Chạy lệnh sau:
```sh
juju bootstrap
```
Điều này cũng cho phép bạn chọn một nhà cung cấp như AWS, Azure, Google, localhost,...


