git config --global user.name "GSHongDev"
git config --global user.email "shihong.gan@zohomail.cn"
单人开发
Username:ShihongGan

# Git 分支管理和开发规范 
## 分支管理 
### 长期分支 
- `main/master` - 主分支，只接受 `feature` 分支合并 
- `test` - 测试分支，用于集成测试 
### 短期分支 
- `feature/版本号`：生产发布分支 
- `dev/功能描述-姓名英文缩写`：个人功能开发分支 
- `hotfix/问题描述-姓名英文缩写` - 紧急修复分支 
### 管理流程 
1. 从当前的 `feature` 分支新建特定功能的 `dev` 分支； 
2. 开发完成后，统一将 `dev` 分支合并到 `test` 分支测试，测试通过后，合并成新 `feature` 分支； 
3. 对于发生在 `feature` 中的紧急问题，从当前 `feature` 分支新建 `hotfix` 分支进行修复，测试后合并回 `feature` 发布。 
## 提交信息规范 
> 提交信息前缀，可快速定位。 
- `feat`: 新功能 
- `fix`: 修复问题 
- `perf`: 代码优化 
- `docs`: 文档更新 
- `style`: 代码格式调整（不影响代码） 
- `refactor`: 重构 
- `test`: 测试相关 
- `chore`: 构建过程或辅助工具变动