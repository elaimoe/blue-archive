
`create-favor.mjs`: 从学生好感剧情索引模板创建索引

参数：

`args[0]`: 学生ID
`args[1]`: 分布类型，默认 0
`args[2]`: 分布模式，默认为空数组

分布类型：

- 0: 正常分布
- 1: 有爱用品
- 2: 自定义分布，此时传入使用空格分隔的故事组 ID

示例：

```bash
pnpm create-favor 10000 0 # 在对应目录创建一个包含 *02, *03, *05, *06 的索引
pnpm create-favor 10000 1 # 在对应目录创建一个包含 *02, *03, *05, *06, *15 的索引
pnpm create-favor 10000 2 1 2 3 # 在对应目录创建一个包含 *01, *02, *03 的索引
```
