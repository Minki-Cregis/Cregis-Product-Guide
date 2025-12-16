# 什么是TEE环境？

TEE（Trusted Execution Environment，可信执行环境）是一种专门的安全技术，用于在计算设备中创建一个隔离且可信的执行空间。TEE 作为独立隔离的内存环境，将敏感代码和数据保存在 TEE 中，对其进行修改或运算操作时，需要证书授权。此防护机制可在进行加密计算和信息处理时，防止黑客在内存中篡改或窃取数据。

Cregis的TEE（可信执行环境）基于Intel SGX技术和AWS Nitro Enclaves构建境。
