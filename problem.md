1. raft 内部的 heartbeatimeout 和 electiontimeout 怎么设置? 和 Config中的 heartbeatick 和 electiontick 有什么关系?

2. raft的内部逻辑时钟用什么实现?

3. Step 方法的检查是否stale 具体怎么实现?   Message 中的各个参数具体意义是什么?

4. 对于日志匹配, 是否 AppendEntriesRPC 和  HeartBeatRPC都要进行日志检查?

5. requestVoteRPC , 什么条件下去投票?

6. 所有服务器都要保持的活动用什么去保持?  (猜测一个循环?)

   becomeXXX 如何逻辑时钟?

7. requesetVoteRPC 返回的term 如何供候选者使用? (领导者是否应该因为这个而去做出改变?)