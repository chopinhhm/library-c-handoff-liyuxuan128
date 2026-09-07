# 第二天：C 模块借阅筛选与续借规则

对应成员：`Liyuxuan128`  
目标分支：`feature/C-circulation`

## 改动内容

- 管理员可按借阅状态和逾期状态筛选记录。
- 读者端同步支持借阅记录筛选。
- 逾期图书禁止续借并返回明确提示。
- 增加借阅规则单元测试并更新 API 文档。

## 操作命令

```bash
git clone https://github.com/chopinhhm/library-borrowing-system.git
cd library-borrowing-system
git checkout feature/C-circulation
git pull origin feature/C-circulation

git apply ../library-c-handoff-liyuxuan128/day02-C-circulation-rules.patch
mvn clean test
git diff

git add .
git commit -m "feat(C): improve loan filters and renewal rules"
git push origin feature/C-circulation
```

提交前确认 Git 用户名和邮箱属于本人。
