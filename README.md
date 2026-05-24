# AES-256-GCM Secure Encryption Tool v2.0

一个基于现代密码学标准的纯客户端安全加密/解密工具，采用零信任（Zero-Trust）架构，确保所有敏感数据均在本地安全处理。

🔗 **Live Demo:** [aes-eight.vercel.app](https://aes-eight.vercel.app/)

---

## ✨ 核心特性 (Key Features)

* **AES-256-GCM 认证加密**：采用 GCM 模式，在提供高强度加密的同时，具备密文完整性校验（Authenticated Encryption），杜绝密文被恶意篡改。
* **PBKDF2 密钥拉伸**：内置 PBKDF2 算法进行 60,000 次哈希迭代加盐，有效抵御彩虹表与暴力破解攻击。
* **零信任 / 纯客户端处理**：所有加解密逻辑全量在用户浏览器本地完成，**100% 无网络传输**，绝对保障数据隐私。
* **安全兜底机制**：引入尝试次数限制与智能延迟，防止本地遭受自动化密码爆破。

## 🚀 本地开发与运行 (Local Setup)

由于采用纯前端架构，无需复杂的后端配置，克隆即可运行：

1. 克隆仓库：
   ```bash
   git clone [https://github.com/Lim728/aes.git](https://github.com/Lim728/aes.git)
