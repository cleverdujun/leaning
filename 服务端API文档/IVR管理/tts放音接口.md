队列创建


## <span id="URL">URL</span>

- 请求方法：POST
- URL：`http://voip-host/api/v1/voip/cti/app/ivr/tts`

## <span id="请求参数">请求参数</span>

<table>
<tr>
<td width=13%><b>参数名称</b></td>
<td width=10%><b>类型</b></td>
<td width=10%><b>是否必选</b></td>
<td width=13%><b>示例</b></td>
<td width=40%><b>描述</b></td>
</tr>

<tr>
<td>appId</td>
<td>String</td>
<td>必填</td>
<td>eca23f68c66d4acfceee77c200200359</td>
<td>应用ID。</td>
</tr>

<tr>
<td>callId</td>
<td>String</td>
<td>必填</td>
<td>eca23f68c66d4acfceee77c200200444</td>
<td>会话ID。</td>
</tr>

<tr>
<td>tts</td>
<td>string</td>
<td>必填</td>
<td>你好，我现在在写restpai文档，没有时间</td>
<td>文本或文件url，放音文本长度不能超过500 。</td>
</tr>

<tr>
<td>type</td>
<td>int</td>
<td>选填</td>
<td>1</td>
<td>类型。0：文本；1：文件名，默认 0 。</td>
</tr>


<tr>
<td>repeat</td>
<td>int</td>
<td>选填</td>
<td>1</td>
<td>重复次数，默认 1 次，参数repeat的取值范围为1-10。</td>
</tr>

<tr>
<td>data</td>
<td>string</td>
<td>选填</td>
<td>我是透传数据</td>
<td>透传数据。</td>
</tr>

<tr>
<td>funcType</td>
<td>int</td>
<td>选填</td>
<td>1</td>
<td>功能类型. 0: 普通呼叫, 1: 智能呼叫。</td>
</tr>

</table>

## <span id="返回参数">返回参数</span>

<table>
<tr>
<td width=13%><b>参数名称</b></td>
<td width=13%><b>类型</b></td>
<td width=13%><b>示例</b></td>
<td width=40%><b>描述</b></td>
</tr>
<tr>
<td>code</td>
<td>int</td>
<td>0</td>
<td>状态码。</td>
</tr>
<tr>
<td>message</td>
<td>string</td>
<td>OK</td>
<td>请求成功或者失败描述信息。</td>
</tr>
</table>

## <span id="示例">示例</span>

### <span id="请求示例">请求示例</span>

```
{
  "appId": "eca23f68c66d4acfceee77c200200359",
  "callId": "eca23f68c66d4acfceee77c200200444",
  "data": "我就是要放音的句子",
  "funcType": 0,
  "repeat": 1,
  "tts": "你好，我现在在写restpai文档，没有时间",
  "type": 0
}
```

### <span id="正常返回示例">正常返回示例</span> 

```
{
  "code": 0,
  "message": "OK"
}
```

## <span id="错误码">错误码</span>

- header 中的状态码：
    
    状态码列表请参考 [header 中的 HTTP 状态码](/docs/jcyOTA0ODM/DY2NDIwMTM)。
)

- body 中的错误码（code）

    该接口在 HTTP Body 中返回错误码（code），错误码列表请参考[业务错误码](/docs/jcyOTA0ODM/TQ3Njc1Nzg)。