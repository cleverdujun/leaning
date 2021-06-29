除客户端 API 外，XX还提供 RESTful 形式的服务端 API，通过发送 HTTPS 请求就可以获取 （GET），更新（PUT）, 创建 （POST），删除 （DELETE） 应用、坐席、呼叫等相关数据或执行相关操作。



## <span id="能力开通">能力开通</span>

<table>
<tr>
<th width="15%"><b>API</b></th>
<th width="10%"><b>方法</b></th>
<th width="40%"><b>请求 URL</b></th>
</tr>
<tr>
<td><a href="/docs/jcyOTA0ODM/jg3NjcyNTE">创建租户</a></td>
<td>POST</td>
<td><code>http://voip-test-21.v1.yunxin.jd1.vpc:7702/api/v1/voip/account/tenants</code></td>
</tr>
<tr>
<td><a href="/docs/jcyOTA0ODM/TI5MTIwNDc">删除租户</a></td>
<td>DELETE</td>
<td><ul><li><code>http://voip-test-21.v1.yunxin.jd1.vpc:7702/api/v1/voip/account/tenants/{tenant}</code></td>
</tr>
<tr>
<td><a href="/docs/jcyOTA0ODM/jUzODcwODE">更新租户</a></td>
<td>GET</td>
<td><ul><li><code>https://logic-dev.netease.im/v2/api/rooms/{cid}/members</code><li><code>https://logic-dev.netease.im/v3/api/rooms/members?cname={cname}</code></td>
</tr>
<tr>
<td><a href="/docs/jcyOTA0ODM/TA5MTExNjg">查回租户调地址</a></td>
<td>POST</td>
<td><ul><li><code>https://logic-dev.netease.im/v2/api/kicklist/{cid}/members/{uid}</code><li><code>https://logic-dev.netease.im/v3/api/kicklist/members?cname={cname}&uid={uid}</code></td>
</tr>
<tr>
<td><a href="/docs/jcyOTA0ODM/zAzNjE5NTM">应用创建</a></td>
<td>GET</td>
<td><ul><li><code>https://logic-dev.netease.im/v2/api/kicklist/{cid}</code><li><code>https://logic-dev.netease.im/v3/api/kicklist?cname={cname}</code></td>
</tr>
<tr>
<td><a href="/docs/jcyOTA0ODM/TA2NTYzMTQ">更新应用状态</a></td>
<td>DELETE</td>
<td><ul><li><code>https://logic-dev.netease.im/v2/api/kicklist/{cid}/members/{uid}</code><li><code>https://logic-dev.netease.im/v3/api/kicklist/members?cname={cname}&uid={uid}</code></td>
</tr>
<tr>
<td><a href="/docs/jcyOTA0ODM/DM2NzQyMTc">更新应用租户信息</a></td>
<td>DELETE</td>
<td><ul><li><code>https://logic-dev.netease.im/v2/api/rooms/{cid}</code><li><code>https://logic-dev.netease.im/v3/api/rooms?cname={cname}</code></td>
</tr>
</table>


## 云端录制

<table>
<tr>
<th width="15%"><b>API</b></th>
<th width="10%"><b>方法</b></th>
<th width="40%"><b>请求 URL</b></th>
</tr>
<tr>
<td><a href="/docs/jcyOTA0ODM/jA5NTIzOTY">云端录制</a></td>
<td>POST</td>
<td><ul><li><code>https://logic-dev.netease.im/v2/api/record/{cid}</code><li><code>https://logic-dev.netease.im/v3/api/record?cname={cname}</code></td>
</tr>
<tr>
<td><a href="/docs/jcyOTA0ODM/jYwNzI3MDk">查询云端录制文件信息</a></td>
<td>POST</td>
<td><code>https://api.netease.im/nimserver/history/queryMediaFileByChannelId.action</code></td>
</tr>
</table>
