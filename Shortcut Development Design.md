# 快捷指令开发设计

### 设计原则

- 可读性、复用性、扩展性、高可用性
- 可统一处理的数据保持数据结构统一，不可统一处理的数据遍历处理

### 京东系列流程设计



```flow
st=>start: Start
e=>end: End
Account.menu=>operation: Account.menu
账号选择
Task.menu=>operation: Task.menu
任务选择
Func.cookies=>condition: Func.cookies
遍历选择的账号列表
Func.main=>operation: Func.main
主方法
Func.getHomeData=>operation: Func.getHomeData
获取活动秘钥和信息
Func.getTaskDetail=>operation: Func.getTaskDetail
获取任务详情
Func.taskList=>condition: Func.taskList
遍历选择的任务列表
Func.handleTask=>operation: Func.handleTask
处理任务信息使得数据结构统一
Func.doTask=>operation: Func.doTask
发送模拟做任务的数据
Func.taskResult=>operation: Func.taskResult
根据返回值处理输出结果内容
Func.log=>inputoutput: Func.log
将结果存入log变量并通知
Func.logging=>inputoutput: Func.logging
当前账号完成所有任务后将log保存文件并通知
Func.finish=>operation: Func.finish
当选择的所有账号均完成任务执行结束指令流程
Func.request=>subroutine: Func.request
访问网络的一个公共方法带有回调功能

st(right)->Account.menu(right)->Task.menu(right)->Func.cookies
Func.cookies(no)->Func.finish(right)->e
Func.cookies(yes)->Func.main->Func.getHomeData->Func.getTaskDetail->Func.taskList
Func.taskList(no,right)->Func.logging(top)->Func.cookies
Func.taskList(yes)->Func.handleTask->Func.doTask->Func.taskResult->Func.log(left)->Func.taskList
```
