# 查询所有网络ACL组<a name="vpc_firewall_0013"></a>

## 功能介绍<a name="section11380465132652"></a>

查询提交请求的租户有权限操作的所有网络ACL组信息。单次查询最多返回2000条数据，超过2000后会返回分页标记。分页查询请参考[分页查询](分页查询.md)。

## URI<a name="section38164372132652"></a>

GET /v2.0/fwaas/firewall\_groups

分页查询样例：

```
GET https://{Endpoint}/v2.0/fwaas/firewall_groups?limit=2&marker=cd600d47-0045-483f-87a1-5041ae2f513b&page_reverse=False
```

参数说明请参见[表1](#table2285151162120)。

**表 1**  参数说明

<a name="table2285151162120"></a>
<table><thead align="left"><tr id="row439021115215"><th class="cellrowborder" valign="top" width="19.971997199719972%" id="mcps1.2.5.1.1"><p id="p19390141117210"><a name="p19390141117210"></a><a name="p19390141117210"></a>名称</p>
</th>
<th class="cellrowborder" valign="top" width="16.39163916391639%" id="mcps1.2.5.1.2"><p id="p163901911102116"><a name="p163901911102116"></a><a name="p163901911102116"></a>是否必选</p>
</th>
<th class="cellrowborder" valign="top" width="19.851985198519852%" id="mcps1.2.5.1.3"><p id="p15390171102117"><a name="p15390171102117"></a><a name="p15390171102117"></a>参数类型</p>
</th>
<th class="cellrowborder" valign="top" width="43.784378437843785%" id="mcps1.2.5.1.4"><p id="p339051116218"><a name="p339051116218"></a><a name="p339051116218"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row1739012116211"><td class="cellrowborder" valign="top" width="19.971997199719972%" headers="mcps1.2.5.1.1 "><p id="p1139011142114"><a name="p1139011142114"></a><a name="p1139011142114"></a>id</p>
</td>
<td class="cellrowborder" valign="top" width="16.39163916391639%" headers="mcps1.2.5.1.2 "><p id="p0390511162114"><a name="p0390511162114"></a><a name="p0390511162114"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="19.851985198519852%" headers="mcps1.2.5.1.3 "><p id="p83901011172115"><a name="p83901011172115"></a><a name="p83901011172115"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="43.784378437843785%" headers="mcps1.2.5.1.4 "><p id="p23908114217"><a name="p23908114217"></a><a name="p23908114217"></a>按照网络ACL组对应的ID过滤查询</p>
</td>
</tr>
<tr id="row83901711182112"><td class="cellrowborder" valign="top" width="19.971997199719972%" headers="mcps1.2.5.1.1 "><p id="p2390911172112"><a name="p2390911172112"></a><a name="p2390911172112"></a>name</p>
</td>
<td class="cellrowborder" valign="top" width="16.39163916391639%" headers="mcps1.2.5.1.2 "><p id="p539041162115"><a name="p539041162115"></a><a name="p539041162115"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="19.851985198519852%" headers="mcps1.2.5.1.3 "><p id="p3390141110213"><a name="p3390141110213"></a><a name="p3390141110213"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="43.784378437843785%" headers="mcps1.2.5.1.4 "><p id="p133901211162112"><a name="p133901211162112"></a><a name="p133901211162112"></a>按照网络ACL组的名称过滤查询</p>
</td>
</tr>
<tr id="row03901117211"><td class="cellrowborder" valign="top" width="19.971997199719972%" headers="mcps1.2.5.1.1 "><p id="p139013118211"><a name="p139013118211"></a><a name="p139013118211"></a>description</p>
</td>
<td class="cellrowborder" valign="top" width="16.39163916391639%" headers="mcps1.2.5.1.2 "><p id="p163901211192116"><a name="p163901211192116"></a><a name="p163901211192116"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="19.851985198519852%" headers="mcps1.2.5.1.3 "><p id="p4391101182113"><a name="p4391101182113"></a><a name="p4391101182113"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="43.784378437843785%" headers="mcps1.2.5.1.4 "><p id="p14391161112114"><a name="p14391161112114"></a><a name="p14391161112114"></a>按照网络ACL组的描述过滤查询</p>
</td>
</tr>
<tr id="row2391191118211"><td class="cellrowborder" valign="top" width="19.971997199719972%" headers="mcps1.2.5.1.1 "><p id="p43911911112110"><a name="p43911911112110"></a><a name="p43911911112110"></a>admin_state_up</p>
</td>
<td class="cellrowborder" valign="top" width="16.39163916391639%" headers="mcps1.2.5.1.2 "><p id="p163911311132119"><a name="p163911311132119"></a><a name="p163911311132119"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="19.851985198519852%" headers="mcps1.2.5.1.3 "><p id="p11391181115216"><a name="p11391181115216"></a><a name="p11391181115216"></a>Booleab</p>
</td>
<td class="cellrowborder" valign="top" width="43.784378437843785%" headers="mcps1.2.5.1.4 "><p id="p2715182372114"><a name="p2715182372114"></a><a name="p2715182372114"></a>按照网络ACL组的管理状态过滤查询</p>
<p id="p1339181115217"><a name="p1339181115217"></a><a name="p1339181115217"></a>取值范围：true or false</p>
</td>
</tr>
<tr id="row83911211112115"><td class="cellrowborder" valign="top" width="19.971997199719972%" headers="mcps1.2.5.1.1 "><p id="p16391181172119"><a name="p16391181172119"></a><a name="p16391181172119"></a>tenant_id</p>
</td>
<td class="cellrowborder" valign="top" width="16.39163916391639%" headers="mcps1.2.5.1.2 "><p id="p439151115210"><a name="p439151115210"></a><a name="p439151115210"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="19.851985198519852%" headers="mcps1.2.5.1.3 "><p id="p7391171114213"><a name="p7391171114213"></a><a name="p7391171114213"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="43.784378437843785%" headers="mcps1.2.5.1.4 "><p id="p143911111142114"><a name="p143911111142114"></a><a name="p143911111142114"></a>按照网络ACL组所属的项目ID过滤查询</p>
</td>
</tr>
<tr id="row1239110118217"><td class="cellrowborder" valign="top" width="19.971997199719972%" headers="mcps1.2.5.1.1 "><p id="p20391111142113"><a name="p20391111142113"></a><a name="p20391111142113"></a>marker</p>
</td>
<td class="cellrowborder" valign="top" width="16.39163916391639%" headers="mcps1.2.5.1.2 "><p id="p2391161142119"><a name="p2391161142119"></a><a name="p2391161142119"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="19.851985198519852%" headers="mcps1.2.5.1.3 "><p id="p83911911142119"><a name="p83911911142119"></a><a name="p83911911142119"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="43.784378437843785%" headers="mcps1.2.5.1.4 "><p id="p639191113214"><a name="p639191113214"></a><a name="p639191113214"></a>分页查询起始的资源ID，为空时为查询第一页</p>
</td>
</tr>
<tr id="row039113115215"><td class="cellrowborder" valign="top" width="19.971997199719972%" headers="mcps1.2.5.1.1 "><p id="p43911611132116"><a name="p43911611132116"></a><a name="p43911611132116"></a>limit</p>
</td>
<td class="cellrowborder" valign="top" width="16.39163916391639%" headers="mcps1.2.5.1.2 "><p id="p163911811172115"><a name="p163911811172115"></a><a name="p163911811172115"></a>否</p>
</td>
<td class="cellrowborder" valign="top" width="19.851985198519852%" headers="mcps1.2.5.1.3 "><p id="p1039131162116"><a name="p1039131162116"></a><a name="p1039131162116"></a>Integer</p>
</td>
<td class="cellrowborder" valign="top" width="43.784378437843785%" headers="mcps1.2.5.1.4 "><p id="p6190327172119"><a name="p6190327172119"></a><a name="p6190327172119"></a>每页返回的个数</p>
<p id="p193911011122112"><a name="p193911011122112"></a><a name="p193911011122112"></a>取值范围：0~intmax</p>
</td>
</tr>
</tbody>
</table>

## 请求消息<a name="section30244758132652"></a>

无。

## 响应消息<a name="section48852885132652"></a>

**表 2**  响应参数

<a name="table25605667132652"></a>
<table><thead align="left"><tr id="row26621002132652"><th class="cellrowborder" valign="top" width="23.330000000000002%" id="mcps1.2.4.1.1"><p id="p17188156132652"><a name="p17188156132652"></a><a name="p17188156132652"></a>参数名称</p>
</th>
<th class="cellrowborder" valign="top" width="17.78%" id="mcps1.2.4.1.2"><p id="p29579284132652"><a name="p29579284132652"></a><a name="p29579284132652"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="58.89%" id="mcps1.2.4.1.3"><p id="p37495801132652"><a name="p37495801132652"></a><a name="p37495801132652"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row29258567132652"><td class="cellrowborder" valign="top" width="23.330000000000002%" headers="mcps1.2.4.1.1 "><p id="p7598331132652"><a name="p7598331132652"></a><a name="p7598331132652"></a>firewall_groups</p>
</td>
<td class="cellrowborder" valign="top" width="17.78%" headers="mcps1.2.4.1.2 "><p id="p50785846132652"><a name="p50785846132652"></a><a name="p50785846132652"></a>Array of <a href="#table31629250121127">Firewall Group</a> objects</p>
</td>
<td class="cellrowborder" valign="top" width="58.89%" headers="mcps1.2.4.1.3 "><p id="p48871362132652"><a name="p48871362132652"></a><a name="p48871362132652"></a>firewall group对象列表。请参见<a href="#table31629250121127">表3</a>。</p>
</td>
</tr>
</tbody>
</table>

**表 3**  Firewall Group对象

<a name="table31629250121127"></a>
<table><thead align="left"><tr id="row45711693121127"><th class="cellrowborder" valign="top" width="35.3%" id="mcps1.2.4.1.1"><p id="p46819705121127"><a name="p46819705121127"></a><a name="p46819705121127"></a>属性</p>
</th>
<th class="cellrowborder" valign="top" width="21.57%" id="mcps1.2.4.1.2"><p id="p35064605121127"><a name="p35064605121127"></a><a name="p35064605121127"></a>类型</p>
</th>
<th class="cellrowborder" valign="top" width="43.13%" id="mcps1.2.4.1.3"><p id="p11952850121127"><a name="p11952850121127"></a><a name="p11952850121127"></a>说明</p>
</th>
</tr>
</thead>
<tbody><tr id="row20395689121127"><td class="cellrowborder" valign="top" width="35.3%" headers="mcps1.2.4.1.1 "><p id="p50168503121127"><a name="p50168503121127"></a><a name="p50168503121127"></a>id</p>
</td>
<td class="cellrowborder" valign="top" width="21.57%" headers="mcps1.2.4.1.2 "><p id="p47513116121127"><a name="p47513116121127"></a><a name="p47513116121127"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="43.13%" headers="mcps1.2.4.1.3 "><p id="p62072725121127"><a name="p62072725121127"></a><a name="p62072725121127"></a>网络ACL组的uuid标识。</p>
</td>
</tr>
<tr id="row34896104121127"><td class="cellrowborder" valign="top" width="35.3%" headers="mcps1.2.4.1.1 "><p id="p52608071121127"><a name="p52608071121127"></a><a name="p52608071121127"></a>name</p>
</td>
<td class="cellrowborder" valign="top" width="21.57%" headers="mcps1.2.4.1.2 "><p id="p59846605121127"><a name="p59846605121127"></a><a name="p59846605121127"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="43.13%" headers="mcps1.2.4.1.3 "><p id="p28604909121127"><a name="p28604909121127"></a><a name="p28604909121127"></a>网络ACL组名称。</p>
</td>
</tr>
<tr id="row11129246121127"><td class="cellrowborder" valign="top" width="35.3%" headers="mcps1.2.4.1.1 "><p id="p39887063121127"><a name="p39887063121127"></a><a name="p39887063121127"></a>description</p>
</td>
<td class="cellrowborder" valign="top" width="21.57%" headers="mcps1.2.4.1.2 "><p id="p28745735121127"><a name="p28745735121127"></a><a name="p28745735121127"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="43.13%" headers="mcps1.2.4.1.3 "><p id="p35639020121127"><a name="p35639020121127"></a><a name="p35639020121127"></a>网络ACL组描述。</p>
</td>
</tr>
<tr id="row677472121127"><td class="cellrowborder" valign="top" width="35.3%" headers="mcps1.2.4.1.1 "><p id="p60717947121127"><a name="p60717947121127"></a><a name="p60717947121127"></a>tenant_id</p>
</td>
<td class="cellrowborder" valign="top" width="21.57%" headers="mcps1.2.4.1.2 "><p id="p65871708121127"><a name="p65871708121127"></a><a name="p65871708121127"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="43.13%" headers="mcps1.2.4.1.3 "><p id="p10487112"><a name="p10487112"></a><a name="p10487112"></a>项目ID</p>
</td>
</tr>
<tr id="row38137474121127"><td class="cellrowborder" valign="top" width="35.3%" headers="mcps1.2.4.1.1 "><p id="p35500294121127"><a name="p35500294121127"></a><a name="p35500294121127"></a>ingress_firewall_policy_id</p>
</td>
<td class="cellrowborder" valign="top" width="21.57%" headers="mcps1.2.4.1.2 "><p id="p49995809121127"><a name="p49995809121127"></a><a name="p49995809121127"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="43.13%" headers="mcps1.2.4.1.3 "><p id="p56499442121127"><a name="p56499442121127"></a><a name="p56499442121127"></a>入方向网络ACL策略。</p>
</td>
</tr>
<tr id="row9094936121127"><td class="cellrowborder" valign="top" width="35.3%" headers="mcps1.2.4.1.1 "><p id="p34911245121127"><a name="p34911245121127"></a><a name="p34911245121127"></a>egress_firewall_policy_id</p>
</td>
<td class="cellrowborder" valign="top" width="21.57%" headers="mcps1.2.4.1.2 "><p id="p44624490121127"><a name="p44624490121127"></a><a name="p44624490121127"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="43.13%" headers="mcps1.2.4.1.3 "><p id="p37100641121127"><a name="p37100641121127"></a><a name="p37100641121127"></a>出方向网络ACL策略。</p>
</td>
</tr>
<tr id="row31622902121127"><td class="cellrowborder" valign="top" width="35.3%" headers="mcps1.2.4.1.1 "><p id="p65911012121127"><a name="p65911012121127"></a><a name="p65911012121127"></a>ports</p>
</td>
<td class="cellrowborder" valign="top" width="21.57%" headers="mcps1.2.4.1.2 "><p id="p5459978121127"><a name="p5459978121127"></a><a name="p5459978121127"></a>Array of strings</p>
</td>
<td class="cellrowborder" valign="top" width="43.13%" headers="mcps1.2.4.1.3 "><p id="p61002567121127"><a name="p61002567121127"></a><a name="p61002567121127"></a>网络ACL组绑定的端口列表。</p>
</td>
</tr>
<tr id="row48186031121127"><td class="cellrowborder" valign="top" width="35.3%" headers="mcps1.2.4.1.1 "><p id="p33368479121127"><a name="p33368479121127"></a><a name="p33368479121127"></a>public</p>
</td>
<td class="cellrowborder" valign="top" width="21.57%" headers="mcps1.2.4.1.2 "><p id="p7938198121127"><a name="p7938198121127"></a><a name="p7938198121127"></a>Boolean</p>
</td>
<td class="cellrowborder" valign="top" width="43.13%" headers="mcps1.2.4.1.3 "><p id="p56166201121127"><a name="p56166201121127"></a><a name="p56166201121127"></a>是否支持跨租户共享。</p>
</td>
</tr>
<tr id="row60912436121127"><td class="cellrowborder" valign="top" width="35.3%" headers="mcps1.2.4.1.1 "><p id="p66273781121127"><a name="p66273781121127"></a><a name="p66273781121127"></a>status</p>
</td>
<td class="cellrowborder" valign="top" width="21.57%" headers="mcps1.2.4.1.2 "><p id="p7141533121127"><a name="p7141533121127"></a><a name="p7141533121127"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="43.13%" headers="mcps1.2.4.1.3 "><p id="p6468335121127"><a name="p6468335121127"></a><a name="p6468335121127"></a>网络ACL策略的状态。</p>
</td>
</tr>
<tr id="row59833296121127"><td class="cellrowborder" valign="top" width="35.3%" headers="mcps1.2.4.1.1 "><p id="p44051842121127"><a name="p44051842121127"></a><a name="p44051842121127"></a>admin_state_up</p>
</td>
<td class="cellrowborder" valign="top" width="21.57%" headers="mcps1.2.4.1.2 "><p id="p58587899121127"><a name="p58587899121127"></a><a name="p58587899121127"></a>Boolean</p>
</td>
<td class="cellrowborder" valign="top" width="43.13%" headers="mcps1.2.4.1.3 "><p id="p3428646121127"><a name="p3428646121127"></a><a name="p3428646121127"></a>网络ACL是否受管理员控制。</p>
</td>
</tr>
<tr id="row7228115213486"><td class="cellrowborder" valign="top" width="35.3%" headers="mcps1.2.4.1.1 "><p id="p53071912134918"><a name="p53071912134918"></a><a name="p53071912134918"></a>project_id</p>
</td>
<td class="cellrowborder" valign="top" width="21.57%" headers="mcps1.2.4.1.2 "><p id="p1731011220498"><a name="p1731011220498"></a><a name="p1731011220498"></a>String</p>
</td>
<td class="cellrowborder" valign="top" width="43.13%" headers="mcps1.2.4.1.3 "><p id="p2078552513296"><a name="p2078552513296"></a><a name="p2078552513296"></a>项目ID，请参见<a href="获取项目ID.md">获取项目ID</a>。</p>
</td>
</tr>
</tbody>
</table>

## 样例<a name="section19537091132652"></a>

请求样例

```
GET https://{Endpoint}/v2.0/fwaas/firewall_groups
```

响应样例

```
{
    "firewall_groups": [
        {
            "status": "INACTIVE", 
            "public": false, 
            "egress_firewall_policy_id": null, 
            "name": "", 
            "admin_state_up": true, 
            "ports": [ ], 
            "tenant_id": "23c8a121505047b6869edf39f3062712", 
            "id": "cd600d47-0045-483f-87a1-5041ae2f513b", 
            "ingress_firewall_policy_id": null, 
            "description": "",
            "project_id": "23c8a121505047b6869edf39f3062712"
        }, 
        {
            "status": "INACTIVE", 
            "public": false, 
            "egress_firewall_policy_id": "d939df29-fe76-4089-90c3-3778e4d53141", 
            "name": "fwg-1475475043", 
            "admin_state_up": true, 
            "ports": [ ], 
            "tenant_id": "0af57070695044ea9a70f04779e6aa1f", 
            "id": "ca971b45-70ce-4879-9734-b6cac1d00845", 
            "ingress_firewall_policy_id": "d939df29-fe76-4089-90c3-3778e4d53141", 
            "description": "",
            "project_id": "0af57070695044ea9a70f04779e6aa1f"
        }
    ]
}
```

## 状态码<a name="section10470352390"></a>

请参见[状态码](状态码.md)。

## 错误码<a name="section85821649202813"></a>

请参见[错误码](错误码.md)。

