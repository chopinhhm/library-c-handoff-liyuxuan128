# C 核心业务流程 每日代码交接

对应成员：**Liyuxuan128**  
目标主仓库分支：$(System.Collections.Hashtable.branch)

本仓库用于存放按日期发布的代码改动包和说明。成员在自己的电脑上下载改动、应用到主仓库、运行测试，再使用自己的 GitHub 身份提交和推送。

## 每日操作

`ash
git clone https://github.com/chopinhhm/library-borrowing-system.git
cd library-borrowing-system
git checkout feature/C-circulation
git pull origin feature/C-circulation

# 将当天补丁下载到当前目录后
git apply dayXX.patch
mvn test
git diff

git add .
git commit -m "feat: complete assigned module improvement"
git push origin feature/C-circulation
`

提交前请确认 git config user.email 是本人 GitHub 已验证邮箱。不要共享 GitHub Token。