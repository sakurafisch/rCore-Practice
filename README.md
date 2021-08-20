# rCore Practice

```zsh
cargo build --target riscv64gc-unknown-none-elf
qemu-riscv64 target/riscv64gc-unknown-none-elf/debug/os; echo $?
```

## 阅读记录

[自定义测试框架](https://zhuanlan.zhihu.com/p/90710559)