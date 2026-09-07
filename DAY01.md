# 第一天：B 模块馆藏多条件筛选

对应成员：`0xiaohe333`  
目标分支：`feature/B-data`

## 改动内容

- 支持按书名/作者、分类、书架位置组合查询。
- 支持“仅看可借”筛选。
- 网页增加筛选和重置控件。
- 增加馆藏筛选集成测试并更新 API 文档。

## 操作命令

```bash
git clone https://github.com/chopinhhm/library-b-handoff-0xiaohe333.git
git clone https://github.com/chopinhhm/library-borrowing-system.git
cd library-borrowing-system
git checkout feature/B-data
git pull origin feature/B-data

git apply ../library-b-handoff-0xiaohe333/day01-B-catalog-filter.patch
mvn clean test
git diff

git add .
git commit -m "feat(B): add advanced catalog filters"
git push origin feature/B-data
```

提交前确认 Git 用户名和邮箱属于本人。
