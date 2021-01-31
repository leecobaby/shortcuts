# 快捷指令开发设计

### 设计原则

可读性、复用性、扩展性、高可用性

### 京东系列设计流程

```flow
st=>start: Start
e=>end: End
Account.menu=>operation: 账号选择
Task.menu=>operation: 任务选择
Func.cookies=>condition: 遍历选择的账号列表
Func.main=>operation: 主方法
Func.getHomeData=>operation: 获取秘钥和分数
Func.getTaskDetail=>operation: 获取任务详情
Func.taskList=>condition: 遍历选择的任务列表
op1=>operation: My Operation
sub1=>subroutine: My Subroutine

cond=>condition: Yes or No?
io=>inputoutput: catch something...
st->op1->cond
cond(yes)->io->e
cond(no)->sub1(right)->op1
```
