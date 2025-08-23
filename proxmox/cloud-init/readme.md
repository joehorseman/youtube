1. Download the ISO wget https://cloud-images.ubuntu.com/noble/current/noble-server-cloudimg-amd64.img

```bash
2. mv noble-server-cloudimg-amd64.img ubuntu-cloudinit.qcow2
3. qemu-img resize ubuntu-cloudinit.qcow2 40G
4. qm importdisk 8002 ubuntu-cloudinit.qcow2 local-lvm
5. qm set 8002 --serial0 socket --vga serial0
```

