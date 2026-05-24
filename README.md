# AES-256-GCM Secure Encryption Tool v2.0

一个基于现代密码学标准的纯客户端安全加密/解密工具。采用**单文件架构**与**零信任（Zero-Trust）设计**，确保所有敏感数据均在浏览器本地安全处理，绝不经过任何云端服务器。

🔗 **Live Demo:** [aes-eight.vercel.app](https://aes-eight.vercel.app/)

---

## ✨ 核心特性 (Key Features)

* **极简无依赖 (Single File)**：全量逻辑集成于单个 `index.html`，100% 纯原生 Web 技术（Vanilla JS），无任何复杂的编译、打包或构建流程。
* **AES-256-GCM 认证加密**：调用浏览器原生的 `Web Crypto API` 进行 GCM 模式加密，自带密文完整性校验（Authenticated Encryption），杜绝密文在传输或存储时被恶意篡改。
* **PBKDF2 密钥拉伸**：内置 PBKDF2 算法进行 60,000 次哈希迭代加盐，有效抵御彩虹表与硬件级别的暴力破解攻击。
* **零知识隐私保护**：所有加解密操作在客户端本地瞬时完成，**零网络请求发出**，从源头上绝对保障数据隐私。
* **安全兜底机制**：引入本地尝试次数限制与智能延迟机制，有效防止针对本地脚本的自动化爆破。


## 🚀 部署与运行 (Deployment & Setup)

由于采用极致纯前端架构，该项目支持多种开箱即用的运行方式：

### 1. 本地双击运行 (Local Execute)
克隆本仓库到本地，无需安装 Node.js 或任何依赖，**直接双击 `index.html`** 即可在任意现代浏览器中完美运行。
```bash
git clone [https://github.com/Lim728/aes.git](https://github.com/Lim728/aes.git)
