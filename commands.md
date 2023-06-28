---
layout: index
title: Redis命令中心（Redis commands）
permalink: commands.html
disqusIdentifier: commands
disqusUrl: http://redis.cn/commands.html
excerpt : Redis命令大全，显示全部已知的redis命令，redis集群相关命令，近期也会翻译过来,Redis命令参考，也可以直接输入命令进行命令检索。
discuzTid: 850
---
<section id='commands'>
<div class='container'>
	<div class='text' style='text-align:left;'>
		 &nbsp; &nbsp;Redis命令十分丰富，包括的命令组有Cluster、Connection、Geo、Hashes、HyperLogLog、Keys、Lists、Pub/Sub、Scripting、Server、Sets、Sorted Sets、Strings、Transactions一共14个redis命令组两百多个redis命令，Redis中文命令大全。您可以通过下面的检索功能快速查找命令，已下是全部已知的redis命令列表。如果您有兴趣的话也可以查看我们的<a href="/rediscn/map.html">网站结构图</a>,它以节点图的形式展示了所有redis命令。
	</div>
</div>
<nav>
          <div class='container'>
            <label>
              <span>过滤命令组:</span>
              <select class='command-reference-filter'>
                <option value=''>全部命令</option>
                <option value='cluster'>Cluster</option>
                <option value='connection'>Connection</option>
                <option value='geo'>Geo</option>
                <option value='hash'>Hashes</option>
                <option value='hyperloglog'>HyperLogLog</option>
                <option value='generic'>Keys</option>
                <option value='list'>Lists</option>
                <option value='pubsub'>Pub/Sub</option>
                <option value='scripting'>Scripting</option>
                <option value='server'>Server</option>
                <option value='set'>Sets</option>
                <option value='sorted_set'>Sorted Sets</option>
				<option value='streams'>Streams</option>
                <option value='string'>Strings</option>
                <option value='transactions'>Transactions</option>
				
              </select>
            </label>
            或者
            <label>
              <span>直接搜索:</span>
              <input autofocus='autofocus' class='js-command-reference-search' placeholder='例如 PING' />
            </label>
          </div>
        </nav>
<div class='container'>
          <ul>
            <li data-group='string' data-name='append'>
              <a href='/rediscn/commands/append.html'>
                <span class='command'>
                  APPEND
                  <span class='args'>
                    key
                    value
                  </span>
                </span>
                <span class='summary'>追加一个值到key上</span>
              </a>
            </li>
            <li data-group='connection' data-name='auth'>
              <a href='/rediscn/commands/auth.html'>
                <span class='command'>
                  AUTH
                  <span class='args'>
                    password
                  </span>
                </span>
                <span class='summary'>验证服务器命令</span>
              </a>
            </li>
            <li data-group='server' data-name='bgrewriteaof'>
              <a href='/rediscn/commands/bgrewriteaof.html'>
                <span class='command'>
                  BGREWRITEAOF
                  <span class='args'>
                  </span>
                </span>
                <span class='summary'>异步重写追加文件命令</span>
              </a>
            </li>
            <li data-group='server' data-name='bgsave'>
              <a href='/rediscn/commands/bgsave.html'>
                <span class='command'>
                  BGSAVE
                  <span class='args'>
                  </span>
                </span>
                <span class='summary'>异步保存数据集到磁盘上</span>
              </a>
            </li>
            <li data-group='string' data-name='bitcount'>
              <a href='/rediscn/commands/bitcount.html'>
                <span class='command'>
                  BITCOUNT
                  <span class='args'>
                    key
                    [start end]
                  </span>
                </span>
                <span class='summary'>统计字符串指定起始位置的字节数</span>
              </a>
            </li>
             <li data-group='string' data-name='bitfield'>
              <a href='/rediscn/commands/bitfield.html'>
                <span class='command'>
                  BITFIELD
                  <span class='args'>
                    key
                    [GET type offset]
                    [SET type offset value]
                    [INCRBY type offset increment]
                    [OVERFLOW WRAP|SAT|FAIL]
                  </span>
                </span>
                <span class='summary'>Perform arbitrary bitfield integer operations on strings</span>
              </a>
            </li>
            <li data-group='string' data-name='bitop'>
              <a href='/rediscn/commands/bitop.html'>
                <span class='command'>
                  BITOP
                  <span class='args'>
                    operation
                    destkey
                    key [key ...]
                  </span>
                </span>
                <span class='summary'>Perform bitwise operations between strings</span>
              </a>
            </li>
            <li data-group='string' data-name='bitpos'>
              <a href='/rediscn/commands/bitpos.html'>
                <span class='command'>
                  BITPOS
                  <span class='args'>
                    key
                    bit
                    [start]
                    [end]
                  </span>
                </span>
                <span class='summary'>Find first bit set or clear in a string</span>
              </a>
            </li>
            <li data-group='list' data-name='blpop'>
              <a href='/rediscn/commands/blpop.html'>
                <span class='command'>
                  BLPOP
                  <span class='args'>
                    key [key ...]
                    timeout
                  </span>
                </span>
                <span class='summary'>删除，并获得该列表中的第一元素，或阻塞，直到有一个可用</span>
              </a>
            </li>
            <li data-group='list' data-name='brpop'>
              <a href='/rediscn/commands/brpop.html'>
                <span class='command'>
                  BRPOP
                  <span class='args'>
                    key [key ...]
                    timeout
                  </span>
                </span>
                <span class='summary'>删除，并获得该列表中的最后一个元素，或阻塞，直到有一个可用</span>
              </a>
            </li>
            <li data-group='list' data-name='brpoplpush'>
              <a href='/rediscn/commands/brpoplpush.html'>
                <span class='command'>
                  BRPOPLPUSH
                  <span class='args'>
                    source
                    destination
                    timeout
                  </span>
                </span>
                <span class='summary'>弹出一个列表的值，将它推到另一个列表，并返回它;或阻塞，直到有一个可用</span>
              </a>
            </li>
			<li data-group='sortedsets' data-name='bzpopmax'>
              <a href='/rediscn/commands/bzpopmax.html'>
                <span class='command'>
                  BZPOPMAX
                  <span class='args'>
                    key [key ...] timeout
                  </span>
                </span>
                <span class='summary'>从一个或多个排序集中弹出一个得分最高的成员，或阻塞，直到有一个可用</span>
              </a>
            </li>
			<li data-group='sortedsets' data-name='bzpopmin'>
              <a href='/rediscn/commands/bzpopmin.html'>
                <span class='command'>
                  BZPOPMIN
                  <span class='args'>
                    key [key ...] timeout
                  </span>
                </span>
                <span class='summary'>从一个或多个排序集中弹出一个得分最低的成员，或阻塞，直到有一个可用</span>
              </a>
            </li>
            <li data-group='server' data-name='client kill'>
              <a href='/rediscn/commands/client-kill.html'>
                <span class='command'>
                  CLIENT KILL
                  <span class='args'>
                    [ip:port]
                    [ID client-id]
                    [TYPE normal|slave|pubsub]
                    [ADDR ip:port]
                    [SKIPME yes/no]
                  </span>
                </span>
                <span class='summary'>关闭客户端连接</span>
              </a>
            </li>
            <li data-group='server' data-name='client list'>
              <a href='/rediscn/commands/client-list.html'>
                <span class='command'>
                  CLIENT LIST
                  <span class='args'>
                  </span>
                </span>
                <span class='summary'>获得客户端连接列表</span>
              </a>
            </li>
            <li data-group='server' data-name='client getname'>
              <a href='/rediscn/commands/client-getname.html'>
                <span class='command'>
                  CLIENT GETNAME
                  <span class='args'>
                  </span>
                </span>
                <span class='summary'>获得当前连接名称</span>
              </a>
            </li>
			<li data-group='server' data-name='client id'>
              <a href='/rediscn/commands/client-id.html'>
                <span class='command'>
                  CLIENT ID
                  <span class='args'>
                  </span>
                </span>
                <span class='summary'>返回当前连接的客户端 ID</span>
              </a>
            </li>
            <li data-group='server' data-name='client pause'>
              <a href='/rediscn/commands/client-pause.html'>
                <span class='command'>
                  CLIENT PAUSE
                  <span class='args'>
                    timeout
                  </span>
                </span>
                <span class='summary'>暂停处理客户端命令</span>
              </a>
            </li>
			<li data-group='server' data-name='client reply'>
              <a href='/rediscn/commands/client-reply.html'>
                <span class='command'>
                  CLIENT REPLY
                  <span class='args'>
					          ON|OFF|SKIP
                  </span>
                </span>
                <span class='summary'>设置 redis 服务器对当前客户端的响应回复状态</span>
              </a>
            </li>
            <li data-group='server' data-name='client setname'>
              <a href='/rediscn/commands/client-setname.html'>
                <span class='command'>
                  CLIENT SETNAME
                  <span class='args'>
                    connection-name
                  </span>
                </span>
                <span class='summary'>设置当前连接的名字</span>
              </a>
            </li>
			<li data-group='server' data-name='client unblock'>
              <a href='/rediscn/commands/client-unblock.html'>
                <span class='command'>
                  CLIENT UNBLOCK
                  <span class='args'>
                    client-id [TIMEOUT|ERROR]
                  </span>
                </span>
                <span class='summary'>Unblock a client blocked in a blocking command from a different connection</span>
              </a>
            </li>
            <li data-group='cluster' data-name='cluster addslots'>
              <a href='/rediscn/commands/cluster-addslots.html'>
                <span class='command'>
                  CLUSTER ADDSLOTS
                  <span class='args'>
                    slot [slot ...]
                  </span>
                </span>
                <span class='summary'>Assign new hash slots to receiving node</span>
              </a>
            </li>
            <li data-group='cluster' data-name='cluster count-failure-reports'>
              <a href='/rediscn/commands/cluster-count-failure-reports.html'>
                <span class='command'>
                  CLUSTER COUNT-FAILURE-REPORTS
                  <span class='args'>
                    node-id
                  </span>
                </span>
                <span class='summary'>Return the number of failure reports active for a given node</span>
              </a>
            </li>
            <li data-group='cluster' data-name='cluster countkeysinslot'>
              <a href='/rediscn/commands/cluster-countkeysinslot.html'>
                <span class='command'>
                  CLUSTER COUNTKEYSINSLOT
                  <span class='args'>
                    slot
                  </span>
                </span>
                <span class='summary'>Return the number of local keys in the specified hash slot</span>
              </a>
            </li>
            <li data-group='cluster' data-name='cluster delslots'>
              <a href='/rediscn/commands/cluster-delslots.html'>
                <span class='command'>
                  CLUSTER DELSLOTS
                  <span class='args'>
                    slot [slot ...]
                  </span>
                </span>
                <span class='summary'>Set hash slots as unbound in receiving node</span>
              </a>
            </li>
            <li data-group='cluster' data-name='cluster failover'>
              <a href='/rediscn/commands/cluster-failover.html'>
                <span class='command'>
                  CLUSTER FAILOVER
                  <span class='args'>
                    [FORCE|TAKEOVER]
                  </span>
                </span>
                <span class='summary'>Forces a slave to perform a manual failover of its master.</span>
              </a>
            </li>
            <li data-group='cluster' data-name='cluster forget'>
              <a href='/rediscn/commands/cluster-forget.html'>
                <span class='command'>
                  CLUSTER FORGET
                  <span class='args'>
                    node-id
                  </span>
                </span>
                <span class='summary'>Remove a node from the nodes table</span>
              </a>
            </li>
            <li data-group='cluster' data-name='cluster getkeysinslot'>
              <a href='/rediscn/commands/cluster-getkeysinslot.html'>
                <span class='command'>
                  CLUSTER GETKEYSINSLOT
                  <span class='args'>
                    slot
                    count
                  </span>
                </span>
                <span class='summary'>Return local key names in the specified hash slot</span>
              </a>
            </li>
            <li data-group='cluster' data-name='cluster info'>
              <a href='/rediscn/commands/cluster-info.html'>
                <span class='command'>
                  CLUSTER INFO
                  <span class='args'>
                  </span>
                </span>
                <span class='summary'>Provides info about Redis Cluster node state</span>
              </a>
            </li>
            <li data-group='cluster' data-name='cluster keyslot'>
              <a href='/rediscn/commands/cluster-keyslot.html'>
                <span class='command'>
                  CLUSTER KEYSLOT
                  <span class='args'>
                    key
                  </span>
                </span>
                <span class='summary'>Returns the hash slot of the specified key</span>
              </a>
            </li>
            <li data-group='cluster' data-name='cluster meet'>
              <a href='/rediscn/commands/cluster-meet.html'>
                <span class='command'>
                  CLUSTER MEET
                  <span class='args'>
                    ip
                    port
                  </span>
                </span>
                <span class='summary'>Force a node cluster to handshake with another node</span>
              </a>
            </li>
            <li data-group='cluster' data-name='cluster nodes'>
              <a href='/rediscn/commands/cluster-nodes.html'>
                <span class='command'>
                  CLUSTER NODES
                  <span class='args'>
                  </span>
                </span>
                <span class='summary'>Get Cluster config for the node</span>
              </a>
            </li>
			<li data-group='cluster' data-name='cluster replicas'>
              <a href='/rediscn/commands/cluster-replicas.html'>
                <span class='command'>
                  CLUSTER REPLICAS
                  <span class='args'>
					node-id
                  </span>
                </span>
                <span class='summary'>List replica nodes of the specified master node</span>
              </a>
            </li>
            <li data-group='cluster' data-name='cluster replicate'>
              <a href='/rediscn/commands/cluster-replicate.html'>
                <span class='command'>
                  CLUSTER REPLICATE
                  <span class='args'>
                    node-id
                  </span>
                </span>
                <span class='summary'>Reconfigure a node as a slave of the specified master node</span>
              </a>
            </li>
            <li data-group='cluster' data-name='cluster reset'>
              <a href='/rediscn/commands/cluster-reset.html'>
                <span class='command'>
                  CLUSTER RESET
                  <span class='args'>
                    [HARD|SOFT]
                  </span>
                </span>
                <span class='summary'>Reset a Redis Cluster node</span>
              </a>
            </li>
            <li data-group='cluster' data-name='cluster saveconfig'>
              <a href='/rediscn/commands/cluster-saveconfig.html'>
                <span class='command'>
                  CLUSTER SAVECONFIG
                  <span class='args'>
                  </span>
                </span>
                <span class='summary'>Forces the node to save cluster state on disk</span>
              </a>
            </li>
            <li data-group='cluster' data-name='cluster set-config-epoch'>
              <a href='/rediscn/commands/cluster-set-config-epoch.html'>
                <span class='command'>
                  CLUSTER SET-CONFIG-EPOCH
                  <span class='args'>
                    config-epoch
                  </span>
                </span>
                <span class='summary'>Set the configuration epoch in a new node</span>
              </a>
            </li>
            <li data-group='cluster' data-name='cluster setslot'>
              <a href='/rediscn/commands/cluster-setslot.html'>
                <span class='command'>
                  CLUSTER SETSLOT
                  <span class='args'>
                    slot
                    IMPORTING|MIGRATING|STABLE|NODE
                    [node-id]
                  </span>
                </span>
                <span class='summary'>Bind an hash slot to a specific node</span>
              </a>
            </li>
            <li data-group='cluster' data-name='cluster slaves'>
              <a href='/rediscn/commands/cluster-slaves.html'>
                <span class='command'>
                  CLUSTER SLAVES
                  <span class='args'>
                    node-id
                  </span>
                </span>
                <span class='summary'>List slave nodes of the specified master node</span>
              </a>
            </li>
            <li data-group='cluster' data-name='cluster slots'>
              <a href='/rediscn/commands/cluster-slots.html'>
                <span class='command'>
                  CLUSTER SLOTS
                  <span class='args'>
                  </span>
                </span>
                <span class='summary'>Get array of Cluster slot to node mappings</span>
              </a>
            </li>
            <li data-group='server' data-name='command'>
              <a href='/rediscn/commands/command.html'>
                <span class='command'>
                  COMMAND
                  <span class='args'>
                  </span>
                </span>
                <span class='summary'>Get array of Redis command details</span>
              </a>
            </li>
            <li data-group='server' data-name='command count'>
              <a href='/rediscn/commands/command-count.html'>
                <span class='command'>
                  COMMAND COUNT
                  <span class='args'>
                  </span>
                </span>
                <span class='summary'>Get total number of Redis commands</span>
              </a>
            </li>
            <li data-group='server' data-name='command getkeys'>
              <a href='/rediscn/commands/command-getkeys.html'>
                <span class='command'>
                  COMMAND GETKEYS
                  <span class='args'>
                  </span>
                </span>
                <span class='summary'>Extract keys given a full Redis command</span>
              </a>
            </li>
            <li data-group='server' data-name='command info'>
              <a href='/rediscn/commands/command-info.html'>
                <span class='command'>
                  COMMAND INFO
                  <span class='args'>
                    command-name [command-name ...]
                  </span>
                </span>
                <span class='summary'>Get array of specific Redis command details</span>
              </a>
            </li>
            <li data-group='server' data-name='config get'>
              <a href='/rediscn/commands/config-get.html'>
                <span class='command'>
                  CONFIG GET
                  <span class='args'>
                    parameter
                  </span>
                </span>
                <span class='summary'>获取配置参数的值</span>
              </a>
            </li>
            <li data-group='server' data-name='config rewrite'>
              <a href='/rediscn/commands/config-rewrite.html'>
                <span class='command'>
                  CONFIG REWRITE
                  <span class='args'>
                  </span>
                </span>
                <span class='summary'>从写内存中的配置文件</span>
              </a>
            </li>
            <li data-group='server' data-name='config set'>
              <a href='/rediscn/commands/config-set.html'>
                <span class='command'>
                  CONFIG SET
                  <span class='args'>
                    parameter
                    value
                  </span>
                </span>
                <span class='summary'>设置配置文件</span>
              </a>
            </li>
            <li data-group='server' data-name='config resetstat'>
              <a href='/rediscn/commands/config-resetstat.html'>
                <span class='command'>
                  CONFIG RESETSTAT
                  <span class='args'>
                  </span>
                </span>
                <span class='summary'>复位再分配使用info命令报告的统计</span>
              </a>
            </li>
            <li data-group='server' data-name='dbsize'>
              <a href='/rediscn/commands/dbsize.html'>
                <span class='command'>
                  DBSIZE
                  <span class='args'>
                  </span>
                </span>
                <span class='summary'>返回当前数据库里面的keys数量</span>
              </a>
            </li>
            <li data-group='server' data-name='debug object'>
              <a href='/rediscn/commands/debug-object.html'>
                <span class='command'>
                  DEBUG OBJECT
                  <span class='args'>
                    key
                  </span>
                </span>
                <span class='summary'>获取一个key的debug信息</span>
              </a>
            </li>
            <li data-group='server' data-name='debug segfault'>
              <a href='/rediscn/commands/debug-segfault.html'>
                <span class='command'>
                  DEBUG SEGFAULT
                  <span class='args'>
                  </span>
                </span>
                <span class='summary'>使服务器崩溃命令</span>
              </a>
            </li>
            <li data-group='string' data-name='decr'>
              <a href='/rediscn/commands/decr.html'>
                <span class='command'>
                  DECR
                  <span class='args'>
                    key
                  </span>
                </span>
                <span class='summary'>整数原子减1</span>
              </a>
            </li>
            <li data-group='string' data-name='decrby'>
              <a href='/rediscn/commands/decrby.html'>
                <span class='command'>
                  DECRBY
                  <span class='args'>
                    key
                    decrement
                  </span>
                </span>
                <span class='summary'>原子减指定的整数</span>
              </a>
            </li>
            <li data-group='generic' data-name='del'>
              <a href='/rediscn/commands/del.html'>
                <span class='command'>
                  DEL
                  <span class='args'>
                    key [key ...]
                  </span>
                </span>
                <span class='summary'>删除指定的key（一个或多个）</span>
              </a>
            </li>
            <li data-group='transactions' data-name='discard'>
              <a href='/rediscn/commands/discard.html'>
                <span class='command'>
                  DISCARD
                  <span class='args'>
                  </span>
                </span>
                <span class='summary'>丢弃所有 MULTI 之后发的命令</span>
              </a>
            </li>
            <li data-group='generic' data-name='dump'>
              <a href='/rediscn/commands/dump.html'>
                <span class='command'>
                  DUMP
                  <span class='args'>
                    key
                  </span>
                </span>
                <span class='summary'>导出key的值</span>
              </a>
            </li>
            <li data-group='connection' data-name='echo'>
              <a href='/rediscn/commands/echo.html'>
                <span class='command'>
                  ECHO
                  <span class='args'>
                    message
                  </span>
                </span>
                <span class='summary'>回显输入的字符串</span>
              </a>
            </li>
            <li data-group='scripting' data-name='eval'>
              <a href='/rediscn/commands/eval.html'>
                <span class='command'>
                  EVAL
                  <span class='args'>
                    script
                    numkeys
                    key [key ...]
                    arg [arg ...]
                  </span>
                </span>
                <span class='summary'>在服务器端执行 LUA 脚本</span>
              </a>
            </li>
            <li data-group='scripting' data-name='evalsha'>
              <a href='/rediscn/commands/evalsha.html'>
                <span class='command'>
                  EVALSHA
                  <span class='args'>
                    sha1
                    numkeys
                    key [key ...]
                    arg [arg ...]
                  </span>
                </span>
                <span class='summary'>在服务器端执行 LUA 脚本</span>
              </a>
            </li>
            <li data-group='transactions' data-name='exec'>
              <a href='/rediscn/commands/exec.html'>
                <span class='command'>
                  EXEC
                  <span class='args'>
                  </span>
                </span>
                <span class='summary'>执行所有 MULTI 之后发的命令</span>
              </a>
            </li>
            <li data-group='generic' data-name='exists'>
              <a href='/rediscn/commands/exists.html'>
                <span class='command'>
                  EXISTS
                  <span class='args'>
                    key [key ...]
                  </span>
                </span>
                <span class='summary'>查询一个key是否存在</span>
              </a>
            </li>
            <li data-group='generic' data-name='expire'>
              <a href='/rediscn/commands/expire.html'>
                <span class='command'>
                  EXPIRE
                  <span class='args'>
                    key
                    seconds
                  </span>
                </span>
                <span class='summary'>设置一个key的过期的秒数</span>
              </a>
            </li>
            <li data-group='generic' data-name='expireat'>
              <a href='/rediscn/commands/expireat.html'>
                <span class='command'>
                  EXPIREAT
                  <span class='args'>
                    key
                    timestamp
                  </span>
                </span>
                <span class='summary'>设置一个UNIX时间戳的过期时间</span>
              </a>
            </li>
            <li data-group='server' data-name='flushall'>
              <a href='/rediscn/commands/flushall.html'>
                <span class='command'>
                  FLUSHALL
                  <span class='args'>
                  </span>
                </span>
                <span class='summary'>清空所有数据库命令</span>
              </a>
            </li>
            <li data-group='server' data-name='flushdb'>
              <a href='/rediscn/commands/flushdb.html'>
                <span class='command'>
                  FLUSHDB
                  <span class='args'>
                  </span>
                </span>
                <span class='summary'>清空当前的数据库命令</span>
              </a>
            </li>
            <li data-group='geo' data-name='geoadd'>
              <a href='/rediscn/commands/geoadd.html'>
                <span class='command'>
                  GEOADD
                  <span class='args'>
                    key
                    longitude latitude member [longitude latitude member ...]
                  </span>
                </span>
                <span class='summary'>添加一个或多个地理空间位置到sorted set</span>
              </a>
            </li>
            <li data-group='geo' data-name='geohash'>
              <a href='/rediscn/commands/geohash.html'>
                <span class='command'>
                  GEOHASH
                  <span class='args'>
                    key
                    member [member ...]
                  </span>
                </span>
                <span class='summary'>返回一个标准的地理空间的Geohash字符串</span>
              </a>
            </li>
            <li data-group='geo' data-name='geopos'>
              <a href='/rediscn/commands/geopos.html'>
                <span class='command'>
                  GEOPOS
                  <span class='args'>
                    key
                    member [member ...]
                  </span>
                </span>
                <span class='summary'>返回地理空间的经纬度</span>
              </a>
            </li>
            <li data-group='geo' data-name='geodist'>
              <a href='/rediscn/commands/geodist.html'>
                <span class='command'>
                  GEODIST
                  <span class='args'>
                    key
                    member1
                    member2
                    [unit]
                  </span>
                </span>
                <span class='summary'>返回两个地理空间之间的距离</span>
              </a>
            </li>
            <li data-group='geo' data-name='georadius'>
              <a href='/rediscn/commands/georadius.html'>
                <span class='command'>
                  GEORADIUS
                  <span class='args'>
                    key
                    longitude
                    latitude
                    radius
                    m|km|ft|mi
                    [WITHCOORD]
                    [WITHDIST]
                    [WITHHASH]
                    [COUNT count]
                  </span>
                </span>
                <span class='summary'>查询指定半径内所有的地理空间元素的集合。</span>
              </a>
            </li>
            <li data-group='geo' data-name='georadiusbymember'>
              <a href='/rediscn/commands/georadiusbymember.html'>
                <span class='command'>
                  GEORADIUSBYMEMBER
                  <span class='args'>
                    key
                    member
                    radius
                    m|km|ft|mi
                    [WITHCOORD]
                    [WITHDIST]
                    [WITHHASH]
                    [COUNT count]
                  </span>
                </span>
                <span class='summary'>查询指定半径内匹配到的最大距离的一个地理空间元素。</span>
              </a>
            </li>
            <li data-group='string' data-name='get'>
              <a href='/rediscn/commands/get.html'>
                <span class='command'>
                  GET
                  <span class='args'>
                    key
                  </span>
                </span>
                <span class='summary'>返回key的value</span>
              </a>
            </li>
            <li data-group='string' data-name='getbit'>
              <a href='/rediscn/commands/getbit.html'>
                <span class='command'>
                  GETBIT
                  <span class='args'>
                    key
                    offset
                  </span>
                </span>
                <span class='summary'>返回位的值存储在关键的字符串值的偏移量。</span>
              </a>
            </li>
            <li data-group='string' data-name='getrange'>
              <a href='/rediscn/commands/getrange.html'>
                <span class='command'>
                  GETRANGE
                  <span class='args'>
                    key
                    start
                    end
                  </span>
                </span>
                <span class='summary'>获取存储在key上的值的一个子字符串</span>
              </a>
            </li>
            <li data-group='string' data-name='getset'>
              <a href='/rediscn/commands/getset.html'>
                <span class='command'>
                  GETSET
                  <span class='args'>
                    key
                    value
                  </span>
                </span>
                <span class='summary'>设置一个key的value，并获取设置前的值</span>
              </a>
            </li>
            <li data-group='hash' data-name='hdel'>
              <a href='/rediscn/commands/hdel.html'>
                <span class='command'>
                  HDEL
                  <span class='args'>
                    key
                    field [field ...]
                  </span>
                </span>
                <span class='summary'>删除一个或多个Hash的field</span>
              </a>
            </li>
            <li data-group='hash' data-name='hexists'>
              <a href='/rediscn/commands/hexists.html'>
                <span class='command'>
                  HEXISTS
                  <span class='args'>
                    key
                    field
                  </span>
                </span>
                <span class='summary'>判断field是否存在于hash中</span>
              </a>
            </li>
            <li data-group='hash' data-name='hget'>
              <a href='/rediscn/commands/hget.html'>
                <span class='command'>
                  HGET
                  <span class='args'>
                    key
                    field
                  </span>
                </span>
                <span class='summary'>获取hash中field的值</span>
              </a>
            </li>
            <li data-group='hash' data-name='hgetall'>
              <a href='/rediscn/commands/hgetall.html'>
                <span class='command'>
                  HGETALL
                  <span class='args'>
                    key
                  </span>
                </span>
                <span class='summary'>从hash中读取全部的域和值</span>
              </a>
            </li>
            <li data-group='hash' data-name='hincrby'>
              <a href='/rediscn/commands/hincrby.html'>
                <span class='command'>
                  HINCRBY
                  <span class='args'>
                    key
                    field
                    increment
                  </span>
                </span>
                <span class='summary'>将hash中指定域的值增加给定的数字</span>
              </a>
            </li>
            <li data-group='hash' data-name='hincrbyfloat'>
              <a href='/rediscn/commands/hincrbyfloat.html'>
                <span class='command'>
                  HINCRBYFLOAT
                  <span class='args'>
                    key
                    field
                    increment
                  </span>
                </span>
                <span class='summary'>将hash中指定域的值增加给定的浮点数</span>
              </a>
            </li>
            <li data-group='hash' data-name='hkeys'>
              <a href='/rediscn/commands/hkeys.html'>
                <span class='command'>
                  HKEYS
                  <span class='args'>
                    key
                  </span>
                </span>
                <span class='summary'>获取hash的所有字段</span>
              </a>
            </li>
            <li data-group='hash' data-name='hlen'>
              <a href='/rediscn/commands/hlen.html'>
                <span class='command'>
                  HLEN
                  <span class='args'>
                    key
                  </span>
                </span>
                <span class='summary'>获取hash里所有字段的数量</span>
              </a>
            </li>
            <li data-group='hash' data-name='hmget'>
              <a href='/rediscn/commands/hmget.html'>
                <span class='command'>
                  HMGET
                  <span class='args'>
                    key
                    field [field ...]
                  </span>
                </span>
                <span class='summary'>获取hash里面指定字段的值</span>
              </a>
            </li>
            <li data-group='hash' data-name='hmset'>
              <a href='/rediscn/commands/hmset.html'>
                <span class='command'>
                  HMSET
                  <span class='args'>
                    key
                    field value [field value ...]
                  </span>
                </span>
                <span class='summary'>设置hash字段值</span>
              </a>
            </li>
            <li data-group='hash' data-name='hset'>
              <a href='/rediscn/commands/hset.html'>
                <span class='command'>
                  HSET
                  <span class='args'>
                    key
                    field
                    value
                  </span>
                </span>
                <span class='summary'>设置hash里面一个字段的值</span>
              </a>
            </li>
            <li data-group='hash' data-name='hsetnx'>
              <a href='/rediscn/commands/hsetnx.html'>
                <span class='command'>
                  HSETNX
                  <span class='args'>
                    key
                    field
                    value
                  </span>
                </span>
                <span class='summary'>设置hash的一个字段，只有当这个字段不存在时有效</span>
              </a>
            </li>
            <li data-group='hash' data-name='hstrlen'>
              <a href='/rediscn/commands/hstrlen.html'>
                <span class='command'>
                  HSTRLEN
                  <span class='args'>
                    key
                    field
                  </span>
                </span>
                <span class='summary'>获取hash里面指定field的长度</span>
              </a>
            </li>
            <li data-group='hash' data-name='hvals'>
              <a href='/rediscn/commands/hvals.html'>
                <span class='command'>
                  HVALS
                  <span class='args'>
                    key
                  </span>
                </span>
                <span class='summary'>获得hash的所有值</span>
              </a>
            </li>
            <li data-group='string' data-name='incr'>
              <a href='/rediscn/commands/incr.html'>
                <span class='command'>
                  INCR
                  <span class='args'>
                    key
                  </span>
                </span>
                <span class='summary'>执行原子加1操作</span>
              </a>
            </li>
            <li data-group='string' data-name='incrby'>
              <a href='/rediscn/commands/incrby.html'>
                <span class='command'>
                  INCRBY
                  <span class='args'>
                    key
                    increment
                  </span>
                </span>
                <span class='summary'>执行原子增加一个整数</span>
              </a>
            </li>
            <li data-group='string' data-name='incrbyfloat'>
              <a href='/rediscn/commands/incrbyfloat.html'>
                <span class='command'>
                  INCRBYFLOAT
                  <span class='args'>
                    key
                    increment
                  </span>
                </span>
                <span class='summary'>执行原子增加一个浮点数</span>
              </a>
            </li>
            <li data-group='server' data-name='info'>
              <a href='/rediscn/commands/info.html'>
                <span class='command'>
                  INFO
                  <span class='args'>
                    [section]
                  </span>
                </span>
                <span class='summary'>获得服务器的详细信息</span>
              </a>
            </li>
            <li data-group='generic' data-name='keys'>
              <a href='/rediscn/commands/keys.html'>
                <span class='command'>
                  KEYS
                  <span class='args'>
                    pattern
                  </span>
                </span>
                <span class='summary'>查找所有匹配给定的模式的键</span>
              </a>
            </li>
            <li data-group='server' data-name='lastsave'>
              <a href='/rediscn/commands/lastsave.html'>
                <span class='command'>
                  LASTSAVE
                  <span class='args'>
                  </span>
                </span>
                <span class='summary'>获得最后一次同步磁盘的时间</span>
              </a>
            </li>
            <li data-group='list' data-name='lindex'>
              <a href='/rediscn/commands/lindex.html'>
                <span class='command'>
                  LINDEX
                  <span class='args'>
                    key
                    index
                  </span>
                </span>
                <span class='summary'>获取一个元素，通过其索引列表</span>
              </a>
            </li>
            <li data-group='list' data-name='linsert'>
              <a href='/rediscn/commands/linsert.html'>
                <span class='command'>
                  LINSERT
                  <span class='args'>
                    key
                    BEFORE|AFTER
                    pivot
                    value
                  </span>
                </span>
                <span class='summary'>在列表中的另一个元素之前或之后插入一个元素</span>
              </a>
            </li>
            <li data-group='list' data-name='llen'>
              <a href='/rediscn/commands/llen.html'>
                <span class='command'>
                  LLEN
                  <span class='args'>
                    key
                  </span>
                </span>
                <span class='summary'>获得队列(List)的长度</span>
              </a>
            </li>
            <li data-group='list' data-name='lpop'>
              <a href='/rediscn/commands/lpop.html'>
                <span class='command'>
                  LPOP
                  <span class='args'>
                    key
                  </span>
                </span>
                <span class='summary'>从队列的左边出队一个元素</span>
              </a>
            </li>
            <li data-group='list' data-name='lpush'>
              <a href='/rediscn/commands/lpush.html'>
                <span class='command'>
                  LPUSH
                  <span class='args'>
                    key
                    value [value ...]
                  </span>
                </span>
                <span class='summary'>从队列的左边入队一个或多个元素</span>
              </a>
            </li>
            <li data-group='list' data-name='lpushx'>
              <a href='/rediscn/commands/lpushx.html'>
                <span class='command'>
                  LPUSHX
                  <span class='args'>
                    key
                    value
                  </span>
                </span>
                <span class='summary'>当队列存在时，从队到左边入队一个元素</span>
              </a>
            </li>
            <li data-group='list' data-name='lrange'>
              <a href='/rediscn/commands/lrange.html'>
                <span class='command'>
                  LRANGE
                  <span class='args'>
                    key
                    start
                    stop
                  </span>
                </span>
                <span class='summary'>从列表中获取指定返回的元素</span>
              </a>
            </li>
            <li data-group='list' data-name='lrem'>
              <a href='/rediscn/commands/lrem.html'>
                <span class='command'>
                  LREM
                  <span class='args'>
                    key
                    count
                    value
                  </span>
                </span>
                <span class='summary'>从列表中删除元素</span>
              </a>
            </li>
            <li data-group='list' data-name='lset'>
              <a href='/rediscn/commands/lset.html'>
                <span class='command'>
                  LSET
                  <span class='args'>
                    key
                    index
                    value
                  </span>
                </span>
                <span class='summary'>设置队列里面一个元素的值</span>
              </a>
            </li>
            <li data-group='list' data-name='ltrim'>
              <a href='/rediscn/commands/ltrim.html'>
                <span class='command'>
                  LTRIM
                  <span class='args'>
                    key
                    start
                    stop
                  </span>
                </span>
                <span class='summary'>修剪到指定范围内的清单</span>
              </a>
            </li>
			<li data-group='server' data-name='memory doctor'>
              <a href='/rediscn/commands/memory-doctor.html'>
                <span class='command'>
                  MEMORY DOCTOR
                  <span class='args'>
                  </span>
                </span>
                <span class='summary'>输出内存问题报告</span>
              </a>
            </li>
			<li data-group='server' data-name='memory help'>
              <a href='/rediscn/commands/memory-help.html'>
                <span class='command'>
                  MEMORY HELP
                  <span class='args'>
                  </span>
                </span>
                <span class='summary'>显示有关子命令的帮助说明</span>
              </a>
            </li>
			<li data-group='server' data-name='memory malloc stats'>
              <a href='/rediscn/commands/memory-malloc-stats.html'>
                <span class='command'>
                  MEMORY-MALLOC-STATS
                  <span class='args'>
                  </span>
                </span>
                <span class='summary'>显示分配器内部统计信息</span>
              </a>
            </li>
			<li data-group='server' data-name='memory purge'>
              <a href='/rediscn/commands/memory-purge.html'>
                <span class='command'>
                  MEMORY-PURGE
                  <span class='args'>
                  </span>
                </span>
                <span class='summary'>要求分配器释放内存</span>
              </a>
            </li>
			<li data-group='server' data-name='memory stats'>
              <a href='/rediscn/commands/memory-stats.html'>
                <span class='command'>
                  MEMORY-STATS
                  <span class='args'>
                  </span>
                </span>
                <span class='summary'>显示内存使用情况详细信息</span>
              </a>
            </li>
			<li data-group='server' data-name='memory usage'>
              <a href='/rediscn/commands/memory-usage.html'>
                <span class='command'>
                  MEMORY-USAGE
                  <span class='args'>
					key [SAMPLES count]
                  </span>
                </span>
                <span class='summary'>估计 key 的内存使用量</span>
              </a>
            </li>
            <li data-group='string' data-name='mget'>
              <a href='/rediscn/commands/mget.html'>
                <span class='command'>
                  MGET
                  <span class='args'>
                    key [key ...]
                  </span>
                </span>
                <span class='summary'>获得所有key的值</span>
              </a>
            </li>
            <li data-group='generic' data-name='migrate'>
              <a href='/rediscn/commands/migrate.html'>
                <span class='command'>
                  MIGRATE
                  <span class='args'>
                    host
                    port
                    key
                    destination-db
                    timeout
                    [COPY]
                    [REPLACE]
                  </span>
                </span>
                <span class='summary'>原子性的将key从redis的一个实例移到另一个实例</span>
              </a>
            </li>
            <li data-group='server' data-name='monitor'>
              <a href='/rediscn/commands/monitor.html'>
                <span class='command'>
                  MONITOR
                  <span class='args'>
                  </span>
                </span>
                <span class='summary'>实时监控服务器</span>
              </a>
            </li>
            <li data-group='generic' data-name='move'>
              <a href='/rediscn/commands/move.html'>
                <span class='command'>
                  MOVE
                  <span class='args'>
                    key
                    db
                  </span>
                </span>
                <span class='summary'>移动一个key到另一个数据库</span>
              </a>
            </li>
            <li data-group='string' data-name='mset'>
              <a href='/rediscn/commands/mset.html'>
                <span class='command'>
                  MSET
                  <span class='args'>
                    key value [key value ...]
                  </span>
                </span>
                <span class='summary'>设置多个key value</span>
              </a>
            </li>
            <li data-group='string' data-name='msetnx'>
              <a href='/rediscn/commands/msetnx.html'>
                <span class='command'>
                  MSETNX
                  <span class='args'>
                    key value [key value ...]
                  </span>
                </span>
                <span class='summary'>设置多个key value,仅当key存在时</span>
              </a>
            </li>
            <li data-group='transactions' data-name='multi'>
              <a href='/rediscn/commands/multi.html'>
                <span class='command'>
                  MULTI
                  <span class='args'>
                  </span>
                </span>
                <span class='summary'>标记一个事务块开始</span>
              </a>
            </li>
            <li data-group='generic' data-name='object'>
              <a href='/rediscn/commands/object.html'>
                <span class='command'>
                  OBJECT
                  <span class='args'>
                    subcommand
                    [arguments [arguments ...]]
                  </span>
                </span>
                <span class='summary'>检查内部的再分配对象</span>
              </a>
            </li>
            <li data-group='generic' data-name='persist'>
              <a href='/rediscn/commands/persist.html'>
                <span class='command'>
                  PERSIST
                  <span class='args'>
                    key
                  </span>
                </span>
                <span class='summary'>移除key的过期时间</span>
              </a>
            </li>
            <li data-group='generic' data-name='pexpire'>
              <a href='/rediscn/commands/pexpire.html'>
                <span class='command'>
                  PEXPIRE
                  <span class='args'>
                    key
                    milliseconds
                  </span>
                </span>
                <span class='summary'>设置key的有效时间以毫秒为单位</span>
              </a>
            </li>
            <li data-group='generic' data-name='pexpireat'>
              <a href='/rediscn/commands/pexpireat.html'>
                <span class='command'>
                  PEXPIREAT
                  <span class='args'>
                    key
                    milliseconds-timestamp
                  </span>
                </span>
                <span class='summary'>设置key的到期UNIX时间戳以毫秒为单位</span>
              </a>
            </li>
            <li data-group='hyperloglog' data-name='pfadd'>
              <a href='/rediscn/commands/pfadd.html'>
                <span class='command'>
                  PFADD
                  <span class='args'>
                    key
                    element [element ...]
                  </span>
                </span>
                <span class='summary'>将指定元素添加到HyperLogLog</span>
              </a>
            </li>
            <li data-group='hyperloglog' data-name='pfcount'>
              <a href='/rediscn/commands/pfcount.html'>
                <span class='command'>
                  PFCOUNT
                  <span class='args'>
                    key [key ...]
                  </span>
                </span>
                <span class='summary'>Return the approximated cardinality of the set(s) observed by the HyperLogLog at key(s).</span>
              </a>
            </li>
            <li data-group='hyperloglog' data-name='pfmerge'>
              <a href='/rediscn/commands/pfmerge.html'>
                <span class='command'>
                  PFMERGE
                  <span class='args'>
                    destkey
                    sourcekey [sourcekey ...]
                  </span>
                </span>
                <span class='summary'>Merge N different HyperLogLogs into a single one.</span>
              </a>
            </li>
            <li data-group='connection' data-name='ping'>
              <a href='/rediscn/commands/ping.html'>
                <span class='command'>
                  PING
                  <span class='args'>
                  </span>
                </span>
                <span class='summary'>Ping 服务器</span>
              </a>
            </li>
            <li data-group='string' data-name='psetex'>
              <a href='/rediscn/commands/psetex.html'>
                <span class='command'>
                  PSETEX
                  <span class='args'>
                    key
                    milliseconds
                    value
                  </span>
                </span>
                <span class='summary'>设置 key 的值和过期时间（以毫秒为单位）</span>
              </a>
            </li>
            <li data-group='pubsub' data-name='psubscribe'>
              <a href='/rediscn/commands/psubscribe.html'>
                <span class='command'>
                  PSUBSCRIBE
                  <span class='args'>
                    pattern [pattern ...]
                  </span>
                </span>
                <span class='summary'>订阅匹配的通道的消息</span>
              </a>
            </li>
            <li data-group='pubsub' data-name='pubsub'>
              <a href='/rediscn/commands/pubsub.html'>
                <span class='command'>
                  PUBSUB
                  <span class='args'>
                    subcommand
                    [argument [argument ...]]
                  </span>
                </span>
                <span class='summary'>命令用于查看订阅与发布系统状态</span>
              </a>
            </li>
            <li data-group='generic' data-name='pttl'>
              <a href='/rediscn/commands/pttl.html'>
                <span class='command'>
                  PTTL
                  <span class='args'>
                    key
                  </span>
                </span>
                <span class='summary'>获取key的有效毫秒数</span>
              </a>
            </li>
            <li data-group='pubsub' data-name='publish'>
              <a href='/rediscn/commands/publish.html'>
                <span class='command'>
                  PUBLISH
                  <span class='args'>
                    channel
                    message
                  </span>
                </span>
                <span class='summary'>发布一条消息到频道</span>
              </a>
            </li>
            <li data-group='pubsub' data-name='punsubscribe'>
              <a href='/rediscn/commands/punsubscribe.html'>
                <span class='command'>
                  PUNSUBSCRIBE
                  <span class='args'>
                    [pattern [pattern ...]]
                  </span>
                </span>
                <span class='summary'>停止发布到匹配给定模式的渠道的消息听</span>
              </a>
            </li>
            <li data-group='connection' data-name='quit'>
              <a href='/rediscn/commands/quit.html'>
                <span class='command'>
                  QUIT
                  <span class='args'>
                  </span>
                </span>
                <span class='summary'>关闭连接，退出</span>
              </a>
            </li>
            <li data-group='generic' data-name='randomkey'>
              <a href='/rediscn/commands/randomkey.html'>
                <span class='command'>
                  RANDOMKEY
                  <span class='args'>
                  </span>
                </span>
                <span class='summary'>返回一个随机的key</span>
              </a>
            </li>
            <li data-group='cluster' data-name='readonly'>
              <a href='/rediscn/commands/readonly.html'>
                <span class='command'>
                  READONLY
                  <span class='args'>
                  </span>
                </span>
                <span class='summary'>启用与 Redis 集群副本节点的连接的只读。</span>
              </a>
            </li>
            <li data-group='cluster' data-name='readwrite'>
              <a href='/rediscn/commands/readwrite.html'>
                <span class='command'>
                  READWRITE
                  <span class='args'>
                  </span>
                </span>
                <span class='summary'>关闭与 Redis 集群副本节点的连接的只读。</span>
              </a>
            </li>
            <li data-group='generic' data-name='rename'>
              <a href='/rediscn/commands/rename.html'>
                <span class='command'>
                  RENAME
                  <span class='args'>
                    key
                    newkey
                  </span>
                </span>
                <span class='summary'>将一个key重命名</span>
              </a>
            </li>
            <li data-group='generic' data-name='renamenx'>
              <a href='/rediscn/commands/renamenx.html'>
                <span class='command'>
                  RENAMENX
                  <span class='args'>
                    key
                    newkey
                  </span>
                </span>
                <span class='summary'>重命名一个key,新的key必须是不存在的key</span>
              </a>
            </li>
			      <li data-group='server' data-name='replicaof'>
              <a href='/rediscn/commands/replicaof.html'>
                <span class='command'>
                  REPLICAOF
                  <span class='args'>
                    host port
                  </span>
                </span>
                <span class='summary'>使服务器成为另一个实例的副本，或将其提升为主实例。</span>
              </a>
            </li>
            <li data-group='generic' data-name='restore'>
              <a href='/rediscn/commands/restore.html'>
                <span class='command'>
                  RESTORE
                  <span class='args'>
                    key
                    ttl
                    serialized-value
                    [REPLACE]
                  </span>
                </span>
                <span class='summary'>Create a key using the provided serialized value, previously obtained using DUMP.</span>
              </a>
            </li>
            <li data-group='server' data-name='role'>
              <a href='/rediscn/commands/role.html'>
                <span class='command'>
                  ROLE
                  <span class='args'>
                  </span>
                </span>
                <span class='summary'>Return the role of the instance in the context of replication</span>
              </a>
            </li>
            <li data-group='list' data-name='rpop'>
              <a href='/rediscn/commands/rpop.html'>
                <span class='command'>
                  RPOP
                  <span class='args'>
                    key
                  </span>
                </span>
                <span class='summary'>从队列的右边出队一个元</span>
              </a>
            </li>
            <li data-group='list' data-name='rpoplpush'>
              <a href='/rediscn/commands/rpoplpush.html'>
                <span class='command'>
                  RPOPLPUSH
                  <span class='args'>
                    source
                    destination
                  </span>
                </span>
                <span class='summary'>删除列表中的最后一个元素，将其追加到另一个列表</span>
              </a>
            </li>
            <li data-group='list' data-name='rpush'>
              <a href='/rediscn/commands/rpush.html'>
                <span class='command'>
                  RPUSH
                  <span class='args'>
                    key
                    value [value ...]
                  </span>
                </span>
                <span class='summary'>从队列的右边入队一个元素</span>
              </a>
            </li>
            <li data-group='list' data-name='rpushx'>
              <a href='/rediscn/commands/rpushx.html'>
                <span class='command'>
                  RPUSHX
                  <span class='args'>
                    key
                    value
                  </span>
                </span>
                <span class='summary'>从队列的右边入队一个元素，仅队列存在时有效</span>
              </a>
            </li>
            <li data-group='set' data-name='sadd'>
              <a href='/rediscn/commands/sadd.html'>
                <span class='command'>
                  SADD
                  <span class='args'>
                    key
                    member [member ...]
                  </span>
                </span>
                <span class='summary'>添加一个或者多个元素到集合(set)里</span>
              </a>
            </li>
            <li data-group='server' data-name='save'>
              <a href='/rediscn/commands/save.html'>
                <span class='command'>
                  SAVE
                  <span class='args'>
                  </span>
                </span>
                <span class='summary'>同步数据到磁盘上</span>
              </a>
            </li>
            <li data-group='set' data-name='scard'>
              <a href='/rediscn/commands/scard.html'>
                <span class='command'>
                  SCARD
                  <span class='args'>
                    key
                  </span>
                </span>
                <span class='summary'>获取集合里面的元素数量</span>
              </a>
            </li>
			<li data-group='scripting' data-name='script debug'>
              <a href='/rediscn/commands/script-debug.html'>
                <span class='command'>
                  SCRIPT DEBUG
                  <span class='args'>
                    YES|SYNC|NO
                  </span>
                </span>
                <span class='summary'>设置脚本的调试模式。</span>
              </a>
            </li>
            <li data-group='scripting' data-name='script exists'>
              <a href='/rediscn/commands/script-exists.html'>
                <span class='command'>
                  SCRIPT EXISTS
                  <span class='args'>
                    script [script ...]
                  </span>
                </span>
                <span class='summary'>检查脚本缓存中是否存在脚本。</span>
              </a>
            </li>
            <li data-group='scripting' data-name='script flush'>
              <a href='/rediscn/commands/script-flush.html'>
                <span class='command'>
                  SCRIPT FLUSH
                  <span class='args'>
                  </span>
                </span>
                <span class='summary'>删除服务器缓存中所有Lua脚本。</span>
              </a>
            </li>
            <li data-group='scripting' data-name='script kill'>
              <a href='/rediscn/commands/script-kill.html'>
                <span class='command'>
                  SCRIPT KILL
                  <span class='args'>
                  </span>
                </span>
                <span class='summary'>杀死当前正在运行的 Lua 脚本。</span>
              </a>
            </li>
            <li data-group='scripting' data-name='script load'>
              <a href='/rediscn/commands/script-load.html'>
                <span class='command'>
                  SCRIPT LOAD
                  <span class='args'>
                    script
                  </span>
                </span>
                <span class='summary'>从服务器缓存中装载一个Lua脚本。</span>
              </a>
            </li>
            <li data-group='set' data-name='sdiff'>
              <a href='/rediscn/commands/sdiff.html'>
                <span class='command'>
                  SDIFF
                  <span class='args'>
                    key [key ...]
                  </span>
                </span>
                <span class='summary'>获得队列不存在的元素</span>
              </a>
            </li>
            <li data-group='set' data-name='sdiffstore'>
              <a href='/rediscn/commands/sdiffstore.html'>
                <span class='command'>
                  SDIFFSTORE
                  <span class='args'>
                    destination
                    key [key ...]
                  </span>
                </span>
                <span class='summary'>获得队列不存在的元素，并存储在一个关键的结果集</span>
              </a>
            </li>
            <li data-group='connection' data-name='select'>
              <a href='/rediscn/commands/select.html'>
                <span class='command'>
                  SELECT
                  <span class='args'>
                    index
                  </span>
                </span>
                <span class='summary'>选择新数据库</span>
              </a>
            </li>
            <li data-group='string' data-name='set'>
              <a href='/rediscn/commands/set.html'>
                <span class='command'>
                  SET
                  <span class='args'>
                    key
                    value
                    [EX seconds]
                    [PX milliseconds]
                    [NX|XX]
                  </span>
                </span>
                <span class='summary'>设置一个key的value值</span>
              </a>
            </li>
            <li data-group='string' data-name='setbit'>
              <a href='/rediscn/commands/setbit.html'>
                <span class='command'>
                  SETBIT
                  <span class='args'>
                    key
                    offset
                    value
                  </span>
                </span>
                <span class='summary'>Sets or clears the bit at offset in the string value stored at key</span>
              </a>
            </li>
            <li data-group='string' data-name='setex'>
              <a href='/rediscn/commands/setex.html'>
                <span class='command'>
                  SETEX
                  <span class='args'>
                    key
                    seconds
                    value
                  </span>
                </span>
                <span class='summary'>设置key-value并设置过期时间（单位：秒）</span>
              </a>
            </li>
            <li data-group='string' data-name='setnx'>
              <a href='/rediscn/commands/setnx.html'>
                <span class='command'>
                  SETNX
                  <span class='args'>
                    key
                    value
                  </span>
                </span>
                <span class='summary'>设置的一个关键的价值，只有当该键不存在</span>
              </a>
            </li>
            <li data-group='string' data-name='setrange'>
              <a href='/rediscn/commands/setrange.html'>
                <span class='command'>
                  SETRANGE
                  <span class='args'>
                    key
                    offset
                    value
                  </span>
                </span>
                <span class='summary'>Overwrite part of a string at key starting at the specified offset</span>
              </a>
            </li>
            <li data-group='server' data-name='shutdown'>
              <a href='/rediscn/commands/shutdown.html'>
                <span class='command'>
                  SHUTDOWN
                  <span class='args'>
                    [NOSAVE]
                    [SAVE]
                  </span>
                </span>
                <span class='summary'>关闭服务</span>
              </a>
            </li>
            <li data-group='set' data-name='sinter'>
              <a href='/rediscn/commands/sinter.html'>
                <span class='command'>
                  SINTER
                  <span class='args'>
                    key [key ...]
                  </span>
                </span>
                <span class='summary'>获得两个集合的交集</span>
              </a>
            </li>
            <li data-group='set' data-name='sinterstore'>
              <a href='/rediscn/commands/sinterstore.html'>
                <span class='command'>
                  SINTERSTORE
                  <span class='args'>
                    destination
                    key [key ...]
                  </span>
                </span>
                <span class='summary'>获得两个集合的交集，并存储在一个关键的结果集</span>
              </a>
            </li>
            <li data-group='set' data-name='sismember'>
              <a href='/rediscn/commands/sismember.html'>
                <span class='command'>
                  SISMEMBER
                  <span class='args'>
                    key
                    member
                  </span>
                </span>
                <span class='summary'>确定一个给定的值是一个集合的成员</span>
              </a>
            </li>
            <li data-group='server' data-name='slaveof'>
              <a href='/rediscn/commands/slaveof.html'>
                <span class='command'>
                  SLAVEOF
                  <span class='args'>
                    host
                    port
                  </span>
                </span>
                <span class='summary'>指定当前服务器的主服务器</span>
              </a>
            </li>
            <li data-group='server' data-name='slowlog'>
              <a href='/rediscn/commands/slowlog.html'>
                <span class='command'>
                  SLOWLOG
                  <span class='args'>
                    subcommand
                    [argument]
                  </span>
                </span>
                <span class='summary'>管理再分配的慢查询日志</span>
              </a>
            </li>
            <li data-group='set' data-name='smembers'>
              <a href='/rediscn/commands/smembers.html'>
                <span class='command'>
                  SMEMBERS
                  <span class='args'>
                    key
                  </span>
                </span>
                <span class='summary'>获取集合里面的所有元素</span>
              </a>
            </li>
            <li data-group='set' data-name='smove'>
              <a href='/rediscn/commands/smove.html'>
                <span class='command'>
                  SMOVE
                  <span class='args'>
                    source
                    destination
                    member
                  </span>
                </span>
                <span class='summary'>移动集合里面的一个元素到另一个集合</span>
              </a>
            </li>
            <li data-group='generic' data-name='sort'>
              <a href='/rediscn/commands/sort.html'>
                <span class='command'>
                  SORT
                  <span class='args'>
                    key
                    [BY pattern]
                    [LIMIT offset count]
                    [GET pattern [GET pattern ...]]
                    [ASC|DESC]
                    [ALPHA]
                    [STORE destination]
                  </span>
                </span>
                <span class='summary'>对队列、集合、有序集合排序</span>
              </a>
            </li>
            <li data-group='set' data-name='spop'>
              <a href='/rediscn/commands/spop.html'>
                <span class='command'>
                  SPOP
                  <span class='args'>
                    key
                    [count]
                  </span>
                </span>
                <span class='summary'>删除并获取一个集合里面的元素</span>
              </a>
            </li>
            <li data-group='set' data-name='srandmember'>
              <a href='/rediscn/commands/srandmember.html'>
                <span class='command'>
                  SRANDMEMBER
                  <span class='args'>
                    key
                    [count]
                  </span>
                </span>
                <span class='summary'>从集合里面随机获取一个元素</span>
              </a>
            </li>
            <li data-group='set' data-name='srem'>
              <a href='/rediscn/commands/srem.html'>
                <span class='command'>
                  SREM
                  <span class='args'>
                    key
                    member [member ...]
                  </span>
                </span>
                <span class='summary'>从集合里删除一个或多个元素</span>
              </a>
            </li>
            <li data-group='string' data-name='strlen'>
              <a href='/rediscn/commands/strlen.html'>
                <span class='command'>
                  STRLEN
                  <span class='args'>
                    key
                  </span>
                </span>
                <span class='summary'>获取指定key值的长度</span>
              </a>
            </li>
            <li data-group='pubsub' data-name='subscribe'>
              <a href='/rediscn/commands/subscribe.html'>
                <span class='command'>
                  SUBSCRIBE
                  <span class='args'>
                    channel [channel ...]
                  </span>
                </span>
                <span class='summary'>监听频道发布的消息</span>
              </a>
            </li>
            <li data-group='set' data-name='sunion'>
              <a href='/rediscn/commands/sunion.html'>
                <span class='command'>
                  SUNION
                  <span class='args'>
                    key [key ...]
                  </span>
                </span>
                <span class='summary'>添加多个set元素</span>
              </a>
            </li>
            <li data-group='set' data-name='sunionstore'>
              <a href='/rediscn/commands/sunionstore.html'>
                <span class='command'>
                  SUNIONSTORE
                  <span class='args'>
                    destination
                    key [key ...]
                  </span>
                </span>
                <span class='summary'>合并set元素，并将结果存入新的set里面</span>
              </a>
            </li>
			<li data-group='connection' data-name='swapdb'>
              <a href='/rediscn/commands/swapdb.html'>
                <span class='command'>
                  SWAPDB
                  <span class='args'>
                    index index
                  </span>
                </span>
                <span class='summary'>交换两个 Redis 数据库</span>
              </a>
            </li>
            <li data-group='server' data-name='sync'>
              <a href='/rediscn/commands/sync.html'>
                <span class='command'>
                  SYNC
                  <span class='args'>
                  </span>
                </span>
                <span class='summary'>用于复制的内部命令</span>
              </a>
            </li>
            <li data-group='server' data-name='time'>
              <a href='/rediscn/commands/time.html'>
                <span class='command'>
                  TIME
                  <span class='args'>
                  </span>
                </span>
                <span class='summary'>返回当前服务器时间</span>
              </a>
            </li>
			      <li data-group='keys' data-name='touch'>
              <a href='/rediscn/commands/touch.html'>
                <span class='command'>
                  TOUCH
                  <span class='args'>
					          key [key ...]
                  </span>
                </span>
                <span class='summary'>Alters the last access time of a key(s). Returns the number of existing keys specified.</span>
              </a>
            </li>
            <li data-group='generic' data-name='ttl'>
              <a href='/rediscn/commands/ttl.html'>
                <span class='command'>
                  TTL
                  <span class='args'>
                    key
                  </span>
                </span>
                <span class='summary'>获取key的有效时间（单位：秒）</span>
              </a>
            </li>
            <li data-group='generic' data-name='type'>
              <a href='/rediscn/commands/type.html'>
                <span class='command'>
                  TYPE
                  <span class='args'>
                    key
                  </span>
                </span>
                <span class='summary'>获取key的存储类型</span>
              </a>
            </li>
			<li data-group='keys' data-name='unlink'>
              <a href='/rediscn/commands/unlink.html'>
                <span class='command'>
                  UNLINK
                  <span class='args'>
                    key [key ...]
                  </span>
                </span>
                <span class='summary'>在另一个线程里异步删除 key。它就像 DEL 一样，但非阻塞。</span>
              </a>
            </li>
            <li data-group='pubsub' data-name='unsubscribe'>
              <a href='/rediscn/commands/unsubscribe.html'>
                <span class='command'>
                  UNSUBSCRIBE
                  <span class='args'>
                    [channel [channel ...]]
                  </span>
                </span>
                <span class='summary'>停止频道监听</span>
              </a>
            </li>
            <li data-group='transactions' data-name='unwatch'>
              <a href='/rediscn/commands/unwatch.html'>
                <span class='command'>
                  UNWATCH
                  <span class='args'>
                  </span>
                </span>
                <span class='summary'>取消事务命令</span>
              </a>
            </li>
            <li data-group='generic' data-name='wait'>
              <a href='/rediscn/commands/wait.html'>
                <span class='command'>
                  WAIT
                  <span class='args'>
                    numslaves
                    timeout
                  </span>
                </span>
                <span class='summary'>等待在当前连接的上下文中发送的所有写入命令的同步复制</span>
              </a>
            </li>
            <li data-group='transactions' data-name='watch'>
              <a href='/rediscn/commands/watch.html'>
                <span class='command'>
                  WATCH
                  <span class='args'>
                    key [key ...]
                  </span>
                </span>
                <span class='summary'>锁定key直到执行了 MULTI/EXEC 命令</span>
              </a>
            </li>
			<li data-group='streams' data-name='xack'>
              <a href='/rediscn/commands/xack.html'>
                <span class='command'>
                  XACK
                  <span class='args'>
                    key group ID [ID ...]
                  </span>
                </span>
                <span class='summary'>将挂起的邮件标记为已正确处理，从而有效地将其从使用者组的挂起条目列表中删除。命令的返回值是成功确认的消息数，即我们实际能够在 PEL 中解析的 ID。</span>
              </a>
            </li>
			<li data-group='streams' data-name='xadd'>
              <a href='/rediscn/commands/xadd.html'>
                <span class='command'>
                  XADD
                  <span class='args'>
                    key ID field string [field string ...]
                  </span>
                </span>
                <span class='summary'>将新条目追加到流</span>
              </a>
            </li>
			<li data-group='streams' data-name='xclaim'>
              <a href='/rediscn/commands/xclaim.html'>
                <span class='command'>
                  XCLAIM
                  <span class='args'>
                    key group consumer min-idle-time ID [ID ...] [IDLE ms] [TIME ms-unix-time] [RETRYCOUNT count] [FORCE] [JUSTID]
                  </span>
                </span>
                <span class='summary'>更改（或获取）使用者组中消息的所有权，就像将消息传递给指定的使用者一样。</span>
              </a>
            </li>
			<li data-group='streams' data-name='xdel'>
              <a href='/rediscn/commands/xdel.html'>
                <span class='command'>
                  XDEL
                  <span class='args'>
                    key ID [ID ...]
                  </span>
                </span>
                <span class='summary'>Removes the specified entries from the stream. Returns the number of items actually deleted, that may be different from the number of IDs passed in case certain IDs do not exist.</span>
              </a>
            </li>
			<li data-group='streams' data-name='xgroup'>
              <a href='/rediscn/commands/xgroup.html'>
                <span class='command'>
                  XGROUP
                  <span class='args'>
                    [CREATE key groupname id-or-$] [SETID key id-or-$] [DESTROY key groupname] [DELCONSUMER key groupname consumername]
                  </span>
                </span>
                <span class='summary'>Create, destroy, and manage consumer groups.</span>
              </a>
            </li>
			<li data-group='streams' data-name='xinfo'>
              <a href='/rediscn/commands/xinfo.html'>
                <span class='command'>
                  XINFO
                  <span class='args'>
                    [CONSUMERS key groupname] [GROUPS key] [STREAM key] [HELP]
                  </span>
                </span>
                <span class='summary'>Get information on streams and consumer groups</span>
              </a>
            </li>
			<li data-group='streams' data-name='xlen'>
              <a href='/rediscn/commands/xlen.html'>
                <span class='command'>
                  XLEN
                  <span class='args'>
                    key
                  </span>
                </span>
                <span class='summary'>Return the number of entires in a stream</span>
              </a>
            </li>
			<li data-group='streams' data-name='xpending'>
              <a href='/rediscn/commands/xpending.html'>
                <span class='command'>
                  XPENDING
                  <span class='args'>
                    key group [start end count] [consumer]
                  </span>
                </span>
                <span class='summary'>Return information and entries from a stream consumer group pending entries list, that are messages fetched but never acknowledged.</span>
              </a>
            </li>
			<li data-group='streams' data-name='xrange'>
              <a href='/rediscn/commands/xrange.html'>
                <span class='command'>
                  XRANGE
                  <span class='args'>
                    key start end [COUNT count]
                  </span>
                </span>
                <span class='summary'>Return a range of elements in a stream, with IDs matching the specified IDs interval</span>
              </a>
            </li>
			<li data-group='streams' data-name='xread'>
              <a href='/rediscn/commands/xread.html'>
                <span class='command'>
                  XREAD
                  <span class='args'>
                    [COUNT count] [BLOCK milliseconds] STREAMS key [key ...] ID [ID ...]
                  </span>
                </span>
                <span class='summary'>Return never seen elements in multiple streams, with IDs greater than the ones reported by the caller for each stream. Can block.</span>
              </a>
            </li>
			<li data-group='streams' data-name='xreadgroup'>
              <a href='/rediscn/commands/xreadgroup.html'>
                <span class='command'>
                  XREADGROUP
                  <span class='args'>
                    GROUP group consumer [COUNT count] [BLOCK milliseconds] STREAMS key [key ...] ID [ID ...]
                  </span>
                </span>
                <span class='summary'>Return new entries from a stream using a consumer group, or access the history of the pending entries for a given consumer. Can block.</span>
              </a>
            </li>
			<li data-group='streams' data-name='xrevrange'>
              <a href='/rediscn/commands/xrevrange.html'>
                <span class='command'>
                  XREVRANGE
                  <span class='args'>
                    key end start [COUNT count]
                  </span>
                </span>
                <span class='summary'>Return a range of elements in a stream, with IDs matching the specified IDs interval, in reverse order (from greater to smaller IDs) compared to XRANGE</span>
              </a>
            </li>
			<li data-group='streams' data-name='xtrim'>
              <a href='/rediscn/commands/xtrim.html'>
                <span class='command'>
                  XTRIM
                  <span class='args'>
                    key MAXLEN [~] count
                  </span>
                </span>
                <span class='summary'>Trims the stream to (approximately if '~' is passed) a certain size</span>
              </a>
            </li>
            <li data-group='sorted_set' data-name='zadd'>
              <a href='/rediscn/commands/zadd.html'>
                <span class='command'>
                  ZADD
                  <span class='args'>
                    key
                    [NX|XX]
                    [CH]
                    [INCR]
                    score member [score member ...]
                  </span>
                </span>
                <span class='summary'>添加到有序set的一个或多个成员，或更新的分数，如果它已经存在</span>
              </a>
            </li>
            <li data-group='sorted_set' data-name='zcard'>
              <a href='/rediscn/commands/zcard.html'>
                <span class='command'>
                  ZCARD
                  <span class='args'>
                    key
                  </span>
                </span>
                <span class='summary'>获取一个排序的集合中的成员数量</span>
              </a>
            </li>
            <li data-group='sorted_set' data-name='zcount'>
              <a href='/rediscn/commands/zcount.html'>
                <span class='command'>
                  ZCOUNT
                  <span class='args'>
                    key
                    min
                    max
                  </span>
                </span>
                <span class='summary'>返回分数范围内的成员数量</span>
              </a>
            </li>
            <li data-group='sorted_set' data-name='zincrby'>
              <a href='/rediscn/commands/zincrby.html'>
                <span class='command'>
                  ZINCRBY
                  <span class='args'>
                    key
                    increment
                    member
                  </span>
                </span>
                <span class='summary'>增量的一名成员在排序设置的评分</span>
              </a>
            </li>
            <li data-group='sorted_set' data-name='zinterstore'>
              <a href='/rediscn/commands/zinterstore.html'>
                <span class='command'>
                  ZINTERSTORE
                  <span class='args'>
                    destination
                    numkeys
                    key [key ...]
                    [WEIGHTS weight [weight ...]]
                    [AGGREGATE SUM|MIN|MAX]
                  </span>
                </span>
                <span class='summary'>相交多个排序集，导致排序的设置存储在一个新的关键</span>
              </a>
            </li>
            <li data-group='sorted_set' data-name='zlexcount'>
              <a href='/rediscn/commands/zlexcount.html'>
                <span class='command'>
                  ZLEXCOUNT
                  <span class='args'>
                    key
                    min
                    max
                  </span>
                </span>
                <span class='summary'>返回成员之间的成员数量</span>
              </a>
            </li>
			<li data-group='sorted_set' data-name='zpopmax'>
              <a href='/rediscn/commands/zpopmax.html'>
                <span class='command'>
                  ZPOPMAX
                  <span class='args'>
                    key [count]
                  </span>
                </span>
                <span class='summary'>弹出 sorted set 中得分最高的成员</span>
              </a>
            </li>
			<li data-group='sorted_set' data-name='zpopmin'>
              <a href='/rediscn/commands/zpopmin.html'>
                <span class='command'>
                  ZPOPMIN
                  <span class='args'>
                    key [count]
                  </span>
                </span>
                <span class='summary'>弹出 sorted set 中得分最低的成员</span>
              </a>
            </li>
            <li data-group='sorted_set' data-name='zrange'>
              <a href='/rediscn/commands/zrange.html'>
                <span class='command'>
                  ZRANGE
                  <span class='args'>
                    key
                    start
                    stop
                    [WITHSCORES]
                  </span>
                </span>
                <span class='summary'>根据指定的index返回，返回sorted set的成员列表</span>
              </a>
            </li>
            <li data-group='sorted_set' data-name='zrangebylex'>
              <a href='/rediscn/commands/zrangebylex.html'>
                <span class='command'>
                  ZRANGEBYLEX
                  <span class='args'>
                    key
                    min
                    max
                    [LIMIT offset count]
                  </span>
                </span>
                <span class='summary'>返回指定成员区间内的成员，按字典正序排列, 分数必须相同。</span>
              </a>
            </li>
            <li data-group='sorted_set' data-name='zrevrangebylex'>
              <a href='/rediscn/commands/zrevrangebylex.html'>
                <span class='command'>
                  ZREVRANGEBYLEX
                  <span class='args'>
                    key
                    max
                    min
                    [LIMIT offset count]
                  </span>
                </span>
                <span class='summary'>返回指定成员区间内的成员，按字典倒序排列, 分数必须相同</span>
              </a>
            </li>
            <li data-group='sorted_set' data-name='zrangebyscore'>
              <a href='/rediscn/commands/zrangebyscore.html'>
                <span class='command'>
                  ZRANGEBYSCORE
                  <span class='args'>
                    key
                    min
                    max
                    [WITHSCORES]
                    [LIMIT offset count]
                  </span>
                </span>
                <span class='summary'>返回有序集合中指定分数区间内的成员，分数由低到高排序。</span>
              </a>
            </li>
            <li data-group='sorted_set' data-name='zrank'>
              <a href='/rediscn/commands/zrank.html'>
                <span class='command'>
                  ZRANK
                  <span class='args'>
                    key
                    member
                  </span>
                </span>
                <span class='summary'>确定在排序集合成员的索引</span>
              </a>
            </li>
            <li data-group='sorted_set' data-name='zrem'>
              <a href='/rediscn/commands/zrem.html'>
                <span class='command'>
                  ZREM
                  <span class='args'>
                    key
                    member [member ...]
                  </span>
                </span>
                <span class='summary'>从排序的集合中删除一个或多个成员</span>
              </a>
            </li>
            <li data-group='sorted_set' data-name='zremrangebylex'>
              <a href='/rediscn/commands/zremrangebylex.html'>
                <span class='command'>
                  ZREMRANGEBYLEX
                  <span class='args'>
                    key
                    min
                    max
                  </span>
                </span>
                <span class='summary'>删除名称按字典由低到高排序成员之间所有成员。</span>
              </a>
            </li>
            <li data-group='sorted_set' data-name='zremrangebyrank'>
              <a href='/rediscn/commands/zremrangebyrank.html'>
                <span class='command'>
                  ZREMRANGEBYRANK
                  <span class='args'>
                    key
                    start
                    stop
                  </span>
                </span>
                <span class='summary'>在排序设置的所有成员在给定的索引中删除</span>
              </a>
            </li>
            <li data-group='sorted_set' data-name='zremrangebyscore'>
              <a href='/rediscn/commands/zremrangebyscore.html'>
                <span class='command'>
                  ZREMRANGEBYSCORE
                  <span class='args'>
                    key
                    min
                    max
                  </span>
                </span>
                <span class='summary'>删除一个排序的设置在给定的分数所有成员</span>
              </a>
            </li>
            <li data-group='sorted_set' data-name='zrevrange'>
              <a href='/rediscn/commands/zrevrange.html'>
                <span class='command'>
                  ZREVRANGE
                  <span class='args'>
                    key
                    start
                    stop
                    [WITHSCORES]
                  </span>
                </span>
                <span class='summary'>在排序的设置返回的成员范围，通过索引，下令从分数高到低</span>
              </a>
            </li>
            <li data-group='sorted_set' data-name='zrevrangebyscore'>
              <a href='/rediscn/commands/zrevrangebyscore.html'>
                <span class='command'>
                  ZREVRANGEBYSCORE
                  <span class='args'>
                    key
                    max
                    min
                    [WITHSCORES]
                    [LIMIT offset count]
                  </span>
                </span>
                <span class='summary'>返回有序集合中指定分数区间内的成员，分数由高到低排序。</span>
              </a>
            </li>
            <li data-group='sorted_set' data-name='zrevrank'>
              <a href='/rediscn/commands/zrevrank.html'>
                <span class='command'>
                  ZREVRANK
                  <span class='args'>
                    key
                    member
                  </span>
                </span>
                <span class='summary'>确定指数在排序集的成员，下令从分数高到低</span>
              </a>
            </li>
            <li data-group='sorted_set' data-name='zscore'>
              <a href='/rediscn/commands/zscore.html'>
                <span class='command'>
                  ZSCORE
                  <span class='args'>
                    key
                    member
                  </span>
                </span>
                <span class='summary'>获取成员在排序设置相关的比分</span>
              </a>
            </li>
            <li data-group='sorted_set' data-name='zunionstore'>
              <a href='/rediscn/commands/zunionstore.html'>
                <span class='command'>
                  ZUNIONSTORE
                  <span class='args'>
                    destination
                    numkeys
                    key [key ...]
                    [WEIGHTS weight [weight ...]]
                    [AGGREGATE SUM|MIN|MAX]
                  </span>
                </span>
                <span class='summary'>添加多个排序集和导致排序的设置存储在一个新的关键</span>
              </a>
            </li>
            <li data-group='generic' data-name='scan'>
              <a href='/rediscn/commands/scan.html'>
                <span class='command'>
                  SCAN
                  <span class='args'>
                    cursor
                    [MATCH pattern]
                    [COUNT count]
                  </span>
                </span>
                <span class='summary'>增量迭代key</span>
              </a>
            </li>
            <li data-group='set' data-name='sscan'>
              <a href='/rediscn/commands/sscan.html'>
                <span class='command'>
                  SSCAN
                  <span class='args'>
                    key
                    cursor
                    [MATCH pattern]
                    [COUNT count]
                  </span>
                </span>
                <span class='summary'>迭代set里面的元素</span>
              </a>
            </li>
            <li data-group='hash' data-name='hscan'>
              <a href='/rediscn/commands/hscan.html'>
                <span class='command'>
                  HSCAN
                  <span class='args'>
                    key
                    cursor
                    [MATCH pattern]
                    [COUNT count]
                  </span>
                </span>
                <span class='summary'>迭代hash里面的元素</span>
              </a>
            </li>
            <li data-group='sorted_set' data-name='zscan'>
              <a href='/rediscn/commands/zscan.html'>
                <span class='command'>
                  ZSCAN
                  <span class='args'>
                    key
                    cursor
                    [MATCH pattern]
                    [COUNT count]
                  </span>
                </span>
                <span class='summary'>迭代sorted sets里面的元素</span>
              </a>
            </li>
          </ul>
        </div>
<div class='container'>
	如果你对Redis命令使用有任何问题，欢迎到<a href="http://bbs.redis.cn/" target="_blank">Redis论坛</a>进行讨论,这里云集国内Redis使用者，一定有你想要的答案。
</div>
</section>