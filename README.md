# rCore Practice

```zsh
cargo build --target riscv64gc-unknown-none-elf
qemu-riscv64 os/target/riscv64gc-unknown-none-elf/debug/os; echo $?
```

```zsh
# 实现关机
qemu-system-riscv64 \
-machine virt \
-nographic \
-bios ./bootloader/rustsbi-qemu.bin \
-device loader,file=os/target/riscv64gc-unknown-none-elf/debug/os,addr=0x80200000
```

## 阅读记录

[自定义测试框架](https://zhuanlan.zhihu.com/p/90710559)