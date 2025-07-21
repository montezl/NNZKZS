# 后台服务API接口文档


**简介**:后台服务API接口文档


**HOST**:116.8.105.191


**联系人**:海南佳创天狮科技有限公司


**Version**:1.0


**接口路径**:/v2/api-docs


[TOC]






# ccccccccccccccccccccccccc


## 测试


**接口地址**:`/nnzk/sfsagag/test`


**请求方式**:`GET`


**请求数据类型**:`application/x-www-form-urlencoded`


**响应数据类型**:`*/*`


**接口描述**:<p>测试</p>



**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|key|key|query|true|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«object»|
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|object||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": {},
	"success": true,
	"timestamp": 0
}
```


# e


## 数据集主表-添加


**接口地址**:`/nnzk/drag/onlDragDatasetHead/add`


**请求方式**:`POST`


**请求数据类型**:`application/json`


**响应数据类型**:`*/*`


**接口描述**:<p>数据集主表-添加</p>



**请求示例**:


```javascript
{
  "apiMethod": "",
  "code": "",
  "content": "",
  "createBy": "",
  "createTime": "",
  "dataType": "",
  "datasetItemList": [
    {
      "createBy": "",
      "createTime": "",
      "dictCode": "",
      "fieldName": "",
      "fieldTxt": "",
      "fieldType": "",
      "headId": "",
      "id": "",
      "izSearch": "",
      "izShow": "",
      "izTotal": "",
      "orderNum": 0,
      "searchMode": "",
      "updateBy": "",
      "updateTime": "",
      "widgetType": ""
    }
  ],
  "datasetParamList": [
    {
      "createBy": "",
      "createTime": "",
      "dictCode": "",
      "headId": "",
      "id": "",
      "izSearch": 0,
      "orderNum": 0,
      "paramName": "",
      "paramTxt": "",
      "paramValue": "",
      "searchMode": 0,
      "updateBy": "",
      "updateTime": "",
      "widgetType": ""
    }
  ],
  "dbSource": "",
  "id": "",
  "izAgent": "",
  "name": "",
  "parentId": "",
  "querySql": "",
  "updateBy": "",
  "updateTime": ""
}
```


**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|param0|param0|body|true|OnlDragDatasetHeadPage|OnlDragDatasetHeadPage|
|&emsp;&emsp;apiMethod|||false|string||
|&emsp;&emsp;code|||false|string||
|&emsp;&emsp;content|||false|string||
|&emsp;&emsp;createBy|||false|string||
|&emsp;&emsp;createTime|||false|string(date-time)||
|&emsp;&emsp;dataType|||false|string||
|&emsp;&emsp;datasetItemList|||false|array|onl_drag_dataset_item对象|
|&emsp;&emsp;&emsp;&emsp;createBy|创建人||false|string||
|&emsp;&emsp;&emsp;&emsp;createTime|创建时间||false|string||
|&emsp;&emsp;&emsp;&emsp;dictCode|字典编码||false|string||
|&emsp;&emsp;&emsp;&emsp;fieldName|字段名||false|string||
|&emsp;&emsp;&emsp;&emsp;fieldTxt|字段文本||false|string||
|&emsp;&emsp;&emsp;&emsp;fieldType|字段类型||false|string||
|&emsp;&emsp;&emsp;&emsp;headId|主表ID||false|string||
|&emsp;&emsp;&emsp;&emsp;id|id||false|string||
|&emsp;&emsp;&emsp;&emsp;izSearch|是否查询||false|string||
|&emsp;&emsp;&emsp;&emsp;izShow|是否显示||false|string||
|&emsp;&emsp;&emsp;&emsp;izTotal|是否计算总计||false|string||
|&emsp;&emsp;&emsp;&emsp;orderNum|排序||false|integer||
|&emsp;&emsp;&emsp;&emsp;searchMode|查询模式||false|string||
|&emsp;&emsp;&emsp;&emsp;updateBy|修改人||false|string||
|&emsp;&emsp;&emsp;&emsp;updateTime|修改时间||false|string||
|&emsp;&emsp;&emsp;&emsp;widgetType|控件类型||false|string||
|&emsp;&emsp;datasetParamList|||false|array|onl_drag_dataset_param对象|
|&emsp;&emsp;&emsp;&emsp;createBy|创建人登录名称||false|string||
|&emsp;&emsp;&emsp;&emsp;createTime|创建日期||false|string||
|&emsp;&emsp;&emsp;&emsp;dictCode|字典||false|string||
|&emsp;&emsp;&emsp;&emsp;headId|动态报表ID||false|string||
|&emsp;&emsp;&emsp;&emsp;id|id||false|string||
|&emsp;&emsp;&emsp;&emsp;izSearch|查询标识0否1是 默认0||false|integer||
|&emsp;&emsp;&emsp;&emsp;orderNum|排序||false|integer||
|&emsp;&emsp;&emsp;&emsp;paramName|参数字段||false|string||
|&emsp;&emsp;&emsp;&emsp;paramTxt|参数文本||false|string||
|&emsp;&emsp;&emsp;&emsp;paramValue|参数默认值||false|string||
|&emsp;&emsp;&emsp;&emsp;searchMode|查询模式1简单2范围||false|integer||
|&emsp;&emsp;&emsp;&emsp;updateBy|更新人登录名称||false|string||
|&emsp;&emsp;&emsp;&emsp;updateTime|更新日期||false|string||
|&emsp;&emsp;&emsp;&emsp;widgetType|查询控件类型||false|string||
|&emsp;&emsp;dbSource|||false|string||
|&emsp;&emsp;id|||false|string||
|&emsp;&emsp;izAgent|||false|string||
|&emsp;&emsp;name|||false|string||
|&emsp;&emsp;parentId|||false|string||
|&emsp;&emsp;querySql|||false|string||
|&emsp;&emsp;updateBy|||false|string||
|&emsp;&emsp;updateTime|||false|string(date-time)||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«object»|
|201|Created||
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|object||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": {},
	"success": true,
	"timestamp": 0
}
```


## 数据集分组-添加


**接口地址**:`/nnzk/drag/onlDragDatasetHead/addGroup`


**请求方式**:`POST`


**请求数据类型**:`application/json`


**响应数据类型**:`*/*`


**接口描述**:<p>数据集分组-添加</p>



**请求示例**:


```javascript
{
  "apiMethod": "",
  "code": "",
  "content": "",
  "createBy": "",
  "createTime": "",
  "dataType": "",
  "dbSource": "",
  "id": "",
  "izAgent": "",
  "lowAppId": "",
  "name": "",
  "parentId": "",
  "querySql": "",
  "tenantId": 0,
  "updateBy": "",
  "updateTime": ""
}
```


**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|param0|param0|body|true|OnlDragDatasetHead|OnlDragDatasetHead|
|&emsp;&emsp;apiMethod|||false|string||
|&emsp;&emsp;code|||false|string||
|&emsp;&emsp;content|||false|string||
|&emsp;&emsp;createBy|||false|string||
|&emsp;&emsp;createTime|||false|string(date-time)||
|&emsp;&emsp;dataType|||false|string||
|&emsp;&emsp;dbSource|||false|string||
|&emsp;&emsp;id|||false|string||
|&emsp;&emsp;izAgent|||false|string||
|&emsp;&emsp;lowAppId|||false|string||
|&emsp;&emsp;name|||false|string||
|&emsp;&emsp;parentId|||false|string||
|&emsp;&emsp;querySql|||false|string||
|&emsp;&emsp;tenantId|||false|integer(int32)||
|&emsp;&emsp;updateBy|||false|string||
|&emsp;&emsp;updateTime|||false|string(date-time)||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«object»|
|201|Created||
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|object||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": {},
	"success": true,
	"timestamp": 0
}
```


## 数据集分组-通过id删除


**接口地址**:`/nnzk/drag/onlDragDatasetHead/delDragDataSetHeadGroup`


**请求方式**:`DELETE`


**请求数据类型**:`application/x-www-form-urlencoded`


**响应数据类型**:`*/*`


**接口描述**:<p>数据集分组-通过id删除</p>



**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|id|id|query|true|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«object»|
|204|No Content||
|401|Unauthorized||
|403|Forbidden||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|object||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": {},
	"success": true,
	"timestamp": 0
}
```


## 数据集主表-通过id删除


**接口地址**:`/nnzk/drag/onlDragDatasetHead/delete`


**请求方式**:`DELETE`


**请求数据类型**:`application/x-www-form-urlencoded`


**响应数据类型**:`*/*`


**接口描述**:<p>数据集主表-通过id删除</p>



**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|id|id|query|true|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«object»|
|204|No Content||
|401|Unauthorized||
|403|Forbidden||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|object||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": {},
	"success": true,
	"timestamp": 0
}
```


## 数据集-编辑


**接口地址**:`/nnzk/drag/onlDragDatasetHead/edit`


**请求方式**:`POST`


**请求数据类型**:`application/json`


**响应数据类型**:`*/*`


**接口描述**:<p>数据集-编辑</p>



**请求示例**:


```javascript
{
  "apiMethod": "",
  "code": "",
  "content": "",
  "createBy": "",
  "createTime": "",
  "dataType": "",
  "datasetItemList": [
    {
      "createBy": "",
      "createTime": "",
      "dictCode": "",
      "fieldName": "",
      "fieldTxt": "",
      "fieldType": "",
      "headId": "",
      "id": "",
      "izSearch": "",
      "izShow": "",
      "izTotal": "",
      "orderNum": 0,
      "searchMode": "",
      "updateBy": "",
      "updateTime": "",
      "widgetType": ""
    }
  ],
  "datasetParamList": [
    {
      "createBy": "",
      "createTime": "",
      "dictCode": "",
      "headId": "",
      "id": "",
      "izSearch": 0,
      "orderNum": 0,
      "paramName": "",
      "paramTxt": "",
      "paramValue": "",
      "searchMode": 0,
      "updateBy": "",
      "updateTime": "",
      "widgetType": ""
    }
  ],
  "dbSource": "",
  "id": "",
  "izAgent": "",
  "name": "",
  "parentId": "",
  "querySql": "",
  "updateBy": "",
  "updateTime": ""
}
```


**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|param0|param0|body|true|OnlDragDatasetHeadPage|OnlDragDatasetHeadPage|
|&emsp;&emsp;apiMethod|||false|string||
|&emsp;&emsp;code|||false|string||
|&emsp;&emsp;content|||false|string||
|&emsp;&emsp;createBy|||false|string||
|&emsp;&emsp;createTime|||false|string(date-time)||
|&emsp;&emsp;dataType|||false|string||
|&emsp;&emsp;datasetItemList|||false|array|onl_drag_dataset_item对象|
|&emsp;&emsp;&emsp;&emsp;createBy|创建人||false|string||
|&emsp;&emsp;&emsp;&emsp;createTime|创建时间||false|string||
|&emsp;&emsp;&emsp;&emsp;dictCode|字典编码||false|string||
|&emsp;&emsp;&emsp;&emsp;fieldName|字段名||false|string||
|&emsp;&emsp;&emsp;&emsp;fieldTxt|字段文本||false|string||
|&emsp;&emsp;&emsp;&emsp;fieldType|字段类型||false|string||
|&emsp;&emsp;&emsp;&emsp;headId|主表ID||false|string||
|&emsp;&emsp;&emsp;&emsp;id|id||false|string||
|&emsp;&emsp;&emsp;&emsp;izSearch|是否查询||false|string||
|&emsp;&emsp;&emsp;&emsp;izShow|是否显示||false|string||
|&emsp;&emsp;&emsp;&emsp;izTotal|是否计算总计||false|string||
|&emsp;&emsp;&emsp;&emsp;orderNum|排序||false|integer||
|&emsp;&emsp;&emsp;&emsp;searchMode|查询模式||false|string||
|&emsp;&emsp;&emsp;&emsp;updateBy|修改人||false|string||
|&emsp;&emsp;&emsp;&emsp;updateTime|修改时间||false|string||
|&emsp;&emsp;&emsp;&emsp;widgetType|控件类型||false|string||
|&emsp;&emsp;datasetParamList|||false|array|onl_drag_dataset_param对象|
|&emsp;&emsp;&emsp;&emsp;createBy|创建人登录名称||false|string||
|&emsp;&emsp;&emsp;&emsp;createTime|创建日期||false|string||
|&emsp;&emsp;&emsp;&emsp;dictCode|字典||false|string||
|&emsp;&emsp;&emsp;&emsp;headId|动态报表ID||false|string||
|&emsp;&emsp;&emsp;&emsp;id|id||false|string||
|&emsp;&emsp;&emsp;&emsp;izSearch|查询标识0否1是 默认0||false|integer||
|&emsp;&emsp;&emsp;&emsp;orderNum|排序||false|integer||
|&emsp;&emsp;&emsp;&emsp;paramName|参数字段||false|string||
|&emsp;&emsp;&emsp;&emsp;paramTxt|参数文本||false|string||
|&emsp;&emsp;&emsp;&emsp;paramValue|参数默认值||false|string||
|&emsp;&emsp;&emsp;&emsp;searchMode|查询模式1简单2范围||false|integer||
|&emsp;&emsp;&emsp;&emsp;updateBy|更新人登录名称||false|string||
|&emsp;&emsp;&emsp;&emsp;updateTime|更新日期||false|string||
|&emsp;&emsp;&emsp;&emsp;widgetType|查询控件类型||false|string||
|&emsp;&emsp;dbSource|||false|string||
|&emsp;&emsp;id|||false|string||
|&emsp;&emsp;izAgent|||false|string||
|&emsp;&emsp;name|||false|string||
|&emsp;&emsp;parentId|||false|string||
|&emsp;&emsp;querySql|||false|string||
|&emsp;&emsp;updateBy|||false|string||
|&emsp;&emsp;updateTime|||false|string(date-time)||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«object»|
|201|Created||
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|object||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": {},
	"success": true,
	"timestamp": 0
}
```


## 数据集-编辑


**接口地址**:`/nnzk/drag/onlDragDatasetHead/edit`


**请求方式**:`PUT`


**请求数据类型**:`application/json`


**响应数据类型**:`*/*`


**接口描述**:<p>数据集-编辑</p>



**请求示例**:


```javascript
{
  "apiMethod": "",
  "code": "",
  "content": "",
  "createBy": "",
  "createTime": "",
  "dataType": "",
  "datasetItemList": [
    {
      "createBy": "",
      "createTime": "",
      "dictCode": "",
      "fieldName": "",
      "fieldTxt": "",
      "fieldType": "",
      "headId": "",
      "id": "",
      "izSearch": "",
      "izShow": "",
      "izTotal": "",
      "orderNum": 0,
      "searchMode": "",
      "updateBy": "",
      "updateTime": "",
      "widgetType": ""
    }
  ],
  "datasetParamList": [
    {
      "createBy": "",
      "createTime": "",
      "dictCode": "",
      "headId": "",
      "id": "",
      "izSearch": 0,
      "orderNum": 0,
      "paramName": "",
      "paramTxt": "",
      "paramValue": "",
      "searchMode": 0,
      "updateBy": "",
      "updateTime": "",
      "widgetType": ""
    }
  ],
  "dbSource": "",
  "id": "",
  "izAgent": "",
  "name": "",
  "parentId": "",
  "querySql": "",
  "updateBy": "",
  "updateTime": ""
}
```


**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|param0|param0|body|true|OnlDragDatasetHeadPage|OnlDragDatasetHeadPage|
|&emsp;&emsp;apiMethod|||false|string||
|&emsp;&emsp;code|||false|string||
|&emsp;&emsp;content|||false|string||
|&emsp;&emsp;createBy|||false|string||
|&emsp;&emsp;createTime|||false|string(date-time)||
|&emsp;&emsp;dataType|||false|string||
|&emsp;&emsp;datasetItemList|||false|array|onl_drag_dataset_item对象|
|&emsp;&emsp;&emsp;&emsp;createBy|创建人||false|string||
|&emsp;&emsp;&emsp;&emsp;createTime|创建时间||false|string||
|&emsp;&emsp;&emsp;&emsp;dictCode|字典编码||false|string||
|&emsp;&emsp;&emsp;&emsp;fieldName|字段名||false|string||
|&emsp;&emsp;&emsp;&emsp;fieldTxt|字段文本||false|string||
|&emsp;&emsp;&emsp;&emsp;fieldType|字段类型||false|string||
|&emsp;&emsp;&emsp;&emsp;headId|主表ID||false|string||
|&emsp;&emsp;&emsp;&emsp;id|id||false|string||
|&emsp;&emsp;&emsp;&emsp;izSearch|是否查询||false|string||
|&emsp;&emsp;&emsp;&emsp;izShow|是否显示||false|string||
|&emsp;&emsp;&emsp;&emsp;izTotal|是否计算总计||false|string||
|&emsp;&emsp;&emsp;&emsp;orderNum|排序||false|integer||
|&emsp;&emsp;&emsp;&emsp;searchMode|查询模式||false|string||
|&emsp;&emsp;&emsp;&emsp;updateBy|修改人||false|string||
|&emsp;&emsp;&emsp;&emsp;updateTime|修改时间||false|string||
|&emsp;&emsp;&emsp;&emsp;widgetType|控件类型||false|string||
|&emsp;&emsp;datasetParamList|||false|array|onl_drag_dataset_param对象|
|&emsp;&emsp;&emsp;&emsp;createBy|创建人登录名称||false|string||
|&emsp;&emsp;&emsp;&emsp;createTime|创建日期||false|string||
|&emsp;&emsp;&emsp;&emsp;dictCode|字典||false|string||
|&emsp;&emsp;&emsp;&emsp;headId|动态报表ID||false|string||
|&emsp;&emsp;&emsp;&emsp;id|id||false|string||
|&emsp;&emsp;&emsp;&emsp;izSearch|查询标识0否1是 默认0||false|integer||
|&emsp;&emsp;&emsp;&emsp;orderNum|排序||false|integer||
|&emsp;&emsp;&emsp;&emsp;paramName|参数字段||false|string||
|&emsp;&emsp;&emsp;&emsp;paramTxt|参数文本||false|string||
|&emsp;&emsp;&emsp;&emsp;paramValue|参数默认值||false|string||
|&emsp;&emsp;&emsp;&emsp;searchMode|查询模式1简单2范围||false|integer||
|&emsp;&emsp;&emsp;&emsp;updateBy|更新人登录名称||false|string||
|&emsp;&emsp;&emsp;&emsp;updateTime|更新日期||false|string||
|&emsp;&emsp;&emsp;&emsp;widgetType|查询控件类型||false|string||
|&emsp;&emsp;dbSource|||false|string||
|&emsp;&emsp;id|||false|string||
|&emsp;&emsp;izAgent|||false|string||
|&emsp;&emsp;name|||false|string||
|&emsp;&emsp;parentId|||false|string||
|&emsp;&emsp;querySql|||false|string||
|&emsp;&emsp;updateBy|||false|string||
|&emsp;&emsp;updateTime|||false|string(date-time)||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«object»|
|201|Created||
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|object||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": {},
	"success": true,
	"timestamp": 0
}
```


## 数据集主表-通过id查询


**接口地址**:`/nnzk/drag/onlDragDatasetHead/queryById`


**请求方式**:`GET`


**请求数据类型**:`application/x-www-form-urlencoded`


**响应数据类型**:`*/*`


**接口描述**:<p>数据集主表-通过id查询</p>



**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|id|id|query|true|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«object»|
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|object||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": {},
	"success": true,
	"timestamp": 0
}
```


## 数据集分组-更新


**接口地址**:`/nnzk/drag/onlDragDatasetHead/updateGroup`


**请求方式**:`POST`


**请求数据类型**:`application/json`


**响应数据类型**:`*/*`


**接口描述**:<p>数据集分组-更新</p>



**请求示例**:


```javascript
{
  "apiMethod": "",
  "code": "",
  "content": "",
  "createBy": "",
  "createTime": "",
  "dataType": "",
  "dbSource": "",
  "id": "",
  "izAgent": "",
  "lowAppId": "",
  "name": "",
  "parentId": "",
  "querySql": "",
  "tenantId": 0,
  "updateBy": "",
  "updateTime": ""
}
```


**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|param0|param0|body|true|OnlDragDatasetHead|OnlDragDatasetHead|
|&emsp;&emsp;apiMethod|||false|string||
|&emsp;&emsp;code|||false|string||
|&emsp;&emsp;content|||false|string||
|&emsp;&emsp;createBy|||false|string||
|&emsp;&emsp;createTime|||false|string(date-time)||
|&emsp;&emsp;dataType|||false|string||
|&emsp;&emsp;dbSource|||false|string||
|&emsp;&emsp;id|||false|string||
|&emsp;&emsp;izAgent|||false|string||
|&emsp;&emsp;lowAppId|||false|string||
|&emsp;&emsp;name|||false|string||
|&emsp;&emsp;parentId|||false|string||
|&emsp;&emsp;querySql|||false|string||
|&emsp;&emsp;tenantId|||false|integer(int32)||
|&emsp;&emsp;updateBy|||false|string||
|&emsp;&emsp;updateTime|||false|string(date-time)||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«object»|
|201|Created||
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|object||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": {},
	"success": true,
	"timestamp": 0
}
```


# 中职专业表


## 中职专业表-添加


**接口地址**:`/nnzk/zzmanagement/zzProfession/add`


**请求方式**:`POST`


**请求数据类型**:`application/json`


**响应数据类型**:`*/*`


**接口描述**:<p>中职专业表-添加</p>



**请求示例**:


```javascript
{
  "createBy": "",
  "createTime": "",
  "delFlag": 0,
  "dispOrder": 0,
  "id": "",
  "proCode": "",
  "proName": "",
  "updateBy": "",
  "updateTime": ""
}
```


**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|zzProfession|中职专业表|body|true|zz_profession对象|zz_profession对象|
|&emsp;&emsp;createBy|创建人||false|string||
|&emsp;&emsp;createTime|创建日期||false|string(date-time)||
|&emsp;&emsp;delFlag|删除标签||false|integer(int32)||
|&emsp;&emsp;dispOrder|填报显示顺序||false|integer(int32)||
|&emsp;&emsp;id|主键||false|string||
|&emsp;&emsp;proCode|专业代码||false|string||
|&emsp;&emsp;proName|专业名称||false|string||
|&emsp;&emsp;updateBy|更新人||false|string||
|&emsp;&emsp;updateTime|更新日期||false|string(date-time)||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«string»|
|201|Created||
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|string||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": "",
	"success": true,
	"timestamp": 0
}
```


## 中职专业表-通过id删除


**接口地址**:`/nnzk/zzmanagement/zzProfession/delete`


**请求方式**:`DELETE`


**请求数据类型**:`application/x-www-form-urlencoded`


**响应数据类型**:`*/*`


**接口描述**:<p>中职专业表-通过id删除</p>



**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|id|id|query|true|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«string»|
|204|No Content||
|401|Unauthorized||
|403|Forbidden||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|string||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": "",
	"success": true,
	"timestamp": 0
}
```


## 中职专业表-批量删除


**接口地址**:`/nnzk/zzmanagement/zzProfession/deleteBatch`


**请求方式**:`DELETE`


**请求数据类型**:`application/x-www-form-urlencoded`


**响应数据类型**:`*/*`


**接口描述**:<p>中职专业表-批量删除</p>



**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|ids|ids|query|true|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«string»|
|204|No Content||
|401|Unauthorized||
|403|Forbidden||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|string||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": "",
	"success": true,
	"timestamp": 0
}
```


## 中职专业表-编辑


**接口地址**:`/nnzk/zzmanagement/zzProfession/edit`


**请求方式**:`POST`


**请求数据类型**:`application/json`


**响应数据类型**:`*/*`


**接口描述**:<p>中职专业表-编辑</p>



**请求示例**:


```javascript
{
  "createBy": "",
  "createTime": "",
  "delFlag": 0,
  "dispOrder": 0,
  "id": "",
  "proCode": "",
  "proName": "",
  "updateBy": "",
  "updateTime": ""
}
```


**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|zzProfession|中职专业表|body|true|zz_profession对象|zz_profession对象|
|&emsp;&emsp;createBy|创建人||false|string||
|&emsp;&emsp;createTime|创建日期||false|string(date-time)||
|&emsp;&emsp;delFlag|删除标签||false|integer(int32)||
|&emsp;&emsp;dispOrder|填报显示顺序||false|integer(int32)||
|&emsp;&emsp;id|主键||false|string||
|&emsp;&emsp;proCode|专业代码||false|string||
|&emsp;&emsp;proName|专业名称||false|string||
|&emsp;&emsp;updateBy|更新人||false|string||
|&emsp;&emsp;updateTime|更新日期||false|string(date-time)||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«string»|
|201|Created||
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|string||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": "",
	"success": true,
	"timestamp": 0
}
```


## 中职专业表-编辑


**接口地址**:`/nnzk/zzmanagement/zzProfession/edit`


**请求方式**:`PUT`


**请求数据类型**:`application/json`


**响应数据类型**:`*/*`


**接口描述**:<p>中职专业表-编辑</p>



**请求示例**:


```javascript
{
  "createBy": "",
  "createTime": "",
  "delFlag": 0,
  "dispOrder": 0,
  "id": "",
  "proCode": "",
  "proName": "",
  "updateBy": "",
  "updateTime": ""
}
```


**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|zzProfession|中职专业表|body|true|zz_profession对象|zz_profession对象|
|&emsp;&emsp;createBy|创建人||false|string||
|&emsp;&emsp;createTime|创建日期||false|string(date-time)||
|&emsp;&emsp;delFlag|删除标签||false|integer(int32)||
|&emsp;&emsp;dispOrder|填报显示顺序||false|integer(int32)||
|&emsp;&emsp;id|主键||false|string||
|&emsp;&emsp;proCode|专业代码||false|string||
|&emsp;&emsp;proName|专业名称||false|string||
|&emsp;&emsp;updateBy|更新人||false|string||
|&emsp;&emsp;updateTime|更新日期||false|string(date-time)||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«string»|
|201|Created||
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|string||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": "",
	"success": true,
	"timestamp": 0
}
```


## 中职专业表-分页列表查询


**接口地址**:`/nnzk/zzmanagement/zzProfession/list`


**请求方式**:`GET`


**请求数据类型**:`application/x-www-form-urlencoded`


**响应数据类型**:`*/*`


**接口描述**:<p>中职专业表-分页列表查询</p>



**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|dispOrder|填报显示顺序|query|true|integer(int32)||
|proCode|专业代码|query|true|string||
|proName|专业名称|query|true|string||
|createBy|创建人|query|false|string||
|createTime|创建日期|query|false|string(date-time)||
|delFlag|删除标签|query|false|integer(int32)||
|id|主键|query|false|string||
|pageNo|pageNo|query|false|integer(int32)||
|pageSize|pageSize|query|false|integer(int32)||
|updateBy|更新人|query|false|string||
|updateTime|更新日期|query|false|string(date-time)||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«IPage«zz_profession对象»»|
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|IPage«zz_profession对象»|IPage«zz_profession对象»|
|&emsp;&emsp;current||integer(int64)||
|&emsp;&emsp;pages||integer(int64)||
|&emsp;&emsp;records||array|zz_profession对象|
|&emsp;&emsp;&emsp;&emsp;createBy|创建人|string||
|&emsp;&emsp;&emsp;&emsp;createTime|创建日期|string||
|&emsp;&emsp;&emsp;&emsp;delFlag|删除标签|integer||
|&emsp;&emsp;&emsp;&emsp;dispOrder|填报显示顺序|integer||
|&emsp;&emsp;&emsp;&emsp;id|主键|string||
|&emsp;&emsp;&emsp;&emsp;proCode|专业代码|string||
|&emsp;&emsp;&emsp;&emsp;proName|专业名称|string||
|&emsp;&emsp;&emsp;&emsp;updateBy|更新人|string||
|&emsp;&emsp;&emsp;&emsp;updateTime|更新日期|string||
|&emsp;&emsp;size||integer(int64)||
|&emsp;&emsp;total||integer(int64)||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": {
		"current": 0,
		"pages": 0,
		"records": [
			{
				"createBy": "",
				"createTime": "",
				"delFlag": 0,
				"dispOrder": 0,
				"id": "",
				"proCode": "",
				"proName": "",
				"updateBy": "",
				"updateTime": ""
			}
		],
		"size": 0,
		"total": 0
	},
	"success": true,
	"timestamp": 0
}
```


## 中职专业表-通过id查询


**接口地址**:`/nnzk/zzmanagement/zzProfession/queryById`


**请求方式**:`GET`


**请求数据类型**:`application/x-www-form-urlencoded`


**响应数据类型**:`*/*`


**接口描述**:<p>中职专业表-通过id查询</p>



**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|id|id|query|true|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«zz_profession对象»|
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|zz_profession对象|zz_profession对象|
|&emsp;&emsp;createBy|创建人|string||
|&emsp;&emsp;createTime|创建日期|string(date-time)||
|&emsp;&emsp;delFlag|删除标签|integer(int32)||
|&emsp;&emsp;dispOrder|填报显示顺序|integer(int32)||
|&emsp;&emsp;id|主键|string||
|&emsp;&emsp;proCode|专业代码|string||
|&emsp;&emsp;proName|专业名称|string||
|&emsp;&emsp;updateBy|更新人|string||
|&emsp;&emsp;updateTime|更新日期|string(date-time)||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": {
		"createBy": "",
		"createTime": "",
		"delFlag": 0,
		"dispOrder": 0,
		"id": "",
		"proCode": "",
		"proName": "",
		"updateBy": "",
		"updateTime": ""
	},
	"success": true,
	"timestamp": 0
}
```


# 中职学校专业表


## 中职学校专业表-添加


**接口地址**:`/nnzk/zzmanagement/zzProOfSch/add`


**请求方式**:`POST`


**请求数据类型**:`application/json`


**响应数据类型**:`*/*`


**接口描述**:<p>中职学校专业表-添加</p>



**请求示例**:


```javascript
{
  "createBy": "",
  "createTime": "",
  "delFlag": 0,
  "direction": "",
  "eduType": "",
  "eduUnion": "",
  "eduYear": "",
  "id": "",
  "levelType": "",
  "num": 0,
  "proCode": "",
  "proIdOfSch": "",
  "schoolCode": "",
  "season": "",
  "state": "",
  "unionSchool": "",
  "updateBy": "",
  "updateTime": ""
}
```


**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|zzProOfSch|中职学校专业表|body|true|zz_pro_of_sch对象|zz_pro_of_sch对象|
|&emsp;&emsp;createBy|创建人||false|string||
|&emsp;&emsp;createTime|创建日期||false|string(date-time)||
|&emsp;&emsp;delFlag|删除标签||false|integer(int32)||
|&emsp;&emsp;direction|专业化方向||false|string||
|&emsp;&emsp;eduType|教学方式||false|string||
|&emsp;&emsp;eduUnion|办学方式||false|string||
|&emsp;&emsp;eduYear|学制||false|string||
|&emsp;&emsp;id|主键||false|string||
|&emsp;&emsp;levelType|招生类别||false|string||
|&emsp;&emsp;num|人数||false|integer(int32)||
|&emsp;&emsp;proCode|专业编号||false|string||
|&emsp;&emsp;proIdOfSch|学校专业代码||false|string||
|&emsp;&emsp;schoolCode|学校代码||false|string||
|&emsp;&emsp;season|招生时段||false|string||
|&emsp;&emsp;state|状态||false|string||
|&emsp;&emsp;unionSchool|联合办学学校||false|string||
|&emsp;&emsp;updateBy|更新人||false|string||
|&emsp;&emsp;updateTime|更新日期||false|string(date-time)||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«string»|
|201|Created||
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|string||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": "",
	"success": true,
	"timestamp": 0
}
```


## 中职学校专业表-通过id删除


**接口地址**:`/nnzk/zzmanagement/zzProOfSch/delete`


**请求方式**:`DELETE`


**请求数据类型**:`application/x-www-form-urlencoded`


**响应数据类型**:`*/*`


**接口描述**:<p>中职学校专业表-通过id删除</p>



**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|id|id|query|true|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«string»|
|204|No Content||
|401|Unauthorized||
|403|Forbidden||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|string||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": "",
	"success": true,
	"timestamp": 0
}
```


## 中职学校专业表-批量删除


**接口地址**:`/nnzk/zzmanagement/zzProOfSch/deleteBatch`


**请求方式**:`DELETE`


**请求数据类型**:`application/x-www-form-urlencoded`


**响应数据类型**:`*/*`


**接口描述**:<p>中职学校专业表-批量删除</p>



**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|ids|ids|query|true|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«string»|
|204|No Content||
|401|Unauthorized||
|403|Forbidden||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|string||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": "",
	"success": true,
	"timestamp": 0
}
```


## 中职学校专业表-编辑


**接口地址**:`/nnzk/zzmanagement/zzProOfSch/edit`


**请求方式**:`POST`


**请求数据类型**:`application/json`


**响应数据类型**:`*/*`


**接口描述**:<p>中职学校专业表-编辑</p>



**请求示例**:


```javascript
{
  "createBy": "",
  "createTime": "",
  "delFlag": 0,
  "direction": "",
  "eduType": "",
  "eduUnion": "",
  "eduYear": "",
  "id": "",
  "levelType": "",
  "num": 0,
  "proCode": "",
  "proIdOfSch": "",
  "schoolCode": "",
  "season": "",
  "state": "",
  "unionSchool": "",
  "updateBy": "",
  "updateTime": ""
}
```


**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|zzProOfSch|中职学校专业表|body|true|zz_pro_of_sch对象|zz_pro_of_sch对象|
|&emsp;&emsp;createBy|创建人||false|string||
|&emsp;&emsp;createTime|创建日期||false|string(date-time)||
|&emsp;&emsp;delFlag|删除标签||false|integer(int32)||
|&emsp;&emsp;direction|专业化方向||false|string||
|&emsp;&emsp;eduType|教学方式||false|string||
|&emsp;&emsp;eduUnion|办学方式||false|string||
|&emsp;&emsp;eduYear|学制||false|string||
|&emsp;&emsp;id|主键||false|string||
|&emsp;&emsp;levelType|招生类别||false|string||
|&emsp;&emsp;num|人数||false|integer(int32)||
|&emsp;&emsp;proCode|专业编号||false|string||
|&emsp;&emsp;proIdOfSch|学校专业代码||false|string||
|&emsp;&emsp;schoolCode|学校代码||false|string||
|&emsp;&emsp;season|招生时段||false|string||
|&emsp;&emsp;state|状态||false|string||
|&emsp;&emsp;unionSchool|联合办学学校||false|string||
|&emsp;&emsp;updateBy|更新人||false|string||
|&emsp;&emsp;updateTime|更新日期||false|string(date-time)||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«string»|
|201|Created||
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|string||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": "",
	"success": true,
	"timestamp": 0
}
```


## 中职学校专业表-编辑


**接口地址**:`/nnzk/zzmanagement/zzProOfSch/edit`


**请求方式**:`PUT`


**请求数据类型**:`application/json`


**响应数据类型**:`*/*`


**接口描述**:<p>中职学校专业表-编辑</p>



**请求示例**:


```javascript
{
  "createBy": "",
  "createTime": "",
  "delFlag": 0,
  "direction": "",
  "eduType": "",
  "eduUnion": "",
  "eduYear": "",
  "id": "",
  "levelType": "",
  "num": 0,
  "proCode": "",
  "proIdOfSch": "",
  "schoolCode": "",
  "season": "",
  "state": "",
  "unionSchool": "",
  "updateBy": "",
  "updateTime": ""
}
```


**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|zzProOfSch|中职学校专业表|body|true|zz_pro_of_sch对象|zz_pro_of_sch对象|
|&emsp;&emsp;createBy|创建人||false|string||
|&emsp;&emsp;createTime|创建日期||false|string(date-time)||
|&emsp;&emsp;delFlag|删除标签||false|integer(int32)||
|&emsp;&emsp;direction|专业化方向||false|string||
|&emsp;&emsp;eduType|教学方式||false|string||
|&emsp;&emsp;eduUnion|办学方式||false|string||
|&emsp;&emsp;eduYear|学制||false|string||
|&emsp;&emsp;id|主键||false|string||
|&emsp;&emsp;levelType|招生类别||false|string||
|&emsp;&emsp;num|人数||false|integer(int32)||
|&emsp;&emsp;proCode|专业编号||false|string||
|&emsp;&emsp;proIdOfSch|学校专业代码||false|string||
|&emsp;&emsp;schoolCode|学校代码||false|string||
|&emsp;&emsp;season|招生时段||false|string||
|&emsp;&emsp;state|状态||false|string||
|&emsp;&emsp;unionSchool|联合办学学校||false|string||
|&emsp;&emsp;updateBy|更新人||false|string||
|&emsp;&emsp;updateTime|更新日期||false|string(date-time)||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«string»|
|201|Created||
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|string||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": "",
	"success": true,
	"timestamp": 0
}
```


## 中职学校专业表-分页列表查询


**接口地址**:`/nnzk/zzmanagement/zzProOfSch/list`


**请求方式**:`GET`


**请求数据类型**:`application/x-www-form-urlencoded`


**响应数据类型**:`*/*`


**接口描述**:<p>中职学校专业表-分页列表查询</p>



**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|direction|专业化方向|query|true|string||
|eduType|教学方式|query|true|string||
|eduUnion|办学方式|query|true|string||
|eduYear|学制|query|true|string||
|levelType|招生类别|query|true|string||
|num|人数|query|true|integer(int32)||
|proCode|专业编号|query|true|string||
|proIdOfSch|学校专业代码|query|true|string||
|schoolCode|学校代码|query|true|string||
|season|招生时段|query|true|string||
|state|状态|query|true|string||
|createBy|创建人|query|false|string||
|createTime|创建日期|query|false|string(date-time)||
|delFlag|删除标签|query|false|integer(int32)||
|id|主键|query|false|string||
|pageNo|pageNo|query|false|integer(int32)||
|pageSize|pageSize|query|false|integer(int32)||
|unionSchool|联合办学学校|query|false|string||
|updateBy|更新人|query|false|string||
|updateTime|更新日期|query|false|string(date-time)||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«IPage«zz_pro_of_sch对象»»|
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|IPage«zz_pro_of_sch对象»|IPage«zz_pro_of_sch对象»|
|&emsp;&emsp;current||integer(int64)||
|&emsp;&emsp;pages||integer(int64)||
|&emsp;&emsp;records||array|zz_pro_of_sch对象|
|&emsp;&emsp;&emsp;&emsp;createBy|创建人|string||
|&emsp;&emsp;&emsp;&emsp;createTime|创建日期|string||
|&emsp;&emsp;&emsp;&emsp;delFlag|删除标签|integer||
|&emsp;&emsp;&emsp;&emsp;direction|专业化方向|string||
|&emsp;&emsp;&emsp;&emsp;eduType|教学方式|string||
|&emsp;&emsp;&emsp;&emsp;eduUnion|办学方式|string||
|&emsp;&emsp;&emsp;&emsp;eduYear|学制|string||
|&emsp;&emsp;&emsp;&emsp;id|主键|string||
|&emsp;&emsp;&emsp;&emsp;levelType|招生类别|string||
|&emsp;&emsp;&emsp;&emsp;num|人数|integer||
|&emsp;&emsp;&emsp;&emsp;proCode|专业编号|string||
|&emsp;&emsp;&emsp;&emsp;proIdOfSch|学校专业代码|string||
|&emsp;&emsp;&emsp;&emsp;schoolCode|学校代码|string||
|&emsp;&emsp;&emsp;&emsp;season|招生时段|string||
|&emsp;&emsp;&emsp;&emsp;state|状态|string||
|&emsp;&emsp;&emsp;&emsp;unionSchool|联合办学学校|string||
|&emsp;&emsp;&emsp;&emsp;updateBy|更新人|string||
|&emsp;&emsp;&emsp;&emsp;updateTime|更新日期|string||
|&emsp;&emsp;size||integer(int64)||
|&emsp;&emsp;total||integer(int64)||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": {
		"current": 0,
		"pages": 0,
		"records": [
			{
				"createBy": "",
				"createTime": "",
				"delFlag": 0,
				"direction": "",
				"eduType": "",
				"eduUnion": "",
				"eduYear": "",
				"id": "",
				"levelType": "",
				"num": 0,
				"proCode": "",
				"proIdOfSch": "",
				"schoolCode": "",
				"season": "",
				"state": "",
				"unionSchool": "",
				"updateBy": "",
				"updateTime": ""
			}
		],
		"size": 0,
		"total": 0
	},
	"success": true,
	"timestamp": 0
}
```


## 中职学校专业表-通过id查询


**接口地址**:`/nnzk/zzmanagement/zzProOfSch/queryById`


**请求方式**:`GET`


**请求数据类型**:`application/x-www-form-urlencoded`


**响应数据类型**:`*/*`


**接口描述**:<p>中职学校专业表-通过id查询</p>



**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|id|id|query|true|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«zz_pro_of_sch对象»|
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|zz_pro_of_sch对象|zz_pro_of_sch对象|
|&emsp;&emsp;createBy|创建人|string||
|&emsp;&emsp;createTime|创建日期|string(date-time)||
|&emsp;&emsp;delFlag|删除标签|integer(int32)||
|&emsp;&emsp;direction|专业化方向|string||
|&emsp;&emsp;eduType|教学方式|string||
|&emsp;&emsp;eduUnion|办学方式|string||
|&emsp;&emsp;eduYear|学制|string||
|&emsp;&emsp;id|主键|string||
|&emsp;&emsp;levelType|招生类别|string||
|&emsp;&emsp;num|人数|integer(int32)||
|&emsp;&emsp;proCode|专业编号|string||
|&emsp;&emsp;proIdOfSch|学校专业代码|string||
|&emsp;&emsp;schoolCode|学校代码|string||
|&emsp;&emsp;season|招生时段|string||
|&emsp;&emsp;state|状态|string||
|&emsp;&emsp;unionSchool|联合办学学校|string||
|&emsp;&emsp;updateBy|更新人|string||
|&emsp;&emsp;updateTime|更新日期|string(date-time)||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": {
		"createBy": "",
		"createTime": "",
		"delFlag": 0,
		"direction": "",
		"eduType": "",
		"eduUnion": "",
		"eduYear": "",
		"id": "",
		"levelType": "",
		"num": 0,
		"proCode": "",
		"proIdOfSch": "",
		"schoolCode": "",
		"season": "",
		"state": "",
		"unionSchool": "",
		"updateBy": "",
		"updateTime": ""
	},
	"success": true,
	"timestamp": 0
}
```


# 中职学校表


## 中职学校表-添加


**接口地址**:`/nnzk/zzmanagement/zzSchool/add`


**请求方式**:`POST`


**请求数据类型**:`application/json`


**响应数据类型**:`*/*`


**接口描述**:<p>中职学校表-添加</p>



**请求示例**:


```javascript
{
  "createBy": "",
  "createTime": "",
  "delFlag": 0,
  "dispOrder": 0,
  "id": "",
  "introduceName": "",
  "planNum": 0,
  "schoolCode": "",
  "schoolName": "",
  "signupStatus": 0,
  "updateBy": "",
  "updateTime": ""
}
```


**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|zzSchool|中职学校表|body|true|zz_school对象|zz_school对象|
|&emsp;&emsp;createBy|创建人||false|string||
|&emsp;&emsp;createTime|创建日期||false|string(date-time)||
|&emsp;&emsp;delFlag|删除标签||false|integer(int32)||
|&emsp;&emsp;dispOrder|填报显示顺序||false|integer(int32)||
|&emsp;&emsp;id|主键||false|string||
|&emsp;&emsp;introduceName|简介显示名称||false|string||
|&emsp;&emsp;planNum|计划数||false|integer(int32)||
|&emsp;&emsp;schoolCode|学校代码||false|string||
|&emsp;&emsp;schoolName|学校名称||false|string||
|&emsp;&emsp;signupStatus|报名状态||false|integer(int32)||
|&emsp;&emsp;updateBy|更新人||false|string||
|&emsp;&emsp;updateTime|更新日期||false|string(date-time)||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«string»|
|201|Created||
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|string||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": "",
	"success": true,
	"timestamp": 0
}
```


## 中职学校表-通过id删除


**接口地址**:`/nnzk/zzmanagement/zzSchool/delete`


**请求方式**:`DELETE`


**请求数据类型**:`application/x-www-form-urlencoded`


**响应数据类型**:`*/*`


**接口描述**:<p>中职学校表-通过id删除</p>



**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|id|id|query|true|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«string»|
|204|No Content||
|401|Unauthorized||
|403|Forbidden||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|string||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": "",
	"success": true,
	"timestamp": 0
}
```


## 中职学校表-批量删除


**接口地址**:`/nnzk/zzmanagement/zzSchool/deleteBatch`


**请求方式**:`DELETE`


**请求数据类型**:`application/x-www-form-urlencoded`


**响应数据类型**:`*/*`


**接口描述**:<p>中职学校表-批量删除</p>



**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|ids|ids|query|true|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«string»|
|204|No Content||
|401|Unauthorized||
|403|Forbidden||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|string||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": "",
	"success": true,
	"timestamp": 0
}
```


## 中职学校表-编辑


**接口地址**:`/nnzk/zzmanagement/zzSchool/edit`


**请求方式**:`POST`


**请求数据类型**:`application/json`


**响应数据类型**:`*/*`


**接口描述**:<p>中职学校表-编辑</p>



**请求示例**:


```javascript
{
  "createBy": "",
  "createTime": "",
  "delFlag": 0,
  "dispOrder": 0,
  "id": "",
  "introduceName": "",
  "planNum": 0,
  "schoolCode": "",
  "schoolName": "",
  "signupStatus": 0,
  "updateBy": "",
  "updateTime": ""
}
```


**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|zzSchool|中职学校表|body|true|zz_school对象|zz_school对象|
|&emsp;&emsp;createBy|创建人||false|string||
|&emsp;&emsp;createTime|创建日期||false|string(date-time)||
|&emsp;&emsp;delFlag|删除标签||false|integer(int32)||
|&emsp;&emsp;dispOrder|填报显示顺序||false|integer(int32)||
|&emsp;&emsp;id|主键||false|string||
|&emsp;&emsp;introduceName|简介显示名称||false|string||
|&emsp;&emsp;planNum|计划数||false|integer(int32)||
|&emsp;&emsp;schoolCode|学校代码||false|string||
|&emsp;&emsp;schoolName|学校名称||false|string||
|&emsp;&emsp;signupStatus|报名状态||false|integer(int32)||
|&emsp;&emsp;updateBy|更新人||false|string||
|&emsp;&emsp;updateTime|更新日期||false|string(date-time)||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«string»|
|201|Created||
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|string||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": "",
	"success": true,
	"timestamp": 0
}
```


## 中职学校表-编辑


**接口地址**:`/nnzk/zzmanagement/zzSchool/edit`


**请求方式**:`PUT`


**请求数据类型**:`application/json`


**响应数据类型**:`*/*`


**接口描述**:<p>中职学校表-编辑</p>



**请求示例**:


```javascript
{
  "createBy": "",
  "createTime": "",
  "delFlag": 0,
  "dispOrder": 0,
  "id": "",
  "introduceName": "",
  "planNum": 0,
  "schoolCode": "",
  "schoolName": "",
  "signupStatus": 0,
  "updateBy": "",
  "updateTime": ""
}
```


**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|zzSchool|中职学校表|body|true|zz_school对象|zz_school对象|
|&emsp;&emsp;createBy|创建人||false|string||
|&emsp;&emsp;createTime|创建日期||false|string(date-time)||
|&emsp;&emsp;delFlag|删除标签||false|integer(int32)||
|&emsp;&emsp;dispOrder|填报显示顺序||false|integer(int32)||
|&emsp;&emsp;id|主键||false|string||
|&emsp;&emsp;introduceName|简介显示名称||false|string||
|&emsp;&emsp;planNum|计划数||false|integer(int32)||
|&emsp;&emsp;schoolCode|学校代码||false|string||
|&emsp;&emsp;schoolName|学校名称||false|string||
|&emsp;&emsp;signupStatus|报名状态||false|integer(int32)||
|&emsp;&emsp;updateBy|更新人||false|string||
|&emsp;&emsp;updateTime|更新日期||false|string(date-time)||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«string»|
|201|Created||
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|string||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": "",
	"success": true,
	"timestamp": 0
}
```


## 中职学校表-分页列表查询


**接口地址**:`/nnzk/zzmanagement/zzSchool/list`


**请求方式**:`GET`


**请求数据类型**:`application/x-www-form-urlencoded`


**响应数据类型**:`*/*`


**接口描述**:<p>中职学校表-分页列表查询</p>



**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|dispOrder|填报显示顺序|query|true|integer(int32)||
|introduceName|简介显示名称|query|true|string||
|planNum|计划数|query|true|integer(int32)||
|schoolCode|学校代码|query|true|string||
|schoolName|学校名称|query|true|string||
|signupStatus|报名状态|query|true|integer(int32)||
|createBy|创建人|query|false|string||
|createTime|创建日期|query|false|string(date-time)||
|delFlag|删除标签|query|false|integer(int32)||
|id|主键|query|false|string||
|pageNo|pageNo|query|false|integer(int32)||
|pageSize|pageSize|query|false|integer(int32)||
|updateBy|更新人|query|false|string||
|updateTime|更新日期|query|false|string(date-time)||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«IPage«zz_school对象»»|
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|IPage«zz_school对象»|IPage«zz_school对象»|
|&emsp;&emsp;current||integer(int64)||
|&emsp;&emsp;pages||integer(int64)||
|&emsp;&emsp;records||array|zz_school对象|
|&emsp;&emsp;&emsp;&emsp;createBy|创建人|string||
|&emsp;&emsp;&emsp;&emsp;createTime|创建日期|string||
|&emsp;&emsp;&emsp;&emsp;delFlag|删除标签|integer||
|&emsp;&emsp;&emsp;&emsp;dispOrder|填报显示顺序|integer||
|&emsp;&emsp;&emsp;&emsp;id|主键|string||
|&emsp;&emsp;&emsp;&emsp;introduceName|简介显示名称|string||
|&emsp;&emsp;&emsp;&emsp;planNum|计划数|integer||
|&emsp;&emsp;&emsp;&emsp;schoolCode|学校代码|string||
|&emsp;&emsp;&emsp;&emsp;schoolName|学校名称|string||
|&emsp;&emsp;&emsp;&emsp;signupStatus|报名状态|integer||
|&emsp;&emsp;&emsp;&emsp;updateBy|更新人|string||
|&emsp;&emsp;&emsp;&emsp;updateTime|更新日期|string||
|&emsp;&emsp;size||integer(int64)||
|&emsp;&emsp;total||integer(int64)||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": {
		"current": 0,
		"pages": 0,
		"records": [
			{
				"createBy": "",
				"createTime": "",
				"delFlag": 0,
				"dispOrder": 0,
				"id": "",
				"introduceName": "",
				"planNum": 0,
				"schoolCode": "",
				"schoolName": "",
				"signupStatus": 0,
				"updateBy": "",
				"updateTime": ""
			}
		],
		"size": 0,
		"total": 0
	},
	"success": true,
	"timestamp": 0
}
```


## 中职学校表-通过id查询


**接口地址**:`/nnzk/zzmanagement/zzSchool/queryById`


**请求方式**:`GET`


**请求数据类型**:`application/x-www-form-urlencoded`


**响应数据类型**:`*/*`


**接口描述**:<p>中职学校表-通过id查询</p>



**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|id|id|query|true|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«zz_school对象»|
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|zz_school对象|zz_school对象|
|&emsp;&emsp;createBy|创建人|string||
|&emsp;&emsp;createTime|创建日期|string(date-time)||
|&emsp;&emsp;delFlag|删除标签|integer(int32)||
|&emsp;&emsp;dispOrder|填报显示顺序|integer(int32)||
|&emsp;&emsp;id|主键|string||
|&emsp;&emsp;introduceName|简介显示名称|string||
|&emsp;&emsp;planNum|计划数|integer(int32)||
|&emsp;&emsp;schoolCode|学校代码|string||
|&emsp;&emsp;schoolName|学校名称|string||
|&emsp;&emsp;signupStatus|报名状态|integer(int32)||
|&emsp;&emsp;updateBy|更新人|string||
|&emsp;&emsp;updateTime|更新日期|string(date-time)||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": {
		"createBy": "",
		"createTime": "",
		"delFlag": 0,
		"dispOrder": 0,
		"id": "",
		"introduceName": "",
		"planNum": 0,
		"schoolCode": "",
		"schoolName": "",
		"signupStatus": 0,
		"updateBy": "",
		"updateTime": ""
	},
	"success": true,
	"timestamp": 0
}
```


## 中职各校招生进度


**接口地址**:`/nnzk/zzmanagement/zzSchool/zzProgress`


**请求方式**:`GET`


**请求数据类型**:`application/x-www-form-urlencoded`


**响应数据类型**:`*/*`


**接口描述**:<p>中职各校招生进度</p>



**请求参数**:


暂无


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«ZzProgressListDTO»|
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|ZzProgressListDTO|ZzProgressListDTO|
|&emsp;&emsp;runTime|当前数据采集时间|DateTime|DateTime|
|&emsp;&emsp;&emsp;&emsp;am||boolean||
|&emsp;&emsp;&emsp;&emsp;date||integer||
|&emsp;&emsp;&emsp;&emsp;day||integer||
|&emsp;&emsp;&emsp;&emsp;firstDayOfWeek|可用值:FRIDAY,MONDAY,SATURDAY,SUNDAY,THURSDAY,TUESDAY,WEDNESDAY|string||
|&emsp;&emsp;&emsp;&emsp;hours||integer||
|&emsp;&emsp;&emsp;&emsp;leapYear||boolean||
|&emsp;&emsp;&emsp;&emsp;minutes||integer||
|&emsp;&emsp;&emsp;&emsp;month||integer||
|&emsp;&emsp;&emsp;&emsp;mutable||boolean||
|&emsp;&emsp;&emsp;&emsp;pm||boolean||
|&emsp;&emsp;&emsp;&emsp;seconds||integer||
|&emsp;&emsp;&emsp;&emsp;time||integer||
|&emsp;&emsp;&emsp;&emsp;timeZone||TimeZone|TimeZone|
|&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;displayName||string||
|&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;dstsavings||integer||
|&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;id||string||
|&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;rawOffset||integer||
|&emsp;&emsp;&emsp;&emsp;timezoneOffset||integer||
|&emsp;&emsp;&emsp;&emsp;weekend||boolean||
|&emsp;&emsp;&emsp;&emsp;year||integer||
|&emsp;&emsp;&emsp;&emsp;zoneId||ZoneId|ZoneId|
|&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;id||string||
|&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;rules||ZoneRules|ZoneRules|
|&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;fixedOffset||boolean||
|&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;transitionRules||array|ZoneOffsetTransitionRule|
|&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;dayOfMonthIndicator||integer||
|&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;dayOfWeek|可用值:FRIDAY,MONDAY,SATURDAY,SUNDAY,THURSDAY,TUESDAY,WEDNESDAY|string||
|&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;localTime||LocalTime|LocalTime|
|&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;hour||integer||
|&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;minute||integer||
|&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;nano||integer||
|&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;second||integer||
|&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;midnightEndOfDay||boolean||
|&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;month|可用值:APRIL,AUGUST,DECEMBER,FEBRUARY,JANUARY,JULY,JUNE,MARCH,MAY,NOVEMBER,OCTOBER,SEPTEMBER|string||
|&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;offsetAfter||ZoneOffset|ZoneOffset|
|&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;id||string||
|&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;rules||ZoneRules|ZoneRules|
|&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;totalSeconds||integer||
|&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;offsetBefore||ZoneOffset|ZoneOffset|
|&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;id||string||
|&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;rules||ZoneRules|ZoneRules|
|&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;totalSeconds||integer||
|&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;standardOffset||ZoneOffset|ZoneOffset|
|&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;id||string||
|&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;rules||ZoneRules|ZoneRules|
|&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;totalSeconds||integer||
|&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;timeDefinition|可用值:STANDARD,UTC,WALL|string||
|&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;transitions||array|ZoneOffsetTransition|
|&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;dateTimeAfter||string||
|&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;dateTimeBefore||string||
|&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;duration||Duration|Duration|
|&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;nano||integer||
|&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;negative||boolean||
|&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;seconds||integer||
|&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;units||array|TemporalUnit|
|&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;dateBased||boolean||
|&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;duration||Duration|Duration|
|&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;durationEstimated||boolean||
|&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;timeBased||boolean||
|&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;zero||boolean||
|&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;gap||boolean||
|&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;instant||string||
|&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;offsetAfter||ZoneOffset|ZoneOffset|
|&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;id||string||
|&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;rules||ZoneRules|ZoneRules|
|&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;totalSeconds||integer||
|&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;offsetBefore||ZoneOffset|ZoneOffset|
|&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;id||string||
|&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;rules||ZoneRules|ZoneRules|
|&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;totalSeconds||integer||
|&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;overlap||boolean||
|&emsp;&emsp;zzProgressList|中职各校招生进度列表|array|ZzProgressDTO|
|&emsp;&emsp;&emsp;&emsp;countNum|报名人数|integer||
|&emsp;&emsp;&emsp;&emsp;schoolCode|学校代码|string||
|&emsp;&emsp;&emsp;&emsp;schoolName|学校名称|string||
|&emsp;&emsp;&emsp;&emsp;signupStatus|当前报名状态|integer||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": {
		"runTime": {
			"am": true,
			"date": 0,
			"day": 0,
			"firstDayOfWeek": "",
			"hours": 0,
			"leapYear": true,
			"minutes": 0,
			"month": 0,
			"mutable": true,
			"pm": true,
			"seconds": 0,
			"time": 0,
			"timeZone": {
				"displayName": "",
				"dstsavings": 0,
				"id": "",
				"rawOffset": 0
			},
			"timezoneOffset": 0,
			"weekend": true,
			"year": 0,
			"zoneId": {
				"id": "",
				"rules": {
					"fixedOffset": true,
					"transitionRules": [
						{
							"dayOfMonthIndicator": 0,
							"dayOfWeek": "",
							"localTime": {
								"hour": 0,
								"minute": 0,
								"nano": 0,
								"second": 0
							},
							"midnightEndOfDay": true,
							"month": "",
							"offsetAfter": {
								"id": "",
								"rules": {},
								"totalSeconds": 0
							},
							"offsetBefore": {
								"id": "",
								"rules": {},
								"totalSeconds": 0
							},
							"standardOffset": {
								"id": "",
								"rules": {},
								"totalSeconds": 0
							},
							"timeDefinition": ""
						}
					],
					"transitions": [
						{
							"dateTimeAfter": "",
							"dateTimeBefore": "",
							"duration": {
								"nano": 0,
								"negative": true,
								"seconds": 0,
								"units": [
									{
										"dateBased": true,
										"duration": {},
										"durationEstimated": true,
										"timeBased": true
									}
								],
								"zero": true
							},
							"gap": true,
							"instant": "",
							"offsetAfter": {
								"id": "",
								"rules": {},
								"totalSeconds": 0
							},
							"offsetBefore": {
								"id": "",
								"rules": {},
								"totalSeconds": 0
							},
							"overlap": true
						}
					]
				}
			}
		},
		"zzProgressList": [
			{
				"countNum": 0,
				"schoolCode": "",
				"schoolName": "",
				"signupStatus": 0
			}
		]
	},
	"success": true,
	"timestamp": 0
}
```


## 中职报名公示信息


**接口地址**:`/nnzk/zzmanagement/zzSchool/zzPublicity`


**请求方式**:`GET`


**请求数据类型**:`application/x-www-form-urlencoded`


**响应数据类型**:`*/*`


**接口描述**:<p>中职报名公示信息</p>



**请求参数**:


暂无


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«ZzPublicityListDTO»|
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|ZzPublicityListDTO|ZzPublicityListDTO|
|&emsp;&emsp;runTime|当前数据采集时间|DateTime|DateTime|
|&emsp;&emsp;&emsp;&emsp;am||boolean||
|&emsp;&emsp;&emsp;&emsp;date||integer||
|&emsp;&emsp;&emsp;&emsp;day||integer||
|&emsp;&emsp;&emsp;&emsp;firstDayOfWeek|可用值:FRIDAY,MONDAY,SATURDAY,SUNDAY,THURSDAY,TUESDAY,WEDNESDAY|string||
|&emsp;&emsp;&emsp;&emsp;hours||integer||
|&emsp;&emsp;&emsp;&emsp;leapYear||boolean||
|&emsp;&emsp;&emsp;&emsp;minutes||integer||
|&emsp;&emsp;&emsp;&emsp;month||integer||
|&emsp;&emsp;&emsp;&emsp;mutable||boolean||
|&emsp;&emsp;&emsp;&emsp;pm||boolean||
|&emsp;&emsp;&emsp;&emsp;seconds||integer||
|&emsp;&emsp;&emsp;&emsp;time||integer||
|&emsp;&emsp;&emsp;&emsp;timeZone||TimeZone|TimeZone|
|&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;displayName||string||
|&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;dstsavings||integer||
|&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;id||string||
|&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;rawOffset||integer||
|&emsp;&emsp;&emsp;&emsp;timezoneOffset||integer||
|&emsp;&emsp;&emsp;&emsp;weekend||boolean||
|&emsp;&emsp;&emsp;&emsp;year||integer||
|&emsp;&emsp;&emsp;&emsp;zoneId||ZoneId|ZoneId|
|&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;id||string||
|&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;rules||ZoneRules|ZoneRules|
|&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;fixedOffset||boolean||
|&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;transitionRules||array|ZoneOffsetTransitionRule|
|&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;dayOfMonthIndicator||integer||
|&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;dayOfWeek|可用值:FRIDAY,MONDAY,SATURDAY,SUNDAY,THURSDAY,TUESDAY,WEDNESDAY|string||
|&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;localTime||LocalTime|LocalTime|
|&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;hour||integer||
|&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;minute||integer||
|&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;nano||integer||
|&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;second||integer||
|&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;midnightEndOfDay||boolean||
|&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;month|可用值:APRIL,AUGUST,DECEMBER,FEBRUARY,JANUARY,JULY,JUNE,MARCH,MAY,NOVEMBER,OCTOBER,SEPTEMBER|string||
|&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;offsetAfter||ZoneOffset|ZoneOffset|
|&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;id||string||
|&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;rules||ZoneRules|ZoneRules|
|&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;totalSeconds||integer||
|&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;offsetBefore||ZoneOffset|ZoneOffset|
|&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;id||string||
|&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;rules||ZoneRules|ZoneRules|
|&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;totalSeconds||integer||
|&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;standardOffset||ZoneOffset|ZoneOffset|
|&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;id||string||
|&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;rules||ZoneRules|ZoneRules|
|&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;totalSeconds||integer||
|&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;timeDefinition|可用值:STANDARD,UTC,WALL|string||
|&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;transitions||array|ZoneOffsetTransition|
|&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;dateTimeAfter||string||
|&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;dateTimeBefore||string||
|&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;duration||Duration|Duration|
|&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;nano||integer||
|&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;negative||boolean||
|&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;seconds||integer||
|&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;units||array|TemporalUnit|
|&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;dateBased||boolean||
|&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;duration||Duration|Duration|
|&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;durationEstimated||boolean||
|&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;timeBased||boolean||
|&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;zero||boolean||
|&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;gap||boolean||
|&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;instant||string||
|&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;offsetAfter||ZoneOffset|ZoneOffset|
|&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;id||string||
|&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;rules||ZoneRules|ZoneRules|
|&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;totalSeconds||integer||
|&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;offsetBefore||ZoneOffset|ZoneOffset|
|&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;id||string||
|&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;rules||ZoneRules|ZoneRules|
|&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;totalSeconds||integer||
|&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;overlap||boolean||
|&emsp;&emsp;zzPublicityDTOList||array|ZzPublicityDTO|
|&emsp;&emsp;&emsp;&emsp;countNum|报名人数|integer||
|&emsp;&emsp;&emsp;&emsp;highScore|报名最高成绩|string||
|&emsp;&emsp;&emsp;&emsp;lowScore|报名最低成绩|string||
|&emsp;&emsp;&emsp;&emsp;schoolCode|学校代码|string||
|&emsp;&emsp;&emsp;&emsp;schoolName|学校名称|string||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": {
		"runTime": {
			"am": true,
			"date": 0,
			"day": 0,
			"firstDayOfWeek": "",
			"hours": 0,
			"leapYear": true,
			"minutes": 0,
			"month": 0,
			"mutable": true,
			"pm": true,
			"seconds": 0,
			"time": 0,
			"timeZone": {
				"displayName": "",
				"dstsavings": 0,
				"id": "",
				"rawOffset": 0
			},
			"timezoneOffset": 0,
			"weekend": true,
			"year": 0,
			"zoneId": {
				"id": "",
				"rules": {
					"fixedOffset": true,
					"transitionRules": [
						{
							"dayOfMonthIndicator": 0,
							"dayOfWeek": "",
							"localTime": {
								"hour": 0,
								"minute": 0,
								"nano": 0,
								"second": 0
							},
							"midnightEndOfDay": true,
							"month": "",
							"offsetAfter": {
								"id": "",
								"rules": {},
								"totalSeconds": 0
							},
							"offsetBefore": {
								"id": "",
								"rules": {},
								"totalSeconds": 0
							},
							"standardOffset": {
								"id": "",
								"rules": {},
								"totalSeconds": 0
							},
							"timeDefinition": ""
						}
					],
					"transitions": [
						{
							"dateTimeAfter": "",
							"dateTimeBefore": "",
							"duration": {
								"nano": 0,
								"negative": true,
								"seconds": 0,
								"units": [
									{
										"dateBased": true,
										"duration": {},
										"durationEstimated": true,
										"timeBased": true
									}
								],
								"zero": true
							},
							"gap": true,
							"instant": "",
							"offsetAfter": {
								"id": "",
								"rules": {},
								"totalSeconds": 0
							},
							"offsetBefore": {
								"id": "",
								"rules": {},
								"totalSeconds": 0
							},
							"overlap": true
						}
					]
				}
			}
		},
		"zzPublicityDTOList": [
			{
				"countNum": 0,
				"highScore": "",
				"lowScore": "",
				"schoolCode": "",
				"schoolName": ""
			}
		]
	},
	"success": true,
	"timestamp": 0
}
```


## 中职报名公示信息详情


**接口地址**:`/nnzk/zzmanagement/zzSchool/zzPublicityDetail`


**请求方式**:`GET`


**请求数据类型**:`application/x-www-form-urlencoded`


**响应数据类型**:`*/*`


**接口描述**:<p>中职报名公示信息详情</p>



**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|schoolCode|schoolCode|query|true|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«ZzPublicityDetailListDTO»|
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|ZzPublicityDetailListDTO|ZzPublicityDetailListDTO|
|&emsp;&emsp;runTime|当前数据采集时间|DateTime|DateTime|
|&emsp;&emsp;&emsp;&emsp;am||boolean||
|&emsp;&emsp;&emsp;&emsp;date||integer||
|&emsp;&emsp;&emsp;&emsp;day||integer||
|&emsp;&emsp;&emsp;&emsp;firstDayOfWeek|可用值:FRIDAY,MONDAY,SATURDAY,SUNDAY,THURSDAY,TUESDAY,WEDNESDAY|string||
|&emsp;&emsp;&emsp;&emsp;hours||integer||
|&emsp;&emsp;&emsp;&emsp;leapYear||boolean||
|&emsp;&emsp;&emsp;&emsp;minutes||integer||
|&emsp;&emsp;&emsp;&emsp;month||integer||
|&emsp;&emsp;&emsp;&emsp;mutable||boolean||
|&emsp;&emsp;&emsp;&emsp;pm||boolean||
|&emsp;&emsp;&emsp;&emsp;seconds||integer||
|&emsp;&emsp;&emsp;&emsp;time||integer||
|&emsp;&emsp;&emsp;&emsp;timeZone||TimeZone|TimeZone|
|&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;displayName||string||
|&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;dstsavings||integer||
|&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;id||string||
|&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;rawOffset||integer||
|&emsp;&emsp;&emsp;&emsp;timezoneOffset||integer||
|&emsp;&emsp;&emsp;&emsp;weekend||boolean||
|&emsp;&emsp;&emsp;&emsp;year||integer||
|&emsp;&emsp;&emsp;&emsp;zoneId||ZoneId|ZoneId|
|&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;id||string||
|&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;rules||ZoneRules|ZoneRules|
|&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;fixedOffset||boolean||
|&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;transitionRules||array|ZoneOffsetTransitionRule|
|&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;dayOfMonthIndicator||integer||
|&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;dayOfWeek|可用值:FRIDAY,MONDAY,SATURDAY,SUNDAY,THURSDAY,TUESDAY,WEDNESDAY|string||
|&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;localTime||LocalTime|LocalTime|
|&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;hour||integer||
|&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;minute||integer||
|&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;nano||integer||
|&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;second||integer||
|&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;midnightEndOfDay||boolean||
|&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;month|可用值:APRIL,AUGUST,DECEMBER,FEBRUARY,JANUARY,JULY,JUNE,MARCH,MAY,NOVEMBER,OCTOBER,SEPTEMBER|string||
|&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;offsetAfter||ZoneOffset|ZoneOffset|
|&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;id||string||
|&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;rules||ZoneRules|ZoneRules|
|&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;totalSeconds||integer||
|&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;offsetBefore||ZoneOffset|ZoneOffset|
|&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;id||string||
|&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;rules||ZoneRules|ZoneRules|
|&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;totalSeconds||integer||
|&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;standardOffset||ZoneOffset|ZoneOffset|
|&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;id||string||
|&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;rules||ZoneRules|ZoneRules|
|&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;totalSeconds||integer||
|&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;timeDefinition|可用值:STANDARD,UTC,WALL|string||
|&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;transitions||array|ZoneOffsetTransition|
|&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;dateTimeAfter||string||
|&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;dateTimeBefore||string||
|&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;duration||Duration|Duration|
|&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;nano||integer||
|&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;negative||boolean||
|&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;seconds||integer||
|&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;units||array|TemporalUnit|
|&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;dateBased||boolean||
|&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;duration||Duration|Duration|
|&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;durationEstimated||boolean||
|&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;timeBased||boolean||
|&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;zero||boolean||
|&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;gap||boolean||
|&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;instant||string||
|&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;offsetAfter||ZoneOffset|ZoneOffset|
|&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;id||string||
|&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;rules||ZoneRules|ZoneRules|
|&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;totalSeconds||integer||
|&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;offsetBefore||ZoneOffset|ZoneOffset|
|&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;id||string||
|&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;rules||ZoneRules|ZoneRules|
|&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;totalSeconds||integer||
|&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;overlap||boolean||
|&emsp;&emsp;zzPublicityDetailList|中职报名公示信息详情列表|array|ZzPublicityDetailDTO|
|&emsp;&emsp;&emsp;&emsp;chineseLevel|语文|string||
|&emsp;&emsp;&emsp;&emsp;chymistLevel|化学|string||
|&emsp;&emsp;&emsp;&emsp;combinedScore|组合分|string||
|&emsp;&emsp;&emsp;&emsp;diathesis|综合素质|string||
|&emsp;&emsp;&emsp;&emsp;englishLevel|英语|string||
|&emsp;&emsp;&emsp;&emsp;experiment|实验|string||
|&emsp;&emsp;&emsp;&emsp;mathLevel|数学|string||
|&emsp;&emsp;&emsp;&emsp;order|排名|integer||
|&emsp;&emsp;&emsp;&emsp;physicalEduLevel|体育|string||
|&emsp;&emsp;&emsp;&emsp;physicsLevel|物理|string||
|&emsp;&emsp;&emsp;&emsp;politicsLevel|政史|string||
|&emsp;&emsp;&emsp;&emsp;serial|序号|integer||
|&emsp;&emsp;&emsp;&emsp;sumScore|总分|string||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": {
		"runTime": {
			"am": true,
			"date": 0,
			"day": 0,
			"firstDayOfWeek": "",
			"hours": 0,
			"leapYear": true,
			"minutes": 0,
			"month": 0,
			"mutable": true,
			"pm": true,
			"seconds": 0,
			"time": 0,
			"timeZone": {
				"displayName": "",
				"dstsavings": 0,
				"id": "",
				"rawOffset": 0
			},
			"timezoneOffset": 0,
			"weekend": true,
			"year": 0,
			"zoneId": {
				"id": "",
				"rules": {
					"fixedOffset": true,
					"transitionRules": [
						{
							"dayOfMonthIndicator": 0,
							"dayOfWeek": "",
							"localTime": {
								"hour": 0,
								"minute": 0,
								"nano": 0,
								"second": 0
							},
							"midnightEndOfDay": true,
							"month": "",
							"offsetAfter": {
								"id": "",
								"rules": {},
								"totalSeconds": 0
							},
							"offsetBefore": {
								"id": "",
								"rules": {},
								"totalSeconds": 0
							},
							"standardOffset": {
								"id": "",
								"rules": {},
								"totalSeconds": 0
							},
							"timeDefinition": ""
						}
					],
					"transitions": [
						{
							"dateTimeAfter": "",
							"dateTimeBefore": "",
							"duration": {
								"nano": 0,
								"negative": true,
								"seconds": 0,
								"units": [
									{
										"dateBased": true,
										"duration": {},
										"durationEstimated": true,
										"timeBased": true
									}
								],
								"zero": true
							},
							"gap": true,
							"instant": "",
							"offsetAfter": {
								"id": "",
								"rules": {},
								"totalSeconds": 0
							},
							"offsetBefore": {
								"id": "",
								"rules": {},
								"totalSeconds": 0
							},
							"overlap": true
						}
					]
				}
			}
		},
		"zzPublicityDetailList": [
			{
				"chineseLevel": "",
				"chymistLevel": "",
				"combinedScore": "",
				"diathesis": "",
				"englishLevel": "",
				"experiment": "",
				"mathLevel": "",
				"order": 0,
				"physicalEduLevel": "",
				"physicsLevel": "",
				"politicsLevel": "",
				"serial": 0,
				"sumScore": ""
			}
		]
	},
	"success": true,
	"timestamp": 0
}
```


# 中职报名表


## 中职报名表-添加


**接口地址**:`/nnzk/zzmanagement/zzSignAndMatriculate/add`


**请求方式**:`POST`


**请求数据类型**:`application/json`


**响应数据类型**:`*/*`


**接口描述**:<p>中职报名表-添加</p>



**请求示例**:


```javascript
{
  "archiveCode": "",
  "createBy": "",
  "createTime": "",
  "delFlag": 0,
  "fillTime": "",
  "id": "",
  "matriculateStatus": 0,
  "matriculateTime": "",
  "proCode": "",
  "proIdOfSch": "",
  "schoolCode": "",
  "source": "",
  "updateBy": "",
  "updateTime": ""
}
```


**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|zzSignAndMatriculate|中职报名表|body|true|zz_sign_and_matriculate对象|zz_sign_and_matriculate对象|
|&emsp;&emsp;archiveCode|准考证号||false|string||
|&emsp;&emsp;createBy|创建人||false|string||
|&emsp;&emsp;createTime|创建日期||false|string(date-time)||
|&emsp;&emsp;delFlag|删除标识||false|integer(int32)||
|&emsp;&emsp;fillTime|填报时间||false|string(date-time)||
|&emsp;&emsp;id|主键||false|string||
|&emsp;&emsp;matriculateStatus|录取状态||false|integer(int32)||
|&emsp;&emsp;matriculateTime|录取时间||false|string(date-time)||
|&emsp;&emsp;proCode|专业代码||false|string||
|&emsp;&emsp;proIdOfSch|学校专业代码||false|string||
|&emsp;&emsp;schoolCode|中职学校||false|string||
|&emsp;&emsp;source|?||false|string||
|&emsp;&emsp;updateBy|更新人||false|string||
|&emsp;&emsp;updateTime|更新日期||false|string(date-time)||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«string»|
|201|Created||
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|string||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": "",
	"success": true,
	"timestamp": 0
}
```


## 中职报名表-通过id删除


**接口地址**:`/nnzk/zzmanagement/zzSignAndMatriculate/delete`


**请求方式**:`DELETE`


**请求数据类型**:`application/x-www-form-urlencoded`


**响应数据类型**:`*/*`


**接口描述**:<p>中职报名表-通过id删除</p>



**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|id|id|query|true|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«string»|
|204|No Content||
|401|Unauthorized||
|403|Forbidden||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|string||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": "",
	"success": true,
	"timestamp": 0
}
```


## 中职报名表-批量删除


**接口地址**:`/nnzk/zzmanagement/zzSignAndMatriculate/deleteBatch`


**请求方式**:`DELETE`


**请求数据类型**:`application/x-www-form-urlencoded`


**响应数据类型**:`*/*`


**接口描述**:<p>中职报名表-批量删除</p>



**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|ids|ids|query|true|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«string»|
|204|No Content||
|401|Unauthorized||
|403|Forbidden||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|string||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": "",
	"success": true,
	"timestamp": 0
}
```


## 中职报名表-编辑


**接口地址**:`/nnzk/zzmanagement/zzSignAndMatriculate/edit`


**请求方式**:`POST`


**请求数据类型**:`application/json`


**响应数据类型**:`*/*`


**接口描述**:<p>中职报名表-编辑</p>



**请求示例**:


```javascript
{
  "archiveCode": "",
  "createBy": "",
  "createTime": "",
  "delFlag": 0,
  "fillTime": "",
  "id": "",
  "matriculateStatus": 0,
  "matriculateTime": "",
  "proCode": "",
  "proIdOfSch": "",
  "schoolCode": "",
  "source": "",
  "updateBy": "",
  "updateTime": ""
}
```


**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|zzSignAndMatriculate|中职报名表|body|true|zz_sign_and_matriculate对象|zz_sign_and_matriculate对象|
|&emsp;&emsp;archiveCode|准考证号||false|string||
|&emsp;&emsp;createBy|创建人||false|string||
|&emsp;&emsp;createTime|创建日期||false|string(date-time)||
|&emsp;&emsp;delFlag|删除标识||false|integer(int32)||
|&emsp;&emsp;fillTime|填报时间||false|string(date-time)||
|&emsp;&emsp;id|主键||false|string||
|&emsp;&emsp;matriculateStatus|录取状态||false|integer(int32)||
|&emsp;&emsp;matriculateTime|录取时间||false|string(date-time)||
|&emsp;&emsp;proCode|专业代码||false|string||
|&emsp;&emsp;proIdOfSch|学校专业代码||false|string||
|&emsp;&emsp;schoolCode|中职学校||false|string||
|&emsp;&emsp;source|?||false|string||
|&emsp;&emsp;updateBy|更新人||false|string||
|&emsp;&emsp;updateTime|更新日期||false|string(date-time)||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«string»|
|201|Created||
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|string||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": "",
	"success": true,
	"timestamp": 0
}
```


## 中职报名表-编辑


**接口地址**:`/nnzk/zzmanagement/zzSignAndMatriculate/edit`


**请求方式**:`PUT`


**请求数据类型**:`application/json`


**响应数据类型**:`*/*`


**接口描述**:<p>中职报名表-编辑</p>



**请求示例**:


```javascript
{
  "archiveCode": "",
  "createBy": "",
  "createTime": "",
  "delFlag": 0,
  "fillTime": "",
  "id": "",
  "matriculateStatus": 0,
  "matriculateTime": "",
  "proCode": "",
  "proIdOfSch": "",
  "schoolCode": "",
  "source": "",
  "updateBy": "",
  "updateTime": ""
}
```


**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|zzSignAndMatriculate|中职报名表|body|true|zz_sign_and_matriculate对象|zz_sign_and_matriculate对象|
|&emsp;&emsp;archiveCode|准考证号||false|string||
|&emsp;&emsp;createBy|创建人||false|string||
|&emsp;&emsp;createTime|创建日期||false|string(date-time)||
|&emsp;&emsp;delFlag|删除标识||false|integer(int32)||
|&emsp;&emsp;fillTime|填报时间||false|string(date-time)||
|&emsp;&emsp;id|主键||false|string||
|&emsp;&emsp;matriculateStatus|录取状态||false|integer(int32)||
|&emsp;&emsp;matriculateTime|录取时间||false|string(date-time)||
|&emsp;&emsp;proCode|专业代码||false|string||
|&emsp;&emsp;proIdOfSch|学校专业代码||false|string||
|&emsp;&emsp;schoolCode|中职学校||false|string||
|&emsp;&emsp;source|?||false|string||
|&emsp;&emsp;updateBy|更新人||false|string||
|&emsp;&emsp;updateTime|更新日期||false|string(date-time)||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«string»|
|201|Created||
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|string||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": "",
	"success": true,
	"timestamp": 0
}
```


## 中职端-根据学校代码获取专业名称和代码


**接口地址**:`/nnzk/zzmanagement/zzSignAndMatriculate/getZzProNameAndProCode`


**请求方式**:`GET`


**请求数据类型**:`application/x-www-form-urlencoded`


**响应数据类型**:`*/*`


**接口描述**:<p>中职端-根据学校代码获取专业名称和代码</p>



**请求参数**:


暂无


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«List«ZzProCodeAndProNameDTO»»|
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|array|ZzProCodeAndProNameDTO|
|&emsp;&emsp;proCode|专业代码|string||
|&emsp;&emsp;proIdOfSch|学校专业代码|string||
|&emsp;&emsp;proName|专业名称|string||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": [
		{
			"proCode": "",
			"proIdOfSch": "",
			"proName": ""
		}
	],
	"success": true,
	"timestamp": 0
}
```


## 中职端-中职报名信息查询


**接口地址**:`/nnzk/zzmanagement/zzSignAndMatriculate/getZzSignInfo`


**请求方式**:`GET`


**请求数据类型**:`application/x-www-form-urlencoded`


**响应数据类型**:`*/*`


**接口描述**:<p>中职端-中职报名信息查询</p>



**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|archiveCode|准考证号|query|false|string||
|birth|出生年月|query|false|string(date-time)||
|chineseLevel|语文|query|false|string||
|chymistLevel|化学|query|false|string||
|combinedScore|组合分|query|false|string||
|diathesis|综合素质|query|false|string||
|eduType|教学方式|query|false|string||
|eduUnion|办学方式|query|false|string||
|eduYear|学制|query|false|string||
|englishLevel|英语|query|false|string||
|experiment|实验|query|false|string||
|finishSchoolName|毕业学校|query|false|string||
|homePlace|户口地址|query|false|string||
|id|id|query|false|string||
|identityCode|身份证号|query|false|string||
|levelType|招生类别|query|false|string||
|mathLevel|数学|query|false|string||
|matriculateStatus|录取状态|query|false|integer(int32)||
|nationCode|民族|query|false|string||
|orderCode|排序码|query|false|number||
|pageNo|pageNo|query|false|integer(int32)||
|pageSize|pageSize|query|false|integer(int32)||
|phoneCode|电话|query|false|string||
|physicalEduLevel|体育|query|false|string||
|physicsLevel|物理|query|false|string||
|politicsLevel|政史|query|false|string||
|proCode|专业代码|query|false|string||
|proIdOfSch|学校专业代码|query|false|string||
|proName|专业名称|query|false|string||
|schoolCode|中职学校|query|false|string||
|season|招生季节|query|false|string||
|sex|性别|query|false|string||
|studentName|姓名|query|false|string||
|sumScore|总分|query|false|string||
|unionSchool|联合办学学校|query|false|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«IPage«GetZzSignInfoDTO»»|
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|IPage«GetZzSignInfoDTO»|IPage«GetZzSignInfoDTO»|
|&emsp;&emsp;current||integer(int64)||
|&emsp;&emsp;pages||integer(int64)||
|&emsp;&emsp;records||array|GetZzSignInfoDTO|
|&emsp;&emsp;&emsp;&emsp;archiveCode|准考证号|string||
|&emsp;&emsp;&emsp;&emsp;birth|出生年月|string||
|&emsp;&emsp;&emsp;&emsp;chineseLevel|语文|string||
|&emsp;&emsp;&emsp;&emsp;chymistLevel|化学|string||
|&emsp;&emsp;&emsp;&emsp;combinedScore|组合分|string||
|&emsp;&emsp;&emsp;&emsp;diathesis|综合素质|string||
|&emsp;&emsp;&emsp;&emsp;eduType|教学方式|string||
|&emsp;&emsp;&emsp;&emsp;eduUnion|办学方式|string||
|&emsp;&emsp;&emsp;&emsp;eduYear|学制|string||
|&emsp;&emsp;&emsp;&emsp;englishLevel|英语|string||
|&emsp;&emsp;&emsp;&emsp;experiment|实验|string||
|&emsp;&emsp;&emsp;&emsp;finishSchoolName|毕业学校|string||
|&emsp;&emsp;&emsp;&emsp;homePlace|户口地址|string||
|&emsp;&emsp;&emsp;&emsp;id|id|string||
|&emsp;&emsp;&emsp;&emsp;identityCode|身份证号|string||
|&emsp;&emsp;&emsp;&emsp;levelType|招生类别|string||
|&emsp;&emsp;&emsp;&emsp;mathLevel|数学|string||
|&emsp;&emsp;&emsp;&emsp;matriculateStatus|录取状态|integer||
|&emsp;&emsp;&emsp;&emsp;nationCode|民族|string||
|&emsp;&emsp;&emsp;&emsp;orderCode|排序码|number||
|&emsp;&emsp;&emsp;&emsp;phoneCode|电话|string||
|&emsp;&emsp;&emsp;&emsp;physicalEduLevel|体育|string||
|&emsp;&emsp;&emsp;&emsp;physicsLevel|物理|string||
|&emsp;&emsp;&emsp;&emsp;politicsLevel|政史|string||
|&emsp;&emsp;&emsp;&emsp;proCode|专业代码|string||
|&emsp;&emsp;&emsp;&emsp;proIdOfSch|学校专业代码|string||
|&emsp;&emsp;&emsp;&emsp;proName|专业名称|string||
|&emsp;&emsp;&emsp;&emsp;schoolCode|中职学校|string||
|&emsp;&emsp;&emsp;&emsp;season|招生季节|string||
|&emsp;&emsp;&emsp;&emsp;sex|性别|string||
|&emsp;&emsp;&emsp;&emsp;studentName|姓名|string||
|&emsp;&emsp;&emsp;&emsp;sumScore|总分|string||
|&emsp;&emsp;&emsp;&emsp;unionSchool|联合办学学校|string||
|&emsp;&emsp;size||integer(int64)||
|&emsp;&emsp;total||integer(int64)||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": {
		"current": 0,
		"pages": 0,
		"records": [
			{
				"archiveCode": "",
				"birth": "",
				"chineseLevel": "",
				"chymistLevel": "",
				"combinedScore": "",
				"diathesis": "",
				"eduType": "",
				"eduUnion": "",
				"eduYear": "",
				"englishLevel": "",
				"experiment": "",
				"finishSchoolName": "",
				"homePlace": "",
				"id": "",
				"identityCode": "",
				"levelType": "",
				"mathLevel": "",
				"matriculateStatus": 0,
				"nationCode": "",
				"orderCode": 0,
				"phoneCode": "",
				"physicalEduLevel": "",
				"physicsLevel": "",
				"politicsLevel": "",
				"proCode": "",
				"proIdOfSch": "",
				"proName": "",
				"schoolCode": "",
				"season": "",
				"sex": "",
				"studentName": "",
				"sumScore": "",
				"unionSchool": ""
			}
		],
		"size": 0,
		"total": 0
	},
	"success": true,
	"timestamp": 0
}
```


## 中职报名表-分页列表查询


**接口地址**:`/nnzk/zzmanagement/zzSignAndMatriculate/list`


**请求方式**:`GET`


**请求数据类型**:`application/x-www-form-urlencoded`


**响应数据类型**:`*/*`


**接口描述**:<p>中职报名表-分页列表查询</p>



**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|archiveCode|准考证号|query|true|string||
|fillTime|填报时间|query|true|string(date-time)||
|createBy|创建人|query|false|string||
|createTime|创建日期|query|false|string(date-time)||
|delFlag|删除标识|query|false|integer(int32)||
|id|主键|query|false|string||
|matriculateStatus|录取状态|query|false|integer(int32)||
|matriculateTime|录取时间|query|false|string(date-time)||
|pageNo|pageNo|query|false|integer(int32)||
|pageSize|pageSize|query|false|integer(int32)||
|proCode|专业代码|query|false|string||
|proIdOfSch|学校专业代码|query|false|string||
|schoolCode|中职学校|query|false|string||
|source|?|query|false|string||
|updateBy|更新人|query|false|string||
|updateTime|更新日期|query|false|string(date-time)||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«IPage«zz_sign_and_matriculate对象»»|
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|IPage«zz_sign_and_matriculate对象»|IPage«zz_sign_and_matriculate对象»|
|&emsp;&emsp;current||integer(int64)||
|&emsp;&emsp;pages||integer(int64)||
|&emsp;&emsp;records||array|zz_sign_and_matriculate对象|
|&emsp;&emsp;&emsp;&emsp;archiveCode|准考证号|string||
|&emsp;&emsp;&emsp;&emsp;createBy|创建人|string||
|&emsp;&emsp;&emsp;&emsp;createTime|创建日期|string||
|&emsp;&emsp;&emsp;&emsp;delFlag|删除标识|integer||
|&emsp;&emsp;&emsp;&emsp;fillTime|填报时间|string||
|&emsp;&emsp;&emsp;&emsp;id|主键|string||
|&emsp;&emsp;&emsp;&emsp;matriculateStatus|录取状态|integer||
|&emsp;&emsp;&emsp;&emsp;matriculateTime|录取时间|string||
|&emsp;&emsp;&emsp;&emsp;proCode|专业代码|string||
|&emsp;&emsp;&emsp;&emsp;proIdOfSch|学校专业代码|string||
|&emsp;&emsp;&emsp;&emsp;schoolCode|中职学校|string||
|&emsp;&emsp;&emsp;&emsp;source|?|string||
|&emsp;&emsp;&emsp;&emsp;updateBy|更新人|string||
|&emsp;&emsp;&emsp;&emsp;updateTime|更新日期|string||
|&emsp;&emsp;size||integer(int64)||
|&emsp;&emsp;total||integer(int64)||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": {
		"current": 0,
		"pages": 0,
		"records": [
			{
				"archiveCode": "",
				"createBy": "",
				"createTime": "",
				"delFlag": 0,
				"fillTime": "",
				"id": "",
				"matriculateStatus": 0,
				"matriculateTime": "",
				"proCode": "",
				"proIdOfSch": "",
				"schoolCode": "",
				"source": "",
				"updateBy": "",
				"updateTime": ""
			}
		],
		"size": 0,
		"total": 0
	},
	"success": true,
	"timestamp": 0
}
```


## 中职报名表-通过id查询


**接口地址**:`/nnzk/zzmanagement/zzSignAndMatriculate/queryById`


**请求方式**:`GET`


**请求数据类型**:`application/x-www-form-urlencoded`


**响应数据类型**:`*/*`


**接口描述**:<p>中职报名表-通过id查询</p>



**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|id|id|query|true|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«zz_sign_and_matriculate对象»|
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|zz_sign_and_matriculate对象|zz_sign_and_matriculate对象|
|&emsp;&emsp;archiveCode|准考证号|string||
|&emsp;&emsp;createBy|创建人|string||
|&emsp;&emsp;createTime|创建日期|string(date-time)||
|&emsp;&emsp;delFlag|删除标识|integer(int32)||
|&emsp;&emsp;fillTime|填报时间|string(date-time)||
|&emsp;&emsp;id|主键|string||
|&emsp;&emsp;matriculateStatus|录取状态|integer(int32)||
|&emsp;&emsp;matriculateTime|录取时间|string(date-time)||
|&emsp;&emsp;proCode|专业代码|string||
|&emsp;&emsp;proIdOfSch|学校专业代码|string||
|&emsp;&emsp;schoolCode|中职学校|string||
|&emsp;&emsp;source|?|string||
|&emsp;&emsp;updateBy|更新人|string||
|&emsp;&emsp;updateTime|更新日期|string(date-time)||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": {
		"archiveCode": "",
		"createBy": "",
		"createTime": "",
		"delFlag": 0,
		"fillTime": "",
		"id": "",
		"matriculateStatus": 0,
		"matriculateTime": "",
		"proCode": "",
		"proIdOfSch": "",
		"schoolCode": "",
		"source": "",
		"updateBy": "",
		"updateTime": ""
	},
	"success": true,
	"timestamp": 0
}
```


# 临时报名结果表


## 临时报名结果表-添加


**接口地址**:`/nnzk/sign/tempResultOfSign/add`


**请求方式**:`POST`


**请求数据类型**:`application/json`


**响应数据类型**:`*/*`


**接口描述**:<p>临时报名结果表-添加</p>



**请求示例**:


```javascript
{
  "additionalReason": "",
  "archiveCode": "",
  "calculateType": "",
  "combinedScore": "",
  "directionalReason": "",
  "finishSchoolCode": "",
  "guideReason": "",
  "highSchoolCode": "",
  "id": "",
  "instructionalReason": "",
  "isAreaStudent": 0,
  "orderCode": "",
  "runtime": "",
  "signupType": "",
  "tempOrder": 0
}
```


**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|tempResultOfSign|临时报名结果表|body|true|temp_result_of_sign对象|temp_result_of_sign对象|
|&emsp;&emsp;additionalReason|补录未入围原因||false|string||
|&emsp;&emsp;archiveCode|准考证号||false|string||
|&emsp;&emsp;calculateType|入围类型||false|string||
|&emsp;&emsp;combinedScore|组合分||false|string||
|&emsp;&emsp;directionalReason|定向未入围原因||false|string||
|&emsp;&emsp;finishSchoolCode|毕业学校代码||false|string||
|&emsp;&emsp;guideReason|指导未入围原因||false|string||
|&emsp;&emsp;highSchoolCode|高中学校代码||false|string||
|&emsp;&emsp;id|主键||false|string||
|&emsp;&emsp;instructionalReason|指令未入围原因||false|string||
|&emsp;&emsp;isAreaStudent|是否地段生||false|integer(int32)||
|&emsp;&emsp;orderCode|成绩排序码||false|string||
|&emsp;&emsp;runtime|运算时间||false|string(date-time)||
|&emsp;&emsp;signupType|报考类型||false|string||
|&emsp;&emsp;tempOrder|排名||false|integer(int32)||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«string»|
|201|Created||
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|string||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": "",
	"success": true,
	"timestamp": 0
}
```


## 临时报名结果表-通过id删除


**接口地址**:`/nnzk/sign/tempResultOfSign/delete`


**请求方式**:`DELETE`


**请求数据类型**:`application/x-www-form-urlencoded`


**响应数据类型**:`*/*`


**接口描述**:<p>临时报名结果表-通过id删除</p>



**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|id|id|query|true|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«string»|
|204|No Content||
|401|Unauthorized||
|403|Forbidden||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|string||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": "",
	"success": true,
	"timestamp": 0
}
```


## 临时报名结果表-批量删除


**接口地址**:`/nnzk/sign/tempResultOfSign/deleteBatch`


**请求方式**:`DELETE`


**请求数据类型**:`application/x-www-form-urlencoded`


**响应数据类型**:`*/*`


**接口描述**:<p>临时报名结果表-批量删除</p>



**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|ids|ids|query|true|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«string»|
|204|No Content||
|401|Unauthorized||
|403|Forbidden||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|string||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": "",
	"success": true,
	"timestamp": 0
}
```


## 临时报名结果表-编辑


**接口地址**:`/nnzk/sign/tempResultOfSign/edit`


**请求方式**:`POST`


**请求数据类型**:`application/json`


**响应数据类型**:`*/*`


**接口描述**:<p>临时报名结果表-编辑</p>



**请求示例**:


```javascript
{
  "additionalReason": "",
  "archiveCode": "",
  "calculateType": "",
  "combinedScore": "",
  "directionalReason": "",
  "finishSchoolCode": "",
  "guideReason": "",
  "highSchoolCode": "",
  "id": "",
  "instructionalReason": "",
  "isAreaStudent": 0,
  "orderCode": "",
  "runtime": "",
  "signupType": "",
  "tempOrder": 0
}
```


**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|tempResultOfSign|临时报名结果表|body|true|temp_result_of_sign对象|temp_result_of_sign对象|
|&emsp;&emsp;additionalReason|补录未入围原因||false|string||
|&emsp;&emsp;archiveCode|准考证号||false|string||
|&emsp;&emsp;calculateType|入围类型||false|string||
|&emsp;&emsp;combinedScore|组合分||false|string||
|&emsp;&emsp;directionalReason|定向未入围原因||false|string||
|&emsp;&emsp;finishSchoolCode|毕业学校代码||false|string||
|&emsp;&emsp;guideReason|指导未入围原因||false|string||
|&emsp;&emsp;highSchoolCode|高中学校代码||false|string||
|&emsp;&emsp;id|主键||false|string||
|&emsp;&emsp;instructionalReason|指令未入围原因||false|string||
|&emsp;&emsp;isAreaStudent|是否地段生||false|integer(int32)||
|&emsp;&emsp;orderCode|成绩排序码||false|string||
|&emsp;&emsp;runtime|运算时间||false|string(date-time)||
|&emsp;&emsp;signupType|报考类型||false|string||
|&emsp;&emsp;tempOrder|排名||false|integer(int32)||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«string»|
|201|Created||
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|string||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": "",
	"success": true,
	"timestamp": 0
}
```


## 临时报名结果表-编辑


**接口地址**:`/nnzk/sign/tempResultOfSign/edit`


**请求方式**:`PUT`


**请求数据类型**:`application/json`


**响应数据类型**:`*/*`


**接口描述**:<p>临时报名结果表-编辑</p>



**请求示例**:


```javascript
{
  "additionalReason": "",
  "archiveCode": "",
  "calculateType": "",
  "combinedScore": "",
  "directionalReason": "",
  "finishSchoolCode": "",
  "guideReason": "",
  "highSchoolCode": "",
  "id": "",
  "instructionalReason": "",
  "isAreaStudent": 0,
  "orderCode": "",
  "runtime": "",
  "signupType": "",
  "tempOrder": 0
}
```


**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|tempResultOfSign|临时报名结果表|body|true|temp_result_of_sign对象|temp_result_of_sign对象|
|&emsp;&emsp;additionalReason|补录未入围原因||false|string||
|&emsp;&emsp;archiveCode|准考证号||false|string||
|&emsp;&emsp;calculateType|入围类型||false|string||
|&emsp;&emsp;combinedScore|组合分||false|string||
|&emsp;&emsp;directionalReason|定向未入围原因||false|string||
|&emsp;&emsp;finishSchoolCode|毕业学校代码||false|string||
|&emsp;&emsp;guideReason|指导未入围原因||false|string||
|&emsp;&emsp;highSchoolCode|高中学校代码||false|string||
|&emsp;&emsp;id|主键||false|string||
|&emsp;&emsp;instructionalReason|指令未入围原因||false|string||
|&emsp;&emsp;isAreaStudent|是否地段生||false|integer(int32)||
|&emsp;&emsp;orderCode|成绩排序码||false|string||
|&emsp;&emsp;runtime|运算时间||false|string(date-time)||
|&emsp;&emsp;signupType|报考类型||false|string||
|&emsp;&emsp;tempOrder|排名||false|integer(int32)||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«string»|
|201|Created||
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|string||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": "",
	"success": true,
	"timestamp": 0
}
```


## 临时报名结果表-分页列表查询


**接口地址**:`/nnzk/sign/tempResultOfSign/list`


**请求方式**:`GET`


**请求数据类型**:`application/x-www-form-urlencoded`


**响应数据类型**:`*/*`


**接口描述**:<p>临时报名结果表-分页列表查询</p>



**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|additionalReason|补录未入围原因|query|false|string||
|archiveCode|准考证号|query|false|string||
|calculateType|入围类型|query|false|string||
|combinedScore|组合分|query|false|string||
|directionalReason|定向未入围原因|query|false|string||
|finishSchoolCode|毕业学校代码|query|false|string||
|guideReason|指导未入围原因|query|false|string||
|highSchoolCode|高中学校代码|query|false|string||
|id|主键|query|false|string||
|instructionalReason|指令未入围原因|query|false|string||
|isAreaStudent|是否地段生|query|false|integer(int32)||
|orderCode|成绩排序码|query|false|string||
|pageNo|pageNo|query|false|integer(int32)||
|pageSize|pageSize|query|false|integer(int32)||
|runtime|运算时间|query|false|string(date-time)||
|signupType|报考类型|query|false|string||
|tempOrder|排名|query|false|integer(int32)||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«IPage«temp_result_of_sign对象»»|
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|IPage«temp_result_of_sign对象»|IPage«temp_result_of_sign对象»|
|&emsp;&emsp;current||integer(int64)||
|&emsp;&emsp;pages||integer(int64)||
|&emsp;&emsp;records||array|temp_result_of_sign对象|
|&emsp;&emsp;&emsp;&emsp;additionalReason|补录未入围原因|string||
|&emsp;&emsp;&emsp;&emsp;archiveCode|准考证号|string||
|&emsp;&emsp;&emsp;&emsp;calculateType|入围类型|string||
|&emsp;&emsp;&emsp;&emsp;combinedScore|组合分|string||
|&emsp;&emsp;&emsp;&emsp;directionalReason|定向未入围原因|string||
|&emsp;&emsp;&emsp;&emsp;finishSchoolCode|毕业学校代码|string||
|&emsp;&emsp;&emsp;&emsp;guideReason|指导未入围原因|string||
|&emsp;&emsp;&emsp;&emsp;highSchoolCode|高中学校代码|string||
|&emsp;&emsp;&emsp;&emsp;id|主键|string||
|&emsp;&emsp;&emsp;&emsp;instructionalReason|指令未入围原因|string||
|&emsp;&emsp;&emsp;&emsp;isAreaStudent|是否地段生|integer||
|&emsp;&emsp;&emsp;&emsp;orderCode|成绩排序码|string||
|&emsp;&emsp;&emsp;&emsp;runtime|运算时间|string||
|&emsp;&emsp;&emsp;&emsp;signupType|报考类型|string||
|&emsp;&emsp;&emsp;&emsp;tempOrder|排名|integer||
|&emsp;&emsp;size||integer(int64)||
|&emsp;&emsp;total||integer(int64)||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": {
		"current": 0,
		"pages": 0,
		"records": [
			{
				"additionalReason": "",
				"archiveCode": "",
				"calculateType": "",
				"combinedScore": "",
				"directionalReason": "",
				"finishSchoolCode": "",
				"guideReason": "",
				"highSchoolCode": "",
				"id": "",
				"instructionalReason": "",
				"isAreaStudent": 0,
				"orderCode": "",
				"runtime": "",
				"signupType": "",
				"tempOrder": 0
			}
		],
		"size": 0,
		"total": 0
	},
	"success": true,
	"timestamp": 0
}
```


## 临时报名结果表-通过id查询


**接口地址**:`/nnzk/sign/tempResultOfSign/queryById`


**请求方式**:`GET`


**请求数据类型**:`application/x-www-form-urlencoded`


**响应数据类型**:`*/*`


**接口描述**:<p>临时报名结果表-通过id查询</p>



**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|id|id|query|true|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«temp_result_of_sign对象»|
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|temp_result_of_sign对象|temp_result_of_sign对象|
|&emsp;&emsp;additionalReason|补录未入围原因|string||
|&emsp;&emsp;archiveCode|准考证号|string||
|&emsp;&emsp;calculateType|入围类型|string||
|&emsp;&emsp;combinedScore|组合分|string||
|&emsp;&emsp;directionalReason|定向未入围原因|string||
|&emsp;&emsp;finishSchoolCode|毕业学校代码|string||
|&emsp;&emsp;guideReason|指导未入围原因|string||
|&emsp;&emsp;highSchoolCode|高中学校代码|string||
|&emsp;&emsp;id|主键|string||
|&emsp;&emsp;instructionalReason|指令未入围原因|string||
|&emsp;&emsp;isAreaStudent|是否地段生|integer(int32)||
|&emsp;&emsp;orderCode|成绩排序码|string||
|&emsp;&emsp;runtime|运算时间|string(date-time)||
|&emsp;&emsp;signupType|报考类型|string||
|&emsp;&emsp;tempOrder|排名|integer(int32)||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": {
		"additionalReason": "",
		"archiveCode": "",
		"calculateType": "",
		"combinedScore": "",
		"directionalReason": "",
		"finishSchoolCode": "",
		"guideReason": "",
		"highSchoolCode": "",
		"id": "",
		"instructionalReason": "",
		"isAreaStudent": 0,
		"orderCode": "",
		"runtime": "",
		"signupType": "",
		"tempOrder": 0
	},
	"success": true,
	"timestamp": 0
}
```


# 临时运算结果表-总和


## 临时运算结果表-总和-添加


**接口地址**:`/nnzk/sign/tempResultOfSignMated/add`


**请求方式**:`POST`


**请求数据类型**:`application/json`


**响应数据类型**:`*/*`


**接口描述**:<p>临时运算结果表-总和-添加</p>



**请求示例**:


```javascript
{
  "additionalReason": "",
  "archiveCode": "",
  "calculateType": "",
  "combinedScore": "",
  "directionalReason": "",
  "finishSchoolCode": "",
  "guideReason": "",
  "highSchoolCode": "",
  "id": "",
  "instructionalReason": "",
  "isAreaStudent": 0,
  "orderCode": "",
  "runtime": "",
  "signupType": "",
  "tempOrder": 0
}
```


**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|tempResultOfSignMated|临时运算结果表-总和|body|true|temp_result_of_sign_mated对象|temp_result_of_sign_mated对象|
|&emsp;&emsp;additionalReason|补录未入围原因||false|string||
|&emsp;&emsp;archiveCode|准考证号||false|string||
|&emsp;&emsp;calculateType|入围类型||false|string||
|&emsp;&emsp;combinedScore|组合分||false|string||
|&emsp;&emsp;directionalReason|定向未入围原因||false|string||
|&emsp;&emsp;finishSchoolCode|毕业学校代码||false|string||
|&emsp;&emsp;guideReason|指导未入围原因||false|string||
|&emsp;&emsp;highSchoolCode|高中学校代码||false|string||
|&emsp;&emsp;id|主键||false|string||
|&emsp;&emsp;instructionalReason|指令未入围原因||false|string||
|&emsp;&emsp;isAreaStudent|是否地段生||false|integer(int32)||
|&emsp;&emsp;orderCode|成绩排序码||false|string||
|&emsp;&emsp;runtime|运算时间||false|string(date-time)||
|&emsp;&emsp;signupType|报考类型||false|string||
|&emsp;&emsp;tempOrder|排名||false|integer(int32)||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«string»|
|201|Created||
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|string||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": "",
	"success": true,
	"timestamp": 0
}
```


## 临时运算结果表-总和-通过id删除


**接口地址**:`/nnzk/sign/tempResultOfSignMated/delete`


**请求方式**:`DELETE`


**请求数据类型**:`application/x-www-form-urlencoded`


**响应数据类型**:`*/*`


**接口描述**:<p>临时运算结果表-总和-通过id删除</p>



**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|id|id|query|true|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«string»|
|204|No Content||
|401|Unauthorized||
|403|Forbidden||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|string||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": "",
	"success": true,
	"timestamp": 0
}
```


## 临时运算结果表-总和-批量删除


**接口地址**:`/nnzk/sign/tempResultOfSignMated/deleteBatch`


**请求方式**:`DELETE`


**请求数据类型**:`application/x-www-form-urlencoded`


**响应数据类型**:`*/*`


**接口描述**:<p>临时运算结果表-总和-批量删除</p>



**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|ids|ids|query|true|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«string»|
|204|No Content||
|401|Unauthorized||
|403|Forbidden||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|string||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": "",
	"success": true,
	"timestamp": 0
}
```


## 临时运算结果表-总和-编辑


**接口地址**:`/nnzk/sign/tempResultOfSignMated/edit`


**请求方式**:`POST`


**请求数据类型**:`application/json`


**响应数据类型**:`*/*`


**接口描述**:<p>临时运算结果表-总和-编辑</p>



**请求示例**:


```javascript
{
  "additionalReason": "",
  "archiveCode": "",
  "calculateType": "",
  "combinedScore": "",
  "directionalReason": "",
  "finishSchoolCode": "",
  "guideReason": "",
  "highSchoolCode": "",
  "id": "",
  "instructionalReason": "",
  "isAreaStudent": 0,
  "orderCode": "",
  "runtime": "",
  "signupType": "",
  "tempOrder": 0
}
```


**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|tempResultOfSignMated|临时运算结果表-总和|body|true|temp_result_of_sign_mated对象|temp_result_of_sign_mated对象|
|&emsp;&emsp;additionalReason|补录未入围原因||false|string||
|&emsp;&emsp;archiveCode|准考证号||false|string||
|&emsp;&emsp;calculateType|入围类型||false|string||
|&emsp;&emsp;combinedScore|组合分||false|string||
|&emsp;&emsp;directionalReason|定向未入围原因||false|string||
|&emsp;&emsp;finishSchoolCode|毕业学校代码||false|string||
|&emsp;&emsp;guideReason|指导未入围原因||false|string||
|&emsp;&emsp;highSchoolCode|高中学校代码||false|string||
|&emsp;&emsp;id|主键||false|string||
|&emsp;&emsp;instructionalReason|指令未入围原因||false|string||
|&emsp;&emsp;isAreaStudent|是否地段生||false|integer(int32)||
|&emsp;&emsp;orderCode|成绩排序码||false|string||
|&emsp;&emsp;runtime|运算时间||false|string(date-time)||
|&emsp;&emsp;signupType|报考类型||false|string||
|&emsp;&emsp;tempOrder|排名||false|integer(int32)||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«string»|
|201|Created||
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|string||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": "",
	"success": true,
	"timestamp": 0
}
```


## 临时运算结果表-总和-编辑


**接口地址**:`/nnzk/sign/tempResultOfSignMated/edit`


**请求方式**:`PUT`


**请求数据类型**:`application/json`


**响应数据类型**:`*/*`


**接口描述**:<p>临时运算结果表-总和-编辑</p>



**请求示例**:


```javascript
{
  "additionalReason": "",
  "archiveCode": "",
  "calculateType": "",
  "combinedScore": "",
  "directionalReason": "",
  "finishSchoolCode": "",
  "guideReason": "",
  "highSchoolCode": "",
  "id": "",
  "instructionalReason": "",
  "isAreaStudent": 0,
  "orderCode": "",
  "runtime": "",
  "signupType": "",
  "tempOrder": 0
}
```


**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|tempResultOfSignMated|临时运算结果表-总和|body|true|temp_result_of_sign_mated对象|temp_result_of_sign_mated对象|
|&emsp;&emsp;additionalReason|补录未入围原因||false|string||
|&emsp;&emsp;archiveCode|准考证号||false|string||
|&emsp;&emsp;calculateType|入围类型||false|string||
|&emsp;&emsp;combinedScore|组合分||false|string||
|&emsp;&emsp;directionalReason|定向未入围原因||false|string||
|&emsp;&emsp;finishSchoolCode|毕业学校代码||false|string||
|&emsp;&emsp;guideReason|指导未入围原因||false|string||
|&emsp;&emsp;highSchoolCode|高中学校代码||false|string||
|&emsp;&emsp;id|主键||false|string||
|&emsp;&emsp;instructionalReason|指令未入围原因||false|string||
|&emsp;&emsp;isAreaStudent|是否地段生||false|integer(int32)||
|&emsp;&emsp;orderCode|成绩排序码||false|string||
|&emsp;&emsp;runtime|运算时间||false|string(date-time)||
|&emsp;&emsp;signupType|报考类型||false|string||
|&emsp;&emsp;tempOrder|排名||false|integer(int32)||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«string»|
|201|Created||
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|string||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": "",
	"success": true,
	"timestamp": 0
}
```


## 临时运算结果表-总和-分页列表查询


**接口地址**:`/nnzk/sign/tempResultOfSignMated/list`


**请求方式**:`GET`


**请求数据类型**:`application/x-www-form-urlencoded`


**响应数据类型**:`*/*`


**接口描述**:<p>临时运算结果表-总和-分页列表查询</p>



**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|additionalReason|补录未入围原因|query|false|string||
|archiveCode|准考证号|query|false|string||
|calculateType|入围类型|query|false|string||
|combinedScore|组合分|query|false|string||
|directionalReason|定向未入围原因|query|false|string||
|finishSchoolCode|毕业学校代码|query|false|string||
|guideReason|指导未入围原因|query|false|string||
|highSchoolCode|高中学校代码|query|false|string||
|id|主键|query|false|string||
|instructionalReason|指令未入围原因|query|false|string||
|isAreaStudent|是否地段生|query|false|integer(int32)||
|orderCode|成绩排序码|query|false|string||
|pageNo|pageNo|query|false|integer(int32)||
|pageSize|pageSize|query|false|integer(int32)||
|runtime|运算时间|query|false|string(date-time)||
|signupType|报考类型|query|false|string||
|tempOrder|排名|query|false|integer(int32)||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«IPage«temp_result_of_sign_mated对象»»|
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|IPage«temp_result_of_sign_mated对象»|IPage«temp_result_of_sign_mated对象»|
|&emsp;&emsp;current||integer(int64)||
|&emsp;&emsp;pages||integer(int64)||
|&emsp;&emsp;records||array|temp_result_of_sign_mated对象|
|&emsp;&emsp;&emsp;&emsp;additionalReason|补录未入围原因|string||
|&emsp;&emsp;&emsp;&emsp;archiveCode|准考证号|string||
|&emsp;&emsp;&emsp;&emsp;calculateType|入围类型|string||
|&emsp;&emsp;&emsp;&emsp;combinedScore|组合分|string||
|&emsp;&emsp;&emsp;&emsp;directionalReason|定向未入围原因|string||
|&emsp;&emsp;&emsp;&emsp;finishSchoolCode|毕业学校代码|string||
|&emsp;&emsp;&emsp;&emsp;guideReason|指导未入围原因|string||
|&emsp;&emsp;&emsp;&emsp;highSchoolCode|高中学校代码|string||
|&emsp;&emsp;&emsp;&emsp;id|主键|string||
|&emsp;&emsp;&emsp;&emsp;instructionalReason|指令未入围原因|string||
|&emsp;&emsp;&emsp;&emsp;isAreaStudent|是否地段生|integer||
|&emsp;&emsp;&emsp;&emsp;orderCode|成绩排序码|string||
|&emsp;&emsp;&emsp;&emsp;runtime|运算时间|string||
|&emsp;&emsp;&emsp;&emsp;signupType|报考类型|string||
|&emsp;&emsp;&emsp;&emsp;tempOrder|排名|integer||
|&emsp;&emsp;size||integer(int64)||
|&emsp;&emsp;total||integer(int64)||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": {
		"current": 0,
		"pages": 0,
		"records": [
			{
				"additionalReason": "",
				"archiveCode": "",
				"calculateType": "",
				"combinedScore": "",
				"directionalReason": "",
				"finishSchoolCode": "",
				"guideReason": "",
				"highSchoolCode": "",
				"id": "",
				"instructionalReason": "",
				"isAreaStudent": 0,
				"orderCode": "",
				"runtime": "",
				"signupType": "",
				"tempOrder": 0
			}
		],
		"size": 0,
		"total": 0
	},
	"success": true,
	"timestamp": 0
}
```


## 临时运算结果表-总和-通过id查询


**接口地址**:`/nnzk/sign/tempResultOfSignMated/queryById`


**请求方式**:`GET`


**请求数据类型**:`application/x-www-form-urlencoded`


**响应数据类型**:`*/*`


**接口描述**:<p>临时运算结果表-总和-通过id查询</p>



**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|id|id|query|true|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«temp_result_of_sign_mated对象»|
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|temp_result_of_sign_mated对象|temp_result_of_sign_mated对象|
|&emsp;&emsp;additionalReason|补录未入围原因|string||
|&emsp;&emsp;archiveCode|准考证号|string||
|&emsp;&emsp;calculateType|入围类型|string||
|&emsp;&emsp;combinedScore|组合分|string||
|&emsp;&emsp;directionalReason|定向未入围原因|string||
|&emsp;&emsp;finishSchoolCode|毕业学校代码|string||
|&emsp;&emsp;guideReason|指导未入围原因|string||
|&emsp;&emsp;highSchoolCode|高中学校代码|string||
|&emsp;&emsp;id|主键|string||
|&emsp;&emsp;instructionalReason|指令未入围原因|string||
|&emsp;&emsp;isAreaStudent|是否地段生|integer(int32)||
|&emsp;&emsp;orderCode|成绩排序码|string||
|&emsp;&emsp;runtime|运算时间|string(date-time)||
|&emsp;&emsp;signupType|报考类型|string||
|&emsp;&emsp;tempOrder|排名|integer(int32)||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": {
		"additionalReason": "",
		"archiveCode": "",
		"calculateType": "",
		"combinedScore": "",
		"directionalReason": "",
		"finishSchoolCode": "",
		"guideReason": "",
		"highSchoolCode": "",
		"id": "",
		"instructionalReason": "",
		"isAreaStudent": 0,
		"orderCode": "",
		"runtime": "",
		"signupType": "",
		"tempOrder": 0
	},
	"success": true,
	"timestamp": 0
}
```


# 八年级学生信息


## 八年级学生信息-添加


**接口地址**:`/nnzk/eighthgrade/eighthGradeStuInfor/add`


**请求方式**:`POST`


**请求数据类型**:`application/json`


**响应数据类型**:`*/*`


**接口描述**:<p>八年级学生信息-添加</p>



**请求示例**:


```javascript
{
  "archiveCode": "",
  "boeLevel": "",
  "createBy": "",
  "createTime": "",
  "geographyAndBiologyLevel": "",
  "id": "",
  "inforTechLevel": "",
  "stuName": "",
  "updateBy": "",
  "updateTime": ""
}
```


**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|eighthGradeStuInfor|八年级学生信息|body|true|eighth_grade_stu_infor对象|eighth_grade_stu_infor对象|
|&emsp;&emsp;archiveCode|准考证号||false|string||
|&emsp;&emsp;boeLevel|生物操作实验成绩||false|string||
|&emsp;&emsp;createBy|创建人||false|string||
|&emsp;&emsp;createTime|创建日期||false|string(date-time)||
|&emsp;&emsp;geographyAndBiologyLevel|地理和生物成绩||false|string||
|&emsp;&emsp;id|主键||false|string||
|&emsp;&emsp;inforTechLevel|信息技术成绩||false|string||
|&emsp;&emsp;stuName|学生姓名||false|string||
|&emsp;&emsp;updateBy|更新人||false|string||
|&emsp;&emsp;updateTime|更新日期||false|string(date-time)||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«string»|
|201|Created||
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|string||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": "",
	"success": true,
	"timestamp": 0
}
```


## 八年级学生信息-通过id删除


**接口地址**:`/nnzk/eighthgrade/eighthGradeStuInfor/delete`


**请求方式**:`DELETE`


**请求数据类型**:`application/x-www-form-urlencoded`


**响应数据类型**:`*/*`


**接口描述**:<p>八年级学生信息-通过id删除</p>



**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|id|id|query|true|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«string»|
|204|No Content||
|401|Unauthorized||
|403|Forbidden||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|string||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": "",
	"success": true,
	"timestamp": 0
}
```


## 八年级学生信息-批量删除


**接口地址**:`/nnzk/eighthgrade/eighthGradeStuInfor/deleteBatch`


**请求方式**:`DELETE`


**请求数据类型**:`application/x-www-form-urlencoded`


**响应数据类型**:`*/*`


**接口描述**:<p>八年级学生信息-批量删除</p>



**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|ids|ids|query|true|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«string»|
|204|No Content||
|401|Unauthorized||
|403|Forbidden||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|string||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": "",
	"success": true,
	"timestamp": 0
}
```


## 八年级学生信息-编辑


**接口地址**:`/nnzk/eighthgrade/eighthGradeStuInfor/edit`


**请求方式**:`POST`


**请求数据类型**:`application/json`


**响应数据类型**:`*/*`


**接口描述**:<p>八年级学生信息-编辑</p>



**请求示例**:


```javascript
{
  "archiveCode": "",
  "boeLevel": "",
  "createBy": "",
  "createTime": "",
  "geographyAndBiologyLevel": "",
  "id": "",
  "inforTechLevel": "",
  "stuName": "",
  "updateBy": "",
  "updateTime": ""
}
```


**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|eighthGradeStuInfor|八年级学生信息|body|true|eighth_grade_stu_infor对象|eighth_grade_stu_infor对象|
|&emsp;&emsp;archiveCode|准考证号||false|string||
|&emsp;&emsp;boeLevel|生物操作实验成绩||false|string||
|&emsp;&emsp;createBy|创建人||false|string||
|&emsp;&emsp;createTime|创建日期||false|string(date-time)||
|&emsp;&emsp;geographyAndBiologyLevel|地理和生物成绩||false|string||
|&emsp;&emsp;id|主键||false|string||
|&emsp;&emsp;inforTechLevel|信息技术成绩||false|string||
|&emsp;&emsp;stuName|学生姓名||false|string||
|&emsp;&emsp;updateBy|更新人||false|string||
|&emsp;&emsp;updateTime|更新日期||false|string(date-time)||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«string»|
|201|Created||
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|string||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": "",
	"success": true,
	"timestamp": 0
}
```


## 八年级学生信息-编辑


**接口地址**:`/nnzk/eighthgrade/eighthGradeStuInfor/edit`


**请求方式**:`PUT`


**请求数据类型**:`application/json`


**响应数据类型**:`*/*`


**接口描述**:<p>八年级学生信息-编辑</p>



**请求示例**:


```javascript
{
  "archiveCode": "",
  "boeLevel": "",
  "createBy": "",
  "createTime": "",
  "geographyAndBiologyLevel": "",
  "id": "",
  "inforTechLevel": "",
  "stuName": "",
  "updateBy": "",
  "updateTime": ""
}
```


**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|eighthGradeStuInfor|八年级学生信息|body|true|eighth_grade_stu_infor对象|eighth_grade_stu_infor对象|
|&emsp;&emsp;archiveCode|准考证号||false|string||
|&emsp;&emsp;boeLevel|生物操作实验成绩||false|string||
|&emsp;&emsp;createBy|创建人||false|string||
|&emsp;&emsp;createTime|创建日期||false|string(date-time)||
|&emsp;&emsp;geographyAndBiologyLevel|地理和生物成绩||false|string||
|&emsp;&emsp;id|主键||false|string||
|&emsp;&emsp;inforTechLevel|信息技术成绩||false|string||
|&emsp;&emsp;stuName|学生姓名||false|string||
|&emsp;&emsp;updateBy|更新人||false|string||
|&emsp;&emsp;updateTime|更新日期||false|string(date-time)||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«string»|
|201|Created||
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|string||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": "",
	"success": true,
	"timestamp": 0
}
```


## 八年级学生信息-查询生地成绩


**接口地址**:`/nnzk/eighthgrade/eighthGradeStuInfor/getScoreInfo`


**请求方式**:`GET`


**请求数据类型**:`application/x-www-form-urlencoded`


**响应数据类型**:`*/*`


**接口描述**:<p>八年级学生信息-查询生地成绩</p>



**请求参数**:


暂无


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«EighthGradeStuScoreVO»|
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|EighthGradeStuScoreVO|EighthGradeStuScoreVO|
|&emsp;&emsp;archiveCode|准考证号|string||
|&emsp;&emsp;boeLevel|生物操作实验成绩|string||
|&emsp;&emsp;geographyAndBiologyLevel|地理和生物成绩|string||
|&emsp;&emsp;inforTechLevel|信息技术成绩|string||
|&emsp;&emsp;queryTime|查询时间|string(date-time)||
|&emsp;&emsp;scoreMd5|成绩校验码|string||
|&emsp;&emsp;stuName|学生姓名|string||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": {
		"archiveCode": "",
		"boeLevel": "",
		"geographyAndBiologyLevel": "",
		"inforTechLevel": "",
		"queryTime": "",
		"scoreMd5": "",
		"stuName": ""
	},
	"success": true,
	"timestamp": 0
}
```


## 八年级学生信息-分页列表查询


**接口地址**:`/nnzk/eighthgrade/eighthGradeStuInfor/list`


**请求方式**:`GET`


**请求数据类型**:`application/x-www-form-urlencoded`


**响应数据类型**:`*/*`


**接口描述**:<p>八年级学生信息-分页列表查询</p>



**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|archiveCode|准考证号|query|false|string||
|boeLevel|生物操作实验成绩|query|false|string||
|createBy|创建人|query|false|string||
|createTime|创建日期|query|false|string(date-time)||
|geographyAndBiologyLevel|地理和生物成绩|query|false|string||
|id|主键|query|false|string||
|inforTechLevel|信息技术成绩|query|false|string||
|pageNo|pageNo|query|false|integer(int32)||
|pageSize|pageSize|query|false|integer(int32)||
|stuName|学生姓名|query|false|string||
|updateBy|更新人|query|false|string||
|updateTime|更新日期|query|false|string(date-time)||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«IPage«eighth_grade_stu_infor对象»»|
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|IPage«eighth_grade_stu_infor对象»|IPage«eighth_grade_stu_infor对象»|
|&emsp;&emsp;current||integer(int64)||
|&emsp;&emsp;pages||integer(int64)||
|&emsp;&emsp;records||array|eighth_grade_stu_infor对象|
|&emsp;&emsp;&emsp;&emsp;archiveCode|准考证号|string||
|&emsp;&emsp;&emsp;&emsp;boeLevel|生物操作实验成绩|string||
|&emsp;&emsp;&emsp;&emsp;createBy|创建人|string||
|&emsp;&emsp;&emsp;&emsp;createTime|创建日期|string||
|&emsp;&emsp;&emsp;&emsp;geographyAndBiologyLevel|地理和生物成绩|string||
|&emsp;&emsp;&emsp;&emsp;id|主键|string||
|&emsp;&emsp;&emsp;&emsp;inforTechLevel|信息技术成绩|string||
|&emsp;&emsp;&emsp;&emsp;stuName|学生姓名|string||
|&emsp;&emsp;&emsp;&emsp;updateBy|更新人|string||
|&emsp;&emsp;&emsp;&emsp;updateTime|更新日期|string||
|&emsp;&emsp;size||integer(int64)||
|&emsp;&emsp;total||integer(int64)||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": {
		"current": 0,
		"pages": 0,
		"records": [
			{
				"archiveCode": "",
				"boeLevel": "",
				"createBy": "",
				"createTime": "",
				"geographyAndBiologyLevel": "",
				"id": "",
				"inforTechLevel": "",
				"stuName": "",
				"updateBy": "",
				"updateTime": ""
			}
		],
		"size": 0,
		"total": 0
	},
	"success": true,
	"timestamp": 0
}
```


## 八年级学生信息-通过id查询


**接口地址**:`/nnzk/eighthgrade/eighthGradeStuInfor/queryById`


**请求方式**:`GET`


**请求数据类型**:`application/x-www-form-urlencoded`


**响应数据类型**:`*/*`


**接口描述**:<p>八年级学生信息-通过id查询</p>



**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|id|id|query|true|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«eighth_grade_stu_infor对象»|
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|eighth_grade_stu_infor对象|eighth_grade_stu_infor对象|
|&emsp;&emsp;archiveCode|准考证号|string||
|&emsp;&emsp;boeLevel|生物操作实验成绩|string||
|&emsp;&emsp;createBy|创建人|string||
|&emsp;&emsp;createTime|创建日期|string(date-time)||
|&emsp;&emsp;geographyAndBiologyLevel|地理和生物成绩|string||
|&emsp;&emsp;id|主键|string||
|&emsp;&emsp;inforTechLevel|信息技术成绩|string||
|&emsp;&emsp;stuName|学生姓名|string||
|&emsp;&emsp;updateBy|更新人|string||
|&emsp;&emsp;updateTime|更新日期|string(date-time)||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": {
		"archiveCode": "",
		"boeLevel": "",
		"createBy": "",
		"createTime": "",
		"geographyAndBiologyLevel": "",
		"id": "",
		"inforTechLevel": "",
		"stuName": "",
		"updateBy": "",
		"updateTime": ""
	},
	"success": true,
	"timestamp": 0
}
```


# 公示表


## 公示表-添加


**接口地址**:`/nnzk/config/article/add`


**请求方式**:`POST`


**请求数据类型**:`application/json`


**响应数据类型**:`*/*`


**接口描述**:<p>公示表-添加</p>



**请求示例**:


```javascript
{
  "content": "",
  "createBy": "",
  "createTime": "",
  "delFlag": 0,
  "filePath": "",
  "id": "",
  "isImage": 0,
  "isShowTitle": 0,
  "isTop": 0,
  "isValid": 0,
  "ordNum": 0,
  "title": "",
  "type": "",
  "updateBy": "",
  "updateTime": ""
}
```


**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|article|公示表|body|true|article对象|article对象|
|&emsp;&emsp;content|内容||false|string||
|&emsp;&emsp;createBy|创建人||false|string||
|&emsp;&emsp;createTime|创建日期||false|string(date-time)||
|&emsp;&emsp;delFlag|删除标签||false|integer(int32)||
|&emsp;&emsp;filePath|文件路径||false|string||
|&emsp;&emsp;id|主键||false|string||
|&emsp;&emsp;isImage|是否图像||false|integer(int32)||
|&emsp;&emsp;isShowTitle|是否显示标题||false|integer(int32)||
|&emsp;&emsp;isTop|是否置顶||false|integer(int32)||
|&emsp;&emsp;isValid|是否启用||false|integer(int32)||
|&emsp;&emsp;ordNum|排序码||false|integer(int32)||
|&emsp;&emsp;title|标题||false|string||
|&emsp;&emsp;type|类型||false|string||
|&emsp;&emsp;updateBy|更新人||false|string||
|&emsp;&emsp;updateTime|更新日期||false|string(date-time)||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«string»|
|201|Created||
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|string||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": "",
	"success": true,
	"timestamp": 0
}
```


## 公示表-通过id删除


**接口地址**:`/nnzk/config/article/delete`


**请求方式**:`DELETE`


**请求数据类型**:`application/x-www-form-urlencoded`


**响应数据类型**:`*/*`


**接口描述**:<p>公示表-通过id删除</p>



**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|id|id|query|true|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«string»|
|204|No Content||
|401|Unauthorized||
|403|Forbidden||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|string||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": "",
	"success": true,
	"timestamp": 0
}
```


## 公示表-批量删除


**接口地址**:`/nnzk/config/article/deleteBatch`


**请求方式**:`DELETE`


**请求数据类型**:`application/x-www-form-urlencoded`


**响应数据类型**:`*/*`


**接口描述**:<p>公示表-批量删除</p>



**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|ids|ids|query|true|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«string»|
|204|No Content||
|401|Unauthorized||
|403|Forbidden||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|string||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": "",
	"success": true,
	"timestamp": 0
}
```


## 公示表-编辑


**接口地址**:`/nnzk/config/article/edit`


**请求方式**:`POST`


**请求数据类型**:`application/json`


**响应数据类型**:`*/*`


**接口描述**:<p>公示表-编辑</p>



**请求示例**:


```javascript
{
  "content": "",
  "createBy": "",
  "createTime": "",
  "delFlag": 0,
  "filePath": "",
  "id": "",
  "isImage": 0,
  "isShowTitle": 0,
  "isTop": 0,
  "isValid": 0,
  "ordNum": 0,
  "title": "",
  "type": "",
  "updateBy": "",
  "updateTime": ""
}
```


**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|article|公示表|body|true|article对象|article对象|
|&emsp;&emsp;content|内容||false|string||
|&emsp;&emsp;createBy|创建人||false|string||
|&emsp;&emsp;createTime|创建日期||false|string(date-time)||
|&emsp;&emsp;delFlag|删除标签||false|integer(int32)||
|&emsp;&emsp;filePath|文件路径||false|string||
|&emsp;&emsp;id|主键||false|string||
|&emsp;&emsp;isImage|是否图像||false|integer(int32)||
|&emsp;&emsp;isShowTitle|是否显示标题||false|integer(int32)||
|&emsp;&emsp;isTop|是否置顶||false|integer(int32)||
|&emsp;&emsp;isValid|是否启用||false|integer(int32)||
|&emsp;&emsp;ordNum|排序码||false|integer(int32)||
|&emsp;&emsp;title|标题||false|string||
|&emsp;&emsp;type|类型||false|string||
|&emsp;&emsp;updateBy|更新人||false|string||
|&emsp;&emsp;updateTime|更新日期||false|string(date-time)||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«string»|
|201|Created||
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|string||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": "",
	"success": true,
	"timestamp": 0
}
```


## 公示表-编辑


**接口地址**:`/nnzk/config/article/edit`


**请求方式**:`PUT`


**请求数据类型**:`application/json`


**响应数据类型**:`*/*`


**接口描述**:<p>公示表-编辑</p>



**请求示例**:


```javascript
{
  "content": "",
  "createBy": "",
  "createTime": "",
  "delFlag": 0,
  "filePath": "",
  "id": "",
  "isImage": 0,
  "isShowTitle": 0,
  "isTop": 0,
  "isValid": 0,
  "ordNum": 0,
  "title": "",
  "type": "",
  "updateBy": "",
  "updateTime": ""
}
```


**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|article|公示表|body|true|article对象|article对象|
|&emsp;&emsp;content|内容||false|string||
|&emsp;&emsp;createBy|创建人||false|string||
|&emsp;&emsp;createTime|创建日期||false|string(date-time)||
|&emsp;&emsp;delFlag|删除标签||false|integer(int32)||
|&emsp;&emsp;filePath|文件路径||false|string||
|&emsp;&emsp;id|主键||false|string||
|&emsp;&emsp;isImage|是否图像||false|integer(int32)||
|&emsp;&emsp;isShowTitle|是否显示标题||false|integer(int32)||
|&emsp;&emsp;isTop|是否置顶||false|integer(int32)||
|&emsp;&emsp;isValid|是否启用||false|integer(int32)||
|&emsp;&emsp;ordNum|排序码||false|integer(int32)||
|&emsp;&emsp;title|标题||false|string||
|&emsp;&emsp;type|类型||false|string||
|&emsp;&emsp;updateBy|更新人||false|string||
|&emsp;&emsp;updateTime|更新日期||false|string(date-time)||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«string»|
|201|Created||
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|string||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": "",
	"success": true,
	"timestamp": 0
}
```


## 公示表-分页列表查询


**接口地址**:`/nnzk/config/article/list`


**请求方式**:`GET`


**请求数据类型**:`application/x-www-form-urlencoded`


**响应数据类型**:`*/*`


**接口描述**:<p>公示表-分页列表查询</p>



**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|content|内容|query|true|string||
|isImage|是否图像|query|true|integer(int32)||
|isShowTitle|是否显示标题|query|true|integer(int32)||
|isTop|是否置顶|query|true|integer(int32)||
|isValid|是否启用|query|true|integer(int32)||
|ordNum|排序码|query|true|integer(int32)||
|title|标题|query|true|string||
|type|类型|query|true|string||
|createBy|创建人|query|false|string||
|createTime|创建日期|query|false|string(date-time)||
|delFlag|删除标签|query|false|integer(int32)||
|filePath|文件路径|query|false|string||
|id|主键|query|false|string||
|pageNo|pageNo|query|false|integer(int32)||
|pageSize|pageSize|query|false|integer(int32)||
|updateBy|更新人|query|false|string||
|updateTime|更新日期|query|false|string(date-time)||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«IPage«article对象»»|
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|IPage«article对象»|IPage«article对象»|
|&emsp;&emsp;current||integer(int64)||
|&emsp;&emsp;pages||integer(int64)||
|&emsp;&emsp;records||array|article对象|
|&emsp;&emsp;&emsp;&emsp;content|内容|string||
|&emsp;&emsp;&emsp;&emsp;createBy|创建人|string||
|&emsp;&emsp;&emsp;&emsp;createTime|创建日期|string||
|&emsp;&emsp;&emsp;&emsp;delFlag|删除标签|integer||
|&emsp;&emsp;&emsp;&emsp;filePath|文件路径|string||
|&emsp;&emsp;&emsp;&emsp;id|主键|string||
|&emsp;&emsp;&emsp;&emsp;isImage|是否图像|integer||
|&emsp;&emsp;&emsp;&emsp;isShowTitle|是否显示标题|integer||
|&emsp;&emsp;&emsp;&emsp;isTop|是否置顶|integer||
|&emsp;&emsp;&emsp;&emsp;isValid|是否启用|integer||
|&emsp;&emsp;&emsp;&emsp;ordNum|排序码|integer||
|&emsp;&emsp;&emsp;&emsp;title|标题|string||
|&emsp;&emsp;&emsp;&emsp;type|类型|string||
|&emsp;&emsp;&emsp;&emsp;updateBy|更新人|string||
|&emsp;&emsp;&emsp;&emsp;updateTime|更新日期|string||
|&emsp;&emsp;size||integer(int64)||
|&emsp;&emsp;total||integer(int64)||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": {
		"current": 0,
		"pages": 0,
		"records": [
			{
				"content": "",
				"createBy": "",
				"createTime": "",
				"delFlag": 0,
				"filePath": "",
				"id": "",
				"isImage": 0,
				"isShowTitle": 0,
				"isTop": 0,
				"isValid": 0,
				"ordNum": 0,
				"title": "",
				"type": "",
				"updateBy": "",
				"updateTime": ""
			}
		],
		"size": 0,
		"total": 0
	},
	"success": true,
	"timestamp": 0
}
```


## 公示表-（启用）分页列表查询标题


**接口地址**:`/nnzk/config/article/listTitleValid`


**请求方式**:`GET`


**请求数据类型**:`application/x-www-form-urlencoded`


**响应数据类型**:`*/*`


**接口描述**:<p>公示表-（启用）分页列表查询标题</p>



**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|pageNo|pageNo|query|false|integer(int32)||
|pageSize|pageSize|query|false|integer(int32)||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«IPage«ArticleIdTitleVO»»|
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|IPage«ArticleIdTitleVO»|IPage«ArticleIdTitleVO»|
|&emsp;&emsp;current||integer(int64)||
|&emsp;&emsp;pages||integer(int64)||
|&emsp;&emsp;records||array|ArticleIdTitleVO|
|&emsp;&emsp;&emsp;&emsp;id|主键|string||
|&emsp;&emsp;&emsp;&emsp;title|标题|string||
|&emsp;&emsp;size||integer(int64)||
|&emsp;&emsp;total||integer(int64)||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": {
		"current": 0,
		"pages": 0,
		"records": [
			{
				"id": "",
				"title": ""
			}
		],
		"size": 0,
		"total": 0
	},
	"success": true,
	"timestamp": 0
}
```


## 公示表-通过id查询


**接口地址**:`/nnzk/config/article/queryById`


**请求方式**:`GET`


**请求数据类型**:`application/x-www-form-urlencoded`


**响应数据类型**:`*/*`


**接口描述**:<p>公示表-通过id查询</p>



**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|id|id|query|true|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«ArticleIdContentTitleVO»|
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|ArticleIdContentTitleVO|ArticleIdContentTitleVO|
|&emsp;&emsp;content|内容|string||
|&emsp;&emsp;id|主键|string||
|&emsp;&emsp;title|标题|string||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": {
		"content": "",
		"id": "",
		"title": ""
	},
	"success": true,
	"timestamp": 0
}
```


# 内部录取


## 内部录取-添加


**接口地址**:`/nnzk/sign/privateRegiste/add`


**请求方式**:`POST`


**请求数据类型**:`application/json`


**响应数据类型**:`*/*`


**接口描述**:<p>内部录取-添加</p>



**请求示例**:


```javascript
{
  "archiveCode": "",
  "commandType": "",
  "commander": "",
  "commanderPhone": "",
  "connector": "",
  "createBy": "",
  "createTime": "",
  "delFlag": 0,
  "id": "",
  "matriculateStatus": 0,
  "matriculateTime": "",
  "premat": 0,
  "registTime": "",
  "registeDept": "",
  "register": "",
  "setType": "",
  "signupSchoolCode": "",
  "studentType": "",
  "updateBy": "",
  "updateTime": ""
}
```


**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|privateRegiste|内部录取表|body|true|private_registe对象|private_registe对象|
|&emsp;&emsp;archiveCode|准考证号||false|string||
|&emsp;&emsp;commandType|推荐类型||false|string||
|&emsp;&emsp;commander|推荐人||false|string||
|&emsp;&emsp;commanderPhone|推荐人电话||false|string||
|&emsp;&emsp;connector|联系单位或联系人||false|string||
|&emsp;&emsp;createBy|创建人||false|string||
|&emsp;&emsp;createTime|创建日期||false|string(date-time)||
|&emsp;&emsp;delFlag|逻辑删除||false|integer(int32)||
|&emsp;&emsp;id|主键||false|string||
|&emsp;&emsp;matriculateStatus|录取状态||false|integer(int32)||
|&emsp;&emsp;matriculateTime|录取时间||false|string(date-time)||
|&emsp;&emsp;premat|?||false|integer(int32)||
|&emsp;&emsp;registTime|登记时间||false|string(date-time)||
|&emsp;&emsp;registeDept|登记部门||false|string||
|&emsp;&emsp;register|登记人||false|string||
|&emsp;&emsp;setType|设置类型||false|string||
|&emsp;&emsp;signupSchoolCode|报名学校||false|string||
|&emsp;&emsp;studentType|学生类型||false|string||
|&emsp;&emsp;updateBy|更新人||false|string||
|&emsp;&emsp;updateTime|更新日期||false|string(date-time)||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«string»|
|201|Created||
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|string||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": "",
	"success": true,
	"timestamp": 0
}
```


## 内部录取-取消本市其他登记


**接口地址**:`/nnzk/sign/privateRegiste/cancelRegCityOthers`


**请求方式**:`DELETE`


**请求数据类型**:`application/x-www-form-urlencoded`


**响应数据类型**:`*/*`


**接口描述**:<p>内部录取-取消本市其他登记</p>



**请求示例**:


```javascript
{
  "archiveCodes": [],
  "studentType": ""
}
```


**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|cancelRegDTO|cancelRegDTO|body|true|CancelRegDTO|CancelRegDTO|
|&emsp;&emsp;archiveCodes|准考证号数组||false|array|string|
|&emsp;&emsp;studentType|学生类型||false|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«string»|
|204|No Content||
|401|Unauthorized||
|403|Forbidden||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|string||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": "",
	"success": true,
	"timestamp": 0
}
```


## 内部录取-取消外地生登记


**接口地址**:`/nnzk/sign/privateRegiste/cancelRegForeign`


**请求方式**:`DELETE`


**请求数据类型**:`application/x-www-form-urlencoded`


**响应数据类型**:`*/*`


**接口描述**:<p>内部录取-取消外地生登记</p>



**请求示例**:


```javascript
{
  "archiveCodes": [],
  "studentType": ""
}
```


**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|cancelRegDTO|cancelRegDTO|body|true|CancelRegDTO|CancelRegDTO|
|&emsp;&emsp;archiveCodes|准考证号数组||false|array|string|
|&emsp;&emsp;studentType|学生类型||false|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«string»|
|204|No Content||
|401|Unauthorized||
|403|Forbidden||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|string||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": "",
	"success": true,
	"timestamp": 0
}
```


## 内部录取-取消国际班登记


**接口地址**:`/nnzk/sign/privateRegiste/cancelRegINTClass`


**请求方式**:`DELETE`


**请求数据类型**:`application/x-www-form-urlencoded`


**响应数据类型**:`*/*`


**接口描述**:<p>内部录取-取消国际班登记</p>



**请求示例**:


```javascript
{
  "archiveCodes": [],
  "studentType": ""
}
```


**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|cancelRegDTO|cancelRegDTO|body|true|CancelRegDTO|CancelRegDTO|
|&emsp;&emsp;archiveCodes|准考证号数组||false|array|string|
|&emsp;&emsp;studentType|学生类型||false|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«string»|
|204|No Content||
|401|Unauthorized||
|403|Forbidden||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|string||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": "",
	"success": true,
	"timestamp": 0
}
```


## 内部录取-取消特长生登记


**接口地址**:`/nnzk/sign/privateRegiste/cancelRegSpec`


**请求方式**:`DELETE`


**请求数据类型**:`application/x-www-form-urlencoded`


**响应数据类型**:`*/*`


**接口描述**:<p>内部录取-取消特长生登记</p>



**请求示例**:


```javascript
{
  "archiveCodes": [],
  "studentType": ""
}
```


**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|cancelRegDTO|cancelRegDTO|body|true|CancelRegDTO|CancelRegDTO|
|&emsp;&emsp;archiveCodes|准考证号数组||false|array|string|
|&emsp;&emsp;studentType|学生类型||false|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«string»|
|204|No Content||
|401|Unauthorized||
|403|Forbidden||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|string||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": "",
	"success": true,
	"timestamp": 0
}
```


## 内部录取-取消特长生报名


**接口地址**:`/nnzk/sign/privateRegiste/cancelSpecBM`


**请求方式**:`DELETE`


**请求数据类型**:`application/x-www-form-urlencoded`


**响应数据类型**:`*/*`


**接口描述**:<p>内部录取-取消特长生报名</p>



**请求示例**:


```javascript
{
  "ids": []
}
```


**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|input|input|body|true|CancelSpecBMInputDTO|CancelSpecBMInputDTO|
|&emsp;&emsp;ids|||false|array|string|


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«string»|
|204|No Content||
|401|Unauthorized||
|403|Forbidden||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|string||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": "",
	"success": true,
	"timestamp": 0
}
```


## 内部录取-检查考生是否可本市其他登记


**接口地址**:`/nnzk/sign/privateRegiste/checkIfMatCityOthers`


**请求方式**:`GET`


**请求数据类型**:`application/x-www-form-urlencoded`


**响应数据类型**:`*/*`


**接口描述**:<p>内部录取-检查考生是否可本市其他登记</p>



**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|archiveCode|archiveCode|query|true|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«CheckIfMatInfoDTO»|
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|CheckIfMatInfoDTO|CheckIfMatInfoDTO|
|&emsp;&emsp;chineseLevel|语文|string||
|&emsp;&emsp;chymistLevel|化学|string||
|&emsp;&emsp;combinedScore|组合分|string||
|&emsp;&emsp;diathesis|综合素质|string||
|&emsp;&emsp;englishLevel|英语|string||
|&emsp;&emsp;experiment|实验|string||
|&emsp;&emsp;finishSchoolCode|毕业学校|string||
|&emsp;&emsp;finishSchoolName|毕业学校名称|string||
|&emsp;&emsp;guardian|监护人|string||
|&emsp;&emsp;guardianPhone|监护人电话|string||
|&emsp;&emsp;homePlace|户口地址|string||
|&emsp;&emsp;mathLevel|数学|string||
|&emsp;&emsp;physicsLevel|物理|string||
|&emsp;&emsp;politicsLevel|政史|string||
|&emsp;&emsp;sex|性别|string||
|&emsp;&emsp;studentName|姓名|string||
|&emsp;&emsp;sumScore|总分|string||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": {
		"chineseLevel": "",
		"chymistLevel": "",
		"combinedScore": "",
		"diathesis": "",
		"englishLevel": "",
		"experiment": "",
		"finishSchoolCode": "",
		"finishSchoolName": "",
		"guardian": "",
		"guardianPhone": "",
		"homePlace": "",
		"mathLevel": "",
		"physicsLevel": "",
		"politicsLevel": "",
		"sex": "",
		"studentName": "",
		"sumScore": ""
	},
	"success": true,
	"timestamp": 0
}
```


## 内部录取-检查考生是否可外地生登记


**接口地址**:`/nnzk/sign/privateRegiste/checkIfMatForeign`


**请求方式**:`GET`


**请求数据类型**:`application/x-www-form-urlencoded`


**响应数据类型**:`*/*`


**接口描述**:<p>内部录取-检查考生是否可外地生登记</p>



**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|archiveCode|archiveCode|query|true|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«CheckIfMatInfoDTO»|
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|CheckIfMatInfoDTO|CheckIfMatInfoDTO|
|&emsp;&emsp;chineseLevel|语文|string||
|&emsp;&emsp;chymistLevel|化学|string||
|&emsp;&emsp;combinedScore|组合分|string||
|&emsp;&emsp;diathesis|综合素质|string||
|&emsp;&emsp;englishLevel|英语|string||
|&emsp;&emsp;experiment|实验|string||
|&emsp;&emsp;finishSchoolCode|毕业学校|string||
|&emsp;&emsp;finishSchoolName|毕业学校名称|string||
|&emsp;&emsp;guardian|监护人|string||
|&emsp;&emsp;guardianPhone|监护人电话|string||
|&emsp;&emsp;homePlace|户口地址|string||
|&emsp;&emsp;mathLevel|数学|string||
|&emsp;&emsp;physicsLevel|物理|string||
|&emsp;&emsp;politicsLevel|政史|string||
|&emsp;&emsp;sex|性别|string||
|&emsp;&emsp;studentName|姓名|string||
|&emsp;&emsp;sumScore|总分|string||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": {
		"chineseLevel": "",
		"chymistLevel": "",
		"combinedScore": "",
		"diathesis": "",
		"englishLevel": "",
		"experiment": "",
		"finishSchoolCode": "",
		"finishSchoolName": "",
		"guardian": "",
		"guardianPhone": "",
		"homePlace": "",
		"mathLevel": "",
		"physicsLevel": "",
		"politicsLevel": "",
		"sex": "",
		"studentName": "",
		"sumScore": ""
	},
	"success": true,
	"timestamp": 0
}
```


## 内部录取-检查考生是否可国际班本地考生登记


**接口地址**:`/nnzk/sign/privateRegiste/checkIfMatPrivilegeNative`


**请求方式**:`GET`


**请求数据类型**:`application/x-www-form-urlencoded`


**响应数据类型**:`*/*`


**接口描述**:<p>内部录取-检查考生是否可国际班本地考生登记</p>



**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|archiveCode|archiveCode|query|true|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«CheckIfMatInfoDTO»|
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|CheckIfMatInfoDTO|CheckIfMatInfoDTO|
|&emsp;&emsp;chineseLevel|语文|string||
|&emsp;&emsp;chymistLevel|化学|string||
|&emsp;&emsp;combinedScore|组合分|string||
|&emsp;&emsp;diathesis|综合素质|string||
|&emsp;&emsp;englishLevel|英语|string||
|&emsp;&emsp;experiment|实验|string||
|&emsp;&emsp;finishSchoolCode|毕业学校|string||
|&emsp;&emsp;finishSchoolName|毕业学校名称|string||
|&emsp;&emsp;guardian|监护人|string||
|&emsp;&emsp;guardianPhone|监护人电话|string||
|&emsp;&emsp;homePlace|户口地址|string||
|&emsp;&emsp;mathLevel|数学|string||
|&emsp;&emsp;physicsLevel|物理|string||
|&emsp;&emsp;politicsLevel|政史|string||
|&emsp;&emsp;sex|性别|string||
|&emsp;&emsp;studentName|姓名|string||
|&emsp;&emsp;sumScore|总分|string||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": {
		"chineseLevel": "",
		"chymistLevel": "",
		"combinedScore": "",
		"diathesis": "",
		"englishLevel": "",
		"experiment": "",
		"finishSchoolCode": "",
		"finishSchoolName": "",
		"guardian": "",
		"guardianPhone": "",
		"homePlace": "",
		"mathLevel": "",
		"physicsLevel": "",
		"politicsLevel": "",
		"sex": "",
		"studentName": "",
		"sumScore": ""
	},
	"success": true,
	"timestamp": 0
}
```


## 内部录取-检查考生是否可特长生登记


**接口地址**:`/nnzk/sign/privateRegiste/checkIfMatSpec`


**请求方式**:`GET`


**请求数据类型**:`application/x-www-form-urlencoded`


**响应数据类型**:`*/*`


**接口描述**:<p>内部录取-检查考生是否可特长生登记</p>



**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|archiveCode|archiveCode|query|true|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«CheckIfMatInfoDTO»|
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|CheckIfMatInfoDTO|CheckIfMatInfoDTO|
|&emsp;&emsp;chineseLevel|语文|string||
|&emsp;&emsp;chymistLevel|化学|string||
|&emsp;&emsp;combinedScore|组合分|string||
|&emsp;&emsp;diathesis|综合素质|string||
|&emsp;&emsp;englishLevel|英语|string||
|&emsp;&emsp;experiment|实验|string||
|&emsp;&emsp;finishSchoolCode|毕业学校|string||
|&emsp;&emsp;finishSchoolName|毕业学校名称|string||
|&emsp;&emsp;guardian|监护人|string||
|&emsp;&emsp;guardianPhone|监护人电话|string||
|&emsp;&emsp;homePlace|户口地址|string||
|&emsp;&emsp;mathLevel|数学|string||
|&emsp;&emsp;physicsLevel|物理|string||
|&emsp;&emsp;politicsLevel|政史|string||
|&emsp;&emsp;sex|性别|string||
|&emsp;&emsp;studentName|姓名|string||
|&emsp;&emsp;sumScore|总分|string||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": {
		"chineseLevel": "",
		"chymistLevel": "",
		"combinedScore": "",
		"diathesis": "",
		"englishLevel": "",
		"experiment": "",
		"finishSchoolCode": "",
		"finishSchoolName": "",
		"guardian": "",
		"guardianPhone": "",
		"homePlace": "",
		"mathLevel": "",
		"physicsLevel": "",
		"politicsLevel": "",
		"sex": "",
		"studentName": "",
		"sumScore": ""
	},
	"success": true,
	"timestamp": 0
}
```


## 内部录取-检查考生是否可特长生报名


**接口地址**:`/nnzk/sign/privateRegiste/checkIfMatSpecForBm`


**请求方式**:`GET`


**请求数据类型**:`application/x-www-form-urlencoded`


**响应数据类型**:`*/*`


**接口描述**:<p>内部录取-检查考生是否可特长生报名</p>



**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|archiveCode|archiveCode|query|true|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«CheckIfMatInfoDTO»|
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|CheckIfMatInfoDTO|CheckIfMatInfoDTO|
|&emsp;&emsp;chineseLevel|语文|string||
|&emsp;&emsp;chymistLevel|化学|string||
|&emsp;&emsp;combinedScore|组合分|string||
|&emsp;&emsp;diathesis|综合素质|string||
|&emsp;&emsp;englishLevel|英语|string||
|&emsp;&emsp;experiment|实验|string||
|&emsp;&emsp;finishSchoolCode|毕业学校|string||
|&emsp;&emsp;finishSchoolName|毕业学校名称|string||
|&emsp;&emsp;guardian|监护人|string||
|&emsp;&emsp;guardianPhone|监护人电话|string||
|&emsp;&emsp;homePlace|户口地址|string||
|&emsp;&emsp;mathLevel|数学|string||
|&emsp;&emsp;physicsLevel|物理|string||
|&emsp;&emsp;politicsLevel|政史|string||
|&emsp;&emsp;sex|性别|string||
|&emsp;&emsp;studentName|姓名|string||
|&emsp;&emsp;sumScore|总分|string||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": {
		"chineseLevel": "",
		"chymistLevel": "",
		"combinedScore": "",
		"diathesis": "",
		"englishLevel": "",
		"experiment": "",
		"finishSchoolCode": "",
		"finishSchoolName": "",
		"guardian": "",
		"guardianPhone": "",
		"homePlace": "",
		"mathLevel": "",
		"physicsLevel": "",
		"politicsLevel": "",
		"sex": "",
		"studentName": "",
		"sumScore": ""
	},
	"success": true,
	"timestamp": 0
}
```


## 内部录取-招办端本市其他内部录取(检查学校录取人数)


**接口地址**:`/nnzk/sign/privateRegiste/checkMatNumCityOthers`


**请求方式**:`GET`


**请求数据类型**:`application/x-www-form-urlencoded`


**响应数据类型**:`*/*`


**接口描述**:<p>内部录取-招办端本市其他内部录取(检查学校录取人数)</p>



**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|signupSchoolCode|signupSchoolCode|query|false|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«string»|
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|string||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": "",
	"success": true,
	"timestamp": 0
}
```


## 内部录取-招办端外地生内部录取(检查学校录取人数)


**接口地址**:`/nnzk/sign/privateRegiste/checkMatNumForeign`


**请求方式**:`GET`


**请求数据类型**:`application/x-www-form-urlencoded`


**响应数据类型**:`*/*`


**接口描述**:<p>内部录取-招办端外地生内部录取(检查学校录取人数)</p>



**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|signupSchoolCode|signupSchoolCode|query|false|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«string»|
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|string||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": "",
	"success": true,
	"timestamp": 0
}
```


## 内部录取-招办端特长生内部录取(检查学校录取人数)


**接口地址**:`/nnzk/sign/privateRegiste/checkMatNumSpec`


**请求方式**:`GET`


**请求数据类型**:`application/x-www-form-urlencoded`


**响应数据类型**:`*/*`


**接口描述**:<p>内部录取-招办端特长生内部录取(检查学校录取人数)</p>



**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|signupSchoolCode|signupSchoolCode|query|false|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«string»|
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|string||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": "",
	"success": true,
	"timestamp": 0
}
```


## 内部录取-招办端内部录取本市其他列表


**接口地址**:`/nnzk/sign/privateRegiste/cityOthersOrderList`


**请求方式**:`GET`


**请求数据类型**:`application/x-www-form-urlencoded`


**响应数据类型**:`*/*`


**接口描述**:<p>内部录取-招办端内部录取本市其他列表</p>



**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|isSpecOrder|是否特殊排序|query|true|boolean||
|archiveCode|准考证号|query|false|string||
|commander|推荐人|query|false|string||
|connector|联系单位或联系人|query|false|string||
|ddlPrivilegeClass|特招班|query|false|string||
|finishSchoolCode|毕业学校|query|false|string||
|matEndTime|录取时间|query|false|string(date-time)||
|matriculateStatus|录取状态|query|false|integer(int32)||
|matStartTime|录取时间|query|false|string(date-time)||
|pageNo|pageNo|query|false|integer(int32)||
|pageSize|pageSize|query|false|integer(int32)||
|registeDept|登记部门|query|false|string||
|register|登记人|query|false|string||
|signupSchoolCode|报名学校代码|query|false|string||
|signupSchoolName|报名学校名称|query|false|string||
|studentName|姓名|query|false|string||
|studentType|考生类型|query|false|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«IPage«PrivateRegistList»»|
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|IPage«PrivateRegistList»|IPage«PrivateRegistList»|
|&emsp;&emsp;current||integer(int64)||
|&emsp;&emsp;pages||integer(int64)||
|&emsp;&emsp;records||array|PrivateRegistList|
|&emsp;&emsp;&emsp;&emsp;archiveCode|准考证号|string||
|&emsp;&emsp;&emsp;&emsp;chineseLevel|语文|string||
|&emsp;&emsp;&emsp;&emsp;chymistLevel|化学|string||
|&emsp;&emsp;&emsp;&emsp;combinedScore|组合分|string||
|&emsp;&emsp;&emsp;&emsp;commandType|推荐类型|string||
|&emsp;&emsp;&emsp;&emsp;commander|推荐人|string||
|&emsp;&emsp;&emsp;&emsp;commanderPhone|推荐人电话|string||
|&emsp;&emsp;&emsp;&emsp;connector|联系单位或联系人|string||
|&emsp;&emsp;&emsp;&emsp;diathesis|综合素质|string||
|&emsp;&emsp;&emsp;&emsp;englishLevel|英语|string||
|&emsp;&emsp;&emsp;&emsp;experiment|实验|string||
|&emsp;&emsp;&emsp;&emsp;finishSchoolCode|毕业学校|string||
|&emsp;&emsp;&emsp;&emsp;guardian|监护人|string||
|&emsp;&emsp;&emsp;&emsp;guardianPhone|监护人电话|string||
|&emsp;&emsp;&emsp;&emsp;mathLevel|数学|string||
|&emsp;&emsp;&emsp;&emsp;matriculateStatus|录取状态|integer||
|&emsp;&emsp;&emsp;&emsp;matriculateTime|录取时间|string||
|&emsp;&emsp;&emsp;&emsp;matriculateType|录取类型|string||
|&emsp;&emsp;&emsp;&emsp;physicalEduLevel|体育|string||
|&emsp;&emsp;&emsp;&emsp;physicsLevel|物理|string||
|&emsp;&emsp;&emsp;&emsp;politicsLevel|政史|string||
|&emsp;&emsp;&emsp;&emsp;postCode|邮政编码|string||
|&emsp;&emsp;&emsp;&emsp;premat|预处理标志|integer||
|&emsp;&emsp;&emsp;&emsp;registTime|登记时间|string||
|&emsp;&emsp;&emsp;&emsp;registeDept|登记部门|string||
|&emsp;&emsp;&emsp;&emsp;register|登记人|string||
|&emsp;&emsp;&emsp;&emsp;remark|说明|string||
|&emsp;&emsp;&emsp;&emsp;serialNum|序号|integer||
|&emsp;&emsp;&emsp;&emsp;setType|分类|string||
|&emsp;&emsp;&emsp;&emsp;sex|性别|string||
|&emsp;&emsp;&emsp;&emsp;signupSchoolCode|报名学校|string||
|&emsp;&emsp;&emsp;&emsp;studentName|姓名|string||
|&emsp;&emsp;&emsp;&emsp;studentType|学生类型|string||
|&emsp;&emsp;&emsp;&emsp;sumScore|总分|string||
|&emsp;&emsp;size||integer(int64)||
|&emsp;&emsp;total||integer(int64)||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": {
		"current": 0,
		"pages": 0,
		"records": [
			{
				"archiveCode": "",
				"chineseLevel": "",
				"chymistLevel": "",
				"combinedScore": "",
				"commandType": "",
				"commander": "",
				"commanderPhone": "",
				"connector": "",
				"diathesis": "",
				"englishLevel": "",
				"experiment": "",
				"finishSchoolCode": "",
				"guardian": "",
				"guardianPhone": "",
				"mathLevel": "",
				"matriculateStatus": 0,
				"matriculateTime": "",
				"matriculateType": "",
				"physicalEduLevel": "",
				"physicsLevel": "",
				"politicsLevel": "",
				"postCode": "",
				"premat": 0,
				"registTime": "",
				"registeDept": "",
				"register": "",
				"remark": "",
				"serialNum": 0,
				"setType": "",
				"sex": "",
				"signupSchoolCode": "",
				"studentName": "",
				"studentType": "",
				"sumScore": ""
			}
		],
		"size": 0,
		"total": 0
	},
	"success": true,
	"timestamp": 0
}
```


## 内部录取-通过id删除


**接口地址**:`/nnzk/sign/privateRegiste/delete`


**请求方式**:`DELETE`


**请求数据类型**:`application/x-www-form-urlencoded`


**响应数据类型**:`*/*`


**接口描述**:<p>内部录取-通过id删除</p>



**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|id|id|query|true|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«string»|
|204|No Content||
|401|Unauthorized||
|403|Forbidden||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|string||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": "",
	"success": true,
	"timestamp": 0
}
```


## 内部录取-批量删除


**接口地址**:`/nnzk/sign/privateRegiste/deleteBatch`


**请求方式**:`DELETE`


**请求数据类型**:`application/x-www-form-urlencoded`


**响应数据类型**:`*/*`


**接口描述**:<p>内部录取-批量删除</p>



**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|ids|ids|query|true|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«string»|
|204|No Content||
|401|Unauthorized||
|403|Forbidden||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|string||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": "",
	"success": true,
	"timestamp": 0
}
```


## 内部录取-招办端内部录取(删除登记)


**接口地址**:`/nnzk/sign/privateRegiste/deleteRegistBatch`


**请求方式**:`PUT`


**请求数据类型**:`application/json`


**响应数据类型**:`*/*`


**接口描述**:<p>内部录取-内部录取(删除登记)</p>



**请求示例**:


```javascript
{
  "archiveCodes": []
}
```


**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|input|input|body|true|ArchiveCodesDTO|ArchiveCodesDTO|
|&emsp;&emsp;archiveCodes|||false|array|string|


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«string»|
|201|Created||
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|string||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": "",
	"success": true,
	"timestamp": 0
}
```


## 内部录取-招办端内部录取(本市其他录取)


**接口地址**:`/nnzk/sign/privateRegiste/doPrivateMatriCityOthers`


**请求方式**:`PUT`


**请求数据类型**:`application/json`


**响应数据类型**:`*/*`


**接口描述**:<p>内部录取-内部录取(本市其他录取)</p>



**请求示例**:


```javascript
{
  "archiveCodes": []
}
```


**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|input|input|body|true|ArchiveCodesDTO|ArchiveCodesDTO|
|&emsp;&emsp;archiveCodes|||false|array|string|


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«string»|
|201|Created||
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|string||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": "",
	"success": true,
	"timestamp": 0
}
```


## 内部录取-招办端内部录取(外地生录取)


**接口地址**:`/nnzk/sign/privateRegiste/doPrivateMatriForeign`


**请求方式**:`PUT`


**请求数据类型**:`application/json`


**响应数据类型**:`*/*`


**接口描述**:<p>内部录取-内部录取(外地生录取)</p>



**请求示例**:


```javascript
{
  "archiveCodes": []
}
```


**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|input|input|body|true|ArchiveCodesDTO|ArchiveCodesDTO|
|&emsp;&emsp;archiveCodes|||false|array|string|


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«int»|
|201|Created||
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|integer(int32)|integer(int32)|
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": 0,
	"success": true,
	"timestamp": 0
}
```


## 内部录取-招办端内部录取(国际班录取)


**接口地址**:`/nnzk/sign/privateRegiste/doPrivateMatriINTClass`


**请求方式**:`PUT`


**请求数据类型**:`application/json`


**响应数据类型**:`*/*`


**接口描述**:<p>内部录取-内部录取(国际班班录取)</p>



**请求示例**:


```javascript
{
  "archiveCodes": []
}
```


**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|input|input|body|true|ArchiveCodesDTO|ArchiveCodesDTO|
|&emsp;&emsp;archiveCodes|||false|array|string|


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«int»|
|201|Created||
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|integer(int32)|integer(int32)|
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": 0,
	"success": true,
	"timestamp": 0
}
```


## 内部录取-招办端内部录取(特长生录取)


**接口地址**:`/nnzk/sign/privateRegiste/doPrivateMatriSpec`


**请求方式**:`PUT`


**请求数据类型**:`application/json`


**响应数据类型**:`*/*`


**接口描述**:<p>内部录取-内部录取(特长生录取)</p>



**请求示例**:


```javascript
{
  "archiveCodes": []
}
```


**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|input|input|body|true|ArchiveCodesDTO|ArchiveCodesDTO|
|&emsp;&emsp;archiveCodes|||false|array|string|


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«string»|
|201|Created||
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|string||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": "",
	"success": true,
	"timestamp": 0
}
```


## 内部录取-特长生报名


**接口地址**:`/nnzk/sign/privateRegiste/doSpecBM`


**请求方式**:`POST`


**请求数据类型**:`application/json`


**响应数据类型**:`*/*`


**接口描述**:<p>内部录取-特长生报名</p>



**请求示例**:


```javascript
{
  "archiveCode": "",
  "commandType": "",
  "commander": "",
  "connector": "",
  "registeDept": "",
  "signupSchoolCode": "",
  "studentType": ""
}
```


**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|input|input|body|true|PrivateRegistDTO|PrivateRegistDTO|
|&emsp;&emsp;archiveCode|准考证号||false|string||
|&emsp;&emsp;commandType|推荐类型||false|string||
|&emsp;&emsp;commander|推荐人||false|string||
|&emsp;&emsp;connector|联系单位或联系人||false|string||
|&emsp;&emsp;registeDept|登记部门||false|string||
|&emsp;&emsp;signupSchoolCode|报名学校||false|string||
|&emsp;&emsp;studentType|学生类型||false|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«string»|
|201|Created||
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|string||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": "",
	"success": true,
	"timestamp": 0
}
```


## 内部录取-编辑


**接口地址**:`/nnzk/sign/privateRegiste/edit`


**请求方式**:`POST`


**请求数据类型**:`application/json`


**响应数据类型**:`*/*`


**接口描述**:<p>内部录取-编辑</p>



**请求示例**:


```javascript
{
  "archiveCode": "",
  "commandType": "",
  "commander": "",
  "commanderPhone": "",
  "connector": "",
  "createBy": "",
  "createTime": "",
  "delFlag": 0,
  "id": "",
  "matriculateStatus": 0,
  "matriculateTime": "",
  "premat": 0,
  "registTime": "",
  "registeDept": "",
  "register": "",
  "setType": "",
  "signupSchoolCode": "",
  "studentType": "",
  "updateBy": "",
  "updateTime": ""
}
```


**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|privateRegiste|内部录取表|body|true|private_registe对象|private_registe对象|
|&emsp;&emsp;archiveCode|准考证号||false|string||
|&emsp;&emsp;commandType|推荐类型||false|string||
|&emsp;&emsp;commander|推荐人||false|string||
|&emsp;&emsp;commanderPhone|推荐人电话||false|string||
|&emsp;&emsp;connector|联系单位或联系人||false|string||
|&emsp;&emsp;createBy|创建人||false|string||
|&emsp;&emsp;createTime|创建日期||false|string(date-time)||
|&emsp;&emsp;delFlag|逻辑删除||false|integer(int32)||
|&emsp;&emsp;id|主键||false|string||
|&emsp;&emsp;matriculateStatus|录取状态||false|integer(int32)||
|&emsp;&emsp;matriculateTime|录取时间||false|string(date-time)||
|&emsp;&emsp;premat|?||false|integer(int32)||
|&emsp;&emsp;registTime|登记时间||false|string(date-time)||
|&emsp;&emsp;registeDept|登记部门||false|string||
|&emsp;&emsp;register|登记人||false|string||
|&emsp;&emsp;setType|设置类型||false|string||
|&emsp;&emsp;signupSchoolCode|报名学校||false|string||
|&emsp;&emsp;studentType|学生类型||false|string||
|&emsp;&emsp;updateBy|更新人||false|string||
|&emsp;&emsp;updateTime|更新日期||false|string(date-time)||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«string»|
|201|Created||
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|string||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": "",
	"success": true,
	"timestamp": 0
}
```


## 内部录取-编辑


**接口地址**:`/nnzk/sign/privateRegiste/edit`


**请求方式**:`PUT`


**请求数据类型**:`application/json`


**响应数据类型**:`*/*`


**接口描述**:<p>内部录取-编辑</p>



**请求示例**:


```javascript
{
  "archiveCode": "",
  "commandType": "",
  "commander": "",
  "commanderPhone": "",
  "connector": "",
  "createBy": "",
  "createTime": "",
  "delFlag": 0,
  "id": "",
  "matriculateStatus": 0,
  "matriculateTime": "",
  "premat": 0,
  "registTime": "",
  "registeDept": "",
  "register": "",
  "setType": "",
  "signupSchoolCode": "",
  "studentType": "",
  "updateBy": "",
  "updateTime": ""
}
```


**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|privateRegiste|内部录取表|body|true|private_registe对象|private_registe对象|
|&emsp;&emsp;archiveCode|准考证号||false|string||
|&emsp;&emsp;commandType|推荐类型||false|string||
|&emsp;&emsp;commander|推荐人||false|string||
|&emsp;&emsp;commanderPhone|推荐人电话||false|string||
|&emsp;&emsp;connector|联系单位或联系人||false|string||
|&emsp;&emsp;createBy|创建人||false|string||
|&emsp;&emsp;createTime|创建日期||false|string(date-time)||
|&emsp;&emsp;delFlag|逻辑删除||false|integer(int32)||
|&emsp;&emsp;id|主键||false|string||
|&emsp;&emsp;matriculateStatus|录取状态||false|integer(int32)||
|&emsp;&emsp;matriculateTime|录取时间||false|string(date-time)||
|&emsp;&emsp;premat|?||false|integer(int32)||
|&emsp;&emsp;registTime|登记时间||false|string(date-time)||
|&emsp;&emsp;registeDept|登记部门||false|string||
|&emsp;&emsp;register|登记人||false|string||
|&emsp;&emsp;setType|设置类型||false|string||
|&emsp;&emsp;signupSchoolCode|报名学校||false|string||
|&emsp;&emsp;studentType|学生类型||false|string||
|&emsp;&emsp;updateBy|更新人||false|string||
|&emsp;&emsp;updateTime|更新日期||false|string(date-time)||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«string»|
|201|Created||
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|string||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": "",
	"success": true,
	"timestamp": 0
}
```


## 编辑学校登记限制


**接口地址**:`/nnzk/sign/privateRegiste/editRegRestriction`


**请求方式**:`POST`


**请求数据类型**:`application/json`


**响应数据类型**:`*/*`


**接口描述**:<p>编辑学校登记限制</p>



**请求示例**:


```javascript
{
  "innerSumScoreLimit": "",
  "lowestLevel": "",
  "schoolCode": "",
  "specSumScoreLimit": ""
}
```


**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|input|input|body|true|EditRegRestrictionDTO|EditRegRestrictionDTO|
|&emsp;&emsp;innerSumScoreLimit|内录最低控制总分-本市其他||false|string||
|&emsp;&emsp;lowestLevel|正录总分线||false|string||
|&emsp;&emsp;schoolCode|学校代码||false|string||
|&emsp;&emsp;specSumScoreLimit|内录最低控制总分-特长生/特招||false|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«string»|
|201|Created||
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|string||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": "",
	"success": true,
	"timestamp": 0
}
```


## 内部录取-招办端内部录取外地生列表


**接口地址**:`/nnzk/sign/privateRegiste/foreignOrderList`


**请求方式**:`GET`


**请求数据类型**:`application/x-www-form-urlencoded`


**响应数据类型**:`*/*`


**接口描述**:<p>内部录取-招办端内部录取外地生列表</p>



**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|isSpecOrder|是否特殊排序|query|true|boolean||
|archiveCode|准考证号|query|false|string||
|commander|推荐人|query|false|string||
|connector|联系单位或联系人|query|false|string||
|ddlPrivilegeClass|特招班|query|false|string||
|finishSchoolCode|毕业学校|query|false|string||
|matEndTime|录取时间|query|false|string(date-time)||
|matriculateStatus|录取状态|query|false|integer(int32)||
|matStartTime|录取时间|query|false|string(date-time)||
|pageNo|pageNo|query|false|integer(int32)||
|pageSize|pageSize|query|false|integer(int32)||
|registeDept|登记部门|query|false|string||
|register|登记人|query|false|string||
|signupSchoolCode|报名学校代码|query|false|string||
|signupSchoolName|报名学校名称|query|false|string||
|studentName|姓名|query|false|string||
|studentType|考生类型|query|false|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«IPage«PrivateRegistList»»|
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|IPage«PrivateRegistList»|IPage«PrivateRegistList»|
|&emsp;&emsp;current||integer(int64)||
|&emsp;&emsp;pages||integer(int64)||
|&emsp;&emsp;records||array|PrivateRegistList|
|&emsp;&emsp;&emsp;&emsp;archiveCode|准考证号|string||
|&emsp;&emsp;&emsp;&emsp;chineseLevel|语文|string||
|&emsp;&emsp;&emsp;&emsp;chymistLevel|化学|string||
|&emsp;&emsp;&emsp;&emsp;combinedScore|组合分|string||
|&emsp;&emsp;&emsp;&emsp;commandType|推荐类型|string||
|&emsp;&emsp;&emsp;&emsp;commander|推荐人|string||
|&emsp;&emsp;&emsp;&emsp;commanderPhone|推荐人电话|string||
|&emsp;&emsp;&emsp;&emsp;connector|联系单位或联系人|string||
|&emsp;&emsp;&emsp;&emsp;diathesis|综合素质|string||
|&emsp;&emsp;&emsp;&emsp;englishLevel|英语|string||
|&emsp;&emsp;&emsp;&emsp;experiment|实验|string||
|&emsp;&emsp;&emsp;&emsp;finishSchoolCode|毕业学校|string||
|&emsp;&emsp;&emsp;&emsp;guardian|监护人|string||
|&emsp;&emsp;&emsp;&emsp;guardianPhone|监护人电话|string||
|&emsp;&emsp;&emsp;&emsp;mathLevel|数学|string||
|&emsp;&emsp;&emsp;&emsp;matriculateStatus|录取状态|integer||
|&emsp;&emsp;&emsp;&emsp;matriculateTime|录取时间|string||
|&emsp;&emsp;&emsp;&emsp;matriculateType|录取类型|string||
|&emsp;&emsp;&emsp;&emsp;physicalEduLevel|体育|string||
|&emsp;&emsp;&emsp;&emsp;physicsLevel|物理|string||
|&emsp;&emsp;&emsp;&emsp;politicsLevel|政史|string||
|&emsp;&emsp;&emsp;&emsp;postCode|邮政编码|string||
|&emsp;&emsp;&emsp;&emsp;premat|预处理标志|integer||
|&emsp;&emsp;&emsp;&emsp;registTime|登记时间|string||
|&emsp;&emsp;&emsp;&emsp;registeDept|登记部门|string||
|&emsp;&emsp;&emsp;&emsp;register|登记人|string||
|&emsp;&emsp;&emsp;&emsp;remark|说明|string||
|&emsp;&emsp;&emsp;&emsp;serialNum|序号|integer||
|&emsp;&emsp;&emsp;&emsp;setType|分类|string||
|&emsp;&emsp;&emsp;&emsp;sex|性别|string||
|&emsp;&emsp;&emsp;&emsp;signupSchoolCode|报名学校|string||
|&emsp;&emsp;&emsp;&emsp;studentName|姓名|string||
|&emsp;&emsp;&emsp;&emsp;studentType|学生类型|string||
|&emsp;&emsp;&emsp;&emsp;sumScore|总分|string||
|&emsp;&emsp;size||integer(int64)||
|&emsp;&emsp;total||integer(int64)||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": {
		"current": 0,
		"pages": 0,
		"records": [
			{
				"archiveCode": "",
				"chineseLevel": "",
				"chymistLevel": "",
				"combinedScore": "",
				"commandType": "",
				"commander": "",
				"commanderPhone": "",
				"connector": "",
				"diathesis": "",
				"englishLevel": "",
				"experiment": "",
				"finishSchoolCode": "",
				"guardian": "",
				"guardianPhone": "",
				"mathLevel": "",
				"matriculateStatus": 0,
				"matriculateTime": "",
				"matriculateType": "",
				"physicalEduLevel": "",
				"physicsLevel": "",
				"politicsLevel": "",
				"postCode": "",
				"premat": 0,
				"registTime": "",
				"registeDept": "",
				"register": "",
				"remark": "",
				"serialNum": 0,
				"setType": "",
				"sex": "",
				"signupSchoolCode": "",
				"studentName": "",
				"studentType": "",
				"sumScore": ""
			}
		],
		"size": 0,
		"total": 0
	},
	"success": true,
	"timestamp": 0
}
```


## 内部录取-列表(国际班登记)


**接口地址**:`/nnzk/sign/privateRegiste/getOtherRegInfoINTClass`


**请求方式**:`GET`


**请求数据类型**:`application/x-www-form-urlencoded`


**响应数据类型**:`*/*`


**接口描述**:<p>内部录取-列表(国际班登记)</p>



**请求参数**:


暂无


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«GetRegInfoOutputDTO»|
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|GetRegInfoOutputDTO|GetRegInfoOutputDTO|
|&emsp;&emsp;count|学生登记总数|string||
|&emsp;&emsp;currentNum|当前数？|integer(int32)||
|&emsp;&emsp;makeUpPeopleNum|??|integer(int32)||
|&emsp;&emsp;minScore|最低分|string||
|&emsp;&emsp;mixScore|？？？|string||
|&emsp;&emsp;records|学生登记列表？|array|StudentRegDTO|
|&emsp;&emsp;&emsp;&emsp;archiveCode|准考证号|string||
|&emsp;&emsp;&emsp;&emsp;chineseLevel|语文|string||
|&emsp;&emsp;&emsp;&emsp;chymistLevel|化学|string||
|&emsp;&emsp;&emsp;&emsp;combinedScore|组合分|string||
|&emsp;&emsp;&emsp;&emsp;commandType|???|string||
|&emsp;&emsp;&emsp;&emsp;commander|???|string||
|&emsp;&emsp;&emsp;&emsp;connector|???|string||
|&emsp;&emsp;&emsp;&emsp;diathesis|综合素质|string||
|&emsp;&emsp;&emsp;&emsp;englishLevel|英语|string||
|&emsp;&emsp;&emsp;&emsp;experiment|实验|string||
|&emsp;&emsp;&emsp;&emsp;id|主键|string||
|&emsp;&emsp;&emsp;&emsp;mathLevel|数学|string||
|&emsp;&emsp;&emsp;&emsp;matriculateStatus|录取状态|integer||
|&emsp;&emsp;&emsp;&emsp;orderCode|排序码|string||
|&emsp;&emsp;&emsp;&emsp;physicsLevel|物理|string||
|&emsp;&emsp;&emsp;&emsp;politicsLevel|政史|string||
|&emsp;&emsp;&emsp;&emsp;registeDept|???|string||
|&emsp;&emsp;&emsp;&emsp;schoolCode|毕业学校代码|string||
|&emsp;&emsp;&emsp;&emsp;schoolName|毕业学校名称|string||
|&emsp;&emsp;&emsp;&emsp;studentName|学生名字|string||
|&emsp;&emsp;&emsp;&emsp;studentSource|学生生源地?|string||
|&emsp;&emsp;&emsp;&emsp;studentType|学生类型|string||
|&emsp;&emsp;&emsp;&emsp;sumScore|总分|string||
|&emsp;&emsp;&emsp;&emsp;type|类型MatriculateType?|string||
|&emsp;&emsp;url|？？？|string||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": {
		"count": "",
		"currentNum": 0,
		"makeUpPeopleNum": 0,
		"minScore": "",
		"mixScore": "",
		"records": [
			{
				"archiveCode": "",
				"chineseLevel": "",
				"chymistLevel": "",
				"combinedScore": "",
				"commandType": "",
				"commander": "",
				"connector": "",
				"diathesis": "",
				"englishLevel": "",
				"experiment": "",
				"id": "",
				"mathLevel": "",
				"matriculateStatus": 0,
				"orderCode": "",
				"physicsLevel": "",
				"politicsLevel": "",
				"registeDept": "",
				"schoolCode": "",
				"schoolName": "",
				"studentName": "",
				"studentSource": "",
				"studentType": "",
				"sumScore": "",
				"type": ""
			}
		],
		"url": ""
	},
	"success": true,
	"timestamp": 0
}
```


## 内部录取-特招班报名计划数


**接口地址**:`/nnzk/sign/privateRegiste/getPrivilegeClassSignupNum`


**请求方式**:`GET`


**请求数据类型**:`application/x-www-form-urlencoded`


**响应数据类型**:`*/*`


**接口描述**:<p>内部录取-特招班报名计划数</p>



**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|classId|classId|query|true|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«int»|
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|integer(int32)|integer(int32)|
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": 0,
	"success": true,
	"timestamp": 0
}
```


## 内部录取-列表(本市其他登记)


**接口地址**:`/nnzk/sign/privateRegiste/getRegInfoCityOthers`


**请求方式**:`GET`


**请求数据类型**:`application/x-www-form-urlencoded`


**响应数据类型**:`*/*`


**接口描述**:<p>内部录取-列表(本市其他登记)</p>



**请求参数**:


暂无


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«GetRegInfoOutputDTO»|
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|GetRegInfoOutputDTO|GetRegInfoOutputDTO|
|&emsp;&emsp;count|学生登记总数|string||
|&emsp;&emsp;currentNum|当前数？|integer(int32)||
|&emsp;&emsp;makeUpPeopleNum|??|integer(int32)||
|&emsp;&emsp;minScore|最低分|string||
|&emsp;&emsp;mixScore|？？？|string||
|&emsp;&emsp;records|学生登记列表？|array|StudentRegDTO|
|&emsp;&emsp;&emsp;&emsp;archiveCode|准考证号|string||
|&emsp;&emsp;&emsp;&emsp;chineseLevel|语文|string||
|&emsp;&emsp;&emsp;&emsp;chymistLevel|化学|string||
|&emsp;&emsp;&emsp;&emsp;combinedScore|组合分|string||
|&emsp;&emsp;&emsp;&emsp;commandType|???|string||
|&emsp;&emsp;&emsp;&emsp;commander|???|string||
|&emsp;&emsp;&emsp;&emsp;connector|???|string||
|&emsp;&emsp;&emsp;&emsp;diathesis|综合素质|string||
|&emsp;&emsp;&emsp;&emsp;englishLevel|英语|string||
|&emsp;&emsp;&emsp;&emsp;experiment|实验|string||
|&emsp;&emsp;&emsp;&emsp;id|主键|string||
|&emsp;&emsp;&emsp;&emsp;mathLevel|数学|string||
|&emsp;&emsp;&emsp;&emsp;matriculateStatus|录取状态|integer||
|&emsp;&emsp;&emsp;&emsp;orderCode|排序码|string||
|&emsp;&emsp;&emsp;&emsp;physicsLevel|物理|string||
|&emsp;&emsp;&emsp;&emsp;politicsLevel|政史|string||
|&emsp;&emsp;&emsp;&emsp;registeDept|???|string||
|&emsp;&emsp;&emsp;&emsp;schoolCode|毕业学校代码|string||
|&emsp;&emsp;&emsp;&emsp;schoolName|毕业学校名称|string||
|&emsp;&emsp;&emsp;&emsp;studentName|学生名字|string||
|&emsp;&emsp;&emsp;&emsp;studentSource|学生生源地?|string||
|&emsp;&emsp;&emsp;&emsp;studentType|学生类型|string||
|&emsp;&emsp;&emsp;&emsp;sumScore|总分|string||
|&emsp;&emsp;&emsp;&emsp;type|类型MatriculateType?|string||
|&emsp;&emsp;url|？？？|string||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": {
		"count": "",
		"currentNum": 0,
		"makeUpPeopleNum": 0,
		"minScore": "",
		"mixScore": "",
		"records": [
			{
				"archiveCode": "",
				"chineseLevel": "",
				"chymistLevel": "",
				"combinedScore": "",
				"commandType": "",
				"commander": "",
				"connector": "",
				"diathesis": "",
				"englishLevel": "",
				"experiment": "",
				"id": "",
				"mathLevel": "",
				"matriculateStatus": 0,
				"orderCode": "",
				"physicsLevel": "",
				"politicsLevel": "",
				"registeDept": "",
				"schoolCode": "",
				"schoolName": "",
				"studentName": "",
				"studentSource": "",
				"studentType": "",
				"sumScore": "",
				"type": ""
			}
		],
		"url": ""
	},
	"success": true,
	"timestamp": 0
}
```


## 内部录取-列表(外地生登记)


**接口地址**:`/nnzk/sign/privateRegiste/getRegInfoForeign`


**请求方式**:`GET`


**请求数据类型**:`application/x-www-form-urlencoded`


**响应数据类型**:`*/*`


**接口描述**:<p>内部录取-列表(外地生登记)</p>



**请求参数**:


暂无


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«GetRegInfoOutputDTO»|
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|GetRegInfoOutputDTO|GetRegInfoOutputDTO|
|&emsp;&emsp;count|学生登记总数|string||
|&emsp;&emsp;currentNum|当前数？|integer(int32)||
|&emsp;&emsp;makeUpPeopleNum|??|integer(int32)||
|&emsp;&emsp;minScore|最低分|string||
|&emsp;&emsp;mixScore|？？？|string||
|&emsp;&emsp;records|学生登记列表？|array|StudentRegDTO|
|&emsp;&emsp;&emsp;&emsp;archiveCode|准考证号|string||
|&emsp;&emsp;&emsp;&emsp;chineseLevel|语文|string||
|&emsp;&emsp;&emsp;&emsp;chymistLevel|化学|string||
|&emsp;&emsp;&emsp;&emsp;combinedScore|组合分|string||
|&emsp;&emsp;&emsp;&emsp;commandType|???|string||
|&emsp;&emsp;&emsp;&emsp;commander|???|string||
|&emsp;&emsp;&emsp;&emsp;connector|???|string||
|&emsp;&emsp;&emsp;&emsp;diathesis|综合素质|string||
|&emsp;&emsp;&emsp;&emsp;englishLevel|英语|string||
|&emsp;&emsp;&emsp;&emsp;experiment|实验|string||
|&emsp;&emsp;&emsp;&emsp;id|主键|string||
|&emsp;&emsp;&emsp;&emsp;mathLevel|数学|string||
|&emsp;&emsp;&emsp;&emsp;matriculateStatus|录取状态|integer||
|&emsp;&emsp;&emsp;&emsp;orderCode|排序码|string||
|&emsp;&emsp;&emsp;&emsp;physicsLevel|物理|string||
|&emsp;&emsp;&emsp;&emsp;politicsLevel|政史|string||
|&emsp;&emsp;&emsp;&emsp;registeDept|???|string||
|&emsp;&emsp;&emsp;&emsp;schoolCode|毕业学校代码|string||
|&emsp;&emsp;&emsp;&emsp;schoolName|毕业学校名称|string||
|&emsp;&emsp;&emsp;&emsp;studentName|学生名字|string||
|&emsp;&emsp;&emsp;&emsp;studentSource|学生生源地?|string||
|&emsp;&emsp;&emsp;&emsp;studentType|学生类型|string||
|&emsp;&emsp;&emsp;&emsp;sumScore|总分|string||
|&emsp;&emsp;&emsp;&emsp;type|类型MatriculateType?|string||
|&emsp;&emsp;url|？？？|string||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": {
		"count": "",
		"currentNum": 0,
		"makeUpPeopleNum": 0,
		"minScore": "",
		"mixScore": "",
		"records": [
			{
				"archiveCode": "",
				"chineseLevel": "",
				"chymistLevel": "",
				"combinedScore": "",
				"commandType": "",
				"commander": "",
				"connector": "",
				"diathesis": "",
				"englishLevel": "",
				"experiment": "",
				"id": "",
				"mathLevel": "",
				"matriculateStatus": 0,
				"orderCode": "",
				"physicsLevel": "",
				"politicsLevel": "",
				"registeDept": "",
				"schoolCode": "",
				"schoolName": "",
				"studentName": "",
				"studentSource": "",
				"studentType": "",
				"sumScore": "",
				"type": ""
			}
		],
		"url": ""
	},
	"success": true,
	"timestamp": 0
}
```


## 内部录取-列表(特长生登记)


**接口地址**:`/nnzk/sign/privateRegiste/getRegInfoSpec`


**请求方式**:`GET`


**请求数据类型**:`application/x-www-form-urlencoded`


**响应数据类型**:`*/*`


**接口描述**:<p>内部录取-列表(特长生登记)</p>



**请求参数**:


暂无


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«GetRegInfoOutputDTO»|
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|GetRegInfoOutputDTO|GetRegInfoOutputDTO|
|&emsp;&emsp;count|学生登记总数|string||
|&emsp;&emsp;currentNum|当前数？|integer(int32)||
|&emsp;&emsp;makeUpPeopleNum|??|integer(int32)||
|&emsp;&emsp;minScore|最低分|string||
|&emsp;&emsp;mixScore|？？？|string||
|&emsp;&emsp;records|学生登记列表？|array|StudentRegDTO|
|&emsp;&emsp;&emsp;&emsp;archiveCode|准考证号|string||
|&emsp;&emsp;&emsp;&emsp;chineseLevel|语文|string||
|&emsp;&emsp;&emsp;&emsp;chymistLevel|化学|string||
|&emsp;&emsp;&emsp;&emsp;combinedScore|组合分|string||
|&emsp;&emsp;&emsp;&emsp;commandType|???|string||
|&emsp;&emsp;&emsp;&emsp;commander|???|string||
|&emsp;&emsp;&emsp;&emsp;connector|???|string||
|&emsp;&emsp;&emsp;&emsp;diathesis|综合素质|string||
|&emsp;&emsp;&emsp;&emsp;englishLevel|英语|string||
|&emsp;&emsp;&emsp;&emsp;experiment|实验|string||
|&emsp;&emsp;&emsp;&emsp;id|主键|string||
|&emsp;&emsp;&emsp;&emsp;mathLevel|数学|string||
|&emsp;&emsp;&emsp;&emsp;matriculateStatus|录取状态|integer||
|&emsp;&emsp;&emsp;&emsp;orderCode|排序码|string||
|&emsp;&emsp;&emsp;&emsp;physicsLevel|物理|string||
|&emsp;&emsp;&emsp;&emsp;politicsLevel|政史|string||
|&emsp;&emsp;&emsp;&emsp;registeDept|???|string||
|&emsp;&emsp;&emsp;&emsp;schoolCode|毕业学校代码|string||
|&emsp;&emsp;&emsp;&emsp;schoolName|毕业学校名称|string||
|&emsp;&emsp;&emsp;&emsp;studentName|学生名字|string||
|&emsp;&emsp;&emsp;&emsp;studentSource|学生生源地?|string||
|&emsp;&emsp;&emsp;&emsp;studentType|学生类型|string||
|&emsp;&emsp;&emsp;&emsp;sumScore|总分|string||
|&emsp;&emsp;&emsp;&emsp;type|类型MatriculateType?|string||
|&emsp;&emsp;url|？？？|string||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": {
		"count": "",
		"currentNum": 0,
		"makeUpPeopleNum": 0,
		"minScore": "",
		"mixScore": "",
		"records": [
			{
				"archiveCode": "",
				"chineseLevel": "",
				"chymistLevel": "",
				"combinedScore": "",
				"commandType": "",
				"commander": "",
				"connector": "",
				"diathesis": "",
				"englishLevel": "",
				"experiment": "",
				"id": "",
				"mathLevel": "",
				"matriculateStatus": 0,
				"orderCode": "",
				"physicsLevel": "",
				"politicsLevel": "",
				"registeDept": "",
				"schoolCode": "",
				"schoolName": "",
				"studentName": "",
				"studentSource": "",
				"studentType": "",
				"sumScore": "",
				"type": ""
			}
		],
		"url": ""
	},
	"success": true,
	"timestamp": 0
}
```


## 内部录取-列表(特长生报名)


**接口地址**:`/nnzk/sign/privateRegiste/getRegInfoSpecBm`


**请求方式**:`GET`


**请求数据类型**:`application/x-www-form-urlencoded`


**响应数据类型**:`*/*`


**接口描述**:<p>内部录取-列表(特长生报名)</p>



**请求参数**:


暂无


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«GetRegInfoOutputDTO»|
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|GetRegInfoOutputDTO|GetRegInfoOutputDTO|
|&emsp;&emsp;count|学生登记总数|string||
|&emsp;&emsp;currentNum|当前数？|integer(int32)||
|&emsp;&emsp;makeUpPeopleNum|??|integer(int32)||
|&emsp;&emsp;minScore|最低分|string||
|&emsp;&emsp;mixScore|？？？|string||
|&emsp;&emsp;records|学生登记列表？|array|StudentRegDTO|
|&emsp;&emsp;&emsp;&emsp;archiveCode|准考证号|string||
|&emsp;&emsp;&emsp;&emsp;chineseLevel|语文|string||
|&emsp;&emsp;&emsp;&emsp;chymistLevel|化学|string||
|&emsp;&emsp;&emsp;&emsp;combinedScore|组合分|string||
|&emsp;&emsp;&emsp;&emsp;commandType|???|string||
|&emsp;&emsp;&emsp;&emsp;commander|???|string||
|&emsp;&emsp;&emsp;&emsp;connector|???|string||
|&emsp;&emsp;&emsp;&emsp;diathesis|综合素质|string||
|&emsp;&emsp;&emsp;&emsp;englishLevel|英语|string||
|&emsp;&emsp;&emsp;&emsp;experiment|实验|string||
|&emsp;&emsp;&emsp;&emsp;id|主键|string||
|&emsp;&emsp;&emsp;&emsp;mathLevel|数学|string||
|&emsp;&emsp;&emsp;&emsp;matriculateStatus|录取状态|integer||
|&emsp;&emsp;&emsp;&emsp;orderCode|排序码|string||
|&emsp;&emsp;&emsp;&emsp;physicsLevel|物理|string||
|&emsp;&emsp;&emsp;&emsp;politicsLevel|政史|string||
|&emsp;&emsp;&emsp;&emsp;registeDept|???|string||
|&emsp;&emsp;&emsp;&emsp;schoolCode|毕业学校代码|string||
|&emsp;&emsp;&emsp;&emsp;schoolName|毕业学校名称|string||
|&emsp;&emsp;&emsp;&emsp;studentName|学生名字|string||
|&emsp;&emsp;&emsp;&emsp;studentSource|学生生源地?|string||
|&emsp;&emsp;&emsp;&emsp;studentType|学生类型|string||
|&emsp;&emsp;&emsp;&emsp;sumScore|总分|string||
|&emsp;&emsp;&emsp;&emsp;type|类型MatriculateType?|string||
|&emsp;&emsp;url|？？？|string||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": {
		"count": "",
		"currentNum": 0,
		"makeUpPeopleNum": 0,
		"minScore": "",
		"mixScore": "",
		"records": [
			{
				"archiveCode": "",
				"chineseLevel": "",
				"chymistLevel": "",
				"combinedScore": "",
				"commandType": "",
				"commander": "",
				"connector": "",
				"diathesis": "",
				"englishLevel": "",
				"experiment": "",
				"id": "",
				"mathLevel": "",
				"matriculateStatus": 0,
				"orderCode": "",
				"physicsLevel": "",
				"politicsLevel": "",
				"registeDept": "",
				"schoolCode": "",
				"schoolName": "",
				"studentName": "",
				"studentSource": "",
				"studentType": "",
				"sumScore": "",
				"type": ""
			}
		],
		"url": ""
	},
	"success": true,
	"timestamp": 0
}
```


## 内部录取-分页列表查询


**接口地址**:`/nnzk/sign/privateRegiste/list`


**请求方式**:`GET`


**请求数据类型**:`application/x-www-form-urlencoded`


**响应数据类型**:`*/*`


**接口描述**:<p>内部录取-分页列表查询</p>



**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|archiveCode|准考证号|query|false|string||
|commander|推荐人|query|false|string||
|commanderPhone|推荐人电话|query|false|string||
|commandType|推荐类型|query|false|string||
|connector|联系单位或联系人|query|false|string||
|createBy|创建人|query|false|string||
|createTime|创建日期|query|false|string(date-time)||
|delFlag|逻辑删除|query|false|integer(int32)||
|id|主键|query|false|string||
|matriculateStatus|录取状态|query|false|integer(int32)||
|matriculateTime|录取时间|query|false|string(date-time)||
|pageNo|pageNo|query|false|integer(int32)||
|pageSize|pageSize|query|false|integer(int32)||
|premat|?|query|false|integer(int32)||
|registeDept|登记部门|query|false|string||
|register|登记人|query|false|string||
|registTime|登记时间|query|false|string(date-time)||
|setType|设置类型|query|false|string||
|signupSchoolCode|报名学校|query|false|string||
|studentType|学生类型|query|false|string||
|updateBy|更新人|query|false|string||
|updateTime|更新日期|query|false|string(date-time)||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«IPage«private_registe对象»»|
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|IPage«private_registe对象»|IPage«private_registe对象»|
|&emsp;&emsp;current||integer(int64)||
|&emsp;&emsp;pages||integer(int64)||
|&emsp;&emsp;records||array|private_registe对象|
|&emsp;&emsp;&emsp;&emsp;archiveCode|准考证号|string||
|&emsp;&emsp;&emsp;&emsp;commandType|推荐类型|string||
|&emsp;&emsp;&emsp;&emsp;commander|推荐人|string||
|&emsp;&emsp;&emsp;&emsp;commanderPhone|推荐人电话|string||
|&emsp;&emsp;&emsp;&emsp;connector|联系单位或联系人|string||
|&emsp;&emsp;&emsp;&emsp;createBy|创建人|string||
|&emsp;&emsp;&emsp;&emsp;createTime|创建日期|string||
|&emsp;&emsp;&emsp;&emsp;delFlag|逻辑删除|integer||
|&emsp;&emsp;&emsp;&emsp;id|主键|string||
|&emsp;&emsp;&emsp;&emsp;matriculateStatus|录取状态|integer||
|&emsp;&emsp;&emsp;&emsp;matriculateTime|录取时间|string||
|&emsp;&emsp;&emsp;&emsp;premat|?|integer||
|&emsp;&emsp;&emsp;&emsp;registTime|登记时间|string||
|&emsp;&emsp;&emsp;&emsp;registeDept|登记部门|string||
|&emsp;&emsp;&emsp;&emsp;register|登记人|string||
|&emsp;&emsp;&emsp;&emsp;setType|设置类型|string||
|&emsp;&emsp;&emsp;&emsp;signupSchoolCode|报名学校|string||
|&emsp;&emsp;&emsp;&emsp;studentType|学生类型|string||
|&emsp;&emsp;&emsp;&emsp;updateBy|更新人|string||
|&emsp;&emsp;&emsp;&emsp;updateTime|更新日期|string||
|&emsp;&emsp;size||integer(int64)||
|&emsp;&emsp;total||integer(int64)||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": {
		"current": 0,
		"pages": 0,
		"records": [
			{
				"archiveCode": "",
				"commandType": "",
				"commander": "",
				"commanderPhone": "",
				"connector": "",
				"createBy": "",
				"createTime": "",
				"delFlag": 0,
				"id": "",
				"matriculateStatus": 0,
				"matriculateTime": "",
				"premat": 0,
				"registTime": "",
				"registeDept": "",
				"register": "",
				"setType": "",
				"signupSchoolCode": "",
				"studentType": "",
				"updateBy": "",
				"updateTime": ""
			}
		],
		"size": 0,
		"total": 0
	},
	"success": true,
	"timestamp": 0
}
```


## 内部录取-招办端打印通知


**接口地址**:`/nnzk/sign/privateRegiste/print`


**请求方式**:`GET`


**请求数据类型**:`application/x-www-form-urlencoded`


**响应数据类型**:`*/*`


**接口描述**:<p>内部录取-招办端打印通知</p>



**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|ddlPrivilegeClass|特招班类型（国际班、民族班、外地生班。。）|query|false|string||
|highSchoolCode|录取学校代码|query|false|string||
|matBeginTime|录取时间范围（开始）|query|false|string(date-time)||
|matEndTime|录取时间（结束）|query|false|string(date-time)||
|matType|录取类型|query|false|string||
|selectedArchiveCode|选择打印的单个准考证号|query|false|string||
|selectedArchiveCodeList|选择打印的准考证号数组|query|false|array|string|


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|OrdMatAndPriRegPrintOutputDTO|
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|count|总条数|integer(int32)|integer(int32)|
|data|学生列表|array|OrdMatAndPriRegPrintDTO|
|&emsp;&emsp;archiveCode|准考证号|string||
|&emsp;&emsp;chineseLevel|语文|string||
|&emsp;&emsp;chymistLevel|化学|string||
|&emsp;&emsp;diathesis|综合素质|string||
|&emsp;&emsp;englishLevel|英语|string||
|&emsp;&emsp;experiment|实验|string||
|&emsp;&emsp;finishSchoolName|毕业学校|string||
|&emsp;&emsp;highSchoolName|录取学校|string||
|&emsp;&emsp;mathLevel|数学|string||
|&emsp;&emsp;matriculateType|录取类型|string||
|&emsp;&emsp;physicsLevel|物理|string||
|&emsp;&emsp;politicsLevel|政史|string||
|&emsp;&emsp;serialNum|序号|integer(int64)||
|&emsp;&emsp;sex|性别|string||
|&emsp;&emsp;studentName|学生姓名|string||
|&emsp;&emsp;sumScore|总分|string||
|total|总页数|integer(int32)|integer(int32)|


**响应示例**:
```javascript
{
	"count": 0,
	"data": [
		{
			"archiveCode": "",
			"chineseLevel": "",
			"chymistLevel": "",
			"diathesis": "",
			"englishLevel": "",
			"experiment": "",
			"finishSchoolName": "",
			"highSchoolName": "",
			"mathLevel": "",
			"matriculateType": "",
			"physicsLevel": "",
			"politicsLevel": "",
			"serialNum": 0,
			"sex": "",
			"studentName": "",
			"sumScore": ""
		}
	],
	"total": 0
}
```


## 内部录取-招办端打印发榜数据


**接口地址**:`/nnzk/sign/privateRegiste/printAnnounce`


**请求方式**:`GET`


**请求数据类型**:`application/x-www-form-urlencoded`


**响应数据类型**:`*/*`


**接口描述**:<p>内部录取-招办端打印发榜数据</p>



**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|ddlPrivilegeClass|特招班类型（国际班、民族班、外地生班。。）|query|false|string||
|highSchoolCode|录取学校代码|query|false|string||
|matBeginTime|录取时间范围（开始）|query|false|string(date-time)||
|matEndTime|录取时间（结束）|query|false|string(date-time)||
|matType|录取类型|query|false|string||
|selectedArchiveCode|选择打印的单个准考证号|query|false|string||
|selectedArchiveCodeList|选择打印的准考证号数组|query|false|array|string|


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|OrdMatAndPriRegPrintOutputDTO|
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|count|总条数|integer(int32)|integer(int32)|
|data|学生列表|array|OrdMatAndPriRegPrintDTO|
|&emsp;&emsp;archiveCode|准考证号|string||
|&emsp;&emsp;chineseLevel|语文|string||
|&emsp;&emsp;chymistLevel|化学|string||
|&emsp;&emsp;diathesis|综合素质|string||
|&emsp;&emsp;englishLevel|英语|string||
|&emsp;&emsp;experiment|实验|string||
|&emsp;&emsp;finishSchoolName|毕业学校|string||
|&emsp;&emsp;highSchoolName|录取学校|string||
|&emsp;&emsp;mathLevel|数学|string||
|&emsp;&emsp;matriculateType|录取类型|string||
|&emsp;&emsp;physicsLevel|物理|string||
|&emsp;&emsp;politicsLevel|政史|string||
|&emsp;&emsp;serialNum|序号|integer(int64)||
|&emsp;&emsp;sex|性别|string||
|&emsp;&emsp;studentName|学生姓名|string||
|&emsp;&emsp;sumScore|总分|string||
|total|总页数|integer(int32)|integer(int32)|


**响应示例**:
```javascript
{
	"count": 0,
	"data": [
		{
			"archiveCode": "",
			"chineseLevel": "",
			"chymistLevel": "",
			"diathesis": "",
			"englishLevel": "",
			"experiment": "",
			"finishSchoolName": "",
			"highSchoolName": "",
			"mathLevel": "",
			"matriculateType": "",
			"physicsLevel": "",
			"politicsLevel": "",
			"serialNum": 0,
			"sex": "",
			"studentName": "",
			"sumScore": ""
		}
	],
	"total": 0
}
```


## 内部录取-招办端打印名单


**接口地址**:`/nnzk/sign/privateRegiste/printList`


**请求方式**:`GET`


**请求数据类型**:`application/x-www-form-urlencoded`


**响应数据类型**:`*/*`


**接口描述**:<p>内部录取-招办端打印名单</p>



**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|isSpecOrder|是否特殊排序|query|true|boolean||
|archiveCode|准考证号|query|false|string||
|commander|推荐人|query|false|string||
|connector|联系单位或联系人|query|false|string||
|ddlPrivilegeClass|特招班|query|false|string||
|finishSchoolCode|毕业学校|query|false|string||
|matEndTime|录取时间|query|false|string(date-time)||
|matriculateStatus|录取状态|query|false|integer(int32)||
|matStartTime|录取时间|query|false|string(date-time)||
|registeDept|登记部门|query|false|string||
|register|登记人|query|false|string||
|signupSchoolCode|报名学校代码|query|false|string||
|signupSchoolName|报名学校名称|query|false|string||
|studentName|姓名|query|false|string||
|studentType|考生类型|query|false|string||
|type|type|query|false|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|PriRegPrintListOutputDTO|
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|count|总条数|integer(int32)|integer(int32)|
|data|列表|array|PrivateRegistList|
|&emsp;&emsp;archiveCode|准考证号|string||
|&emsp;&emsp;chineseLevel|语文|string||
|&emsp;&emsp;chymistLevel|化学|string||
|&emsp;&emsp;combinedScore|组合分|string||
|&emsp;&emsp;commandType|推荐类型|string||
|&emsp;&emsp;commander|推荐人|string||
|&emsp;&emsp;commanderPhone|推荐人电话|string||
|&emsp;&emsp;connector|联系单位或联系人|string||
|&emsp;&emsp;diathesis|综合素质|string||
|&emsp;&emsp;englishLevel|英语|string||
|&emsp;&emsp;experiment|实验|string||
|&emsp;&emsp;finishSchoolCode|毕业学校|string||
|&emsp;&emsp;guardian|监护人|string||
|&emsp;&emsp;guardianPhone|监护人电话|string||
|&emsp;&emsp;mathLevel|数学|string||
|&emsp;&emsp;matriculateStatus|录取状态|integer(int32)||
|&emsp;&emsp;matriculateTime|录取时间|string(date-time)||
|&emsp;&emsp;matriculateType|录取类型|string||
|&emsp;&emsp;physicalEduLevel|体育|string||
|&emsp;&emsp;physicsLevel|物理|string||
|&emsp;&emsp;politicsLevel|政史|string||
|&emsp;&emsp;postCode|邮政编码|string||
|&emsp;&emsp;premat|预处理标志|integer(int32)||
|&emsp;&emsp;registTime|登记时间|string(date-time)||
|&emsp;&emsp;registeDept|登记部门|string||
|&emsp;&emsp;register|登记人|string||
|&emsp;&emsp;remark|说明|string||
|&emsp;&emsp;serialNum|序号|integer(int32)||
|&emsp;&emsp;setType|分类|string||
|&emsp;&emsp;sex|性别|string||
|&emsp;&emsp;signupSchoolCode|报名学校|string||
|&emsp;&emsp;studentName|姓名|string||
|&emsp;&emsp;studentType|学生类型|string||
|&emsp;&emsp;sumScore|总分|string||
|total|总页数|integer(int32)|integer(int32)|


**响应示例**:
```javascript
{
	"count": 0,
	"data": [
		{
			"archiveCode": "",
			"chineseLevel": "",
			"chymistLevel": "",
			"combinedScore": "",
			"commandType": "",
			"commander": "",
			"commanderPhone": "",
			"connector": "",
			"diathesis": "",
			"englishLevel": "",
			"experiment": "",
			"finishSchoolCode": "",
			"guardian": "",
			"guardianPhone": "",
			"mathLevel": "",
			"matriculateStatus": 0,
			"matriculateTime": "",
			"matriculateType": "",
			"physicalEduLevel": "",
			"physicsLevel": "",
			"politicsLevel": "",
			"postCode": "",
			"premat": 0,
			"registTime": "",
			"registeDept": "",
			"register": "",
			"remark": "",
			"serialNum": 0,
			"setType": "",
			"sex": "",
			"signupSchoolCode": "",
			"studentName": "",
			"studentType": "",
			"sumScore": ""
		}
	],
	"total": 0
}
```


## 内部录取-打印其他登记未录取列表


**接口地址**:`/nnzk/sign/privateRegiste/printPriRegNotMat`


**请求方式**:`GET`


**请求数据类型**:`application/x-www-form-urlencoded`


**响应数据类型**:`*/*`


**接口描述**:<p>内部录取-打印其他登记未录取列表</p>



**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|studentType|studentType|query|true|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|OtherRegPrintDTO|
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|count|总条数|integer(int32)|integer(int32)|
|data|学生登记列表|array|StudentRegDTO|
|&emsp;&emsp;archiveCode|准考证号|string||
|&emsp;&emsp;chineseLevel|语文|string||
|&emsp;&emsp;chymistLevel|化学|string||
|&emsp;&emsp;combinedScore|组合分|string||
|&emsp;&emsp;commandType|???|string||
|&emsp;&emsp;commander|???|string||
|&emsp;&emsp;connector|???|string||
|&emsp;&emsp;diathesis|综合素质|string||
|&emsp;&emsp;englishLevel|英语|string||
|&emsp;&emsp;experiment|实验|string||
|&emsp;&emsp;id|主键|string||
|&emsp;&emsp;mathLevel|数学|string||
|&emsp;&emsp;matriculateStatus|录取状态|integer(int32)||
|&emsp;&emsp;orderCode|排序码|string||
|&emsp;&emsp;physicsLevel|物理|string||
|&emsp;&emsp;politicsLevel|政史|string||
|&emsp;&emsp;registeDept|???|string||
|&emsp;&emsp;schoolCode|毕业学校代码|string||
|&emsp;&emsp;schoolName|毕业学校名称|string||
|&emsp;&emsp;studentName|学生名字|string||
|&emsp;&emsp;studentSource|学生生源地?|string||
|&emsp;&emsp;studentType|学生类型|string||
|&emsp;&emsp;sumScore|总分|string||
|&emsp;&emsp;type|类型MatriculateType?|string||
|total|总页数|integer(int32)|integer(int32)|


**响应示例**:
```javascript
{
	"count": 0,
	"data": [
		{
			"archiveCode": "",
			"chineseLevel": "",
			"chymistLevel": "",
			"combinedScore": "",
			"commandType": "",
			"commander": "",
			"connector": "",
			"diathesis": "",
			"englishLevel": "",
			"experiment": "",
			"id": "",
			"mathLevel": "",
			"matriculateStatus": 0,
			"orderCode": "",
			"physicsLevel": "",
			"politicsLevel": "",
			"registeDept": "",
			"schoolCode": "",
			"schoolName": "",
			"studentName": "",
			"studentSource": "",
			"studentType": "",
			"sumScore": "",
			"type": ""
		}
	],
	"total": 0
}
```


## 内部录取-打印其他登记列表


**接口地址**:`/nnzk/sign/privateRegiste/printPrivateReg`


**请求方式**:`GET`


**请求数据类型**:`application/x-www-form-urlencoded`


**响应数据类型**:`*/*`


**接口描述**:<p>内部录取-打印其他登记列表</p>



**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|studentType|studentType|query|true|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|OtherRegPrintDTO|
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|count|总条数|integer(int32)|integer(int32)|
|data|学生登记列表|array|StudentRegDTO|
|&emsp;&emsp;archiveCode|准考证号|string||
|&emsp;&emsp;chineseLevel|语文|string||
|&emsp;&emsp;chymistLevel|化学|string||
|&emsp;&emsp;combinedScore|组合分|string||
|&emsp;&emsp;commandType|???|string||
|&emsp;&emsp;commander|???|string||
|&emsp;&emsp;connector|???|string||
|&emsp;&emsp;diathesis|综合素质|string||
|&emsp;&emsp;englishLevel|英语|string||
|&emsp;&emsp;experiment|实验|string||
|&emsp;&emsp;id|主键|string||
|&emsp;&emsp;mathLevel|数学|string||
|&emsp;&emsp;matriculateStatus|录取状态|integer(int32)||
|&emsp;&emsp;orderCode|排序码|string||
|&emsp;&emsp;physicsLevel|物理|string||
|&emsp;&emsp;politicsLevel|政史|string||
|&emsp;&emsp;registeDept|???|string||
|&emsp;&emsp;schoolCode|毕业学校代码|string||
|&emsp;&emsp;schoolName|毕业学校名称|string||
|&emsp;&emsp;studentName|学生名字|string||
|&emsp;&emsp;studentSource|学生生源地?|string||
|&emsp;&emsp;studentType|学生类型|string||
|&emsp;&emsp;sumScore|总分|string||
|&emsp;&emsp;type|类型MatriculateType?|string||
|total|总页数|integer(int32)|integer(int32)|


**响应示例**:
```javascript
{
	"count": 0,
	"data": [
		{
			"archiveCode": "",
			"chineseLevel": "",
			"chymistLevel": "",
			"combinedScore": "",
			"commandType": "",
			"commander": "",
			"connector": "",
			"diathesis": "",
			"englishLevel": "",
			"experiment": "",
			"id": "",
			"mathLevel": "",
			"matriculateStatus": 0,
			"orderCode": "",
			"physicsLevel": "",
			"politicsLevel": "",
			"registeDept": "",
			"schoolCode": "",
			"schoolName": "",
			"studentName": "",
			"studentSource": "",
			"studentType": "",
			"sumScore": "",
			"type": ""
		}
	],
	"total": 0
}
```


## 内部录取-招办端内部录取特招班列表


**接口地址**:`/nnzk/sign/privateRegiste/privilegeClassOrderList`


**请求方式**:`GET`


**请求数据类型**:`application/x-www-form-urlencoded`


**响应数据类型**:`*/*`


**接口描述**:<p>内部录取-招办端内部录取特招班列表</p>



**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|isSpecOrder|是否特殊排序|query|true|boolean||
|archiveCode|准考证号|query|false|string||
|commander|推荐人|query|false|string||
|connector|联系单位或联系人|query|false|string||
|ddlPrivilegeClass|特招班|query|false|string||
|finishSchoolCode|毕业学校|query|false|string||
|matEndTime|录取时间|query|false|string(date-time)||
|matriculateStatus|录取状态|query|false|integer(int32)||
|matStartTime|录取时间|query|false|string(date-time)||
|pageNo|pageNo|query|false|integer(int32)||
|pageSize|pageSize|query|false|integer(int32)||
|registeDept|登记部门|query|false|string||
|register|登记人|query|false|string||
|signupSchoolCode|报名学校代码|query|false|string||
|signupSchoolName|报名学校名称|query|false|string||
|studentName|姓名|query|false|string||
|studentType|考生类型|query|false|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«IPage«PrivateRegistList»»|
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|IPage«PrivateRegistList»|IPage«PrivateRegistList»|
|&emsp;&emsp;current||integer(int64)||
|&emsp;&emsp;pages||integer(int64)||
|&emsp;&emsp;records||array|PrivateRegistList|
|&emsp;&emsp;&emsp;&emsp;archiveCode|准考证号|string||
|&emsp;&emsp;&emsp;&emsp;chineseLevel|语文|string||
|&emsp;&emsp;&emsp;&emsp;chymistLevel|化学|string||
|&emsp;&emsp;&emsp;&emsp;combinedScore|组合分|string||
|&emsp;&emsp;&emsp;&emsp;commandType|推荐类型|string||
|&emsp;&emsp;&emsp;&emsp;commander|推荐人|string||
|&emsp;&emsp;&emsp;&emsp;commanderPhone|推荐人电话|string||
|&emsp;&emsp;&emsp;&emsp;connector|联系单位或联系人|string||
|&emsp;&emsp;&emsp;&emsp;diathesis|综合素质|string||
|&emsp;&emsp;&emsp;&emsp;englishLevel|英语|string||
|&emsp;&emsp;&emsp;&emsp;experiment|实验|string||
|&emsp;&emsp;&emsp;&emsp;finishSchoolCode|毕业学校|string||
|&emsp;&emsp;&emsp;&emsp;guardian|监护人|string||
|&emsp;&emsp;&emsp;&emsp;guardianPhone|监护人电话|string||
|&emsp;&emsp;&emsp;&emsp;mathLevel|数学|string||
|&emsp;&emsp;&emsp;&emsp;matriculateStatus|录取状态|integer||
|&emsp;&emsp;&emsp;&emsp;matriculateTime|录取时间|string||
|&emsp;&emsp;&emsp;&emsp;matriculateType|录取类型|string||
|&emsp;&emsp;&emsp;&emsp;physicalEduLevel|体育|string||
|&emsp;&emsp;&emsp;&emsp;physicsLevel|物理|string||
|&emsp;&emsp;&emsp;&emsp;politicsLevel|政史|string||
|&emsp;&emsp;&emsp;&emsp;postCode|邮政编码|string||
|&emsp;&emsp;&emsp;&emsp;premat|预处理标志|integer||
|&emsp;&emsp;&emsp;&emsp;registTime|登记时间|string||
|&emsp;&emsp;&emsp;&emsp;registeDept|登记部门|string||
|&emsp;&emsp;&emsp;&emsp;register|登记人|string||
|&emsp;&emsp;&emsp;&emsp;remark|说明|string||
|&emsp;&emsp;&emsp;&emsp;serialNum|序号|integer||
|&emsp;&emsp;&emsp;&emsp;setType|分类|string||
|&emsp;&emsp;&emsp;&emsp;sex|性别|string||
|&emsp;&emsp;&emsp;&emsp;signupSchoolCode|报名学校|string||
|&emsp;&emsp;&emsp;&emsp;studentName|姓名|string||
|&emsp;&emsp;&emsp;&emsp;studentType|学生类型|string||
|&emsp;&emsp;&emsp;&emsp;sumScore|总分|string||
|&emsp;&emsp;size||integer(int64)||
|&emsp;&emsp;total||integer(int64)||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": {
		"current": 0,
		"pages": 0,
		"records": [
			{
				"archiveCode": "",
				"chineseLevel": "",
				"chymistLevel": "",
				"combinedScore": "",
				"commandType": "",
				"commander": "",
				"commanderPhone": "",
				"connector": "",
				"diathesis": "",
				"englishLevel": "",
				"experiment": "",
				"finishSchoolCode": "",
				"guardian": "",
				"guardianPhone": "",
				"mathLevel": "",
				"matriculateStatus": 0,
				"matriculateTime": "",
				"matriculateType": "",
				"physicalEduLevel": "",
				"physicsLevel": "",
				"politicsLevel": "",
				"postCode": "",
				"premat": 0,
				"registTime": "",
				"registeDept": "",
				"register": "",
				"remark": "",
				"serialNum": 0,
				"setType": "",
				"sex": "",
				"signupSchoolCode": "",
				"studentName": "",
				"studentType": "",
				"sumScore": ""
			}
		],
		"size": 0,
		"total": 0
	},
	"success": true,
	"timestamp": 0
}
```


## 内部录取-通过id查询


**接口地址**:`/nnzk/sign/privateRegiste/queryById`


**请求方式**:`GET`


**请求数据类型**:`application/x-www-form-urlencoded`


**响应数据类型**:`*/*`


**接口描述**:<p>内部录取-通过id查询</p>



**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|id|id|query|true|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«private_registe对象»|
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|private_registe对象|private_registe对象|
|&emsp;&emsp;archiveCode|准考证号|string||
|&emsp;&emsp;commandType|推荐类型|string||
|&emsp;&emsp;commander|推荐人|string||
|&emsp;&emsp;commanderPhone|推荐人电话|string||
|&emsp;&emsp;connector|联系单位或联系人|string||
|&emsp;&emsp;createBy|创建人|string||
|&emsp;&emsp;createTime|创建日期|string(date-time)||
|&emsp;&emsp;delFlag|逻辑删除|integer(int32)||
|&emsp;&emsp;id|主键|string||
|&emsp;&emsp;matriculateStatus|录取状态|integer(int32)||
|&emsp;&emsp;matriculateTime|录取时间|string(date-time)||
|&emsp;&emsp;premat|?|integer(int32)||
|&emsp;&emsp;registTime|登记时间|string(date-time)||
|&emsp;&emsp;registeDept|登记部门|string||
|&emsp;&emsp;register|登记人|string||
|&emsp;&emsp;setType|设置类型|string||
|&emsp;&emsp;signupSchoolCode|报名学校|string||
|&emsp;&emsp;studentType|学生类型|string||
|&emsp;&emsp;updateBy|更新人|string||
|&emsp;&emsp;updateTime|更新日期|string(date-time)||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": {
		"archiveCode": "",
		"commandType": "",
		"commander": "",
		"commanderPhone": "",
		"connector": "",
		"createBy": "",
		"createTime": "",
		"delFlag": 0,
		"id": "",
		"matriculateStatus": 0,
		"matriculateTime": "",
		"premat": 0,
		"registTime": "",
		"registeDept": "",
		"register": "",
		"setType": "",
		"signupSchoolCode": "",
		"studentType": "",
		"updateBy": "",
		"updateTime": ""
	},
	"success": true,
	"timestamp": 0
}
```


## 内部录取-本市其他登记


**接口地址**:`/nnzk/sign/privateRegiste/regCityOthers`


**请求方式**:`PUT`


**请求数据类型**:`application/json`


**响应数据类型**:`*/*`


**接口描述**:<p>内部录取-本市其他登记</p>



**请求示例**:


```javascript
{
  "archiveCode": "",
  "commandType": "",
  "commander": "",
  "connector": "",
  "registeDept": "",
  "signupSchoolCode": "",
  "studentType": ""
}
```


**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|input|input|body|true|PrivateRegistDTO|PrivateRegistDTO|
|&emsp;&emsp;archiveCode|准考证号||false|string||
|&emsp;&emsp;commandType|推荐类型||false|string||
|&emsp;&emsp;commander|推荐人||false|string||
|&emsp;&emsp;connector|联系单位或联系人||false|string||
|&emsp;&emsp;registeDept|登记部门||false|string||
|&emsp;&emsp;signupSchoolCode|报名学校||false|string||
|&emsp;&emsp;studentType|学生类型||false|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«string»|
|201|Created||
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|string||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": "",
	"success": true,
	"timestamp": 0
}
```


## 内部录取-外地生登记


**接口地址**:`/nnzk/sign/privateRegiste/regForeign`


**请求方式**:`PUT`


**请求数据类型**:`application/json`


**响应数据类型**:`*/*`


**接口描述**:<p>内部录取-外地生登记</p>



**请求示例**:


```javascript
{
  "archiveCode": "",
  "commandType": "",
  "commander": "",
  "connector": "",
  "foreignStudentDTO": {
    "address": "",
    "archiveCode": "",
    "breakRule": "",
    "check": true,
    "chineseLevel": "",
    "chymistLevel": "",
    "combinedScore": "",
    "diathesis": "",
    "englishLevel": "",
    "experiment": "",
    "finishSchoolName": "",
    "guardian": "",
    "guardianPhone": "",
    "homePlace": "",
    "mathLevel": "",
    "physicalEduLevel": "",
    "physicsLevel": "",
    "politicsLevel": "",
    "registSchool": "",
    "remark": "",
    "sex": "",
    "studentName": "",
    "sumScore": ""
  },
  "registeDept": "",
  "signupSchoolCode": "",
  "studentType": ""
}
```


**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|input|input|body|true|ForeignRegDTO|ForeignRegDTO|
|&emsp;&emsp;archiveCode|准考证号||false|string||
|&emsp;&emsp;commandType|推荐类型||false|string||
|&emsp;&emsp;commander|推荐人||false|string||
|&emsp;&emsp;connector|联系单位或联系人||false|string||
|&emsp;&emsp;foreignStudentDTO|外地生信息||false|ForeignStudentDTO|ForeignStudentDTO|
|&emsp;&emsp;&emsp;&emsp;address|现住地址||false|string||
|&emsp;&emsp;&emsp;&emsp;archiveCode|准考证号||false|string||
|&emsp;&emsp;&emsp;&emsp;breakRule|||false|string||
|&emsp;&emsp;&emsp;&emsp;check|||false|boolean||
|&emsp;&emsp;&emsp;&emsp;chineseLevel|语文||false|string||
|&emsp;&emsp;&emsp;&emsp;chymistLevel|化学||false|string||
|&emsp;&emsp;&emsp;&emsp;combinedScore|组合分||false|string||
|&emsp;&emsp;&emsp;&emsp;diathesis|综合素质||false|string||
|&emsp;&emsp;&emsp;&emsp;englishLevel|英语||false|string||
|&emsp;&emsp;&emsp;&emsp;experiment|实验||false|string||
|&emsp;&emsp;&emsp;&emsp;finishSchoolName|毕业学校||false|string||
|&emsp;&emsp;&emsp;&emsp;guardian|监护人||false|string||
|&emsp;&emsp;&emsp;&emsp;guardianPhone|监护人电话||false|string||
|&emsp;&emsp;&emsp;&emsp;homePlace|户口地址||false|string||
|&emsp;&emsp;&emsp;&emsp;mathLevel|数学||false|string||
|&emsp;&emsp;&emsp;&emsp;physicalEduLevel|物理实验||false|string||
|&emsp;&emsp;&emsp;&emsp;physicsLevel|物理||false|string||
|&emsp;&emsp;&emsp;&emsp;politicsLevel|政史||false|string||
|&emsp;&emsp;&emsp;&emsp;registSchool|登记学校||false|string||
|&emsp;&emsp;&emsp;&emsp;remark|说明||false|string||
|&emsp;&emsp;&emsp;&emsp;sex|性别||false|string||
|&emsp;&emsp;&emsp;&emsp;studentName|姓名||false|string||
|&emsp;&emsp;&emsp;&emsp;sumScore|总分||false|string||
|&emsp;&emsp;registeDept|登记部门||false|string||
|&emsp;&emsp;signupSchoolCode|报名学校||false|string||
|&emsp;&emsp;studentType|学生类型||false|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«string»|
|201|Created||
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|string||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": "",
	"success": true,
	"timestamp": 0
}
```


## 内部录取-国际班外地考生登记


**接口地址**:`/nnzk/sign/privateRegiste/regINTClassForEcdemic`


**请求方式**:`PUT`


**请求数据类型**:`application/json`


**响应数据类型**:`*/*`


**接口描述**:<p>内部录取-国际班外地考生登记</p>



**请求示例**:


```javascript
{
  "archiveCode": "",
  "commandType": "",
  "commander": "",
  "connector": "",
  "foreignStudentDTO": {
    "address": "",
    "archiveCode": "",
    "breakRule": "",
    "check": true,
    "chineseLevel": "",
    "chymistLevel": "",
    "combinedScore": "",
    "diathesis": "",
    "englishLevel": "",
    "experiment": "",
    "finishSchoolName": "",
    "guardian": "",
    "guardianPhone": "",
    "homePlace": "",
    "mathLevel": "",
    "physicalEduLevel": "",
    "physicsLevel": "",
    "politicsLevel": "",
    "registSchool": "",
    "remark": "",
    "sex": "",
    "studentName": "",
    "sumScore": ""
  },
  "registeDept": "",
  "signupSchoolCode": "",
  "studentType": ""
}
```


**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|input|input|body|true|ForeignRegDTO|ForeignRegDTO|
|&emsp;&emsp;archiveCode|准考证号||false|string||
|&emsp;&emsp;commandType|推荐类型||false|string||
|&emsp;&emsp;commander|推荐人||false|string||
|&emsp;&emsp;connector|联系单位或联系人||false|string||
|&emsp;&emsp;foreignStudentDTO|外地生信息||false|ForeignStudentDTO|ForeignStudentDTO|
|&emsp;&emsp;&emsp;&emsp;address|现住地址||false|string||
|&emsp;&emsp;&emsp;&emsp;archiveCode|准考证号||false|string||
|&emsp;&emsp;&emsp;&emsp;breakRule|||false|string||
|&emsp;&emsp;&emsp;&emsp;check|||false|boolean||
|&emsp;&emsp;&emsp;&emsp;chineseLevel|语文||false|string||
|&emsp;&emsp;&emsp;&emsp;chymistLevel|化学||false|string||
|&emsp;&emsp;&emsp;&emsp;combinedScore|组合分||false|string||
|&emsp;&emsp;&emsp;&emsp;diathesis|综合素质||false|string||
|&emsp;&emsp;&emsp;&emsp;englishLevel|英语||false|string||
|&emsp;&emsp;&emsp;&emsp;experiment|实验||false|string||
|&emsp;&emsp;&emsp;&emsp;finishSchoolName|毕业学校||false|string||
|&emsp;&emsp;&emsp;&emsp;guardian|监护人||false|string||
|&emsp;&emsp;&emsp;&emsp;guardianPhone|监护人电话||false|string||
|&emsp;&emsp;&emsp;&emsp;homePlace|户口地址||false|string||
|&emsp;&emsp;&emsp;&emsp;mathLevel|数学||false|string||
|&emsp;&emsp;&emsp;&emsp;physicalEduLevel|物理实验||false|string||
|&emsp;&emsp;&emsp;&emsp;physicsLevel|物理||false|string||
|&emsp;&emsp;&emsp;&emsp;politicsLevel|政史||false|string||
|&emsp;&emsp;&emsp;&emsp;registSchool|登记学校||false|string||
|&emsp;&emsp;&emsp;&emsp;remark|说明||false|string||
|&emsp;&emsp;&emsp;&emsp;sex|性别||false|string||
|&emsp;&emsp;&emsp;&emsp;studentName|姓名||false|string||
|&emsp;&emsp;&emsp;&emsp;sumScore|总分||false|string||
|&emsp;&emsp;registeDept|登记部门||false|string||
|&emsp;&emsp;signupSchoolCode|报名学校||false|string||
|&emsp;&emsp;studentType|学生类型||false|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«string»|
|201|Created||
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|string||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": "",
	"success": true,
	"timestamp": 0
}
```


## 内部录取-国际班本地考生登记


**接口地址**:`/nnzk/sign/privateRegiste/regINTClassForNative`


**请求方式**:`PUT`


**请求数据类型**:`application/json`


**响应数据类型**:`*/*`


**接口描述**:<p>内部录取-国际班本地考生登记</p>



**请求示例**:


```javascript
{
  "archiveCode": "",
  "commandType": "",
  "commander": "",
  "connector": "",
  "registeDept": "",
  "signupSchoolCode": "",
  "studentType": ""
}
```


**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|input|input|body|true|PrivateRegistDTO|PrivateRegistDTO|
|&emsp;&emsp;archiveCode|准考证号||false|string||
|&emsp;&emsp;commandType|推荐类型||false|string||
|&emsp;&emsp;commander|推荐人||false|string||
|&emsp;&emsp;connector|联系单位或联系人||false|string||
|&emsp;&emsp;registeDept|登记部门||false|string||
|&emsp;&emsp;signupSchoolCode|报名学校||false|string||
|&emsp;&emsp;studentType|学生类型||false|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«string»|
|201|Created||
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|string||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": "",
	"success": true,
	"timestamp": 0
}
```


## 学校登记限制列表


**接口地址**:`/nnzk/sign/privateRegiste/regRestrictionList`


**请求方式**:`GET`


**请求数据类型**:`application/x-www-form-urlencoded`


**响应数据类型**:`*/*`


**接口描述**:<p>学校登记限制列表</p>



**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|schoolName|schoolName|query|false|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«List«HighSchoolRegRestrictionsVO»»|
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|array|HighSchoolRegRestrictionsVO|
|&emsp;&emsp;innerSumScoreLimit|内录最低控制总分-本市其他|string||
|&emsp;&emsp;lowestLevel|正录总分线|string||
|&emsp;&emsp;schoolCode|学校代码|string||
|&emsp;&emsp;schoolName|学校名称|string||
|&emsp;&emsp;schoolType|学校类型|integer(int32)||
|&emsp;&emsp;specSumScoreLimit|内录最低控制总分-特长生/特招|string||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": [
		{
			"innerSumScoreLimit": "",
			"lowestLevel": "",
			"schoolCode": "",
			"schoolName": "",
			"schoolType": 0,
			"specSumScoreLimit": ""
		}
	],
	"success": true,
	"timestamp": 0
}
```


## 内部录取-特长生登记


**接口地址**:`/nnzk/sign/privateRegiste/regSpec`


**请求方式**:`PUT`


**请求数据类型**:`application/json`


**响应数据类型**:`*/*`


**接口描述**:<p>内部录取-特长生登记</p>



**请求示例**:


```javascript
{
  "archiveCode": "",
  "commandType": "",
  "commander": "",
  "connector": "",
  "registeDept": "",
  "signupSchoolCode": "",
  "studentType": ""
}
```


**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|input|input|body|true|PrivateRegistDTO|PrivateRegistDTO|
|&emsp;&emsp;archiveCode|准考证号||false|string||
|&emsp;&emsp;commandType|推荐类型||false|string||
|&emsp;&emsp;commander|推荐人||false|string||
|&emsp;&emsp;connector|联系单位或联系人||false|string||
|&emsp;&emsp;registeDept|登记部门||false|string||
|&emsp;&emsp;signupSchoolCode|报名学校||false|string||
|&emsp;&emsp;studentType|学生类型||false|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«string»|
|201|Created||
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|string||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": "",
	"success": true,
	"timestamp": 0
}
```


## 内部录取-招办端内部录取特长生列表


**接口地址**:`/nnzk/sign/privateRegiste/specOrderList`


**请求方式**:`GET`


**请求数据类型**:`application/x-www-form-urlencoded`


**响应数据类型**:`*/*`


**接口描述**:<p>内部录取-招办端内部录取特长生列表</p>



**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|isSpecOrder|是否特殊排序|query|true|boolean||
|archiveCode|准考证号|query|false|string||
|commander|推荐人|query|false|string||
|connector|联系单位或联系人|query|false|string||
|ddlPrivilegeClass|特招班|query|false|string||
|finishSchoolCode|毕业学校|query|false|string||
|matEndTime|录取时间|query|false|string(date-time)||
|matriculateStatus|录取状态|query|false|integer(int32)||
|matStartTime|录取时间|query|false|string(date-time)||
|pageNo|pageNo|query|false|integer(int32)||
|pageSize|pageSize|query|false|integer(int32)||
|registeDept|登记部门|query|false|string||
|register|登记人|query|false|string||
|signupSchoolCode|报名学校代码|query|false|string||
|signupSchoolName|报名学校名称|query|false|string||
|studentName|姓名|query|false|string||
|studentType|考生类型|query|false|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«IPage«PrivateRegistList»»|
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|IPage«PrivateRegistList»|IPage«PrivateRegistList»|
|&emsp;&emsp;current||integer(int64)||
|&emsp;&emsp;pages||integer(int64)||
|&emsp;&emsp;records||array|PrivateRegistList|
|&emsp;&emsp;&emsp;&emsp;archiveCode|准考证号|string||
|&emsp;&emsp;&emsp;&emsp;chineseLevel|语文|string||
|&emsp;&emsp;&emsp;&emsp;chymistLevel|化学|string||
|&emsp;&emsp;&emsp;&emsp;combinedScore|组合分|string||
|&emsp;&emsp;&emsp;&emsp;commandType|推荐类型|string||
|&emsp;&emsp;&emsp;&emsp;commander|推荐人|string||
|&emsp;&emsp;&emsp;&emsp;commanderPhone|推荐人电话|string||
|&emsp;&emsp;&emsp;&emsp;connector|联系单位或联系人|string||
|&emsp;&emsp;&emsp;&emsp;diathesis|综合素质|string||
|&emsp;&emsp;&emsp;&emsp;englishLevel|英语|string||
|&emsp;&emsp;&emsp;&emsp;experiment|实验|string||
|&emsp;&emsp;&emsp;&emsp;finishSchoolCode|毕业学校|string||
|&emsp;&emsp;&emsp;&emsp;guardian|监护人|string||
|&emsp;&emsp;&emsp;&emsp;guardianPhone|监护人电话|string||
|&emsp;&emsp;&emsp;&emsp;mathLevel|数学|string||
|&emsp;&emsp;&emsp;&emsp;matriculateStatus|录取状态|integer||
|&emsp;&emsp;&emsp;&emsp;matriculateTime|录取时间|string||
|&emsp;&emsp;&emsp;&emsp;matriculateType|录取类型|string||
|&emsp;&emsp;&emsp;&emsp;physicalEduLevel|体育|string||
|&emsp;&emsp;&emsp;&emsp;physicsLevel|物理|string||
|&emsp;&emsp;&emsp;&emsp;politicsLevel|政史|string||
|&emsp;&emsp;&emsp;&emsp;postCode|邮政编码|string||
|&emsp;&emsp;&emsp;&emsp;premat|预处理标志|integer||
|&emsp;&emsp;&emsp;&emsp;registTime|登记时间|string||
|&emsp;&emsp;&emsp;&emsp;registeDept|登记部门|string||
|&emsp;&emsp;&emsp;&emsp;register|登记人|string||
|&emsp;&emsp;&emsp;&emsp;remark|说明|string||
|&emsp;&emsp;&emsp;&emsp;serialNum|序号|integer||
|&emsp;&emsp;&emsp;&emsp;setType|分类|string||
|&emsp;&emsp;&emsp;&emsp;sex|性别|string||
|&emsp;&emsp;&emsp;&emsp;signupSchoolCode|报名学校|string||
|&emsp;&emsp;&emsp;&emsp;studentName|姓名|string||
|&emsp;&emsp;&emsp;&emsp;studentType|学生类型|string||
|&emsp;&emsp;&emsp;&emsp;sumScore|总分|string||
|&emsp;&emsp;size||integer(int64)||
|&emsp;&emsp;total||integer(int64)||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": {
		"current": 0,
		"pages": 0,
		"records": [
			{
				"archiveCode": "",
				"chineseLevel": "",
				"chymistLevel": "",
				"combinedScore": "",
				"commandType": "",
				"commander": "",
				"commanderPhone": "",
				"connector": "",
				"diathesis": "",
				"englishLevel": "",
				"experiment": "",
				"finishSchoolCode": "",
				"guardian": "",
				"guardianPhone": "",
				"mathLevel": "",
				"matriculateStatus": 0,
				"matriculateTime": "",
				"matriculateType": "",
				"physicalEduLevel": "",
				"physicsLevel": "",
				"politicsLevel": "",
				"postCode": "",
				"premat": 0,
				"registTime": "",
				"registeDept": "",
				"register": "",
				"remark": "",
				"serialNum": 0,
				"setType": "",
				"sex": "",
				"signupSchoolCode": "",
				"studentName": "",
				"studentType": "",
				"sumScore": ""
			}
		],
		"size": 0,
		"total": 0
	},
	"success": true,
	"timestamp": 0
}
```


## 内部录取-招办端内部录取(取消录取)


**接口地址**:`/nnzk/sign/privateRegiste/undoPrivateMatri`


**请求方式**:`PUT`


**请求数据类型**:`application/json`


**响应数据类型**:`*/*`


**接口描述**:<p>内部录取-内部录取(取消录取)</p>



**请求示例**:


```javascript
{
  "archiveCodes": []
}
```


**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|input|input|body|true|ArchiveCodesDTO|ArchiveCodesDTO|
|&emsp;&emsp;archiveCodes|||false|array|string|


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«string»|
|201|Created||
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|string||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": "",
	"success": true,
	"timestamp": 0
}
```


# 准考证号变更表


## 准考证号变更表-添加


**接口地址**:`/nnzk/base/changedArchiveCode/add`


**请求方式**:`POST`


**请求数据类型**:`application/json`


**响应数据类型**:`*/*`


**接口描述**:<p>准考证号变更表-添加</p>



**请求示例**:


```javascript
{
  "createBy": "",
  "createTime": "",
  "delFlag": 0,
  "id": "",
  "newArchiveCode": "",
  "oldArchiveCode": "",
  "updateBy": "",
  "updateTime": "",
  "writeTime": ""
}
```


**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|changedArchiveCode|准考证号变更表|body|true|changed_archive_code对象|changed_archive_code对象|
|&emsp;&emsp;createBy|创建人||false|string||
|&emsp;&emsp;createTime|创建日期||false|string(date-time)||
|&emsp;&emsp;delFlag|删除标识||false|integer(int32)||
|&emsp;&emsp;id|主键||false|string||
|&emsp;&emsp;newArchiveCode|新准考证号||false|string||
|&emsp;&emsp;oldArchiveCode|旧准考证号||false|string||
|&emsp;&emsp;updateBy|更新人||false|string||
|&emsp;&emsp;updateTime|更新日期||false|string(date-time)||
|&emsp;&emsp;writeTime|操作时间||false|string(date-time)||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«string»|
|201|Created||
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|string||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": "",
	"success": true,
	"timestamp": 0
}
```


## 准考证号变更表-通过id删除


**接口地址**:`/nnzk/base/changedArchiveCode/delete`


**请求方式**:`DELETE`


**请求数据类型**:`application/x-www-form-urlencoded`


**响应数据类型**:`*/*`


**接口描述**:<p>准考证号变更表-通过id删除</p>



**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|id|id|query|true|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«string»|
|204|No Content||
|401|Unauthorized||
|403|Forbidden||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|string||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": "",
	"success": true,
	"timestamp": 0
}
```


## 准考证号变更表-批量删除


**接口地址**:`/nnzk/base/changedArchiveCode/deleteBatch`


**请求方式**:`DELETE`


**请求数据类型**:`application/x-www-form-urlencoded`


**响应数据类型**:`*/*`


**接口描述**:<p>准考证号变更表-批量删除</p>



**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|ids|ids|query|true|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«string»|
|204|No Content||
|401|Unauthorized||
|403|Forbidden||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|string||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": "",
	"success": true,
	"timestamp": 0
}
```


## 准考证号变更表-编辑


**接口地址**:`/nnzk/base/changedArchiveCode/edit`


**请求方式**:`POST`


**请求数据类型**:`application/json`


**响应数据类型**:`*/*`


**接口描述**:<p>准考证号变更表-编辑</p>



**请求示例**:


```javascript
{
  "createBy": "",
  "createTime": "",
  "delFlag": 0,
  "id": "",
  "newArchiveCode": "",
  "oldArchiveCode": "",
  "updateBy": "",
  "updateTime": "",
  "writeTime": ""
}
```


**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|changedArchiveCode|准考证号变更表|body|true|changed_archive_code对象|changed_archive_code对象|
|&emsp;&emsp;createBy|创建人||false|string||
|&emsp;&emsp;createTime|创建日期||false|string(date-time)||
|&emsp;&emsp;delFlag|删除标识||false|integer(int32)||
|&emsp;&emsp;id|主键||false|string||
|&emsp;&emsp;newArchiveCode|新准考证号||false|string||
|&emsp;&emsp;oldArchiveCode|旧准考证号||false|string||
|&emsp;&emsp;updateBy|更新人||false|string||
|&emsp;&emsp;updateTime|更新日期||false|string(date-time)||
|&emsp;&emsp;writeTime|操作时间||false|string(date-time)||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«string»|
|201|Created||
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|string||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": "",
	"success": true,
	"timestamp": 0
}
```


## 准考证号变更表-编辑


**接口地址**:`/nnzk/base/changedArchiveCode/edit`


**请求方式**:`PUT`


**请求数据类型**:`application/json`


**响应数据类型**:`*/*`


**接口描述**:<p>准考证号变更表-编辑</p>



**请求示例**:


```javascript
{
  "createBy": "",
  "createTime": "",
  "delFlag": 0,
  "id": "",
  "newArchiveCode": "",
  "oldArchiveCode": "",
  "updateBy": "",
  "updateTime": "",
  "writeTime": ""
}
```


**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|changedArchiveCode|准考证号变更表|body|true|changed_archive_code对象|changed_archive_code对象|
|&emsp;&emsp;createBy|创建人||false|string||
|&emsp;&emsp;createTime|创建日期||false|string(date-time)||
|&emsp;&emsp;delFlag|删除标识||false|integer(int32)||
|&emsp;&emsp;id|主键||false|string||
|&emsp;&emsp;newArchiveCode|新准考证号||false|string||
|&emsp;&emsp;oldArchiveCode|旧准考证号||false|string||
|&emsp;&emsp;updateBy|更新人||false|string||
|&emsp;&emsp;updateTime|更新日期||false|string(date-time)||
|&emsp;&emsp;writeTime|操作时间||false|string(date-time)||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«string»|
|201|Created||
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|string||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": "",
	"success": true,
	"timestamp": 0
}
```


## 准考证号变更表-分页列表查询


**接口地址**:`/nnzk/base/changedArchiveCode/list`


**请求方式**:`GET`


**请求数据类型**:`application/x-www-form-urlencoded`


**响应数据类型**:`*/*`


**接口描述**:<p>准考证号变更表-分页列表查询</p>



**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|createBy|创建人|query|false|string||
|createTime|创建日期|query|false|string(date-time)||
|delFlag|删除标识|query|false|integer(int32)||
|id|主键|query|false|string||
|newArchiveCode|新准考证号|query|false|string||
|oldArchiveCode|旧准考证号|query|false|string||
|pageNo|pageNo|query|false|integer(int32)||
|pageSize|pageSize|query|false|integer(int32)||
|updateBy|更新人|query|false|string||
|updateTime|更新日期|query|false|string(date-time)||
|writeTime|操作时间|query|false|string(date-time)||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«IPage«changed_archive_code对象»»|
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|IPage«changed_archive_code对象»|IPage«changed_archive_code对象»|
|&emsp;&emsp;current||integer(int64)||
|&emsp;&emsp;pages||integer(int64)||
|&emsp;&emsp;records||array|changed_archive_code对象|
|&emsp;&emsp;&emsp;&emsp;createBy|创建人|string||
|&emsp;&emsp;&emsp;&emsp;createTime|创建日期|string||
|&emsp;&emsp;&emsp;&emsp;delFlag|删除标识|integer||
|&emsp;&emsp;&emsp;&emsp;id|主键|string||
|&emsp;&emsp;&emsp;&emsp;newArchiveCode|新准考证号|string||
|&emsp;&emsp;&emsp;&emsp;oldArchiveCode|旧准考证号|string||
|&emsp;&emsp;&emsp;&emsp;updateBy|更新人|string||
|&emsp;&emsp;&emsp;&emsp;updateTime|更新日期|string||
|&emsp;&emsp;&emsp;&emsp;writeTime|操作时间|string||
|&emsp;&emsp;size||integer(int64)||
|&emsp;&emsp;total||integer(int64)||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": {
		"current": 0,
		"pages": 0,
		"records": [
			{
				"createBy": "",
				"createTime": "",
				"delFlag": 0,
				"id": "",
				"newArchiveCode": "",
				"oldArchiveCode": "",
				"updateBy": "",
				"updateTime": "",
				"writeTime": ""
			}
		],
		"size": 0,
		"total": 0
	},
	"success": true,
	"timestamp": 0
}
```


## 准考证号变更表-通过id查询


**接口地址**:`/nnzk/base/changedArchiveCode/queryById`


**请求方式**:`GET`


**请求数据类型**:`application/x-www-form-urlencoded`


**响应数据类型**:`*/*`


**接口描述**:<p>准考证号变更表-通过id查询</p>



**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|id|id|query|true|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«changed_archive_code对象»|
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|changed_archive_code对象|changed_archive_code对象|
|&emsp;&emsp;createBy|创建人|string||
|&emsp;&emsp;createTime|创建日期|string(date-time)||
|&emsp;&emsp;delFlag|删除标识|integer(int32)||
|&emsp;&emsp;id|主键|string||
|&emsp;&emsp;newArchiveCode|新准考证号|string||
|&emsp;&emsp;oldArchiveCode|旧准考证号|string||
|&emsp;&emsp;updateBy|更新人|string||
|&emsp;&emsp;updateTime|更新日期|string(date-time)||
|&emsp;&emsp;writeTime|操作时间|string(date-time)||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": {
		"createBy": "",
		"createTime": "",
		"delFlag": 0,
		"id": "",
		"newArchiveCode": "",
		"oldArchiveCode": "",
		"updateBy": "",
		"updateTime": "",
		"writeTime": ""
	},
	"success": true,
	"timestamp": 0
}
```


# 分组表


## 分组表-添加


**接口地址**:`/nnzk/school/groupBase/add`


**请求方式**:`POST`


**请求数据类型**:`application/json`


**响应数据类型**:`*/*`


**接口描述**:<p>分组表-添加</p>



**请求示例**:


```javascript
{
  "areaCode": "",
  "groupCode": "",
  "groupName": "",
  "groupType": "",
  "id": "",
  "schoolCodeList": [],
  "schoolGroupList": [
    {
      "createBy": "",
      "createTime": "",
      "delFlag": 0,
      "groupCode": "",
      "id": "",
      "schoolCode": "",
      "updateBy": "",
      "updateTime": ""
    }
  ]
}
```


**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|groupBasePageVO|分组表|body|true|group_basePage对象|group_basePage对象|
|&emsp;&emsp;areaCode|所属县区||false|string||
|&emsp;&emsp;groupCode|分组编码||false|string||
|&emsp;&emsp;groupName|分组名称||false|string||
|&emsp;&emsp;groupType|分组类型(初中组、高中组)||false|string||
|&emsp;&emsp;id|主键||false|string||
|&emsp;&emsp;schoolCodeList|学校代码表||false|array|string|
|&emsp;&emsp;schoolGroupList|学校分组表||false|array|school_group对象|
|&emsp;&emsp;&emsp;&emsp;createBy|创建人||false|string||
|&emsp;&emsp;&emsp;&emsp;createTime|创建日期||false|string||
|&emsp;&emsp;&emsp;&emsp;delFlag|删除标识||false|integer||
|&emsp;&emsp;&emsp;&emsp;groupCode|分组编码||false|string||
|&emsp;&emsp;&emsp;&emsp;id|主键||false|string||
|&emsp;&emsp;&emsp;&emsp;schoolCode|学校代码||false|string||
|&emsp;&emsp;&emsp;&emsp;updateBy|更新人||false|string||
|&emsp;&emsp;&emsp;&emsp;updateTime|更新日期||false|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«string»|
|201|Created||
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|string||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": "",
	"success": true,
	"timestamp": 0
}
```


## 分组表-通过id删除


**接口地址**:`/nnzk/school/groupBase/delete`


**请求方式**:`DELETE`


**请求数据类型**:`application/x-www-form-urlencoded`


**响应数据类型**:`*/*`


**接口描述**:<p>分组表-通过id删除</p>



**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|id|id|query|true|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«string»|
|204|No Content||
|401|Unauthorized||
|403|Forbidden||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|string||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": "",
	"success": true,
	"timestamp": 0
}
```


## 分组表-批量删除


**接口地址**:`/nnzk/school/groupBase/deleteBatch`


**请求方式**:`DELETE`


**请求数据类型**:`application/x-www-form-urlencoded`


**响应数据类型**:`*/*`


**接口描述**:<p>分组表-批量删除</p>



**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|ids|ids|query|true|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«string»|
|204|No Content||
|401|Unauthorized||
|403|Forbidden||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|string||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": "",
	"success": true,
	"timestamp": 0
}
```


## 分组表-编辑


**接口地址**:`/nnzk/school/groupBase/edit`


**请求方式**:`POST`


**请求数据类型**:`application/json`


**响应数据类型**:`*/*`


**接口描述**:<p>分组表-编辑</p>



**请求示例**:


```javascript
{
  "areaCode": "",
  "groupCode": "",
  "groupName": "",
  "groupType": "",
  "id": "",
  "schoolCodeList": [],
  "schoolGroupList": [
    {
      "createBy": "",
      "createTime": "",
      "delFlag": 0,
      "groupCode": "",
      "id": "",
      "schoolCode": "",
      "updateBy": "",
      "updateTime": ""
    }
  ]
}
```


**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|groupBasePageVO|分组表|body|true|group_basePage对象|group_basePage对象|
|&emsp;&emsp;areaCode|所属县区||false|string||
|&emsp;&emsp;groupCode|分组编码||false|string||
|&emsp;&emsp;groupName|分组名称||false|string||
|&emsp;&emsp;groupType|分组类型(初中组、高中组)||false|string||
|&emsp;&emsp;id|主键||false|string||
|&emsp;&emsp;schoolCodeList|学校代码表||false|array|string|
|&emsp;&emsp;schoolGroupList|学校分组表||false|array|school_group对象|
|&emsp;&emsp;&emsp;&emsp;createBy|创建人||false|string||
|&emsp;&emsp;&emsp;&emsp;createTime|创建日期||false|string||
|&emsp;&emsp;&emsp;&emsp;delFlag|删除标识||false|integer||
|&emsp;&emsp;&emsp;&emsp;groupCode|分组编码||false|string||
|&emsp;&emsp;&emsp;&emsp;id|主键||false|string||
|&emsp;&emsp;&emsp;&emsp;schoolCode|学校代码||false|string||
|&emsp;&emsp;&emsp;&emsp;updateBy|更新人||false|string||
|&emsp;&emsp;&emsp;&emsp;updateTime|更新日期||false|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«string»|
|201|Created||
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|string||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": "",
	"success": true,
	"timestamp": 0
}
```


## 分组表-编辑


**接口地址**:`/nnzk/school/groupBase/edit`


**请求方式**:`PUT`


**请求数据类型**:`application/json`


**响应数据类型**:`*/*`


**接口描述**:<p>分组表-编辑</p>



**请求示例**:


```javascript
{
  "areaCode": "",
  "groupCode": "",
  "groupName": "",
  "groupType": "",
  "id": "",
  "schoolCodeList": [],
  "schoolGroupList": [
    {
      "createBy": "",
      "createTime": "",
      "delFlag": 0,
      "groupCode": "",
      "id": "",
      "schoolCode": "",
      "updateBy": "",
      "updateTime": ""
    }
  ]
}
```


**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|groupBasePageVO|分组表|body|true|group_basePage对象|group_basePage对象|
|&emsp;&emsp;areaCode|所属县区||false|string||
|&emsp;&emsp;groupCode|分组编码||false|string||
|&emsp;&emsp;groupName|分组名称||false|string||
|&emsp;&emsp;groupType|分组类型(初中组、高中组)||false|string||
|&emsp;&emsp;id|主键||false|string||
|&emsp;&emsp;schoolCodeList|学校代码表||false|array|string|
|&emsp;&emsp;schoolGroupList|学校分组表||false|array|school_group对象|
|&emsp;&emsp;&emsp;&emsp;createBy|创建人||false|string||
|&emsp;&emsp;&emsp;&emsp;createTime|创建日期||false|string||
|&emsp;&emsp;&emsp;&emsp;delFlag|删除标识||false|integer||
|&emsp;&emsp;&emsp;&emsp;groupCode|分组编码||false|string||
|&emsp;&emsp;&emsp;&emsp;id|主键||false|string||
|&emsp;&emsp;&emsp;&emsp;schoolCode|学校代码||false|string||
|&emsp;&emsp;&emsp;&emsp;updateBy|更新人||false|string||
|&emsp;&emsp;&emsp;&emsp;updateTime|更新日期||false|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«string»|
|201|Created||
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|string||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": "",
	"success": true,
	"timestamp": 0
}
```


## 分组表-通过毕业学校代码获取对应的初中分组


**接口地址**:`/nnzk/school/groupBase/getmGroupByFinishSchoolCode`


**请求方式**:`GET`


**请求数据类型**:`application/x-www-form-urlencoded`


**响应数据类型**:`*/*`


**接口描述**:<p>分组表-通过毕业学校代码获取对应的初中分组</p>



**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|finishSchoolCode|finishSchoolCode|query|true|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«group_base对象»|
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|group_base对象|group_base对象|
|&emsp;&emsp;areaCode|所属县区|string||
|&emsp;&emsp;createBy|创建人|string||
|&emsp;&emsp;createTime|创建日期|string(date-time)||
|&emsp;&emsp;delFlag|删除标识|integer(int32)||
|&emsp;&emsp;groupCode|分组编码|string||
|&emsp;&emsp;groupName|分组名称|string||
|&emsp;&emsp;groupType|分组类型(初中组、高中组)|string||
|&emsp;&emsp;id|主键|string||
|&emsp;&emsp;updateBy|更新人|string||
|&emsp;&emsp;updateTime|更新日期|string(date-time)||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": {
		"areaCode": "",
		"createBy": "",
		"createTime": "",
		"delFlag": 0,
		"groupCode": "",
		"groupName": "",
		"groupType": "",
		"id": "",
		"updateBy": "",
		"updateTime": ""
	},
	"success": true,
	"timestamp": 0
}
```


## 分组表-分页列表查询


**接口地址**:`/nnzk/school/groupBase/list`


**请求方式**:`GET`


**请求数据类型**:`application/x-www-form-urlencoded`


**响应数据类型**:`*/*`


**接口描述**:<p>分组表-分页列表查询</p>



**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|areaCode|所属县区|query|true|string||
|groupCode|分组编码|query|true|string||
|groupName|分组名称|query|true|string||
|groupType|分组类型(初中组、高中组)|query|true|string||
|createBy|创建人|query|false|string||
|createTime|创建日期|query|false|string(date-time)||
|delFlag|删除标识|query|false|integer(int32)||
|id|主键|query|false|string||
|pageNo|pageNo|query|false|integer(int32)||
|pageSize|pageSize|query|false|integer(int32)||
|updateBy|更新人|query|false|string||
|updateTime|更新日期|query|false|string(date-time)||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«IPage«group_base对象»»|
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|IPage«group_base对象»|IPage«group_base对象»|
|&emsp;&emsp;current||integer(int64)||
|&emsp;&emsp;pages||integer(int64)||
|&emsp;&emsp;records||array|group_base对象|
|&emsp;&emsp;&emsp;&emsp;areaCode|所属县区|string||
|&emsp;&emsp;&emsp;&emsp;createBy|创建人|string||
|&emsp;&emsp;&emsp;&emsp;createTime|创建日期|string||
|&emsp;&emsp;&emsp;&emsp;delFlag|删除标识|integer||
|&emsp;&emsp;&emsp;&emsp;groupCode|分组编码|string||
|&emsp;&emsp;&emsp;&emsp;groupName|分组名称|string||
|&emsp;&emsp;&emsp;&emsp;groupType|分组类型(初中组、高中组)|string||
|&emsp;&emsp;&emsp;&emsp;id|主键|string||
|&emsp;&emsp;&emsp;&emsp;updateBy|更新人|string||
|&emsp;&emsp;&emsp;&emsp;updateTime|更新日期|string||
|&emsp;&emsp;size||integer(int64)||
|&emsp;&emsp;total||integer(int64)||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": {
		"current": 0,
		"pages": 0,
		"records": [
			{
				"areaCode": "",
				"createBy": "",
				"createTime": "",
				"delFlag": 0,
				"groupCode": "",
				"groupName": "",
				"groupType": "",
				"id": "",
				"updateBy": "",
				"updateTime": ""
			}
		],
		"size": 0,
		"total": 0
	},
	"success": true,
	"timestamp": 0
}
```


## 分组表-通过分组类型查询


**接口地址**:`/nnzk/school/groupBase/listByGroupType`


**请求方式**:`GET`


**请求数据类型**:`application/x-www-form-urlencoded`


**响应数据类型**:`*/*`


**接口描述**:<p>分组表-通过分组类型查询</p>



**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|groupType|groupType|query|true|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«List«GroupBaseVO»»|
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|array|GroupBaseVO|
|&emsp;&emsp;areaCode|所属县区|string||
|&emsp;&emsp;groupCode|分组编码|string||
|&emsp;&emsp;groupName|分组名称|string||
|&emsp;&emsp;groupType|分组类型(初中组、高中组)|string||
|&emsp;&emsp;id|主键|string||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": [
		{
			"areaCode": "",
			"groupCode": "",
			"groupName": "",
			"groupType": "",
			"id": ""
		}
	],
	"success": true,
	"timestamp": 0
}
```


## 分组表-列表查询


**接口地址**:`/nnzk/school/groupBase/listWithoutPage`


**请求方式**:`GET`


**请求数据类型**:`application/x-www-form-urlencoded`


**响应数据类型**:`*/*`


**接口描述**:<p>分组表-列表查询</p>



**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|areaCode|所属县区|query|true|string||
|groupCode|分组编码|query|true|string||
|groupName|分组名称|query|true|string||
|groupType|分组类型(初中组、高中组)|query|true|string||
|createBy|创建人|query|false|string||
|createTime|创建日期|query|false|string(date-time)||
|delFlag|删除标识|query|false|integer(int32)||
|id|主键|query|false|string||
|updateBy|更新人|query|false|string||
|updateTime|更新日期|query|false|string(date-time)||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«List«group_base对象»»|
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|array|group_base对象|
|&emsp;&emsp;areaCode|所属县区|string||
|&emsp;&emsp;createBy|创建人|string||
|&emsp;&emsp;createTime|创建日期|string(date-time)||
|&emsp;&emsp;delFlag|删除标识|integer(int32)||
|&emsp;&emsp;groupCode|分组编码|string||
|&emsp;&emsp;groupName|分组名称|string||
|&emsp;&emsp;groupType|分组类型(初中组、高中组)|string||
|&emsp;&emsp;id|主键|string||
|&emsp;&emsp;updateBy|更新人|string||
|&emsp;&emsp;updateTime|更新日期|string(date-time)||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": [
		{
			"areaCode": "",
			"createBy": "",
			"createTime": "",
			"delFlag": 0,
			"groupCode": "",
			"groupName": "",
			"groupType": "",
			"id": "",
			"updateBy": "",
			"updateTime": ""
		}
	],
	"success": true,
	"timestamp": 0
}
```


## 分组表-通过id查询


**接口地址**:`/nnzk/school/groupBase/queryById`


**请求方式**:`GET`


**请求数据类型**:`application/x-www-form-urlencoded`


**响应数据类型**:`*/*`


**接口描述**:<p>分组表-通过id查询</p>



**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|id|id|query|true|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«group_base对象»|
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|group_base对象|group_base对象|
|&emsp;&emsp;areaCode|所属县区|string||
|&emsp;&emsp;createBy|创建人|string||
|&emsp;&emsp;createTime|创建日期|string(date-time)||
|&emsp;&emsp;delFlag|删除标识|integer(int32)||
|&emsp;&emsp;groupCode|分组编码|string||
|&emsp;&emsp;groupName|分组名称|string||
|&emsp;&emsp;groupType|分组类型(初中组、高中组)|string||
|&emsp;&emsp;id|主键|string||
|&emsp;&emsp;updateBy|更新人|string||
|&emsp;&emsp;updateTime|更新日期|string(date-time)||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": {
		"areaCode": "",
		"createBy": "",
		"createTime": "",
		"delFlag": 0,
		"groupCode": "",
		"groupName": "",
		"groupType": "",
		"id": "",
		"updateBy": "",
		"updateTime": ""
	},
	"success": true,
	"timestamp": 0
}
```


## 学校分组表-通过主表groupCode查询


**接口地址**:`/nnzk/school/groupBase/querySchoolGroupByMainGroupCode`


**请求方式**:`GET`


**请求数据类型**:`application/x-www-form-urlencoded`


**响应数据类型**:`*/*`


**接口描述**:<p>学校分组表-通过主表groupCode查询</p>



**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|groupCode|groupCode|query|true|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«List«school_group对象»»|
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|array|school_group对象|
|&emsp;&emsp;createBy|创建人|string||
|&emsp;&emsp;createTime|创建日期|string(date-time)||
|&emsp;&emsp;delFlag|删除标识|integer(int32)||
|&emsp;&emsp;groupCode|分组编码|string||
|&emsp;&emsp;id|主键|string||
|&emsp;&emsp;schoolCode|学校代码|string||
|&emsp;&emsp;updateBy|更新人|string||
|&emsp;&emsp;updateTime|更新日期|string(date-time)||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": [
		{
			"createBy": "",
			"createTime": "",
			"delFlag": 0,
			"groupCode": "",
			"id": "",
			"schoolCode": "",
			"updateBy": "",
			"updateTime": ""
		}
	],
	"success": true,
	"timestamp": 0
}
```


## 分组表-通过分组代码获取对应学校


**接口地址**:`/nnzk/school/groupBase/schListByGroupCode`


**请求方式**:`GET`


**请求数据类型**:`application/x-www-form-urlencoded`


**响应数据类型**:`*/*`


**接口描述**:<p>分组表-通过分组代码获取对应学校</p>



**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|groupCode|groupCode|query|true|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«List«SchoolCodeAndNameDTO»»|
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|array|SchoolCodeAndNameDTO|
|&emsp;&emsp;schoolCode|学校代码|string||
|&emsp;&emsp;schoolName|学校名称|string||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": [
		{
			"schoolCode": "",
			"schoolName": ""
		}
	],
	"success": true,
	"timestamp": 0
}
```


# 初中学校表


## 初中学校表-添加


**接口地址**:`/nnzk/school/secondarySchool/add`


**请求方式**:`POST`


**请求数据类型**:`application/json`


**响应数据类型**:`*/*`


**接口描述**:<p>初中学校表-添加</p>



**请求示例**:


```javascript
{
  "areaCode": "",
  "createBy": "",
  "createTime": "",
  "delFlag": 0,
  "dispOrder": 0,
  "id": "",
  "initials": "",
  "keyWord": "",
  "schoolCode": "",
  "schoolName": "",
  "updateBy": "",
  "updateTime": ""
}
```


**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|secondarySchool|初中学校表|body|true|secondary_school|secondary_school|
|&emsp;&emsp;areaCode|所属县区||false|string||
|&emsp;&emsp;createBy|创建人||false|string||
|&emsp;&emsp;createTime|创建日期||false|string(date-time)||
|&emsp;&emsp;delFlag|删除标识||false|integer(int32)||
|&emsp;&emsp;dispOrder|排序码||false|integer(int32)||
|&emsp;&emsp;id|主键||false|string||
|&emsp;&emsp;initials|拼音首字母||false|string||
|&emsp;&emsp;keyWord|学校关键字||false|string||
|&emsp;&emsp;schoolCode|学校代码||false|string||
|&emsp;&emsp;schoolName|学校名称||false|string||
|&emsp;&emsp;updateBy|更新人||false|string||
|&emsp;&emsp;updateTime|更新日期||false|string(date-time)||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«string»|
|201|Created||
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|string||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": "",
	"success": true,
	"timestamp": 0
}
```


## 初中学校表-初中学校列表(不分页)


**接口地址**:`/nnzk/school/secondarySchool/allSecondarySchool`


**请求方式**:`GET`


**请求数据类型**:`application/x-www-form-urlencoded`


**响应数据类型**:`*/*`


**接口描述**:<p>初中学校表-初中学校列表(不分页)</p>



**请求参数**:


暂无


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«List«SecondarySchoolDTO»»|
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|array|SecondarySchoolDTO|
|&emsp;&emsp;areaCode|所属县区|string||
|&emsp;&emsp;dispOrder|排序码|integer(int32)||
|&emsp;&emsp;id|主键|string||
|&emsp;&emsp;initials|拼音首字母|string||
|&emsp;&emsp;keyWord|学校关键字|string||
|&emsp;&emsp;schoolCode|学校代码|string||
|&emsp;&emsp;schoolName|学校名称|string||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": [
		{
			"areaCode": "",
			"dispOrder": 0,
			"id": "",
			"initials": "",
			"keyWord": "",
			"schoolCode": "",
			"schoolName": ""
		}
	],
	"success": true,
	"timestamp": 0
}
```


## 初中学校表-通过id删除


**接口地址**:`/nnzk/school/secondarySchool/delete`


**请求方式**:`DELETE`


**请求数据类型**:`application/x-www-form-urlencoded`


**响应数据类型**:`*/*`


**接口描述**:<p>初中学校表-通过id删除</p>



**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|id|id|query|true|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«string»|
|204|No Content||
|401|Unauthorized||
|403|Forbidden||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|string||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": "",
	"success": true,
	"timestamp": 0
}
```


## 初中学校表-批量删除


**接口地址**:`/nnzk/school/secondarySchool/deleteBatch`


**请求方式**:`DELETE`


**请求数据类型**:`application/x-www-form-urlencoded`


**响应数据类型**:`*/*`


**接口描述**:<p>初中学校表-批量删除</p>



**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|ids|ids|query|true|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«string»|
|204|No Content||
|401|Unauthorized||
|403|Forbidden||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|string||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": "",
	"success": true,
	"timestamp": 0
}
```


## 初中学校表-编辑


**接口地址**:`/nnzk/school/secondarySchool/edit`


**请求方式**:`POST`


**请求数据类型**:`application/json`


**响应数据类型**:`*/*`


**接口描述**:<p>初中学校表-编辑</p>



**请求示例**:


```javascript
{
  "areaCode": "",
  "createBy": "",
  "createTime": "",
  "delFlag": 0,
  "dispOrder": 0,
  "id": "",
  "initials": "",
  "keyWord": "",
  "schoolCode": "",
  "schoolName": "",
  "updateBy": "",
  "updateTime": ""
}
```


**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|secondarySchool|初中学校表|body|true|secondary_school|secondary_school|
|&emsp;&emsp;areaCode|所属县区||false|string||
|&emsp;&emsp;createBy|创建人||false|string||
|&emsp;&emsp;createTime|创建日期||false|string(date-time)||
|&emsp;&emsp;delFlag|删除标识||false|integer(int32)||
|&emsp;&emsp;dispOrder|排序码||false|integer(int32)||
|&emsp;&emsp;id|主键||false|string||
|&emsp;&emsp;initials|拼音首字母||false|string||
|&emsp;&emsp;keyWord|学校关键字||false|string||
|&emsp;&emsp;schoolCode|学校代码||false|string||
|&emsp;&emsp;schoolName|学校名称||false|string||
|&emsp;&emsp;updateBy|更新人||false|string||
|&emsp;&emsp;updateTime|更新日期||false|string(date-time)||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«string»|
|201|Created||
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|string||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": "",
	"success": true,
	"timestamp": 0
}
```


## 初中学校表-编辑


**接口地址**:`/nnzk/school/secondarySchool/edit`


**请求方式**:`PUT`


**请求数据类型**:`application/json`


**响应数据类型**:`*/*`


**接口描述**:<p>初中学校表-编辑</p>



**请求示例**:


```javascript
{
  "areaCode": "",
  "createBy": "",
  "createTime": "",
  "delFlag": 0,
  "dispOrder": 0,
  "id": "",
  "initials": "",
  "keyWord": "",
  "schoolCode": "",
  "schoolName": "",
  "updateBy": "",
  "updateTime": ""
}
```


**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|secondarySchool|初中学校表|body|true|secondary_school|secondary_school|
|&emsp;&emsp;areaCode|所属县区||false|string||
|&emsp;&emsp;createBy|创建人||false|string||
|&emsp;&emsp;createTime|创建日期||false|string(date-time)||
|&emsp;&emsp;delFlag|删除标识||false|integer(int32)||
|&emsp;&emsp;dispOrder|排序码||false|integer(int32)||
|&emsp;&emsp;id|主键||false|string||
|&emsp;&emsp;initials|拼音首字母||false|string||
|&emsp;&emsp;keyWord|学校关键字||false|string||
|&emsp;&emsp;schoolCode|学校代码||false|string||
|&emsp;&emsp;schoolName|学校名称||false|string||
|&emsp;&emsp;updateBy|更新人||false|string||
|&emsp;&emsp;updateTime|更新日期||false|string(date-time)||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«string»|
|201|Created||
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|string||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": "",
	"success": true,
	"timestamp": 0
}
```


## 初中端-未参与过报名考生查询


**接口地址**:`/nnzk/school/secondarySchool/getCzNoSign`


**请求方式**:`GET`


**请求数据类型**:`application/x-www-form-urlencoded`


**响应数据类型**:`*/*`


**接口描述**:<p>初中端-未参与过报名考生查询</p>



**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|archiveCode|准考证号|query|false|string||
|className|班级|query|false|string||
|dateFrom|开始日期|query|false|string(date-time)||
|dateTo|结束日期|query|false|string(date-time)||
|orderBy|排序方式|query|false|array|string|
|pageNo|pageNo|query|false|integer(int32)||
|pageSize|pageSize|query|false|integer(int32)||
|secondarySchoolName|学校名称|query|false|string||
|studentName|学生姓名|query|false|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«IPage«GetCzSignOutputDTO»»|
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|IPage«GetCzSignOutputDTO»|IPage«GetCzSignOutputDTO»|
|&emsp;&emsp;current||integer(int64)||
|&emsp;&emsp;pages||integer(int64)||
|&emsp;&emsp;records||array|GetCzSignOutputDTO|
|&emsp;&emsp;&emsp;&emsp;archiveCode|准考证号|string||
|&emsp;&emsp;&emsp;&emsp;calculateType|入围类型|string||
|&emsp;&emsp;&emsp;&emsp;className|班级|string||
|&emsp;&emsp;&emsp;&emsp;id|id|string||
|&emsp;&emsp;&emsp;&emsp;isAreaStudent|地段生|integer||
|&emsp;&emsp;&emsp;&emsp;matriculateType|录取类型|string||
|&emsp;&emsp;&emsp;&emsp;order|排名|string||
|&emsp;&emsp;&emsp;&emsp;schoolCode|报考学校代码|string||
|&emsp;&emsp;&emsp;&emsp;schoolName|报考学校名称|string||
|&emsp;&emsp;&emsp;&emsp;scoreOrder|成绩排序码|string||
|&emsp;&emsp;&emsp;&emsp;sex|性别|string||
|&emsp;&emsp;&emsp;&emsp;signUpType|报考类型|string||
|&emsp;&emsp;&emsp;&emsp;studentName|学生姓名|string||
|&emsp;&emsp;size||integer(int64)||
|&emsp;&emsp;total||integer(int64)||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": {
		"current": 0,
		"pages": 0,
		"records": [
			{
				"archiveCode": "",
				"calculateType": "",
				"className": "",
				"id": "",
				"isAreaStudent": 0,
				"matriculateType": "",
				"order": "",
				"schoolCode": "",
				"schoolName": "",
				"scoreOrder": "",
				"sex": "",
				"signUpType": "",
				"studentName": ""
			}
		],
		"size": 0,
		"total": 0
	},
	"success": true,
	"timestamp": 0
}
```


## 初中端-填报情况查询


**接口地址**:`/nnzk/school/secondarySchool/getCzSignInfo`


**请求方式**:`GET`


**请求数据类型**:`application/x-www-form-urlencoded`


**响应数据类型**:`*/*`


**接口描述**:<p>初中端-填报情况查询</p>



**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|archiveCode|准考证号|query|false|string||
|className|班级|query|false|string||
|dateFrom|开始日期|query|false|string(date-time)||
|dateTo|结束日期|query|false|string(date-time)||
|orderBy|排序方式|query|false|array|string|
|pageNo|pageNo|query|false|integer(int32)||
|pageSize|pageSize|query|false|integer(int32)||
|secondarySchoolName|学校名称|query|false|string||
|studentName|学生姓名|query|false|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«List«GetCzSignOutputDTO»»|
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|array|GetCzSignOutputDTO|
|&emsp;&emsp;archiveCode|准考证号|string||
|&emsp;&emsp;calculateType|入围类型|string||
|&emsp;&emsp;className|班级|string||
|&emsp;&emsp;id|id|string||
|&emsp;&emsp;isAreaStudent|地段生|integer(int32)||
|&emsp;&emsp;matriculateType|录取类型|string||
|&emsp;&emsp;order|排名|string||
|&emsp;&emsp;schoolCode|报考学校代码|string||
|&emsp;&emsp;schoolName|报考学校名称|string||
|&emsp;&emsp;scoreOrder|成绩排序码|string||
|&emsp;&emsp;sex|性别|string||
|&emsp;&emsp;signUpType|报考类型|string||
|&emsp;&emsp;studentName|学生姓名|string||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": [
		{
			"archiveCode": "",
			"calculateType": "",
			"className": "",
			"id": "",
			"isAreaStudent": 0,
			"matriculateType": "",
			"order": "",
			"schoolCode": "",
			"schoolName": "",
			"scoreOrder": "",
			"sex": "",
			"signUpType": "",
			"studentName": ""
		}
	],
	"success": true,
	"timestamp": 0
}
```


## 初中端-考生查询


**接口地址**:`/nnzk/school/secondarySchool/getCzStuInfo`


**请求方式**:`GET`


**请求数据类型**:`application/x-www-form-urlencoded`


**响应数据类型**:`*/*`


**接口描述**:<p>初中端-考生查询</p>



**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|archiveCode|archiveCode|query|true|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«StuInfoAndScoreVO»|
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|StuInfoAndScoreVO|StuInfoAndScoreVO|
|&emsp;&emsp;archiveCode|准考证号|string||
|&emsp;&emsp;chineseLevel|语文|string||
|&emsp;&emsp;chymistLevel|化学|string||
|&emsp;&emsp;combinedScore|组合分|string||
|&emsp;&emsp;diathesis|综合素质|string||
|&emsp;&emsp;englishLevel|英语|string||
|&emsp;&emsp;experiment|实验|string||
|&emsp;&emsp;mathLevel|数学|string||
|&emsp;&emsp;physicsLevel|物理|string||
|&emsp;&emsp;politicsLevel|政史|string||
|&emsp;&emsp;sex|性别|string||
|&emsp;&emsp;studentName|姓名|string||
|&emsp;&emsp;sumScore|总分|string||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": {
		"archiveCode": "",
		"chineseLevel": "",
		"chymistLevel": "",
		"combinedScore": "",
		"diathesis": "",
		"englishLevel": "",
		"experiment": "",
		"mathLevel": "",
		"physicsLevel": "",
		"politicsLevel": "",
		"sex": "",
		"studentName": "",
		"sumScore": ""
	},
	"success": true,
	"timestamp": 0
}
```


## 初中学校表-获取学校代码和名称


**接口地址**:`/nnzk/school/secondarySchool/getSchoolCodeAndName`


**请求方式**:`GET`


**请求数据类型**:`application/x-www-form-urlencoded`


**响应数据类型**:`*/*`


**接口描述**:<p>初中学校表-获取学校代码和名称</p>



**请求参数**:


暂无


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«SchoolCodeAndNameDTO»|
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|SchoolCodeAndNameDTO|SchoolCodeAndNameDTO|
|&emsp;&emsp;schoolCode|学校代码|string||
|&emsp;&emsp;schoolName|学校名称|string||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": {
		"schoolCode": "",
		"schoolName": ""
	},
	"success": true,
	"timestamp": 0
}
```


## 初中学校表-分页列表查询


**接口地址**:`/nnzk/school/secondarySchool/list`


**请求方式**:`GET`


**请求数据类型**:`application/x-www-form-urlencoded`


**响应数据类型**:`*/*`


**接口描述**:<p>初中学校表-分页列表查询</p>



**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|schoolCode|学校代码|query|true|string||
|areaCode|所属县区|query|false|string||
|createBy|创建人|query|false|string||
|createTime|创建日期|query|false|string(date-time)||
|delFlag|删除标识|query|false|integer(int32)||
|dispOrder|排序码|query|false|integer(int32)||
|id|主键|query|false|string||
|initials|拼音首字母|query|false|string||
|keyWord|学校关键字|query|false|string||
|pageNo|pageNo|query|false|integer(int32)||
|pageSize|pageSize|query|false|integer(int32)||
|schoolName|学校名称|query|false|string||
|updateBy|更新人|query|false|string||
|updateTime|更新日期|query|false|string(date-time)||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«IPage«secondary_school»»|
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|IPage«secondary_school»|IPage«secondary_school»|
|&emsp;&emsp;current||integer(int64)||
|&emsp;&emsp;pages||integer(int64)||
|&emsp;&emsp;records||array|secondary_school|
|&emsp;&emsp;&emsp;&emsp;areaCode|所属县区|string||
|&emsp;&emsp;&emsp;&emsp;createBy|创建人|string||
|&emsp;&emsp;&emsp;&emsp;createTime|创建日期|string||
|&emsp;&emsp;&emsp;&emsp;delFlag|删除标识|integer||
|&emsp;&emsp;&emsp;&emsp;dispOrder|排序码|integer||
|&emsp;&emsp;&emsp;&emsp;id|主键|string||
|&emsp;&emsp;&emsp;&emsp;initials|拼音首字母|string||
|&emsp;&emsp;&emsp;&emsp;keyWord|学校关键字|string||
|&emsp;&emsp;&emsp;&emsp;schoolCode|学校代码|string||
|&emsp;&emsp;&emsp;&emsp;schoolName|学校名称|string||
|&emsp;&emsp;&emsp;&emsp;updateBy|更新人|string||
|&emsp;&emsp;&emsp;&emsp;updateTime|更新日期|string||
|&emsp;&emsp;size||integer(int64)||
|&emsp;&emsp;total||integer(int64)||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": {
		"current": 0,
		"pages": 0,
		"records": [
			{
				"areaCode": "",
				"createBy": "",
				"createTime": "",
				"delFlag": 0,
				"dispOrder": 0,
				"id": "",
				"initials": "",
				"keyWord": "",
				"schoolCode": "",
				"schoolName": "",
				"updateBy": "",
				"updateTime": ""
			}
		],
		"size": 0,
		"total": 0
	},
	"success": true,
	"timestamp": 0
}
```


## 初中学校表-通过id查询


**接口地址**:`/nnzk/school/secondarySchool/queryById`


**请求方式**:`GET`


**请求数据类型**:`application/x-www-form-urlencoded`


**响应数据类型**:`*/*`


**接口描述**:<p>初中学校表-通过id查询</p>



**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|id|id|query|true|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«secondary_school»|
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|secondary_school|secondary_school|
|&emsp;&emsp;areaCode|所属县区|string||
|&emsp;&emsp;createBy|创建人|string||
|&emsp;&emsp;createTime|创建日期|string(date-time)||
|&emsp;&emsp;delFlag|删除标识|integer(int32)||
|&emsp;&emsp;dispOrder|排序码|integer(int32)||
|&emsp;&emsp;id|主键|string||
|&emsp;&emsp;initials|拼音首字母|string||
|&emsp;&emsp;keyWord|学校关键字|string||
|&emsp;&emsp;schoolCode|学校代码|string||
|&emsp;&emsp;schoolName|学校名称|string||
|&emsp;&emsp;updateBy|更新人|string||
|&emsp;&emsp;updateTime|更新日期|string(date-time)||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": {
		"areaCode": "",
		"createBy": "",
		"createTime": "",
		"delFlag": 0,
		"dispOrder": 0,
		"id": "",
		"initials": "",
		"keyWord": "",
		"schoolCode": "",
		"schoolName": "",
		"updateBy": "",
		"updateTime": ""
	},
	"success": true,
	"timestamp": 0
}
```


## 初中端-重置操作员密码


**接口地址**:`/nnzk/school/secondarySchool/resetOperaterAccountPW`


**请求方式**:`POST`


**请求数据类型**:`application/json`


**响应数据类型**:`*/*`


**接口描述**:<p>初中端-重置操作员密码</p>



**请求示例**:


```javascript
{
  "newPassWord": "",
  "realName": "",
  "userName": ""
}
```


**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|input|input|body|true|ResetOpePWDTO|ResetOpePWDTO|
|&emsp;&emsp;newPassWord|新的密码||false|string||
|&emsp;&emsp;realName|姓名||false|string||
|&emsp;&emsp;userName|账号||false|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«string»|
|201|Created||
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|string||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": "",
	"success": true,
	"timestamp": 0
}
```


## 初中端-重置学生密码


**接口地址**:`/nnzk/school/secondarySchool/resetStudentAccountPW`


**请求方式**:`POST`


**请求数据类型**:`application/json`


**响应数据类型**:`*/*`


**接口描述**:<p>初中端-重置学生密码</p>



**请求示例**:


```javascript
{
  "archiveCode": "",
  "newPassWord": "",
  "studentName": ""
}
```


**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|input|input|body|true|ResetStuPWDTO|ResetStuPWDTO|
|&emsp;&emsp;archiveCode|准考证号||false|string||
|&emsp;&emsp;newPassWord|新的密码||false|string||
|&emsp;&emsp;studentName|学生姓名||false|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«string»|
|201|Created||
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|string||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": "",
	"success": true,
	"timestamp": 0
}
```


# 动态数据源测试


## 动态切换数据源


**接口地址**:`/nnzk/test/dynamic/test1`


**请求方式**:`POST`


**请求数据类型**:`application/json`


**响应数据类型**:`*/*`


**接口描述**:<p>动态切换数据源</p>



**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|dsName|dsName|query|false|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«List«测试DEMO对象»»|
|201|Created||
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|array|测试DEMO对象|
|&emsp;&emsp;age|年龄|integer(int32)||
|&emsp;&emsp;birthday|生日|string(date-time)||
|&emsp;&emsp;bonusMoney|奖金|number(double)||
|&emsp;&emsp;content|个人简介|string||
|&emsp;&emsp;createBy|创建人|string||
|&emsp;&emsp;createTime|创建时间|string(date-time)||
|&emsp;&emsp;email|邮箱|string||
|&emsp;&emsp;id|ID|string||
|&emsp;&emsp;keyWord|关键词|string||
|&emsp;&emsp;name|姓名|string||
|&emsp;&emsp;punchTime|打卡时间|string(date-time)||
|&emsp;&emsp;salaryMoney|工资|number||
|&emsp;&emsp;sex|性别|string||
|&emsp;&emsp;sysOrgCode|部门编码|string||
|&emsp;&emsp;tenantId|租户ID|integer(int32)||
|&emsp;&emsp;updateBy|更新人|string||
|&emsp;&emsp;updateCount||integer(int32)||
|&emsp;&emsp;updateTime|更新时间|string(date-time)||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": [
		{
			"age": 0,
			"birthday": "",
			"bonusMoney": 0,
			"content": "",
			"createBy": "",
			"createTime": "",
			"email": "",
			"id": "",
			"keyWord": "",
			"name": "",
			"punchTime": "",
			"salaryMoney": 0,
			"sex": "",
			"sysOrgCode": "",
			"tenantId": 0,
			"updateBy": "",
			"updateCount": 0,
			"updateTime": ""
		}
	],
	"success": true,
	"timestamp": 0
}
```


# 单表DEMO


## 添加DEMO


**接口地址**:`/nnzk/test/jeecgDemo/add`


**请求方式**:`POST`


**请求数据类型**:`application/json`


**响应数据类型**:`*/*`


**接口描述**:<p>添加DEMO</p>



**请求示例**:


```javascript
{
  "age": 0,
  "birthday": "",
  "bonusMoney": 0,
  "content": "",
  "createBy": "",
  "createTime": "",
  "email": "",
  "id": "",
  "keyWord": "",
  "name": "",
  "punchTime": "",
  "salaryMoney": 0,
  "sex": "",
  "sysOrgCode": "",
  "tenantId": 0,
  "updateBy": "",
  "updateCount": 0,
  "updateTime": ""
}
```


**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|jeecgDemo|测试DEMO|body|true|测试DEMO对象|测试DEMO对象|
|&emsp;&emsp;age|年龄||false|integer(int32)||
|&emsp;&emsp;birthday|生日||false|string(date-time)||
|&emsp;&emsp;bonusMoney|奖金||false|number(double)||
|&emsp;&emsp;content|个人简介||false|string||
|&emsp;&emsp;createBy|创建人||false|string||
|&emsp;&emsp;createTime|创建时间||false|string(date-time)||
|&emsp;&emsp;email|邮箱||false|string||
|&emsp;&emsp;id|ID||false|string||
|&emsp;&emsp;keyWord|关键词||false|string||
|&emsp;&emsp;name|姓名||false|string||
|&emsp;&emsp;punchTime|打卡时间||false|string(date-time)||
|&emsp;&emsp;salaryMoney|工资||false|number||
|&emsp;&emsp;sex|性别||false|string||
|&emsp;&emsp;sysOrgCode|部门编码||false|string||
|&emsp;&emsp;tenantId|租户ID||false|integer(int32)||
|&emsp;&emsp;updateBy|更新人||false|string||
|&emsp;&emsp;updateCount|||false|integer(int32)||
|&emsp;&emsp;updateTime|更新时间||false|string(date-time)||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«object»|
|201|Created||
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|object||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": {},
	"success": true,
	"timestamp": 0
}
```


## 通过ID删除DEMO


**接口地址**:`/nnzk/test/jeecgDemo/delete`


**请求方式**:`DELETE`


**请求数据类型**:`application/x-www-form-urlencoded`


**响应数据类型**:`*/*`


**接口描述**:<p>通过ID删除DEMO</p>



**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|id|id|query|true|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«object»|
|204|No Content||
|401|Unauthorized||
|403|Forbidden||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|object||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": {},
	"success": true,
	"timestamp": 0
}
```


## 批量删除DEMO


**接口地址**:`/nnzk/test/jeecgDemo/deleteBatch`


**请求方式**:`DELETE`


**请求数据类型**:`application/x-www-form-urlencoded`


**响应数据类型**:`*/*`


**接口描述**:<p>批量删除DEMO</p>



**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|ids|ids|query|true|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«object»|
|204|No Content||
|401|Unauthorized||
|403|Forbidden||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|object||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": {},
	"success": true,
	"timestamp": 0
}
```


## 编辑DEMO


**接口地址**:`/nnzk/test/jeecgDemo/edit`


**请求方式**:`POST`


**请求数据类型**:`application/json`


**响应数据类型**:`*/*`


**接口描述**:<p>编辑DEMO</p>



**请求示例**:


```javascript
{
  "age": 0,
  "birthday": "",
  "bonusMoney": 0,
  "content": "",
  "createBy": "",
  "createTime": "",
  "email": "",
  "id": "",
  "keyWord": "",
  "name": "",
  "punchTime": "",
  "salaryMoney": 0,
  "sex": "",
  "sysOrgCode": "",
  "tenantId": 0,
  "updateBy": "",
  "updateCount": 0,
  "updateTime": ""
}
```


**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|jeecgDemo|测试DEMO|body|true|测试DEMO对象|测试DEMO对象|
|&emsp;&emsp;age|年龄||false|integer(int32)||
|&emsp;&emsp;birthday|生日||false|string(date-time)||
|&emsp;&emsp;bonusMoney|奖金||false|number(double)||
|&emsp;&emsp;content|个人简介||false|string||
|&emsp;&emsp;createBy|创建人||false|string||
|&emsp;&emsp;createTime|创建时间||false|string(date-time)||
|&emsp;&emsp;email|邮箱||false|string||
|&emsp;&emsp;id|ID||false|string||
|&emsp;&emsp;keyWord|关键词||false|string||
|&emsp;&emsp;name|姓名||false|string||
|&emsp;&emsp;punchTime|打卡时间||false|string(date-time)||
|&emsp;&emsp;salaryMoney|工资||false|number||
|&emsp;&emsp;sex|性别||false|string||
|&emsp;&emsp;sysOrgCode|部门编码||false|string||
|&emsp;&emsp;tenantId|租户ID||false|integer(int32)||
|&emsp;&emsp;updateBy|更新人||false|string||
|&emsp;&emsp;updateCount|||false|integer(int32)||
|&emsp;&emsp;updateTime|更新时间||false|string(date-time)||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«object»|
|201|Created||
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|object||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": {},
	"success": true,
	"timestamp": 0
}
```


## 编辑DEMO


**接口地址**:`/nnzk/test/jeecgDemo/edit`


**请求方式**:`PUT`


**请求数据类型**:`application/json`


**响应数据类型**:`*/*`


**接口描述**:<p>编辑DEMO</p>



**请求示例**:


```javascript
{
  "age": 0,
  "birthday": "",
  "bonusMoney": 0,
  "content": "",
  "createBy": "",
  "createTime": "",
  "email": "",
  "id": "",
  "keyWord": "",
  "name": "",
  "punchTime": "",
  "salaryMoney": 0,
  "sex": "",
  "sysOrgCode": "",
  "tenantId": 0,
  "updateBy": "",
  "updateCount": 0,
  "updateTime": ""
}
```


**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|jeecgDemo|测试DEMO|body|true|测试DEMO对象|测试DEMO对象|
|&emsp;&emsp;age|年龄||false|integer(int32)||
|&emsp;&emsp;birthday|生日||false|string(date-time)||
|&emsp;&emsp;bonusMoney|奖金||false|number(double)||
|&emsp;&emsp;content|个人简介||false|string||
|&emsp;&emsp;createBy|创建人||false|string||
|&emsp;&emsp;createTime|创建时间||false|string(date-time)||
|&emsp;&emsp;email|邮箱||false|string||
|&emsp;&emsp;id|ID||false|string||
|&emsp;&emsp;keyWord|关键词||false|string||
|&emsp;&emsp;name|姓名||false|string||
|&emsp;&emsp;punchTime|打卡时间||false|string(date-time)||
|&emsp;&emsp;salaryMoney|工资||false|number||
|&emsp;&emsp;sex|性别||false|string||
|&emsp;&emsp;sysOrgCode|部门编码||false|string||
|&emsp;&emsp;tenantId|租户ID||false|integer(int32)||
|&emsp;&emsp;updateBy|更新人||false|string||
|&emsp;&emsp;updateCount|||false|integer(int32)||
|&emsp;&emsp;updateTime|更新时间||false|string(date-time)||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«object»|
|201|Created||
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|object||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": {},
	"success": true,
	"timestamp": 0
}
```


## 获取Demo数据列表


**接口地址**:`/nnzk/test/jeecgDemo/list`


**请求方式**:`GET`


**请求数据类型**:`application/x-www-form-urlencoded`


**响应数据类型**:`*/*`


**接口描述**:<p>获取所有Demo数据列表</p>



**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|age|年龄|query|false|integer(int32)||
|birthday|生日|query|false|string(date-time)||
|bonusMoney|奖金|query|false|number(double)||
|content|个人简介|query|false|string||
|createBy|创建人|query|false|string||
|createTime|创建时间|query|false|string(date-time)||
|email|邮箱|query|false|string||
|id|ID|query|false|string||
|keyWord|关键词|query|false|string||
|name|姓名|query|false|string||
|pageNo|pageNo|query|false|integer(int32)||
|pageSize|pageSize|query|false|integer(int32)||
|punchTime|打卡时间|query|false|string(date-time)||
|salaryMoney|工资|query|false|number||
|sex|性别|query|false|string||
|sysOrgCode|部门编码|query|false|string||
|tenantId|租户ID|query|false|integer(int32)||
|updateBy|更新人|query|false|string||
|updateCount||query|false|integer(int32)||
|updateTime|更新时间|query|false|string(date-time)||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«object»|
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|object||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": {},
	"success": true,
	"timestamp": 0
}
```


## 通过ID查询DEMO


**接口地址**:`/nnzk/test/jeecgDemo/queryById`


**请求方式**:`GET`


**请求数据类型**:`application/x-www-form-urlencoded`


**响应数据类型**:`*/*`


**接口描述**:<p>通过ID查询DEMO</p>



**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|id|示例id|query|true|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«object»|
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|object||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": {},
	"success": true,
	"timestamp": 0
}
```


## Mono测试


**接口地址**:`/nnzk/test/jeecgDemo/test`


**请求方式**:`GET`


**请求数据类型**:`application/x-www-form-urlencoded`


**响应数据类型**:`*/*`


**接口描述**:


**请求参数**:


暂无


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|Mono«string»|
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


暂无


**响应示例**:
```javascript
null
```


# 县份学生表


## 县份学生表-添加


**接口地址**:`/nnzk/student/outStudentInfo/add`


**请求方式**:`POST`


**请求数据类型**:`application/json`


**响应数据类型**:`*/*`


**接口描述**:<p>县份学生表-添加</p>



**请求示例**:


```javascript
{
  "address": "",
  "archiveCode": "",
  "birth": "",
  "chineseLevel": "",
  "chymistLevel": "",
  "className": "",
  "combinedScore": "",
  "createBy": "",
  "createTime": "",
  "delFlag": 0,
  "diathesis": "",
  "englishLevel": "",
  "experiment": "",
  "finishSchoolCode": "",
  "finishSchoolName": "",
  "graduateDate": "",
  "highSchoolCode": "",
  "homePlace": "",
  "id": "",
  "identityCode": "",
  "mathLevel": "",
  "matriculateStatus": "",
  "nationCode": "",
  "phonecode": "",
  "physicalEduLevel": "",
  "physicsLevel": "",
  "politicsLevel": "",
  "polity": "",
  "postCode": "",
  "priseHistory": "",
  "sex": "",
  "studentKind": "",
  "studentName": "",
  "sumScore": "",
  "updateBy": "",
  "updateTime": ""
}
```


**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|outStudentInfo|县份学生表|body|true|out_student_info对象|out_student_info对象|
|&emsp;&emsp;address|现住地址||false|string||
|&emsp;&emsp;archiveCode|准考证号||false|string||
|&emsp;&emsp;birth|出生年月||false|string(date-time)||
|&emsp;&emsp;chineseLevel|语文||false|string||
|&emsp;&emsp;chymistLevel|化学||false|string||
|&emsp;&emsp;className|班级||false|string||
|&emsp;&emsp;combinedScore|组合分||false|string||
|&emsp;&emsp;createBy|创建人||false|string||
|&emsp;&emsp;createTime|创建日期||false|string(date-time)||
|&emsp;&emsp;delFlag|删除标识||false|integer(int32)||
|&emsp;&emsp;diathesis|综合素质||false|string||
|&emsp;&emsp;englishLevel|英语||false|string||
|&emsp;&emsp;experiment|实验||false|string||
|&emsp;&emsp;finishSchoolCode|毕业学校代码||false|string||
|&emsp;&emsp;finishSchoolName|毕业学校名称||false|string||
|&emsp;&emsp;graduateDate|毕业时间||false|string(date-time)||
|&emsp;&emsp;highSchoolCode|录取高中||false|string||
|&emsp;&emsp;homePlace|户口地址||false|string||
|&emsp;&emsp;id|主键||false|string||
|&emsp;&emsp;identityCode|身份证号||false|string||
|&emsp;&emsp;mathLevel|数学||false|string||
|&emsp;&emsp;matriculateStatus|是否已录取||false|string||
|&emsp;&emsp;nationCode|民族||false|string||
|&emsp;&emsp;phonecode|电话||false|string||
|&emsp;&emsp;physicalEduLevel|物理实验||false|string||
|&emsp;&emsp;physicsLevel|物理||false|string||
|&emsp;&emsp;politicsLevel|政史||false|string||
|&emsp;&emsp;polity|政治面貌||false|string||
|&emsp;&emsp;postCode|邮政编码||false|string||
|&emsp;&emsp;priseHistory|历史荣誉||false|string||
|&emsp;&emsp;sex|性别||false|string||
|&emsp;&emsp;studentKind|考生类别||false|string||
|&emsp;&emsp;studentName|姓名||false|string||
|&emsp;&emsp;sumScore|总分||false|string||
|&emsp;&emsp;updateBy|更新人||false|string||
|&emsp;&emsp;updateTime|更新日期||false|string(date-time)||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«string»|
|201|Created||
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|string||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": "",
	"success": true,
	"timestamp": 0
}
```


## 县份学生表-通过id删除


**接口地址**:`/nnzk/student/outStudentInfo/delete`


**请求方式**:`DELETE`


**请求数据类型**:`application/x-www-form-urlencoded`


**响应数据类型**:`*/*`


**接口描述**:<p>县份学生表-通过id删除</p>



**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|id|id|query|true|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«string»|
|204|No Content||
|401|Unauthorized||
|403|Forbidden||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|string||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": "",
	"success": true,
	"timestamp": 0
}
```


## 县份学生表-批量删除


**接口地址**:`/nnzk/student/outStudentInfo/deleteBatch`


**请求方式**:`DELETE`


**请求数据类型**:`application/x-www-form-urlencoded`


**响应数据类型**:`*/*`


**接口描述**:<p>县份学生表-批量删除</p>



**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|ids|ids|query|true|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«string»|
|204|No Content||
|401|Unauthorized||
|403|Forbidden||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|string||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": "",
	"success": true,
	"timestamp": 0
}
```


## 县份学生表-编辑


**接口地址**:`/nnzk/student/outStudentInfo/edit`


**请求方式**:`POST`


**请求数据类型**:`application/json`


**响应数据类型**:`*/*`


**接口描述**:<p>县份学生表-编辑</p>



**请求示例**:


```javascript
{
  "address": "",
  "archiveCode": "",
  "birth": "",
  "chineseLevel": "",
  "chymistLevel": "",
  "className": "",
  "combinedScore": "",
  "createBy": "",
  "createTime": "",
  "delFlag": 0,
  "diathesis": "",
  "englishLevel": "",
  "experiment": "",
  "finishSchoolCode": "",
  "finishSchoolName": "",
  "graduateDate": "",
  "highSchoolCode": "",
  "homePlace": "",
  "id": "",
  "identityCode": "",
  "mathLevel": "",
  "matriculateStatus": "",
  "nationCode": "",
  "phonecode": "",
  "physicalEduLevel": "",
  "physicsLevel": "",
  "politicsLevel": "",
  "polity": "",
  "postCode": "",
  "priseHistory": "",
  "sex": "",
  "studentKind": "",
  "studentName": "",
  "sumScore": "",
  "updateBy": "",
  "updateTime": ""
}
```


**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|outStudentInfo|县份学生表|body|true|out_student_info对象|out_student_info对象|
|&emsp;&emsp;address|现住地址||false|string||
|&emsp;&emsp;archiveCode|准考证号||false|string||
|&emsp;&emsp;birth|出生年月||false|string(date-time)||
|&emsp;&emsp;chineseLevel|语文||false|string||
|&emsp;&emsp;chymistLevel|化学||false|string||
|&emsp;&emsp;className|班级||false|string||
|&emsp;&emsp;combinedScore|组合分||false|string||
|&emsp;&emsp;createBy|创建人||false|string||
|&emsp;&emsp;createTime|创建日期||false|string(date-time)||
|&emsp;&emsp;delFlag|删除标识||false|integer(int32)||
|&emsp;&emsp;diathesis|综合素质||false|string||
|&emsp;&emsp;englishLevel|英语||false|string||
|&emsp;&emsp;experiment|实验||false|string||
|&emsp;&emsp;finishSchoolCode|毕业学校代码||false|string||
|&emsp;&emsp;finishSchoolName|毕业学校名称||false|string||
|&emsp;&emsp;graduateDate|毕业时间||false|string(date-time)||
|&emsp;&emsp;highSchoolCode|录取高中||false|string||
|&emsp;&emsp;homePlace|户口地址||false|string||
|&emsp;&emsp;id|主键||false|string||
|&emsp;&emsp;identityCode|身份证号||false|string||
|&emsp;&emsp;mathLevel|数学||false|string||
|&emsp;&emsp;matriculateStatus|是否已录取||false|string||
|&emsp;&emsp;nationCode|民族||false|string||
|&emsp;&emsp;phonecode|电话||false|string||
|&emsp;&emsp;physicalEduLevel|物理实验||false|string||
|&emsp;&emsp;physicsLevel|物理||false|string||
|&emsp;&emsp;politicsLevel|政史||false|string||
|&emsp;&emsp;polity|政治面貌||false|string||
|&emsp;&emsp;postCode|邮政编码||false|string||
|&emsp;&emsp;priseHistory|历史荣誉||false|string||
|&emsp;&emsp;sex|性别||false|string||
|&emsp;&emsp;studentKind|考生类别||false|string||
|&emsp;&emsp;studentName|姓名||false|string||
|&emsp;&emsp;sumScore|总分||false|string||
|&emsp;&emsp;updateBy|更新人||false|string||
|&emsp;&emsp;updateTime|更新日期||false|string(date-time)||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«string»|
|201|Created||
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|string||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": "",
	"success": true,
	"timestamp": 0
}
```


## 县份学生表-编辑


**接口地址**:`/nnzk/student/outStudentInfo/edit`


**请求方式**:`PUT`


**请求数据类型**:`application/json`


**响应数据类型**:`*/*`


**接口描述**:<p>县份学生表-编辑</p>



**请求示例**:


```javascript
{
  "address": "",
  "archiveCode": "",
  "birth": "",
  "chineseLevel": "",
  "chymistLevel": "",
  "className": "",
  "combinedScore": "",
  "createBy": "",
  "createTime": "",
  "delFlag": 0,
  "diathesis": "",
  "englishLevel": "",
  "experiment": "",
  "finishSchoolCode": "",
  "finishSchoolName": "",
  "graduateDate": "",
  "highSchoolCode": "",
  "homePlace": "",
  "id": "",
  "identityCode": "",
  "mathLevel": "",
  "matriculateStatus": "",
  "nationCode": "",
  "phonecode": "",
  "physicalEduLevel": "",
  "physicsLevel": "",
  "politicsLevel": "",
  "polity": "",
  "postCode": "",
  "priseHistory": "",
  "sex": "",
  "studentKind": "",
  "studentName": "",
  "sumScore": "",
  "updateBy": "",
  "updateTime": ""
}
```


**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|outStudentInfo|县份学生表|body|true|out_student_info对象|out_student_info对象|
|&emsp;&emsp;address|现住地址||false|string||
|&emsp;&emsp;archiveCode|准考证号||false|string||
|&emsp;&emsp;birth|出生年月||false|string(date-time)||
|&emsp;&emsp;chineseLevel|语文||false|string||
|&emsp;&emsp;chymistLevel|化学||false|string||
|&emsp;&emsp;className|班级||false|string||
|&emsp;&emsp;combinedScore|组合分||false|string||
|&emsp;&emsp;createBy|创建人||false|string||
|&emsp;&emsp;createTime|创建日期||false|string(date-time)||
|&emsp;&emsp;delFlag|删除标识||false|integer(int32)||
|&emsp;&emsp;diathesis|综合素质||false|string||
|&emsp;&emsp;englishLevel|英语||false|string||
|&emsp;&emsp;experiment|实验||false|string||
|&emsp;&emsp;finishSchoolCode|毕业学校代码||false|string||
|&emsp;&emsp;finishSchoolName|毕业学校名称||false|string||
|&emsp;&emsp;graduateDate|毕业时间||false|string(date-time)||
|&emsp;&emsp;highSchoolCode|录取高中||false|string||
|&emsp;&emsp;homePlace|户口地址||false|string||
|&emsp;&emsp;id|主键||false|string||
|&emsp;&emsp;identityCode|身份证号||false|string||
|&emsp;&emsp;mathLevel|数学||false|string||
|&emsp;&emsp;matriculateStatus|是否已录取||false|string||
|&emsp;&emsp;nationCode|民族||false|string||
|&emsp;&emsp;phonecode|电话||false|string||
|&emsp;&emsp;physicalEduLevel|物理实验||false|string||
|&emsp;&emsp;physicsLevel|物理||false|string||
|&emsp;&emsp;politicsLevel|政史||false|string||
|&emsp;&emsp;polity|政治面貌||false|string||
|&emsp;&emsp;postCode|邮政编码||false|string||
|&emsp;&emsp;priseHistory|历史荣誉||false|string||
|&emsp;&emsp;sex|性别||false|string||
|&emsp;&emsp;studentKind|考生类别||false|string||
|&emsp;&emsp;studentName|姓名||false|string||
|&emsp;&emsp;sumScore|总分||false|string||
|&emsp;&emsp;updateBy|更新人||false|string||
|&emsp;&emsp;updateTime|更新日期||false|string(date-time)||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«string»|
|201|Created||
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|string||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": "",
	"success": true,
	"timestamp": 0
}
```


## 县份学生表-分页列表查询


**接口地址**:`/nnzk/student/outStudentInfo/list`


**请求方式**:`GET`


**请求数据类型**:`application/x-www-form-urlencoded`


**响应数据类型**:`*/*`


**接口描述**:<p>县份学生表-分页列表查询</p>



**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|archiveCode|准考证号|query|true|string||
|address|现住地址|query|false|string||
|birth|出生年月|query|false|string(date-time)||
|chineseLevel|语文|query|false|string||
|chymistLevel|化学|query|false|string||
|className|班级|query|false|string||
|combinedScore|组合分|query|false|string||
|createBy|创建人|query|false|string||
|createTime|创建日期|query|false|string(date-time)||
|delFlag|删除标识|query|false|integer(int32)||
|diathesis|综合素质|query|false|string||
|englishLevel|英语|query|false|string||
|experiment|实验|query|false|string||
|finishSchoolCode|毕业学校代码|query|false|string||
|finishSchoolName|毕业学校名称|query|false|string||
|graduateDate|毕业时间|query|false|string(date-time)||
|highSchoolCode|录取高中|query|false|string||
|homePlace|户口地址|query|false|string||
|id|主键|query|false|string||
|identityCode|身份证号|query|false|string||
|mathLevel|数学|query|false|string||
|matriculateStatus|是否已录取|query|false|string||
|nationCode|民族|query|false|string||
|pageNo|pageNo|query|false|integer(int32)||
|pageSize|pageSize|query|false|integer(int32)||
|phonecode|电话|query|false|string||
|physicalEduLevel|物理实验|query|false|string||
|physicsLevel|物理|query|false|string||
|politicsLevel|政史|query|false|string||
|polity|政治面貌|query|false|string||
|postCode|邮政编码|query|false|string||
|priseHistory|历史荣誉|query|false|string||
|sex|性别|query|false|string||
|studentKind|考生类别|query|false|string||
|studentName|姓名|query|false|string||
|sumScore|总分|query|false|string||
|updateBy|更新人|query|false|string||
|updateTime|更新日期|query|false|string(date-time)||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«IPage«out_student_info对象»»|
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|IPage«out_student_info对象»|IPage«out_student_info对象»|
|&emsp;&emsp;current||integer(int64)||
|&emsp;&emsp;pages||integer(int64)||
|&emsp;&emsp;records||array|out_student_info对象|
|&emsp;&emsp;&emsp;&emsp;address|现住地址|string||
|&emsp;&emsp;&emsp;&emsp;archiveCode|准考证号|string||
|&emsp;&emsp;&emsp;&emsp;birth|出生年月|string||
|&emsp;&emsp;&emsp;&emsp;chineseLevel|语文|string||
|&emsp;&emsp;&emsp;&emsp;chymistLevel|化学|string||
|&emsp;&emsp;&emsp;&emsp;className|班级|string||
|&emsp;&emsp;&emsp;&emsp;combinedScore|组合分|string||
|&emsp;&emsp;&emsp;&emsp;createBy|创建人|string||
|&emsp;&emsp;&emsp;&emsp;createTime|创建日期|string||
|&emsp;&emsp;&emsp;&emsp;delFlag|删除标识|integer||
|&emsp;&emsp;&emsp;&emsp;diathesis|综合素质|string||
|&emsp;&emsp;&emsp;&emsp;englishLevel|英语|string||
|&emsp;&emsp;&emsp;&emsp;experiment|实验|string||
|&emsp;&emsp;&emsp;&emsp;finishSchoolCode|毕业学校代码|string||
|&emsp;&emsp;&emsp;&emsp;finishSchoolName|毕业学校名称|string||
|&emsp;&emsp;&emsp;&emsp;graduateDate|毕业时间|string||
|&emsp;&emsp;&emsp;&emsp;highSchoolCode|录取高中|string||
|&emsp;&emsp;&emsp;&emsp;homePlace|户口地址|string||
|&emsp;&emsp;&emsp;&emsp;id|主键|string||
|&emsp;&emsp;&emsp;&emsp;identityCode|身份证号|string||
|&emsp;&emsp;&emsp;&emsp;mathLevel|数学|string||
|&emsp;&emsp;&emsp;&emsp;matriculateStatus|是否已录取|string||
|&emsp;&emsp;&emsp;&emsp;nationCode|民族|string||
|&emsp;&emsp;&emsp;&emsp;phonecode|电话|string||
|&emsp;&emsp;&emsp;&emsp;physicalEduLevel|物理实验|string||
|&emsp;&emsp;&emsp;&emsp;physicsLevel|物理|string||
|&emsp;&emsp;&emsp;&emsp;politicsLevel|政史|string||
|&emsp;&emsp;&emsp;&emsp;polity|政治面貌|string||
|&emsp;&emsp;&emsp;&emsp;postCode|邮政编码|string||
|&emsp;&emsp;&emsp;&emsp;priseHistory|历史荣誉|string||
|&emsp;&emsp;&emsp;&emsp;sex|性别|string||
|&emsp;&emsp;&emsp;&emsp;studentKind|考生类别|string||
|&emsp;&emsp;&emsp;&emsp;studentName|姓名|string||
|&emsp;&emsp;&emsp;&emsp;sumScore|总分|string||
|&emsp;&emsp;&emsp;&emsp;updateBy|更新人|string||
|&emsp;&emsp;&emsp;&emsp;updateTime|更新日期|string||
|&emsp;&emsp;size||integer(int64)||
|&emsp;&emsp;total||integer(int64)||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": {
		"current": 0,
		"pages": 0,
		"records": [
			{
				"address": "",
				"archiveCode": "",
				"birth": "",
				"chineseLevel": "",
				"chymistLevel": "",
				"className": "",
				"combinedScore": "",
				"createBy": "",
				"createTime": "",
				"delFlag": 0,
				"diathesis": "",
				"englishLevel": "",
				"experiment": "",
				"finishSchoolCode": "",
				"finishSchoolName": "",
				"graduateDate": "",
				"highSchoolCode": "",
				"homePlace": "",
				"id": "",
				"identityCode": "",
				"mathLevel": "",
				"matriculateStatus": "",
				"nationCode": "",
				"phonecode": "",
				"physicalEduLevel": "",
				"physicsLevel": "",
				"politicsLevel": "",
				"polity": "",
				"postCode": "",
				"priseHistory": "",
				"sex": "",
				"studentKind": "",
				"studentName": "",
				"sumScore": "",
				"updateBy": "",
				"updateTime": ""
			}
		],
		"size": 0,
		"total": 0
	},
	"success": true,
	"timestamp": 0
}
```


## 县份学生表-通过id查询


**接口地址**:`/nnzk/student/outStudentInfo/queryById`


**请求方式**:`GET`


**请求数据类型**:`application/x-www-form-urlencoded`


**响应数据类型**:`*/*`


**接口描述**:<p>县份学生表-通过id查询</p>



**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|id|id|query|true|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«out_student_info对象»|
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|out_student_info对象|out_student_info对象|
|&emsp;&emsp;address|现住地址|string||
|&emsp;&emsp;archiveCode|准考证号|string||
|&emsp;&emsp;birth|出生年月|string(date-time)||
|&emsp;&emsp;chineseLevel|语文|string||
|&emsp;&emsp;chymistLevel|化学|string||
|&emsp;&emsp;className|班级|string||
|&emsp;&emsp;combinedScore|组合分|string||
|&emsp;&emsp;createBy|创建人|string||
|&emsp;&emsp;createTime|创建日期|string(date-time)||
|&emsp;&emsp;delFlag|删除标识|integer(int32)||
|&emsp;&emsp;diathesis|综合素质|string||
|&emsp;&emsp;englishLevel|英语|string||
|&emsp;&emsp;experiment|实验|string||
|&emsp;&emsp;finishSchoolCode|毕业学校代码|string||
|&emsp;&emsp;finishSchoolName|毕业学校名称|string||
|&emsp;&emsp;graduateDate|毕业时间|string(date-time)||
|&emsp;&emsp;highSchoolCode|录取高中|string||
|&emsp;&emsp;homePlace|户口地址|string||
|&emsp;&emsp;id|主键|string||
|&emsp;&emsp;identityCode|身份证号|string||
|&emsp;&emsp;mathLevel|数学|string||
|&emsp;&emsp;matriculateStatus|是否已录取|string||
|&emsp;&emsp;nationCode|民族|string||
|&emsp;&emsp;phonecode|电话|string||
|&emsp;&emsp;physicalEduLevel|物理实验|string||
|&emsp;&emsp;physicsLevel|物理|string||
|&emsp;&emsp;politicsLevel|政史|string||
|&emsp;&emsp;polity|政治面貌|string||
|&emsp;&emsp;postCode|邮政编码|string||
|&emsp;&emsp;priseHistory|历史荣誉|string||
|&emsp;&emsp;sex|性别|string||
|&emsp;&emsp;studentKind|考生类别|string||
|&emsp;&emsp;studentName|姓名|string||
|&emsp;&emsp;sumScore|总分|string||
|&emsp;&emsp;updateBy|更新人|string||
|&emsp;&emsp;updateTime|更新日期|string(date-time)||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": {
		"address": "",
		"archiveCode": "",
		"birth": "",
		"chineseLevel": "",
		"chymistLevel": "",
		"className": "",
		"combinedScore": "",
		"createBy": "",
		"createTime": "",
		"delFlag": 0,
		"diathesis": "",
		"englishLevel": "",
		"experiment": "",
		"finishSchoolCode": "",
		"finishSchoolName": "",
		"graduateDate": "",
		"highSchoolCode": "",
		"homePlace": "",
		"id": "",
		"identityCode": "",
		"mathLevel": "",
		"matriculateStatus": "",
		"nationCode": "",
		"phonecode": "",
		"physicalEduLevel": "",
		"physicsLevel": "",
		"politicsLevel": "",
		"polity": "",
		"postCode": "",
		"priseHistory": "",
		"sex": "",
		"studentKind": "",
		"studentName": "",
		"sumScore": "",
		"updateBy": "",
		"updateTime": ""
	},
	"success": true,
	"timestamp": 0
}
```


# 填值规则


## 填值规则-添加


**接口地址**:`/nnzk/sys/fillRule/add`


**请求方式**:`POST`


**请求数据类型**:`application/json`


**响应数据类型**:`*/*`


**接口描述**:<p>填值规则-添加</p>



**请求示例**:


```javascript
{
  "createBy": "",
  "createTime": "",
  "id": "",
  "ruleClass": "",
  "ruleCode": "",
  "ruleName": "",
  "ruleParams": "",
  "updateBy": "",
  "updateTime": ""
}
```


**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|sysFillRule|填值规则|body|true|sys_fill_rule对象|sys_fill_rule对象|
|&emsp;&emsp;createBy|创建人||false|string||
|&emsp;&emsp;createTime|创建时间||false|string(date-time)||
|&emsp;&emsp;id|主键ID||false|string||
|&emsp;&emsp;ruleClass|规则实现类||false|string||
|&emsp;&emsp;ruleCode|规则Code||false|string||
|&emsp;&emsp;ruleName|规则名称||false|string||
|&emsp;&emsp;ruleParams|规则参数||false|string||
|&emsp;&emsp;updateBy|修改人||false|string||
|&emsp;&emsp;updateTime|修改时间||false|string(date-time)||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«object»|
|201|Created||
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|object||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": {},
	"success": true,
	"timestamp": 0
}
```


## 填值规则-通过id删除


**接口地址**:`/nnzk/sys/fillRule/delete`


**请求方式**:`DELETE`


**请求数据类型**:`application/x-www-form-urlencoded`


**响应数据类型**:`*/*`


**接口描述**:<p>填值规则-通过id删除</p>



**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|id|id|query|true|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«object»|
|204|No Content||
|401|Unauthorized||
|403|Forbidden||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|object||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": {},
	"success": true,
	"timestamp": 0
}
```


## 填值规则-批量删除


**接口地址**:`/nnzk/sys/fillRule/deleteBatch`


**请求方式**:`DELETE`


**请求数据类型**:`application/x-www-form-urlencoded`


**响应数据类型**:`*/*`


**接口描述**:<p>填值规则-批量删除</p>



**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|ids|ids|query|true|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«object»|
|204|No Content||
|401|Unauthorized||
|403|Forbidden||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|object||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": {},
	"success": true,
	"timestamp": 0
}
```


## 填值规则-编辑


**接口地址**:`/nnzk/sys/fillRule/edit`


**请求方式**:`POST`


**请求数据类型**:`application/json`


**响应数据类型**:`*/*`


**接口描述**:<p>填值规则-编辑</p>



**请求示例**:


```javascript
{
  "createBy": "",
  "createTime": "",
  "id": "",
  "ruleClass": "",
  "ruleCode": "",
  "ruleName": "",
  "ruleParams": "",
  "updateBy": "",
  "updateTime": ""
}
```


**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|sysFillRule|填值规则|body|true|sys_fill_rule对象|sys_fill_rule对象|
|&emsp;&emsp;createBy|创建人||false|string||
|&emsp;&emsp;createTime|创建时间||false|string(date-time)||
|&emsp;&emsp;id|主键ID||false|string||
|&emsp;&emsp;ruleClass|规则实现类||false|string||
|&emsp;&emsp;ruleCode|规则Code||false|string||
|&emsp;&emsp;ruleName|规则名称||false|string||
|&emsp;&emsp;ruleParams|规则参数||false|string||
|&emsp;&emsp;updateBy|修改人||false|string||
|&emsp;&emsp;updateTime|修改时间||false|string(date-time)||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«object»|
|201|Created||
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|object||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": {},
	"success": true,
	"timestamp": 0
}
```


## 填值规则-编辑


**接口地址**:`/nnzk/sys/fillRule/edit`


**请求方式**:`PUT`


**请求数据类型**:`application/json`


**响应数据类型**:`*/*`


**接口描述**:<p>填值规则-编辑</p>



**请求示例**:


```javascript
{
  "createBy": "",
  "createTime": "",
  "id": "",
  "ruleClass": "",
  "ruleCode": "",
  "ruleName": "",
  "ruleParams": "",
  "updateBy": "",
  "updateTime": ""
}
```


**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|sysFillRule|填值规则|body|true|sys_fill_rule对象|sys_fill_rule对象|
|&emsp;&emsp;createBy|创建人||false|string||
|&emsp;&emsp;createTime|创建时间||false|string(date-time)||
|&emsp;&emsp;id|主键ID||false|string||
|&emsp;&emsp;ruleClass|规则实现类||false|string||
|&emsp;&emsp;ruleCode|规则Code||false|string||
|&emsp;&emsp;ruleName|规则名称||false|string||
|&emsp;&emsp;ruleParams|规则参数||false|string||
|&emsp;&emsp;updateBy|修改人||false|string||
|&emsp;&emsp;updateTime|修改时间||false|string(date-time)||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«object»|
|201|Created||
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|object||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": {},
	"success": true,
	"timestamp": 0
}
```


## 填值规则-分页列表查询


**接口地址**:`/nnzk/sys/fillRule/list`


**请求方式**:`GET`


**请求数据类型**:`application/x-www-form-urlencoded`


**响应数据类型**:`*/*`


**接口描述**:<p>填值规则-分页列表查询</p>



**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|createBy|创建人|query|false|string||
|createTime|创建时间|query|false|string(date-time)||
|id|主键ID|query|false|string||
|pageNo|pageNo|query|false|integer(int32)||
|pageSize|pageSize|query|false|integer(int32)||
|ruleClass|规则实现类|query|false|string||
|ruleCode|规则Code|query|false|string||
|ruleName|规则名称|query|false|string||
|ruleParams|规则参数|query|false|string||
|updateBy|修改人|query|false|string||
|updateTime|修改时间|query|false|string(date-time)||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«object»|
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|object||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": {},
	"success": true,
	"timestamp": 0
}
```


## 填值规则-通过id查询


**接口地址**:`/nnzk/sys/fillRule/queryById`


**请求方式**:`GET`


**请求数据类型**:`application/x-www-form-urlencoded`


**响应数据类型**:`*/*`


**接口描述**:<p>填值规则-通过id查询</p>



**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|id|id|query|true|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«object»|
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|object||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": {},
	"success": true,
	"timestamp": 0
}
```


# 外地学生表


## 外地学生表-添加


**接口地址**:`/nnzk/student/foreignStudent/add`


**请求方式**:`POST`


**请求数据类型**:`application/json`


**响应数据类型**:`*/*`


**接口描述**:<p>外地学生表-添加</p>



**请求示例**:


```javascript
{
  "address": "",
  "archiveCode": "",
  "chineseLevel": "",
  "chymistLevel": "",
  "combinedScore": "",
  "createBy": "",
  "createTime": "",
  "delFlag": 0,
  "diathesis": "",
  "englishLevel": "",
  "experiment": "",
  "finishSchoolName": "",
  "guardian": "",
  "guardianPhone": "",
  "homePlace": "",
  "id": "",
  "identityCode": "",
  "mathLevel": "",
  "physicalEduLevel": "",
  "physicsLevel": "",
  "politicsLevel": "",
  "registSchool": "",
  "remark": "",
  "sex": "",
  "studentName": "",
  "sumScore": "",
  "updateBy": "",
  "updateTime": ""
}
```


**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|foreignStudent|外地学生表|body|true|foreign_student对象|foreign_student对象|
|&emsp;&emsp;address|现住地址||false|string||
|&emsp;&emsp;archiveCode|准考证号||false|string||
|&emsp;&emsp;chineseLevel|语文||false|string||
|&emsp;&emsp;chymistLevel|化学||false|string||
|&emsp;&emsp;combinedScore|组合分||false|string||
|&emsp;&emsp;createBy|创建人||false|string||
|&emsp;&emsp;createTime|创建日期||false|string(date-time)||
|&emsp;&emsp;delFlag|删除标识||false|integer(int32)||
|&emsp;&emsp;diathesis|综合素质||false|string||
|&emsp;&emsp;englishLevel|英语||false|string||
|&emsp;&emsp;experiment|实验||false|string||
|&emsp;&emsp;finishSchoolName|毕业学校||false|string||
|&emsp;&emsp;guardian|监护人||false|string||
|&emsp;&emsp;guardianPhone|监护人电话||false|string||
|&emsp;&emsp;homePlace|户口地址||false|string||
|&emsp;&emsp;id|主键||false|string||
|&emsp;&emsp;identityCode|身份证号||false|string||
|&emsp;&emsp;mathLevel|数学||false|string||
|&emsp;&emsp;physicalEduLevel|物理实验||false|string||
|&emsp;&emsp;physicsLevel|物理||false|string||
|&emsp;&emsp;politicsLevel|政史||false|string||
|&emsp;&emsp;registSchool|登记学校||false|string||
|&emsp;&emsp;remark|说明||false|string||
|&emsp;&emsp;sex|性别||false|string||
|&emsp;&emsp;studentName|姓名||false|string||
|&emsp;&emsp;sumScore|总分||false|string||
|&emsp;&emsp;updateBy|更新人||false|string||
|&emsp;&emsp;updateTime|更新日期||false|string(date-time)||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«string»|
|201|Created||
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|string||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": "",
	"success": true,
	"timestamp": 0
}
```


## 外地学生表-通过id删除


**接口地址**:`/nnzk/student/foreignStudent/delete`


**请求方式**:`DELETE`


**请求数据类型**:`application/x-www-form-urlencoded`


**响应数据类型**:`*/*`


**接口描述**:<p>外地学生表-通过id删除</p>



**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|id|id|query|true|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«string»|
|204|No Content||
|401|Unauthorized||
|403|Forbidden||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|string||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": "",
	"success": true,
	"timestamp": 0
}
```


## 外地学生表-批量删除


**接口地址**:`/nnzk/student/foreignStudent/deleteBatch`


**请求方式**:`DELETE`


**请求数据类型**:`application/x-www-form-urlencoded`


**响应数据类型**:`*/*`


**接口描述**:<p>外地学生表-批量删除</p>



**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|ids|ids|query|true|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«string»|
|204|No Content||
|401|Unauthorized||
|403|Forbidden||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|string||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": "",
	"success": true,
	"timestamp": 0
}
```


## 外地学生表-编辑


**接口地址**:`/nnzk/student/foreignStudent/edit`


**请求方式**:`POST`


**请求数据类型**:`application/json`


**响应数据类型**:`*/*`


**接口描述**:<p>外地学生表-编辑</p>



**请求示例**:


```javascript
{
  "address": "",
  "archiveCode": "",
  "chineseLevel": "",
  "chymistLevel": "",
  "combinedScore": "",
  "createBy": "",
  "createTime": "",
  "delFlag": 0,
  "diathesis": "",
  "englishLevel": "",
  "experiment": "",
  "finishSchoolName": "",
  "guardian": "",
  "guardianPhone": "",
  "homePlace": "",
  "id": "",
  "identityCode": "",
  "mathLevel": "",
  "physicalEduLevel": "",
  "physicsLevel": "",
  "politicsLevel": "",
  "registSchool": "",
  "remark": "",
  "sex": "",
  "studentName": "",
  "sumScore": "",
  "updateBy": "",
  "updateTime": ""
}
```


**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|foreignStudent|外地学生表|body|true|foreign_student对象|foreign_student对象|
|&emsp;&emsp;address|现住地址||false|string||
|&emsp;&emsp;archiveCode|准考证号||false|string||
|&emsp;&emsp;chineseLevel|语文||false|string||
|&emsp;&emsp;chymistLevel|化学||false|string||
|&emsp;&emsp;combinedScore|组合分||false|string||
|&emsp;&emsp;createBy|创建人||false|string||
|&emsp;&emsp;createTime|创建日期||false|string(date-time)||
|&emsp;&emsp;delFlag|删除标识||false|integer(int32)||
|&emsp;&emsp;diathesis|综合素质||false|string||
|&emsp;&emsp;englishLevel|英语||false|string||
|&emsp;&emsp;experiment|实验||false|string||
|&emsp;&emsp;finishSchoolName|毕业学校||false|string||
|&emsp;&emsp;guardian|监护人||false|string||
|&emsp;&emsp;guardianPhone|监护人电话||false|string||
|&emsp;&emsp;homePlace|户口地址||false|string||
|&emsp;&emsp;id|主键||false|string||
|&emsp;&emsp;identityCode|身份证号||false|string||
|&emsp;&emsp;mathLevel|数学||false|string||
|&emsp;&emsp;physicalEduLevel|物理实验||false|string||
|&emsp;&emsp;physicsLevel|物理||false|string||
|&emsp;&emsp;politicsLevel|政史||false|string||
|&emsp;&emsp;registSchool|登记学校||false|string||
|&emsp;&emsp;remark|说明||false|string||
|&emsp;&emsp;sex|性别||false|string||
|&emsp;&emsp;studentName|姓名||false|string||
|&emsp;&emsp;sumScore|总分||false|string||
|&emsp;&emsp;updateBy|更新人||false|string||
|&emsp;&emsp;updateTime|更新日期||false|string(date-time)||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«string»|
|201|Created||
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|string||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": "",
	"success": true,
	"timestamp": 0
}
```


## 外地学生表-编辑


**接口地址**:`/nnzk/student/foreignStudent/edit`


**请求方式**:`PUT`


**请求数据类型**:`application/json`


**响应数据类型**:`*/*`


**接口描述**:<p>外地学生表-编辑</p>



**请求示例**:


```javascript
{
  "address": "",
  "archiveCode": "",
  "chineseLevel": "",
  "chymistLevel": "",
  "combinedScore": "",
  "createBy": "",
  "createTime": "",
  "delFlag": 0,
  "diathesis": "",
  "englishLevel": "",
  "experiment": "",
  "finishSchoolName": "",
  "guardian": "",
  "guardianPhone": "",
  "homePlace": "",
  "id": "",
  "identityCode": "",
  "mathLevel": "",
  "physicalEduLevel": "",
  "physicsLevel": "",
  "politicsLevel": "",
  "registSchool": "",
  "remark": "",
  "sex": "",
  "studentName": "",
  "sumScore": "",
  "updateBy": "",
  "updateTime": ""
}
```


**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|foreignStudent|外地学生表|body|true|foreign_student对象|foreign_student对象|
|&emsp;&emsp;address|现住地址||false|string||
|&emsp;&emsp;archiveCode|准考证号||false|string||
|&emsp;&emsp;chineseLevel|语文||false|string||
|&emsp;&emsp;chymistLevel|化学||false|string||
|&emsp;&emsp;combinedScore|组合分||false|string||
|&emsp;&emsp;createBy|创建人||false|string||
|&emsp;&emsp;createTime|创建日期||false|string(date-time)||
|&emsp;&emsp;delFlag|删除标识||false|integer(int32)||
|&emsp;&emsp;diathesis|综合素质||false|string||
|&emsp;&emsp;englishLevel|英语||false|string||
|&emsp;&emsp;experiment|实验||false|string||
|&emsp;&emsp;finishSchoolName|毕业学校||false|string||
|&emsp;&emsp;guardian|监护人||false|string||
|&emsp;&emsp;guardianPhone|监护人电话||false|string||
|&emsp;&emsp;homePlace|户口地址||false|string||
|&emsp;&emsp;id|主键||false|string||
|&emsp;&emsp;identityCode|身份证号||false|string||
|&emsp;&emsp;mathLevel|数学||false|string||
|&emsp;&emsp;physicalEduLevel|物理实验||false|string||
|&emsp;&emsp;physicsLevel|物理||false|string||
|&emsp;&emsp;politicsLevel|政史||false|string||
|&emsp;&emsp;registSchool|登记学校||false|string||
|&emsp;&emsp;remark|说明||false|string||
|&emsp;&emsp;sex|性别||false|string||
|&emsp;&emsp;studentName|姓名||false|string||
|&emsp;&emsp;sumScore|总分||false|string||
|&emsp;&emsp;updateBy|更新人||false|string||
|&emsp;&emsp;updateTime|更新日期||false|string(date-time)||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«string»|
|201|Created||
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|string||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": "",
	"success": true,
	"timestamp": 0
}
```


## 外地学生表-分页列表查询


**接口地址**:`/nnzk/student/foreignStudent/list`


**请求方式**:`GET`


**请求数据类型**:`application/x-www-form-urlencoded`


**响应数据类型**:`*/*`


**接口描述**:<p>外地学生表-分页列表查询</p>



**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|archiveCode|准考证号|query|true|string||
|finishSchoolName|毕业学校|query|true|string||
|guardian|监护人|query|true|string||
|guardianPhone|监护人电话|query|true|string||
|sex|性别|query|true|string||
|studentName|姓名|query|true|string||
|sumScore|总分|query|true|string||
|address|现住地址|query|false|string||
|chineseLevel|语文|query|false|string||
|chymistLevel|化学|query|false|string||
|combinedScore|组合分|query|false|string||
|createBy|创建人|query|false|string||
|createTime|创建日期|query|false|string(date-time)||
|delFlag|删除标识|query|false|integer(int32)||
|diathesis|综合素质|query|false|string||
|englishLevel|英语|query|false|string||
|experiment|实验|query|false|string||
|homePlace|户口地址|query|false|string||
|id|主键|query|false|string||
|identityCode|身份证号|query|false|string||
|mathLevel|数学|query|false|string||
|pageNo|pageNo|query|false|integer(int32)||
|pageSize|pageSize|query|false|integer(int32)||
|physicalEduLevel|物理实验|query|false|string||
|physicsLevel|物理|query|false|string||
|politicsLevel|政史|query|false|string||
|registSchool|登记学校|query|false|string||
|remark|说明|query|false|string||
|updateBy|更新人|query|false|string||
|updateTime|更新日期|query|false|string(date-time)||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«IPage«foreign_student对象»»|
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|IPage«foreign_student对象»|IPage«foreign_student对象»|
|&emsp;&emsp;current||integer(int64)||
|&emsp;&emsp;pages||integer(int64)||
|&emsp;&emsp;records||array|foreign_student对象|
|&emsp;&emsp;&emsp;&emsp;address|现住地址|string||
|&emsp;&emsp;&emsp;&emsp;archiveCode|准考证号|string||
|&emsp;&emsp;&emsp;&emsp;chineseLevel|语文|string||
|&emsp;&emsp;&emsp;&emsp;chymistLevel|化学|string||
|&emsp;&emsp;&emsp;&emsp;combinedScore|组合分|string||
|&emsp;&emsp;&emsp;&emsp;createBy|创建人|string||
|&emsp;&emsp;&emsp;&emsp;createTime|创建日期|string||
|&emsp;&emsp;&emsp;&emsp;delFlag|删除标识|integer||
|&emsp;&emsp;&emsp;&emsp;diathesis|综合素质|string||
|&emsp;&emsp;&emsp;&emsp;englishLevel|英语|string||
|&emsp;&emsp;&emsp;&emsp;experiment|实验|string||
|&emsp;&emsp;&emsp;&emsp;finishSchoolName|毕业学校|string||
|&emsp;&emsp;&emsp;&emsp;guardian|监护人|string||
|&emsp;&emsp;&emsp;&emsp;guardianPhone|监护人电话|string||
|&emsp;&emsp;&emsp;&emsp;homePlace|户口地址|string||
|&emsp;&emsp;&emsp;&emsp;id|主键|string||
|&emsp;&emsp;&emsp;&emsp;identityCode|身份证号|string||
|&emsp;&emsp;&emsp;&emsp;mathLevel|数学|string||
|&emsp;&emsp;&emsp;&emsp;physicalEduLevel|物理实验|string||
|&emsp;&emsp;&emsp;&emsp;physicsLevel|物理|string||
|&emsp;&emsp;&emsp;&emsp;politicsLevel|政史|string||
|&emsp;&emsp;&emsp;&emsp;registSchool|登记学校|string||
|&emsp;&emsp;&emsp;&emsp;remark|说明|string||
|&emsp;&emsp;&emsp;&emsp;sex|性别|string||
|&emsp;&emsp;&emsp;&emsp;studentName|姓名|string||
|&emsp;&emsp;&emsp;&emsp;sumScore|总分|string||
|&emsp;&emsp;&emsp;&emsp;updateBy|更新人|string||
|&emsp;&emsp;&emsp;&emsp;updateTime|更新日期|string||
|&emsp;&emsp;size||integer(int64)||
|&emsp;&emsp;total||integer(int64)||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": {
		"current": 0,
		"pages": 0,
		"records": [
			{
				"address": "",
				"archiveCode": "",
				"chineseLevel": "",
				"chymistLevel": "",
				"combinedScore": "",
				"createBy": "",
				"createTime": "",
				"delFlag": 0,
				"diathesis": "",
				"englishLevel": "",
				"experiment": "",
				"finishSchoolName": "",
				"guardian": "",
				"guardianPhone": "",
				"homePlace": "",
				"id": "",
				"identityCode": "",
				"mathLevel": "",
				"physicalEduLevel": "",
				"physicsLevel": "",
				"politicsLevel": "",
				"registSchool": "",
				"remark": "",
				"sex": "",
				"studentName": "",
				"sumScore": "",
				"updateBy": "",
				"updateTime": ""
			}
		],
		"size": 0,
		"total": 0
	},
	"success": true,
	"timestamp": 0
}
```


## 外地学生表-通过id查询


**接口地址**:`/nnzk/student/foreignStudent/queryById`


**请求方式**:`GET`


**请求数据类型**:`application/x-www-form-urlencoded`


**响应数据类型**:`*/*`


**接口描述**:<p>外地学生表-通过id查询</p>



**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|id|id|query|true|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«foreign_student对象»|
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|foreign_student对象|foreign_student对象|
|&emsp;&emsp;address|现住地址|string||
|&emsp;&emsp;archiveCode|准考证号|string||
|&emsp;&emsp;chineseLevel|语文|string||
|&emsp;&emsp;chymistLevel|化学|string||
|&emsp;&emsp;combinedScore|组合分|string||
|&emsp;&emsp;createBy|创建人|string||
|&emsp;&emsp;createTime|创建日期|string(date-time)||
|&emsp;&emsp;delFlag|删除标识|integer(int32)||
|&emsp;&emsp;diathesis|综合素质|string||
|&emsp;&emsp;englishLevel|英语|string||
|&emsp;&emsp;experiment|实验|string||
|&emsp;&emsp;finishSchoolName|毕业学校|string||
|&emsp;&emsp;guardian|监护人|string||
|&emsp;&emsp;guardianPhone|监护人电话|string||
|&emsp;&emsp;homePlace|户口地址|string||
|&emsp;&emsp;id|主键|string||
|&emsp;&emsp;identityCode|身份证号|string||
|&emsp;&emsp;mathLevel|数学|string||
|&emsp;&emsp;physicalEduLevel|物理实验|string||
|&emsp;&emsp;physicsLevel|物理|string||
|&emsp;&emsp;politicsLevel|政史|string||
|&emsp;&emsp;registSchool|登记学校|string||
|&emsp;&emsp;remark|说明|string||
|&emsp;&emsp;sex|性别|string||
|&emsp;&emsp;studentName|姓名|string||
|&emsp;&emsp;sumScore|总分|string||
|&emsp;&emsp;updateBy|更新人|string||
|&emsp;&emsp;updateTime|更新日期|string(date-time)||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": {
		"address": "",
		"archiveCode": "",
		"chineseLevel": "",
		"chymistLevel": "",
		"combinedScore": "",
		"createBy": "",
		"createTime": "",
		"delFlag": 0,
		"diathesis": "",
		"englishLevel": "",
		"experiment": "",
		"finishSchoolName": "",
		"guardian": "",
		"guardianPhone": "",
		"homePlace": "",
		"id": "",
		"identityCode": "",
		"mathLevel": "",
		"physicalEduLevel": "",
		"physicsLevel": "",
		"politicsLevel": "",
		"registSchool": "",
		"remark": "",
		"sex": "",
		"studentName": "",
		"sumScore": "",
		"updateBy": "",
		"updateTime": ""
	},
	"success": true,
	"timestamp": 0
}
```


# 多数据源管理


## 多数据源管理-添加


**接口地址**:`/nnzk/sys/dataSource/add`


**请求方式**:`POST`


**请求数据类型**:`application/json`


**响应数据类型**:`*/*`


**接口描述**:<p>多数据源管理-添加</p>



**请求示例**:


```javascript
{
  "code": "",
  "createBy": "",
  "createTime": "",
  "dbDriver": "",
  "dbName": "",
  "dbPassword": "",
  "dbType": "",
  "dbUrl": "",
  "dbUsername": "",
  "id": "",
  "name": "",
  "remark": "",
  "sysOrgCode": "",
  "tenantId": 0,
  "updateBy": "",
  "updateTime": ""
}
```


**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|sysDataSource|多数据源管理|body|true|sys_data_source对象|sys_data_source对象|
|&emsp;&emsp;code|数据源编码||false|string||
|&emsp;&emsp;createBy|创建人||false|string||
|&emsp;&emsp;createTime|创建日期||false|string(date-time)||
|&emsp;&emsp;dbDriver|驱动类||false|string||
|&emsp;&emsp;dbName|数据库名称||false|string||
|&emsp;&emsp;dbPassword|密码||false|string||
|&emsp;&emsp;dbType|数据库类型||false|string||
|&emsp;&emsp;dbUrl|数据源地址||false|string||
|&emsp;&emsp;dbUsername|用户名||false|string||
|&emsp;&emsp;id|id||false|string||
|&emsp;&emsp;name|数据源名称||false|string||
|&emsp;&emsp;remark|备注||false|string||
|&emsp;&emsp;sysOrgCode|所属部门||false|string||
|&emsp;&emsp;tenantId|租户ID||false|integer(int32)||
|&emsp;&emsp;updateBy|更新人||false|string||
|&emsp;&emsp;updateTime|更新日期||false|string(date-time)||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«object»|
|201|Created||
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|object||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": {},
	"success": true,
	"timestamp": 0
}
```


## 多数据源管理-通过id删除


**接口地址**:`/nnzk/sys/dataSource/delete`


**请求方式**:`DELETE`


**请求数据类型**:`application/x-www-form-urlencoded`


**响应数据类型**:`*/*`


**接口描述**:<p>多数据源管理-通过id删除</p>



**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|id|id|query|true|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«object»|
|204|No Content||
|401|Unauthorized||
|403|Forbidden||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|object||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": {},
	"success": true,
	"timestamp": 0
}
```


## 多数据源管理-批量删除


**接口地址**:`/nnzk/sys/dataSource/deleteBatch`


**请求方式**:`DELETE`


**请求数据类型**:`application/x-www-form-urlencoded`


**响应数据类型**:`*/*`


**接口描述**:<p>多数据源管理-批量删除</p>



**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|ids|ids|query|true|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«object»|
|204|No Content||
|401|Unauthorized||
|403|Forbidden||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|object||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": {},
	"success": true,
	"timestamp": 0
}
```


## 多数据源管理-编辑


**接口地址**:`/nnzk/sys/dataSource/edit`


**请求方式**:`POST`


**请求数据类型**:`application/json`


**响应数据类型**:`*/*`


**接口描述**:<p>多数据源管理-编辑</p>



**请求示例**:


```javascript
{
  "code": "",
  "createBy": "",
  "createTime": "",
  "dbDriver": "",
  "dbName": "",
  "dbPassword": "",
  "dbType": "",
  "dbUrl": "",
  "dbUsername": "",
  "id": "",
  "name": "",
  "remark": "",
  "sysOrgCode": "",
  "tenantId": 0,
  "updateBy": "",
  "updateTime": ""
}
```


**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|sysDataSource|多数据源管理|body|true|sys_data_source对象|sys_data_source对象|
|&emsp;&emsp;code|数据源编码||false|string||
|&emsp;&emsp;createBy|创建人||false|string||
|&emsp;&emsp;createTime|创建日期||false|string(date-time)||
|&emsp;&emsp;dbDriver|驱动类||false|string||
|&emsp;&emsp;dbName|数据库名称||false|string||
|&emsp;&emsp;dbPassword|密码||false|string||
|&emsp;&emsp;dbType|数据库类型||false|string||
|&emsp;&emsp;dbUrl|数据源地址||false|string||
|&emsp;&emsp;dbUsername|用户名||false|string||
|&emsp;&emsp;id|id||false|string||
|&emsp;&emsp;name|数据源名称||false|string||
|&emsp;&emsp;remark|备注||false|string||
|&emsp;&emsp;sysOrgCode|所属部门||false|string||
|&emsp;&emsp;tenantId|租户ID||false|integer(int32)||
|&emsp;&emsp;updateBy|更新人||false|string||
|&emsp;&emsp;updateTime|更新日期||false|string(date-time)||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«object»|
|201|Created||
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|object||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": {},
	"success": true,
	"timestamp": 0
}
```


## 多数据源管理-编辑


**接口地址**:`/nnzk/sys/dataSource/edit`


**请求方式**:`PUT`


**请求数据类型**:`application/json`


**响应数据类型**:`*/*`


**接口描述**:<p>多数据源管理-编辑</p>



**请求示例**:


```javascript
{
  "code": "",
  "createBy": "",
  "createTime": "",
  "dbDriver": "",
  "dbName": "",
  "dbPassword": "",
  "dbType": "",
  "dbUrl": "",
  "dbUsername": "",
  "id": "",
  "name": "",
  "remark": "",
  "sysOrgCode": "",
  "tenantId": 0,
  "updateBy": "",
  "updateTime": ""
}
```


**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|sysDataSource|多数据源管理|body|true|sys_data_source对象|sys_data_source对象|
|&emsp;&emsp;code|数据源编码||false|string||
|&emsp;&emsp;createBy|创建人||false|string||
|&emsp;&emsp;createTime|创建日期||false|string(date-time)||
|&emsp;&emsp;dbDriver|驱动类||false|string||
|&emsp;&emsp;dbName|数据库名称||false|string||
|&emsp;&emsp;dbPassword|密码||false|string||
|&emsp;&emsp;dbType|数据库类型||false|string||
|&emsp;&emsp;dbUrl|数据源地址||false|string||
|&emsp;&emsp;dbUsername|用户名||false|string||
|&emsp;&emsp;id|id||false|string||
|&emsp;&emsp;name|数据源名称||false|string||
|&emsp;&emsp;remark|备注||false|string||
|&emsp;&emsp;sysOrgCode|所属部门||false|string||
|&emsp;&emsp;tenantId|租户ID||false|integer(int32)||
|&emsp;&emsp;updateBy|更新人||false|string||
|&emsp;&emsp;updateTime|更新日期||false|string(date-time)||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«object»|
|201|Created||
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|object||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": {},
	"success": true,
	"timestamp": 0
}
```


## 多数据源管理-分页列表查询


**接口地址**:`/nnzk/sys/dataSource/list`


**请求方式**:`GET`


**请求数据类型**:`application/x-www-form-urlencoded`


**响应数据类型**:`*/*`


**接口描述**:<p>多数据源管理-分页列表查询</p>



**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|code|数据源编码|query|false|string||
|createBy|创建人|query|false|string||
|createTime|创建日期|query|false|string(date-time)||
|dbDriver|驱动类|query|false|string||
|dbName|数据库名称|query|false|string||
|dbPassword|密码|query|false|string||
|dbType|数据库类型|query|false|string||
|dbUrl|数据源地址|query|false|string||
|dbUsername|用户名|query|false|string||
|id|id|query|false|string||
|name|数据源名称|query|false|string||
|pageNo|pageNo|query|false|integer(int32)||
|pageSize|pageSize|query|false|integer(int32)||
|remark|备注|query|false|string||
|sysOrgCode|所属部门|query|false|string||
|tenantId|租户ID|query|false|integer(int32)||
|updateBy|更新人|query|false|string||
|updateTime|更新日期|query|false|string(date-time)||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«object»|
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|object||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": {},
	"success": true,
	"timestamp": 0
}
```


## 多数据源管理-通过id查询


**接口地址**:`/nnzk/sys/dataSource/queryById`


**请求方式**:`GET`


**请求数据类型**:`application/x-www-form-urlencoded`


**响应数据类型**:`*/*`


**接口描述**:<p>多数据源管理-通过id查询</p>



**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|id|id|query|true|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«object»|
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|object||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": {},
	"success": true,
	"timestamp": 0
}
```


# 学校端补录


## 学校端补录-检查考生是否可以进行补录


**接口地址**:`/nnzk/alter/privateHighSchool/checkMakeUp`


**请求方式**:`GET`


**请求数据类型**:`application/x-www-form-urlencoded`


**响应数据类型**:`*/*`


**接口描述**:<p>学校端补录-检查考生是否可以进行补录</p>



**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|archiveCode|archiveCode|query|true|string||
|num|num|query|true|integer(int32)||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«string»|
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|string||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": "",
	"success": true,
	"timestamp": 0
}
```


## 学校端补录-检验学校是否开启补录权限


**接口地址**:`/nnzk/alter/privateHighSchool/checkMakeUpPermission`


**请求方式**:`GET`


**请求数据类型**:`application/x-www-form-urlencoded`


**响应数据类型**:`*/*`


**接口描述**:<p>学校端补录-检验学校是否开启补录权限</p>



**请求参数**:


暂无


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«string»|
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|string||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": "",
	"success": true,
	"timestamp": 0
}
```


## 确认录取


**接口地址**:`/nnzk/alter/privateHighSchool/confirmMatriculate`


**请求方式**:`POST`


**请求数据类型**:`application/json`


**响应数据类型**:`*/*`


**接口描述**:<p>确认录取</p>



**请求示例**:


```javascript
{
  "archiveCode": ""
}
```


**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|input|input|body|true|GiveUpMatriculateDTO|GiveUpMatriculateDTO|
|&emsp;&emsp;archiveCode|||false|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«string»|
|201|Created||
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|string||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": "",
	"success": true,
	"timestamp": 0
}
```


## 学校端补录-提交登记学生补录信息


**接口地址**:`/nnzk/alter/privateHighSchool/createMakeUpApplication`


**请求方式**:`POST`


**请求数据类型**:`application/json`


**响应数据类型**:`*/*`


**接口描述**:<p>学校端补录-提交登记学生补录信息</p>



**请求示例**:


```javascript
{
  "archiveCodes": [],
  "makeUpDataId": "",
  "url": ""
}
```


**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|archiveCodesAndUrlDTO|archiveCodesAndUrlDTO|body|true|ArchiveCodesAndUrlDTO|ArchiveCodesAndUrlDTO|
|&emsp;&emsp;archiveCodes|准考证号数组（首元素为学校代码）||false|array|string|
|&emsp;&emsp;makeUpDataId|补录数据make_up_application表id||false|string||
|&emsp;&emsp;url|url||false|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«string»|
|201|Created||
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|string||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": "",
	"success": true,
	"timestamp": 0
}
```


## 学校端补录-补录申请退回后修改


**接口地址**:`/nnzk/alter/privateHighSchool/editMakeUpApplication`


**请求方式**:`POST`


**请求数据类型**:`application/json`


**响应数据类型**:`*/*`


**接口描述**:<p>学校端补录-补录申请退回后修改</p>



**请求示例**:


```javascript
{
  "archiveCodes": [],
  "makeUpDataId": "",
  "url": ""
}
```


**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|archiveCodesAndUrlDTO|archiveCodesAndUrlDTO|body|true|ArchiveCodesAndUrlDTO|ArchiveCodesAndUrlDTO|
|&emsp;&emsp;archiveCodes|准考证号数组（首元素为学校代码）||false|array|string|
|&emsp;&emsp;makeUpDataId|补录数据make_up_application表id||false|string||
|&emsp;&emsp;url|url||false|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«string»|
|201|Created||
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|string||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": "",
	"success": true,
	"timestamp": 0
}
```


## 学校端补录-获取全部补录数据条目


**接口地址**:`/nnzk/alter/privateHighSchool/getMakeUpApplication`


**请求方式**:`GET`


**请求数据类型**:`application/x-www-form-urlencoded`


**响应数据类型**:`*/*`


**接口描述**:<p>学校端补录-获取全部补录数据条目</p>



**请求参数**:


暂无


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«List«MakeUpDataDTO»»|
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|array|MakeUpDataDTO|
|&emsp;&emsp;annexUrl|附件url|string||
|&emsp;&emsp;applicationTime|申请时间|string(date-time)||
|&emsp;&emsp;id|主键id|string||
|&emsp;&emsp;makeUpDataStatus|状态|integer(int32)||
|&emsp;&emsp;makeUpNum|补录次数|integer(int32)||
|&emsp;&emsp;makeUpPeopleNum|补录人数|integer(int32)||
|&emsp;&emsp;schoolCode|学校代码|string||
|&emsp;&emsp;schoolName|学校名称|string||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": [
		{
			"annexUrl": "",
			"applicationTime": "",
			"id": "",
			"makeUpDataStatus": 0,
			"makeUpNum": 0,
			"makeUpPeopleNum": 0,
			"schoolCode": "",
			"schoolName": ""
		}
	],
	"success": true,
	"timestamp": 0
}
```


## 学校端补录-获取补录学生数据


**接口地址**:`/nnzk/alter/privateHighSchool/getMakeUpData`


**请求方式**:`GET`


**请求数据类型**:`application/x-www-form-urlencoded`


**响应数据类型**:`*/*`


**接口描述**:<p>学校端补录-获取补录学生数据</p>



**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|id|id|query|false|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«GetRegInfoOutputDTO»|
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|GetRegInfoOutputDTO|GetRegInfoOutputDTO|
|&emsp;&emsp;count|学生登记总数|string||
|&emsp;&emsp;currentNum|当前数？|integer(int32)||
|&emsp;&emsp;makeUpPeopleNum|??|integer(int32)||
|&emsp;&emsp;minScore|最低分|string||
|&emsp;&emsp;mixScore|？？？|string||
|&emsp;&emsp;records|学生登记列表？|array|StudentRegDTO|
|&emsp;&emsp;&emsp;&emsp;archiveCode|准考证号|string||
|&emsp;&emsp;&emsp;&emsp;chineseLevel|语文|string||
|&emsp;&emsp;&emsp;&emsp;chymistLevel|化学|string||
|&emsp;&emsp;&emsp;&emsp;combinedScore|组合分|string||
|&emsp;&emsp;&emsp;&emsp;commandType|???|string||
|&emsp;&emsp;&emsp;&emsp;commander|???|string||
|&emsp;&emsp;&emsp;&emsp;connector|???|string||
|&emsp;&emsp;&emsp;&emsp;diathesis|综合素质|string||
|&emsp;&emsp;&emsp;&emsp;englishLevel|英语|string||
|&emsp;&emsp;&emsp;&emsp;experiment|实验|string||
|&emsp;&emsp;&emsp;&emsp;id|主键|string||
|&emsp;&emsp;&emsp;&emsp;mathLevel|数学|string||
|&emsp;&emsp;&emsp;&emsp;matriculateStatus|录取状态|integer||
|&emsp;&emsp;&emsp;&emsp;orderCode|排序码|string||
|&emsp;&emsp;&emsp;&emsp;physicsLevel|物理|string||
|&emsp;&emsp;&emsp;&emsp;politicsLevel|政史|string||
|&emsp;&emsp;&emsp;&emsp;registeDept|???|string||
|&emsp;&emsp;&emsp;&emsp;schoolCode|毕业学校代码|string||
|&emsp;&emsp;&emsp;&emsp;schoolName|毕业学校名称|string||
|&emsp;&emsp;&emsp;&emsp;studentName|学生名字|string||
|&emsp;&emsp;&emsp;&emsp;studentSource|学生生源地?|string||
|&emsp;&emsp;&emsp;&emsp;studentType|学生类型|string||
|&emsp;&emsp;&emsp;&emsp;sumScore|总分|string||
|&emsp;&emsp;&emsp;&emsp;type|类型MatriculateType?|string||
|&emsp;&emsp;url|？？？|string||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": {
		"count": "",
		"currentNum": 0,
		"makeUpPeopleNum": 0,
		"minScore": "",
		"mixScore": "",
		"records": [
			{
				"archiveCode": "",
				"chineseLevel": "",
				"chymistLevel": "",
				"combinedScore": "",
				"commandType": "",
				"commander": "",
				"connector": "",
				"diathesis": "",
				"englishLevel": "",
				"experiment": "",
				"id": "",
				"mathLevel": "",
				"matriculateStatus": 0,
				"orderCode": "",
				"physicsLevel": "",
				"politicsLevel": "",
				"registeDept": "",
				"schoolCode": "",
				"schoolName": "",
				"studentName": "",
				"studentSource": "",
				"studentType": "",
				"sumScore": "",
				"type": ""
			}
		],
		"url": ""
	},
	"success": true,
	"timestamp": 0
}
```


## 学校端-入学登记表打印


**接口地址**:`/nnzk/alter/privateHighSchool/getPrintInfoOutput`


**请求方式**:`GET`


**请求数据类型**:`application/x-www-form-urlencoded`


**响应数据类型**:`*/*`


**接口描述**:<p>学校端-入学登记表打印</p>



**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|highSchoolCode|高中学校代码|query|true|string||
|matriculateType|录取类型|query|false|string||
|rangeEnd|按编号范围(结束)|query|false|integer(int32)||
|rangeStart|按编号范围(开始)|query|false|integer(int32)||
|searchByArchiveCode|按准考证号|query|false|string||
|selectBy|查询方式（全部/按准考证号/按编号范围）|query|false|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|GetPrintInfoOutputDTO|
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|data||array|GetPrintInfoDTO|
|&emsp;&emsp;address|现住地址|string||
|&emsp;&emsp;agroSingleton||boolean||
|&emsp;&emsp;agroTwoDauLigation||boolean||
|&emsp;&emsp;archiveCode|准考证号|string||
|&emsp;&emsp;beginTime|开始时间|string(date-time)||
|&emsp;&emsp;birth|出生年月|string(date-time)||
|&emsp;&emsp;chineseLevel|语文|string||
|&emsp;&emsp;chymistLevel|化学|string||
|&emsp;&emsp;className|班级|string||
|&emsp;&emsp;combinedScore|组合分|string||
|&emsp;&emsp;comeFrom|来源类别|string||
|&emsp;&emsp;diathesis|综合素质|string||
|&emsp;&emsp;endTime|结束时间|string(date-time)||
|&emsp;&emsp;englishLevel|英语|string||
|&emsp;&emsp;experiment|实验|string||
|&emsp;&emsp;finishSchoolCode|毕业学校代码|string||
|&emsp;&emsp;finishSchoolName|毕业学校名称|string||
|&emsp;&emsp;graduateDate|毕业时间|string(date-time)||
|&emsp;&emsp;homePlace|户口地址|string||
|&emsp;&emsp;householdAddressOne|家庭成员住址1|string||
|&emsp;&emsp;householdAddressSecond|家庭成员住址2|string||
|&emsp;&emsp;identityCode|身份证号|string||
|&emsp;&emsp;imageSrc|照片src|string||
|&emsp;&emsp;isAreaStudent|地段生|integer(int32)||
|&emsp;&emsp;isMilitary|优抚对象|integer(int32)||
|&emsp;&emsp;mathLevel|数学|string||
|&emsp;&emsp;nationCode|民族|string||
|&emsp;&emsp;numbersOne|家庭成员姓名1|string||
|&emsp;&emsp;numbersSecond|家庭成员姓名2|string||
|&emsp;&emsp;opinion||string||
|&emsp;&emsp;phoneCode|电话|string||
|&emsp;&emsp;phoneOne|家庭成员联系电话1|string||
|&emsp;&emsp;phoneSecond|家庭成员联系电话2|string||
|&emsp;&emsp;physicsLevel|物理|string||
|&emsp;&emsp;politicsLevel|政史|string||
|&emsp;&emsp;polity|政治面貌|string||
|&emsp;&emsp;postCode|邮政编码|string||
|&emsp;&emsp;priseHistory|历史荣誉|string||
|&emsp;&emsp;remarkLevel||string||
|&emsp;&emsp;resumeContent|简历内容|string||
|&emsp;&emsp;scoreOrder||string||
|&emsp;&emsp;serialNum||integer(int32)||
|&emsp;&emsp;sex|性别|string||
|&emsp;&emsp;status||string(byte)||
|&emsp;&emsp;studentFrom||string||
|&emsp;&emsp;studentKind|考生类别|string||
|&emsp;&emsp;studentName|姓名|string||
|&emsp;&emsp;sumScore|总分|string||
|&emsp;&emsp;verifyPassword||string||
|&emsp;&emsp;withConnectionOne|家庭成员关系1|string||
|&emsp;&emsp;withConnectionSecond|家庭成员关系2|string||
|&emsp;&emsp;workPlaceOne|工作地点1|string||
|&emsp;&emsp;workPlaceSecond|工作地点2|string||
|totalNum||integer(int32)|integer(int32)|


**响应示例**:
```javascript
{
	"data": [
		{
			"address": "",
			"agroSingleton": true,
			"agroTwoDauLigation": true,
			"archiveCode": "",
			"beginTime": "",
			"birth": "",
			"chineseLevel": "",
			"chymistLevel": "",
			"className": "",
			"combinedScore": "",
			"comeFrom": "",
			"diathesis": "",
			"endTime": "",
			"englishLevel": "",
			"experiment": "",
			"finishSchoolCode": "",
			"finishSchoolName": "",
			"graduateDate": "",
			"homePlace": "",
			"householdAddressOne": "",
			"householdAddressSecond": "",
			"identityCode": "",
			"imageSrc": "",
			"isAreaStudent": 0,
			"isMilitary": 0,
			"mathLevel": "",
			"nationCode": "",
			"numbersOne": "",
			"numbersSecond": "",
			"opinion": "",
			"phoneCode": "",
			"phoneOne": "",
			"phoneSecond": "",
			"physicsLevel": "",
			"politicsLevel": "",
			"polity": "",
			"postCode": "",
			"priseHistory": "",
			"remarkLevel": "",
			"resumeContent": "",
			"scoreOrder": "",
			"serialNum": 0,
			"sex": "",
			"status": "",
			"studentFrom": "",
			"studentKind": "",
			"studentName": "",
			"sumScore": "",
			"verifyPassword": "",
			"withConnectionOne": "",
			"withConnectionSecond": "",
			"workPlaceOne": "",
			"workPlaceSecond": ""
		}
	],
	"totalNum": 0
}
```


## 学校端补录-获取学校代码和名称


**接口地址**:`/nnzk/alter/privateHighSchool/getSchoolCodeAndName`


**请求方式**:`GET`


**请求数据类型**:`application/x-www-form-urlencoded`


**响应数据类型**:`*/*`


**接口描述**:<p>学校端补录-获取学校代码和名称</p>



**请求参数**:


暂无


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«SchoolCodeAndNameDTO»|
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|SchoolCodeAndNameDTO|SchoolCodeAndNameDTO|
|&emsp;&emsp;schoolCode|学校代码|string||
|&emsp;&emsp;schoolName|学校名称|string||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": {
		"schoolCode": "",
		"schoolName": ""
	},
	"success": true,
	"timestamp": 0
}
```


## 放弃录取


**接口地址**:`/nnzk/alter/privateHighSchool/giveUpMatriculate`


**请求方式**:`POST`


**请求数据类型**:`application/json`


**响应数据类型**:`*/*`


**接口描述**:<p>放弃录取</p>



**请求示例**:


```javascript
{
  "archiveCode": ""
}
```


**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|input|input|body|true|GiveUpMatriculateDTO|GiveUpMatriculateDTO|
|&emsp;&emsp;archiveCode|||false|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«string»|
|201|Created||
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|string||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": "",
	"success": true,
	"timestamp": 0
}
```


# 学校简介表


## 学校简介表-添加


**接口地址**:`/nnzk/base/profileOfSchool/add`


**请求方式**:`POST`


**请求数据类型**:`application/json`


**响应数据类型**:`*/*`


**接口描述**:<p>学校简介表-添加</p>



**请求示例**:


```javascript
{
  "createBy": "",
  "createTime": "",
  "delFlag": 0,
  "fileOfSchoolProfile": "",
  "id": "",
  "isDisplay": 0,
  "schoolCode": "",
  "schoolName": "",
  "schoolType": "",
  "updateBy": "",
  "updateTime": ""
}
```


**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|profileOfSchool|学校简介表|body|true|profile_of_school对象|profile_of_school对象|
|&emsp;&emsp;createBy|创建人||false|string||
|&emsp;&emsp;createTime|创建日期||false|string(date-time)||
|&emsp;&emsp;delFlag|删除标识||false|integer(int32)||
|&emsp;&emsp;fileOfSchoolProfile|学校简介文件||false|string||
|&emsp;&emsp;id|主键||false|string||
|&emsp;&emsp;isDisplay|是否显示||false|integer(int32)||
|&emsp;&emsp;schoolCode|学校代码||false|string||
|&emsp;&emsp;schoolName|学校名称||false|string||
|&emsp;&emsp;schoolType|学校类型||false|string||
|&emsp;&emsp;updateBy|更新人||false|string||
|&emsp;&emsp;updateTime|更新日期||false|string(date-time)||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«string»|
|201|Created||
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|string||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": "",
	"success": true,
	"timestamp": 0
}
```


## 学校简介表-通过id删除


**接口地址**:`/nnzk/base/profileOfSchool/delete`


**请求方式**:`DELETE`


**请求数据类型**:`application/x-www-form-urlencoded`


**响应数据类型**:`*/*`


**接口描述**:<p>学校简介表-通过id删除</p>



**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|id|id|query|true|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«string»|
|204|No Content||
|401|Unauthorized||
|403|Forbidden||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|string||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": "",
	"success": true,
	"timestamp": 0
}
```


## 学校简介表-批量删除


**接口地址**:`/nnzk/base/profileOfSchool/deleteBatch`


**请求方式**:`DELETE`


**请求数据类型**:`application/x-www-form-urlencoded`


**响应数据类型**:`*/*`


**接口描述**:<p>学校简介表-批量删除</p>



**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|ids|ids|query|true|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«string»|
|204|No Content||
|401|Unauthorized||
|403|Forbidden||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|string||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": "",
	"success": true,
	"timestamp": 0
}
```


## 学校简介表-编辑


**接口地址**:`/nnzk/base/profileOfSchool/edit`


**请求方式**:`POST`


**请求数据类型**:`application/json`


**响应数据类型**:`*/*`


**接口描述**:<p>学校简介表-编辑</p>



**请求示例**:


```javascript
{
  "createBy": "",
  "createTime": "",
  "delFlag": 0,
  "fileOfSchoolProfile": "",
  "id": "",
  "isDisplay": 0,
  "schoolCode": "",
  "schoolName": "",
  "schoolType": "",
  "updateBy": "",
  "updateTime": ""
}
```


**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|profileOfSchool|学校简介表|body|true|profile_of_school对象|profile_of_school对象|
|&emsp;&emsp;createBy|创建人||false|string||
|&emsp;&emsp;createTime|创建日期||false|string(date-time)||
|&emsp;&emsp;delFlag|删除标识||false|integer(int32)||
|&emsp;&emsp;fileOfSchoolProfile|学校简介文件||false|string||
|&emsp;&emsp;id|主键||false|string||
|&emsp;&emsp;isDisplay|是否显示||false|integer(int32)||
|&emsp;&emsp;schoolCode|学校代码||false|string||
|&emsp;&emsp;schoolName|学校名称||false|string||
|&emsp;&emsp;schoolType|学校类型||false|string||
|&emsp;&emsp;updateBy|更新人||false|string||
|&emsp;&emsp;updateTime|更新日期||false|string(date-time)||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«string»|
|201|Created||
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|string||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": "",
	"success": true,
	"timestamp": 0
}
```


## 学校简介表-编辑


**接口地址**:`/nnzk/base/profileOfSchool/edit`


**请求方式**:`PUT`


**请求数据类型**:`application/json`


**响应数据类型**:`*/*`


**接口描述**:<p>学校简介表-编辑</p>



**请求示例**:


```javascript
{
  "createBy": "",
  "createTime": "",
  "delFlag": 0,
  "fileOfSchoolProfile": "",
  "id": "",
  "isDisplay": 0,
  "schoolCode": "",
  "schoolName": "",
  "schoolType": "",
  "updateBy": "",
  "updateTime": ""
}
```


**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|profileOfSchool|学校简介表|body|true|profile_of_school对象|profile_of_school对象|
|&emsp;&emsp;createBy|创建人||false|string||
|&emsp;&emsp;createTime|创建日期||false|string(date-time)||
|&emsp;&emsp;delFlag|删除标识||false|integer(int32)||
|&emsp;&emsp;fileOfSchoolProfile|学校简介文件||false|string||
|&emsp;&emsp;id|主键||false|string||
|&emsp;&emsp;isDisplay|是否显示||false|integer(int32)||
|&emsp;&emsp;schoolCode|学校代码||false|string||
|&emsp;&emsp;schoolName|学校名称||false|string||
|&emsp;&emsp;schoolType|学校类型||false|string||
|&emsp;&emsp;updateBy|更新人||false|string||
|&emsp;&emsp;updateTime|更新日期||false|string(date-time)||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«string»|
|201|Created||
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|string||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": "",
	"success": true,
	"timestamp": 0
}
```


## 学校简介表-初始化


**接口地址**:`/nnzk/base/profileOfSchool/initialize`


**请求方式**:`PUT`


**请求数据类型**:`application/json`


**响应数据类型**:`*/*`


**接口描述**:<p>学校简介表-初始化</p>



**请求参数**:


暂无


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«string»|
|201|Created||
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|string||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": "",
	"success": true,
	"timestamp": 0
}
```


## 学校简介表-分页列表查询


**接口地址**:`/nnzk/base/profileOfSchool/list`


**请求方式**:`GET`


**请求数据类型**:`application/x-www-form-urlencoded`


**响应数据类型**:`*/*`


**接口描述**:<p>学校简介表-分页列表查询</p>



**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|isDisplay|是否显示|query|true|integer(int32)||
|schoolCode|学校代码|query|true|string||
|schoolName|学校名称|query|true|string||
|schoolType|学校类型|query|true|string||
|createBy|创建人|query|false|string||
|createTime|创建日期|query|false|string(date-time)||
|delFlag|删除标识|query|false|integer(int32)||
|fileOfSchoolProfile|学校简介文件|query|false|string||
|id|主键|query|false|string||
|pageNo|pageNo|query|false|integer(int32)||
|pageSize|pageSize|query|false|integer(int32)||
|updateBy|更新人|query|false|string||
|updateTime|更新日期|query|false|string(date-time)||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«IPage«profile_of_school对象»»|
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|IPage«profile_of_school对象»|IPage«profile_of_school对象»|
|&emsp;&emsp;current||integer(int64)||
|&emsp;&emsp;pages||integer(int64)||
|&emsp;&emsp;records||array|profile_of_school对象|
|&emsp;&emsp;&emsp;&emsp;createBy|创建人|string||
|&emsp;&emsp;&emsp;&emsp;createTime|创建日期|string||
|&emsp;&emsp;&emsp;&emsp;delFlag|删除标识|integer||
|&emsp;&emsp;&emsp;&emsp;fileOfSchoolProfile|学校简介文件|string||
|&emsp;&emsp;&emsp;&emsp;id|主键|string||
|&emsp;&emsp;&emsp;&emsp;isDisplay|是否显示|integer||
|&emsp;&emsp;&emsp;&emsp;schoolCode|学校代码|string||
|&emsp;&emsp;&emsp;&emsp;schoolName|学校名称|string||
|&emsp;&emsp;&emsp;&emsp;schoolType|学校类型|string||
|&emsp;&emsp;&emsp;&emsp;updateBy|更新人|string||
|&emsp;&emsp;&emsp;&emsp;updateTime|更新日期|string||
|&emsp;&emsp;size||integer(int64)||
|&emsp;&emsp;total||integer(int64)||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": {
		"current": 0,
		"pages": 0,
		"records": [
			{
				"createBy": "",
				"createTime": "",
				"delFlag": 0,
				"fileOfSchoolProfile": "",
				"id": "",
				"isDisplay": 0,
				"schoolCode": "",
				"schoolName": "",
				"schoolType": "",
				"updateBy": "",
				"updateTime": ""
			}
		],
		"size": 0,
		"total": 0
	},
	"success": true,
	"timestamp": 0
}
```


## 学校简介表-学生端列表查询


**接口地址**:`/nnzk/base/profileOfSchool/profileOfSchoolList`


**请求方式**:`GET`


**请求数据类型**:`application/x-www-form-urlencoded`


**响应数据类型**:`*/*`


**接口描述**:<p>学校简介表-学生端列表查询</p>



**请求参数**:


暂无


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«List«ProfileOfSchoolVO»»|
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|array|ProfileOfSchoolVO|
|&emsp;&emsp;fileOfSchoolProfile|学校简介文件|string||
|&emsp;&emsp;id|主键|string||
|&emsp;&emsp;isDisplay|是否显示|integer(int32)||
|&emsp;&emsp;schoolCode|学校代码|string||
|&emsp;&emsp;schoolName|学校名称|string||
|&emsp;&emsp;schoolType|学校类型|string||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": [
		{
			"fileOfSchoolProfile": "",
			"id": "",
			"isDisplay": 0,
			"schoolCode": "",
			"schoolName": "",
			"schoolType": ""
		}
	],
	"success": true,
	"timestamp": 0
}
```


## 学校简介表-通过id查询


**接口地址**:`/nnzk/base/profileOfSchool/queryById`


**请求方式**:`GET`


**请求数据类型**:`application/x-www-form-urlencoded`


**响应数据类型**:`*/*`


**接口描述**:<p>学校简介表-通过id查询</p>



**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|id|id|query|true|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«profile_of_school对象»|
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|profile_of_school对象|profile_of_school对象|
|&emsp;&emsp;createBy|创建人|string||
|&emsp;&emsp;createTime|创建日期|string(date-time)||
|&emsp;&emsp;delFlag|删除标识|integer(int32)||
|&emsp;&emsp;fileOfSchoolProfile|学校简介文件|string||
|&emsp;&emsp;id|主键|string||
|&emsp;&emsp;isDisplay|是否显示|integer(int32)||
|&emsp;&emsp;schoolCode|学校代码|string||
|&emsp;&emsp;schoolName|学校名称|string||
|&emsp;&emsp;schoolType|学校类型|string||
|&emsp;&emsp;updateBy|更新人|string||
|&emsp;&emsp;updateTime|更新日期|string(date-time)||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": {
		"createBy": "",
		"createTime": "",
		"delFlag": 0,
		"fileOfSchoolProfile": "",
		"id": "",
		"isDisplay": 0,
		"schoolCode": "",
		"schoolName": "",
		"schoolType": "",
		"updateBy": "",
		"updateTime": ""
	},
	"success": true,
	"timestamp": 0
}
```


# 学校统计信息


## 学校统计信息-添加


**接口地址**:`/nnzk/base/schoolStatisticsData/add`


**请求方式**:`POST`


**请求数据类型**:`application/json`


**响应数据类型**:`*/*`


**接口描述**:<p>学校统计信息-添加</p>



**请求示例**:


```javascript
{
  "aboveAlterLevel": 0,
  "aboveDirLevel": 0,
  "aboveGuideLevel": 0,
  "aboveInstLevel": 0,
  "alterAppose": 0,
  "alterLevel": "",
  "alterOrderCode": "",
  "dirAppose": 0,
  "dirLevel": "",
  "dirOrderCode": "",
  "dirPlan": 0,
  "guideAppose": 0,
  "guideLevel": "",
  "guideNum": 0,
  "guideOrderCode": "",
  "guidePlan": 0,
  "hguideScore": "",
  "hinstScore": "",
  "hscore": "",
  "id": "",
  "instAppose": 0,
  "instLevel": "",
  "instNum": 0,
  "instOrderCode": "",
  "instPlan": 0,
  "lguideScore": "",
  "linstScore": "",
  "lscore": "",
  "runtime": "",
  "schoolCode": "",
  "schoolName": "",
  "signupNum": 0
}
```


**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|schoolStatisticsData|学校统计信息|body|true|school_statistics_data对象|school_statistics_data对象|
|&emsp;&emsp;aboveAlterLevel|补录入围人数||false|integer(int32)||
|&emsp;&emsp;aboveDirLevel|定向入围人数||false|integer(int32)||
|&emsp;&emsp;aboveGuideLevel|指导入围人数||false|integer(int32)||
|&emsp;&emsp;aboveInstLevel|指令入围人数||false|integer(int32)||
|&emsp;&emsp;alterAppose|补录并列人数||false|integer(int32)||
|&emsp;&emsp;alterLevel|补录等级线||false|string||
|&emsp;&emsp;alterOrderCode|补录成绩顺序号||false|string||
|&emsp;&emsp;dirAppose|定向并列人数||false|integer(int32)||
|&emsp;&emsp;dirLevel|定向等级线||false|string||
|&emsp;&emsp;dirOrderCode|定向成绩顺序号||false|string||
|&emsp;&emsp;dirPlan|定向计划数||false|integer(int32)||
|&emsp;&emsp;guideAppose|指导并列人数||false|integer(int32)||
|&emsp;&emsp;guideLevel|指导等级线||false|string||
|&emsp;&emsp;guideNum|指导报名数||false|integer(int32)||
|&emsp;&emsp;guideOrderCode|指导成绩顺序号||false|string||
|&emsp;&emsp;guidePlan|指导计划数||false|integer(int32)||
|&emsp;&emsp;hguideScore|指导最高分数||false|string||
|&emsp;&emsp;hinstScore|指令最高分数||false|string||
|&emsp;&emsp;hscore|最高分数||false|string||
|&emsp;&emsp;id|主键||false|string||
|&emsp;&emsp;instAppose|指令并列人数||false|integer(int32)||
|&emsp;&emsp;instLevel|指令等级线||false|string||
|&emsp;&emsp;instNum|指令报名数||false|integer(int32)||
|&emsp;&emsp;instOrderCode|指令成绩顺序号||false|string||
|&emsp;&emsp;instPlan|指令计划数||false|integer(int32)||
|&emsp;&emsp;lguideScore|指导最低分数||false|string||
|&emsp;&emsp;linstScore|指令最低分数||false|string||
|&emsp;&emsp;lscore|最低分数||false|string||
|&emsp;&emsp;runtime|运算时间||false|string(date-time)||
|&emsp;&emsp;schoolCode|学校代码||false|string||
|&emsp;&emsp;schoolName|学校名称||false|string||
|&emsp;&emsp;signupNum|报名人数||false|integer(int32)||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«string»|
|201|Created||
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|string||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": "",
	"success": true,
	"timestamp": 0
}
```


## 学校统计信息-通过id删除


**接口地址**:`/nnzk/base/schoolStatisticsData/delete`


**请求方式**:`DELETE`


**请求数据类型**:`application/x-www-form-urlencoded`


**响应数据类型**:`*/*`


**接口描述**:<p>学校统计信息-通过id删除</p>



**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|id|id|query|true|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«string»|
|204|No Content||
|401|Unauthorized||
|403|Forbidden||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|string||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": "",
	"success": true,
	"timestamp": 0
}
```


## 学校统计信息-批量删除


**接口地址**:`/nnzk/base/schoolStatisticsData/deleteBatch`


**请求方式**:`DELETE`


**请求数据类型**:`application/x-www-form-urlencoded`


**响应数据类型**:`*/*`


**接口描述**:<p>学校统计信息-批量删除</p>



**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|ids|ids|query|true|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«string»|
|204|No Content||
|401|Unauthorized||
|403|Forbidden||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|string||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": "",
	"success": true,
	"timestamp": 0
}
```


## 学校统计信息-编辑


**接口地址**:`/nnzk/base/schoolStatisticsData/edit`


**请求方式**:`POST`


**请求数据类型**:`application/json`


**响应数据类型**:`*/*`


**接口描述**:<p>学校统计信息-编辑</p>



**请求示例**:


```javascript
{
  "aboveAlterLevel": 0,
  "aboveDirLevel": 0,
  "aboveGuideLevel": 0,
  "aboveInstLevel": 0,
  "alterAppose": 0,
  "alterLevel": "",
  "alterOrderCode": "",
  "dirAppose": 0,
  "dirLevel": "",
  "dirOrderCode": "",
  "dirPlan": 0,
  "guideAppose": 0,
  "guideLevel": "",
  "guideNum": 0,
  "guideOrderCode": "",
  "guidePlan": 0,
  "hguideScore": "",
  "hinstScore": "",
  "hscore": "",
  "id": "",
  "instAppose": 0,
  "instLevel": "",
  "instNum": 0,
  "instOrderCode": "",
  "instPlan": 0,
  "lguideScore": "",
  "linstScore": "",
  "lscore": "",
  "runtime": "",
  "schoolCode": "",
  "schoolName": "",
  "signupNum": 0
}
```


**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|schoolStatisticsData|学校统计信息|body|true|school_statistics_data对象|school_statistics_data对象|
|&emsp;&emsp;aboveAlterLevel|补录入围人数||false|integer(int32)||
|&emsp;&emsp;aboveDirLevel|定向入围人数||false|integer(int32)||
|&emsp;&emsp;aboveGuideLevel|指导入围人数||false|integer(int32)||
|&emsp;&emsp;aboveInstLevel|指令入围人数||false|integer(int32)||
|&emsp;&emsp;alterAppose|补录并列人数||false|integer(int32)||
|&emsp;&emsp;alterLevel|补录等级线||false|string||
|&emsp;&emsp;alterOrderCode|补录成绩顺序号||false|string||
|&emsp;&emsp;dirAppose|定向并列人数||false|integer(int32)||
|&emsp;&emsp;dirLevel|定向等级线||false|string||
|&emsp;&emsp;dirOrderCode|定向成绩顺序号||false|string||
|&emsp;&emsp;dirPlan|定向计划数||false|integer(int32)||
|&emsp;&emsp;guideAppose|指导并列人数||false|integer(int32)||
|&emsp;&emsp;guideLevel|指导等级线||false|string||
|&emsp;&emsp;guideNum|指导报名数||false|integer(int32)||
|&emsp;&emsp;guideOrderCode|指导成绩顺序号||false|string||
|&emsp;&emsp;guidePlan|指导计划数||false|integer(int32)||
|&emsp;&emsp;hguideScore|指导最高分数||false|string||
|&emsp;&emsp;hinstScore|指令最高分数||false|string||
|&emsp;&emsp;hscore|最高分数||false|string||
|&emsp;&emsp;id|主键||false|string||
|&emsp;&emsp;instAppose|指令并列人数||false|integer(int32)||
|&emsp;&emsp;instLevel|指令等级线||false|string||
|&emsp;&emsp;instNum|指令报名数||false|integer(int32)||
|&emsp;&emsp;instOrderCode|指令成绩顺序号||false|string||
|&emsp;&emsp;instPlan|指令计划数||false|integer(int32)||
|&emsp;&emsp;lguideScore|指导最低分数||false|string||
|&emsp;&emsp;linstScore|指令最低分数||false|string||
|&emsp;&emsp;lscore|最低分数||false|string||
|&emsp;&emsp;runtime|运算时间||false|string(date-time)||
|&emsp;&emsp;schoolCode|学校代码||false|string||
|&emsp;&emsp;schoolName|学校名称||false|string||
|&emsp;&emsp;signupNum|报名人数||false|integer(int32)||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«string»|
|201|Created||
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|string||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": "",
	"success": true,
	"timestamp": 0
}
```


## 学校统计信息-编辑


**接口地址**:`/nnzk/base/schoolStatisticsData/edit`


**请求方式**:`PUT`


**请求数据类型**:`application/json`


**响应数据类型**:`*/*`


**接口描述**:<p>学校统计信息-编辑</p>



**请求示例**:


```javascript
{
  "aboveAlterLevel": 0,
  "aboveDirLevel": 0,
  "aboveGuideLevel": 0,
  "aboveInstLevel": 0,
  "alterAppose": 0,
  "alterLevel": "",
  "alterOrderCode": "",
  "dirAppose": 0,
  "dirLevel": "",
  "dirOrderCode": "",
  "dirPlan": 0,
  "guideAppose": 0,
  "guideLevel": "",
  "guideNum": 0,
  "guideOrderCode": "",
  "guidePlan": 0,
  "hguideScore": "",
  "hinstScore": "",
  "hscore": "",
  "id": "",
  "instAppose": 0,
  "instLevel": "",
  "instNum": 0,
  "instOrderCode": "",
  "instPlan": 0,
  "lguideScore": "",
  "linstScore": "",
  "lscore": "",
  "runtime": "",
  "schoolCode": "",
  "schoolName": "",
  "signupNum": 0
}
```


**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|schoolStatisticsData|学校统计信息|body|true|school_statistics_data对象|school_statistics_data对象|
|&emsp;&emsp;aboveAlterLevel|补录入围人数||false|integer(int32)||
|&emsp;&emsp;aboveDirLevel|定向入围人数||false|integer(int32)||
|&emsp;&emsp;aboveGuideLevel|指导入围人数||false|integer(int32)||
|&emsp;&emsp;aboveInstLevel|指令入围人数||false|integer(int32)||
|&emsp;&emsp;alterAppose|补录并列人数||false|integer(int32)||
|&emsp;&emsp;alterLevel|补录等级线||false|string||
|&emsp;&emsp;alterOrderCode|补录成绩顺序号||false|string||
|&emsp;&emsp;dirAppose|定向并列人数||false|integer(int32)||
|&emsp;&emsp;dirLevel|定向等级线||false|string||
|&emsp;&emsp;dirOrderCode|定向成绩顺序号||false|string||
|&emsp;&emsp;dirPlan|定向计划数||false|integer(int32)||
|&emsp;&emsp;guideAppose|指导并列人数||false|integer(int32)||
|&emsp;&emsp;guideLevel|指导等级线||false|string||
|&emsp;&emsp;guideNum|指导报名数||false|integer(int32)||
|&emsp;&emsp;guideOrderCode|指导成绩顺序号||false|string||
|&emsp;&emsp;guidePlan|指导计划数||false|integer(int32)||
|&emsp;&emsp;hguideScore|指导最高分数||false|string||
|&emsp;&emsp;hinstScore|指令最高分数||false|string||
|&emsp;&emsp;hscore|最高分数||false|string||
|&emsp;&emsp;id|主键||false|string||
|&emsp;&emsp;instAppose|指令并列人数||false|integer(int32)||
|&emsp;&emsp;instLevel|指令等级线||false|string||
|&emsp;&emsp;instNum|指令报名数||false|integer(int32)||
|&emsp;&emsp;instOrderCode|指令成绩顺序号||false|string||
|&emsp;&emsp;instPlan|指令计划数||false|integer(int32)||
|&emsp;&emsp;lguideScore|指导最低分数||false|string||
|&emsp;&emsp;linstScore|指令最低分数||false|string||
|&emsp;&emsp;lscore|最低分数||false|string||
|&emsp;&emsp;runtime|运算时间||false|string(date-time)||
|&emsp;&emsp;schoolCode|学校代码||false|string||
|&emsp;&emsp;schoolName|学校名称||false|string||
|&emsp;&emsp;signupNum|报名人数||false|integer(int32)||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«string»|
|201|Created||
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|string||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": "",
	"success": true,
	"timestamp": 0
}
```


## 学校统计信息-查询单个学校统计


**接口地址**:`/nnzk/base/schoolStatisticsData/getOne`


**请求方式**:`GET`


**请求数据类型**:`application/x-www-form-urlencoded`


**响应数据类型**:`*/*`


**接口描述**:<p>学校统计信息-查询单个学校统计</p>



**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|highSchoolCode|highSchoolCode|query|true|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«SchoolStatisticsDataDTO»|
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|SchoolStatisticsDataDTO|SchoolStatisticsDataDTO|
|&emsp;&emsp;aboveAlterLevel|补录入围人数|integer(int32)||
|&emsp;&emsp;aboveDirLevel|定向入围人数|integer(int32)||
|&emsp;&emsp;aboveGuideLevel|指导入围人数|integer(int32)||
|&emsp;&emsp;aboveInstLevel|指令入围人数|integer(int32)||
|&emsp;&emsp;alterAppose|补录并列人数|integer(int32)||
|&emsp;&emsp;alterLevel|补录等级线|string||
|&emsp;&emsp;alterOrderCode|补录成绩顺序号|string||
|&emsp;&emsp;alterPlan|补录人数|integer(int32)||
|&emsp;&emsp;dirAppose|定向并列人数|integer(int32)||
|&emsp;&emsp;dirLevel|定向等级线|string||
|&emsp;&emsp;dirOrderCode|定向成绩顺序号|string||
|&emsp;&emsp;dirPlan|定向计划数|integer(int32)||
|&emsp;&emsp;guideAppose|指导并列人数|integer(int32)||
|&emsp;&emsp;guideLevel|指导等级线|string||
|&emsp;&emsp;guideNum|指导报名数|integer(int32)||
|&emsp;&emsp;guideOrderCode|指导成绩顺序号|string||
|&emsp;&emsp;guidePlan|指导计划数|integer(int32)||
|&emsp;&emsp;hguideScore|指导最高分数|string||
|&emsp;&emsp;hinstScore|指令最高分数|string||
|&emsp;&emsp;hscore|最高分数|string||
|&emsp;&emsp;instAppose|指令并列人数|integer(int32)||
|&emsp;&emsp;instLevel|指令等级线|string||
|&emsp;&emsp;instNum|指令报名数|integer(int32)||
|&emsp;&emsp;instOrderCode|指令成绩顺序号|string||
|&emsp;&emsp;instPlan|指令计划数|integer(int32)||
|&emsp;&emsp;lguideScore|指导最低分数|string||
|&emsp;&emsp;linstScore|指令最低分数|string||
|&emsp;&emsp;lscore|最低分数|string||
|&emsp;&emsp;runtime|运算时间|string(date-time)||
|&emsp;&emsp;schoolCode|学校代码|string||
|&emsp;&emsp;schoolName|学校名称|string||
|&emsp;&emsp;signupNum|报名人数|integer(int32)||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": {
		"aboveAlterLevel": 0,
		"aboveDirLevel": 0,
		"aboveGuideLevel": 0,
		"aboveInstLevel": 0,
		"alterAppose": 0,
		"alterLevel": "",
		"alterOrderCode": "",
		"alterPlan": 0,
		"dirAppose": 0,
		"dirLevel": "",
		"dirOrderCode": "",
		"dirPlan": 0,
		"guideAppose": 0,
		"guideLevel": "",
		"guideNum": 0,
		"guideOrderCode": "",
		"guidePlan": 0,
		"hguideScore": "",
		"hinstScore": "",
		"hscore": "",
		"instAppose": 0,
		"instLevel": "",
		"instNum": 0,
		"instOrderCode": "",
		"instPlan": 0,
		"lguideScore": "",
		"linstScore": "",
		"lscore": "",
		"runtime": "",
		"schoolCode": "",
		"schoolName": "",
		"signupNum": 0
	},
	"success": true,
	"timestamp": 0
}
```


## 学校统计信息-分页列表查询


**接口地址**:`/nnzk/base/schoolStatisticsData/list`


**请求方式**:`GET`


**请求数据类型**:`application/x-www-form-urlencoded`


**响应数据类型**:`*/*`


**接口描述**:<p>学校统计信息-分页列表查询</p>



**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|aboveAlterLevel|补录入围人数|query|false|integer(int32)||
|aboveDirLevel|定向入围人数|query|false|integer(int32)||
|aboveGuideLevel|指导入围人数|query|false|integer(int32)||
|aboveInstLevel|指令入围人数|query|false|integer(int32)||
|alterAppose|补录并列人数|query|false|integer(int32)||
|alterLevel|补录等级线|query|false|string||
|alterOrderCode|补录成绩顺序号|query|false|string||
|dirAppose|定向并列人数|query|false|integer(int32)||
|dirLevel|定向等级线|query|false|string||
|dirOrderCode|定向成绩顺序号|query|false|string||
|dirPlan|定向计划数|query|false|integer(int32)||
|guideAppose|指导并列人数|query|false|integer(int32)||
|guideLevel|指导等级线|query|false|string||
|guideNum|指导报名数|query|false|integer(int32)||
|guideOrderCode|指导成绩顺序号|query|false|string||
|guidePlan|指导计划数|query|false|integer(int32)||
|hguideScore|指导最高分数|query|false|string||
|hinstScore|指令最高分数|query|false|string||
|hscore|最高分数|query|false|string||
|id|主键|query|false|string||
|instAppose|指令并列人数|query|false|integer(int32)||
|instLevel|指令等级线|query|false|string||
|instNum|指令报名数|query|false|integer(int32)||
|instOrderCode|指令成绩顺序号|query|false|string||
|instPlan|指令计划数|query|false|integer(int32)||
|lguideScore|指导最低分数|query|false|string||
|linstScore|指令最低分数|query|false|string||
|lscore|最低分数|query|false|string||
|pageNo|pageNo|query|false|integer(int32)||
|pageSize|pageSize|query|false|integer(int32)||
|runtime|运算时间|query|false|string(date-time)||
|schoolCode|学校代码|query|false|string||
|schoolName|学校名称|query|false|string||
|signupNum|报名人数|query|false|integer(int32)||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«IPage«school_statistics_data对象»»|
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|IPage«school_statistics_data对象»|IPage«school_statistics_data对象»|
|&emsp;&emsp;current||integer(int64)||
|&emsp;&emsp;pages||integer(int64)||
|&emsp;&emsp;records||array|school_statistics_data对象|
|&emsp;&emsp;&emsp;&emsp;aboveAlterLevel|补录入围人数|integer||
|&emsp;&emsp;&emsp;&emsp;aboveDirLevel|定向入围人数|integer||
|&emsp;&emsp;&emsp;&emsp;aboveGuideLevel|指导入围人数|integer||
|&emsp;&emsp;&emsp;&emsp;aboveInstLevel|指令入围人数|integer||
|&emsp;&emsp;&emsp;&emsp;alterAppose|补录并列人数|integer||
|&emsp;&emsp;&emsp;&emsp;alterLevel|补录等级线|string||
|&emsp;&emsp;&emsp;&emsp;alterOrderCode|补录成绩顺序号|string||
|&emsp;&emsp;&emsp;&emsp;dirAppose|定向并列人数|integer||
|&emsp;&emsp;&emsp;&emsp;dirLevel|定向等级线|string||
|&emsp;&emsp;&emsp;&emsp;dirOrderCode|定向成绩顺序号|string||
|&emsp;&emsp;&emsp;&emsp;dirPlan|定向计划数|integer||
|&emsp;&emsp;&emsp;&emsp;guideAppose|指导并列人数|integer||
|&emsp;&emsp;&emsp;&emsp;guideLevel|指导等级线|string||
|&emsp;&emsp;&emsp;&emsp;guideNum|指导报名数|integer||
|&emsp;&emsp;&emsp;&emsp;guideOrderCode|指导成绩顺序号|string||
|&emsp;&emsp;&emsp;&emsp;guidePlan|指导计划数|integer||
|&emsp;&emsp;&emsp;&emsp;hguideScore|指导最高分数|string||
|&emsp;&emsp;&emsp;&emsp;hinstScore|指令最高分数|string||
|&emsp;&emsp;&emsp;&emsp;hscore|最高分数|string||
|&emsp;&emsp;&emsp;&emsp;id|主键|string||
|&emsp;&emsp;&emsp;&emsp;instAppose|指令并列人数|integer||
|&emsp;&emsp;&emsp;&emsp;instLevel|指令等级线|string||
|&emsp;&emsp;&emsp;&emsp;instNum|指令报名数|integer||
|&emsp;&emsp;&emsp;&emsp;instOrderCode|指令成绩顺序号|string||
|&emsp;&emsp;&emsp;&emsp;instPlan|指令计划数|integer||
|&emsp;&emsp;&emsp;&emsp;lguideScore|指导最低分数|string||
|&emsp;&emsp;&emsp;&emsp;linstScore|指令最低分数|string||
|&emsp;&emsp;&emsp;&emsp;lscore|最低分数|string||
|&emsp;&emsp;&emsp;&emsp;runtime|运算时间|string||
|&emsp;&emsp;&emsp;&emsp;schoolCode|学校代码|string||
|&emsp;&emsp;&emsp;&emsp;schoolName|学校名称|string||
|&emsp;&emsp;&emsp;&emsp;signupNum|报名人数|integer||
|&emsp;&emsp;size||integer(int64)||
|&emsp;&emsp;total||integer(int64)||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": {
		"current": 0,
		"pages": 0,
		"records": [
			{
				"aboveAlterLevel": 0,
				"aboveDirLevel": 0,
				"aboveGuideLevel": 0,
				"aboveInstLevel": 0,
				"alterAppose": 0,
				"alterLevel": "",
				"alterOrderCode": "",
				"dirAppose": 0,
				"dirLevel": "",
				"dirOrderCode": "",
				"dirPlan": 0,
				"guideAppose": 0,
				"guideLevel": "",
				"guideNum": 0,
				"guideOrderCode": "",
				"guidePlan": 0,
				"hguideScore": "",
				"hinstScore": "",
				"hscore": "",
				"id": "",
				"instAppose": 0,
				"instLevel": "",
				"instNum": 0,
				"instOrderCode": "",
				"instPlan": 0,
				"lguideScore": "",
				"linstScore": "",
				"lscore": "",
				"runtime": "",
				"schoolCode": "",
				"schoolName": "",
				"signupNum": 0
			}
		],
		"size": 0,
		"total": 0
	},
	"success": true,
	"timestamp": 0
}
```


## 学校统计信息-通过id查询


**接口地址**:`/nnzk/base/schoolStatisticsData/queryById`


**请求方式**:`GET`


**请求数据类型**:`application/x-www-form-urlencoded`


**响应数据类型**:`*/*`


**接口描述**:<p>学校统计信息-通过id查询</p>



**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|id|id|query|true|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«school_statistics_data对象»|
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|school_statistics_data对象|school_statistics_data对象|
|&emsp;&emsp;aboveAlterLevel|补录入围人数|integer(int32)||
|&emsp;&emsp;aboveDirLevel|定向入围人数|integer(int32)||
|&emsp;&emsp;aboveGuideLevel|指导入围人数|integer(int32)||
|&emsp;&emsp;aboveInstLevel|指令入围人数|integer(int32)||
|&emsp;&emsp;alterAppose|补录并列人数|integer(int32)||
|&emsp;&emsp;alterLevel|补录等级线|string||
|&emsp;&emsp;alterOrderCode|补录成绩顺序号|string||
|&emsp;&emsp;dirAppose|定向并列人数|integer(int32)||
|&emsp;&emsp;dirLevel|定向等级线|string||
|&emsp;&emsp;dirOrderCode|定向成绩顺序号|string||
|&emsp;&emsp;dirPlan|定向计划数|integer(int32)||
|&emsp;&emsp;guideAppose|指导并列人数|integer(int32)||
|&emsp;&emsp;guideLevel|指导等级线|string||
|&emsp;&emsp;guideNum|指导报名数|integer(int32)||
|&emsp;&emsp;guideOrderCode|指导成绩顺序号|string||
|&emsp;&emsp;guidePlan|指导计划数|integer(int32)||
|&emsp;&emsp;hguideScore|指导最高分数|string||
|&emsp;&emsp;hinstScore|指令最高分数|string||
|&emsp;&emsp;hscore|最高分数|string||
|&emsp;&emsp;id|主键|string||
|&emsp;&emsp;instAppose|指令并列人数|integer(int32)||
|&emsp;&emsp;instLevel|指令等级线|string||
|&emsp;&emsp;instNum|指令报名数|integer(int32)||
|&emsp;&emsp;instOrderCode|指令成绩顺序号|string||
|&emsp;&emsp;instPlan|指令计划数|integer(int32)||
|&emsp;&emsp;lguideScore|指导最低分数|string||
|&emsp;&emsp;linstScore|指令最低分数|string||
|&emsp;&emsp;lscore|最低分数|string||
|&emsp;&emsp;runtime|运算时间|string(date-time)||
|&emsp;&emsp;schoolCode|学校代码|string||
|&emsp;&emsp;schoolName|学校名称|string||
|&emsp;&emsp;signupNum|报名人数|integer(int32)||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": {
		"aboveAlterLevel": 0,
		"aboveDirLevel": 0,
		"aboveGuideLevel": 0,
		"aboveInstLevel": 0,
		"alterAppose": 0,
		"alterLevel": "",
		"alterOrderCode": "",
		"dirAppose": 0,
		"dirLevel": "",
		"dirOrderCode": "",
		"dirPlan": 0,
		"guideAppose": 0,
		"guideLevel": "",
		"guideNum": 0,
		"guideOrderCode": "",
		"guidePlan": 0,
		"hguideScore": "",
		"hinstScore": "",
		"hscore": "",
		"id": "",
		"instAppose": 0,
		"instLevel": "",
		"instNum": 0,
		"instOrderCode": "",
		"instPlan": 0,
		"lguideScore": "",
		"linstScore": "",
		"lscore": "",
		"runtime": "",
		"schoolCode": "",
		"schoolName": "",
		"signupNum": 0
	},
	"success": true,
	"timestamp": 0
}
```


# 学生信息


## 学生信息-添加


**接口地址**:`/nnzk/student/studentInfo/add`


**请求方式**:`POST`


**请求数据类型**:`application/json`


**响应数据类型**:`*/*`


**接口描述**:<p>学生信息-添加</p>



**请求示例**:


```javascript
{
  "address": "",
  "archiveCode": "",
  "birth": "",
  "className": "",
  "createBy": "",
  "createTime": "",
  "delFlag": 0,
  "familyList": [
    {
      "archiveCode": "",
      "createBy": "",
      "createTime": "",
      "delFlag": 0,
      "householdAddress": "",
      "id": "",
      "numbers": "",
      "phone": "",
      "updateBy": "",
      "updateTime": "",
      "withConnection": "",
      "workPlace": ""
    }
  ],
  "finishSchoolCode": "",
  "graduateDate": "",
  "homePlace": "",
  "id": "",
  "identityCode": "",
  "isAreaStudent": 0,
  "isMilitary": 0,
  "nationCode": "",
  "phoneCode": "",
  "photosList": [
    {
      "archiveCode": "",
      "createBy": "",
      "createTime": "",
      "delFlag": 0,
      "id": "",
      "picture": "",
      "updateBy": "",
      "updateTime": ""
    }
  ],
  "polity": "",
  "postCode": "",
  "priseHistory": "",
  "resumeList": [
    {
      "archiveCode": "",
      "beginTime": "",
      "createBy": "",
      "createTime": "",
      "delFlag": 0,
      "endTime": "",
      "id": "",
      "resumeContent": "",
      "school": "",
      "updateBy": "",
      "updateTime": ""
    }
  ],
  "sex": "",
  "studentKind": "",
  "studentName": "",
  "updateBy": "",
  "updateTime": ""
}
```


**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|studentInfoPage|学生信息|body|true|student_infoPage对象|student_infoPage对象|
|&emsp;&emsp;address|现住地址||false|string||
|&emsp;&emsp;archiveCode|准考证号||false|string||
|&emsp;&emsp;birth|出生年月||false|string(date-time)||
|&emsp;&emsp;className|班级||false|string||
|&emsp;&emsp;createBy|创建人||false|string||
|&emsp;&emsp;createTime|创建日期||false|string(date-time)||
|&emsp;&emsp;delFlag|删除标识||false|integer(int32)||
|&emsp;&emsp;familyList|学生家庭表||false|array|family对象|
|&emsp;&emsp;&emsp;&emsp;archiveCode|准考证号||false|string||
|&emsp;&emsp;&emsp;&emsp;createBy|创建人||false|string||
|&emsp;&emsp;&emsp;&emsp;createTime|创建日期||false|string||
|&emsp;&emsp;&emsp;&emsp;delFlag|删除标识||false|integer||
|&emsp;&emsp;&emsp;&emsp;householdAddress|住址||false|string||
|&emsp;&emsp;&emsp;&emsp;id|主键||false|string||
|&emsp;&emsp;&emsp;&emsp;numbers|姓名||false|string||
|&emsp;&emsp;&emsp;&emsp;phone|联系电话||false|string||
|&emsp;&emsp;&emsp;&emsp;updateBy|更新人||false|string||
|&emsp;&emsp;&emsp;&emsp;updateTime|更新日期||false|string||
|&emsp;&emsp;&emsp;&emsp;withConnection|关系||false|string||
|&emsp;&emsp;&emsp;&emsp;workPlace|工作地点||false|string||
|&emsp;&emsp;finishSchoolCode|毕业学校||false|string||
|&emsp;&emsp;graduateDate|毕业时间||false|string(date-time)||
|&emsp;&emsp;homePlace|户口地址||false|string||
|&emsp;&emsp;id|主键||false|string||
|&emsp;&emsp;identityCode|身份证号||false|string||
|&emsp;&emsp;isAreaStudent|地段生||false|integer(int32)||
|&emsp;&emsp;isMilitary|优抚对象||false|integer(int32)||
|&emsp;&emsp;nationCode|民族||false|string||
|&emsp;&emsp;phoneCode|电话||false|string||
|&emsp;&emsp;photosList|照片||false|array|photos对象|
|&emsp;&emsp;&emsp;&emsp;archiveCode|准考证号||false|string||
|&emsp;&emsp;&emsp;&emsp;createBy|创建人||false|string||
|&emsp;&emsp;&emsp;&emsp;createTime|创建日期||false|string||
|&emsp;&emsp;&emsp;&emsp;delFlag|删除标识||false|integer||
|&emsp;&emsp;&emsp;&emsp;id|主键||false|string||
|&emsp;&emsp;&emsp;&emsp;picture|照片||false|string||
|&emsp;&emsp;&emsp;&emsp;updateBy|更新人||false|string||
|&emsp;&emsp;&emsp;&emsp;updateTime|更新日期||false|string||
|&emsp;&emsp;polity|政治面貌||false|string||
|&emsp;&emsp;postCode|邮政编码||false|string||
|&emsp;&emsp;priseHistory|历史荣誉||false|string||
|&emsp;&emsp;resumeList|简历||false|array|resume对象|
|&emsp;&emsp;&emsp;&emsp;archiveCode|准考证号||false|string||
|&emsp;&emsp;&emsp;&emsp;beginTime|开始时间||false|string||
|&emsp;&emsp;&emsp;&emsp;createBy|创建人||false|string||
|&emsp;&emsp;&emsp;&emsp;createTime|创建日期||false|string||
|&emsp;&emsp;&emsp;&emsp;delFlag|删除标识||false|integer||
|&emsp;&emsp;&emsp;&emsp;endTime|结束时间||false|string||
|&emsp;&emsp;&emsp;&emsp;id|主键||false|string||
|&emsp;&emsp;&emsp;&emsp;resumeContent|简历内容||false|string||
|&emsp;&emsp;&emsp;&emsp;school|学校||false|string||
|&emsp;&emsp;&emsp;&emsp;updateBy|更新人||false|string||
|&emsp;&emsp;&emsp;&emsp;updateTime|更新日期||false|string||
|&emsp;&emsp;sex|性别||false|string||
|&emsp;&emsp;studentKind|考生类别||false|string||
|&emsp;&emsp;studentName|姓名||false|string||
|&emsp;&emsp;updateBy|更新人||false|string||
|&emsp;&emsp;updateTime|更新日期||false|string(date-time)||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«string»|
|201|Created||
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|string||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": "",
	"success": true,
	"timestamp": 0
}
```


## 学生信息-通过id删除


**接口地址**:`/nnzk/student/studentInfo/delete`


**请求方式**:`DELETE`


**请求数据类型**:`application/x-www-form-urlencoded`


**响应数据类型**:`*/*`


**接口描述**:<p>学生信息-通过id删除</p>



**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|id|id|query|true|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«string»|
|204|No Content||
|401|Unauthorized||
|403|Forbidden||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|string||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": "",
	"success": true,
	"timestamp": 0
}
```


## 学生信息-批量删除


**接口地址**:`/nnzk/student/studentInfo/deleteBatch`


**请求方式**:`DELETE`


**请求数据类型**:`application/x-www-form-urlencoded`


**响应数据类型**:`*/*`


**接口描述**:<p>学生信息-批量删除</p>



**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|ids|ids|query|true|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«string»|
|204|No Content||
|401|Unauthorized||
|403|Forbidden||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|string||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": "",
	"success": true,
	"timestamp": 0
}
```


## 学生信息-编辑


**接口地址**:`/nnzk/student/studentInfo/edit`


**请求方式**:`POST`


**请求数据类型**:`application/json`


**响应数据类型**:`*/*`


**接口描述**:<p>学生信息-编辑</p>



**请求示例**:


```javascript
{
  "address": "",
  "archiveCode": "",
  "birth": "",
  "className": "",
  "createBy": "",
  "createTime": "",
  "delFlag": 0,
  "familyList": [
    {
      "archiveCode": "",
      "createBy": "",
      "createTime": "",
      "delFlag": 0,
      "householdAddress": "",
      "id": "",
      "numbers": "",
      "phone": "",
      "updateBy": "",
      "updateTime": "",
      "withConnection": "",
      "workPlace": ""
    }
  ],
  "finishSchoolCode": "",
  "graduateDate": "",
  "homePlace": "",
  "id": "",
  "identityCode": "",
  "isAreaStudent": 0,
  "isMilitary": 0,
  "nationCode": "",
  "phoneCode": "",
  "photosList": [
    {
      "archiveCode": "",
      "createBy": "",
      "createTime": "",
      "delFlag": 0,
      "id": "",
      "picture": "",
      "updateBy": "",
      "updateTime": ""
    }
  ],
  "polity": "",
  "postCode": "",
  "priseHistory": "",
  "resumeList": [
    {
      "archiveCode": "",
      "beginTime": "",
      "createBy": "",
      "createTime": "",
      "delFlag": 0,
      "endTime": "",
      "id": "",
      "resumeContent": "",
      "school": "",
      "updateBy": "",
      "updateTime": ""
    }
  ],
  "sex": "",
  "studentKind": "",
  "studentName": "",
  "updateBy": "",
  "updateTime": ""
}
```


**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|studentInfoPage|学生信息|body|true|student_infoPage对象|student_infoPage对象|
|&emsp;&emsp;address|现住地址||false|string||
|&emsp;&emsp;archiveCode|准考证号||false|string||
|&emsp;&emsp;birth|出生年月||false|string(date-time)||
|&emsp;&emsp;className|班级||false|string||
|&emsp;&emsp;createBy|创建人||false|string||
|&emsp;&emsp;createTime|创建日期||false|string(date-time)||
|&emsp;&emsp;delFlag|删除标识||false|integer(int32)||
|&emsp;&emsp;familyList|学生家庭表||false|array|family对象|
|&emsp;&emsp;&emsp;&emsp;archiveCode|准考证号||false|string||
|&emsp;&emsp;&emsp;&emsp;createBy|创建人||false|string||
|&emsp;&emsp;&emsp;&emsp;createTime|创建日期||false|string||
|&emsp;&emsp;&emsp;&emsp;delFlag|删除标识||false|integer||
|&emsp;&emsp;&emsp;&emsp;householdAddress|住址||false|string||
|&emsp;&emsp;&emsp;&emsp;id|主键||false|string||
|&emsp;&emsp;&emsp;&emsp;numbers|姓名||false|string||
|&emsp;&emsp;&emsp;&emsp;phone|联系电话||false|string||
|&emsp;&emsp;&emsp;&emsp;updateBy|更新人||false|string||
|&emsp;&emsp;&emsp;&emsp;updateTime|更新日期||false|string||
|&emsp;&emsp;&emsp;&emsp;withConnection|关系||false|string||
|&emsp;&emsp;&emsp;&emsp;workPlace|工作地点||false|string||
|&emsp;&emsp;finishSchoolCode|毕业学校||false|string||
|&emsp;&emsp;graduateDate|毕业时间||false|string(date-time)||
|&emsp;&emsp;homePlace|户口地址||false|string||
|&emsp;&emsp;id|主键||false|string||
|&emsp;&emsp;identityCode|身份证号||false|string||
|&emsp;&emsp;isAreaStudent|地段生||false|integer(int32)||
|&emsp;&emsp;isMilitary|优抚对象||false|integer(int32)||
|&emsp;&emsp;nationCode|民族||false|string||
|&emsp;&emsp;phoneCode|电话||false|string||
|&emsp;&emsp;photosList|照片||false|array|photos对象|
|&emsp;&emsp;&emsp;&emsp;archiveCode|准考证号||false|string||
|&emsp;&emsp;&emsp;&emsp;createBy|创建人||false|string||
|&emsp;&emsp;&emsp;&emsp;createTime|创建日期||false|string||
|&emsp;&emsp;&emsp;&emsp;delFlag|删除标识||false|integer||
|&emsp;&emsp;&emsp;&emsp;id|主键||false|string||
|&emsp;&emsp;&emsp;&emsp;picture|照片||false|string||
|&emsp;&emsp;&emsp;&emsp;updateBy|更新人||false|string||
|&emsp;&emsp;&emsp;&emsp;updateTime|更新日期||false|string||
|&emsp;&emsp;polity|政治面貌||false|string||
|&emsp;&emsp;postCode|邮政编码||false|string||
|&emsp;&emsp;priseHistory|历史荣誉||false|string||
|&emsp;&emsp;resumeList|简历||false|array|resume对象|
|&emsp;&emsp;&emsp;&emsp;archiveCode|准考证号||false|string||
|&emsp;&emsp;&emsp;&emsp;beginTime|开始时间||false|string||
|&emsp;&emsp;&emsp;&emsp;createBy|创建人||false|string||
|&emsp;&emsp;&emsp;&emsp;createTime|创建日期||false|string||
|&emsp;&emsp;&emsp;&emsp;delFlag|删除标识||false|integer||
|&emsp;&emsp;&emsp;&emsp;endTime|结束时间||false|string||
|&emsp;&emsp;&emsp;&emsp;id|主键||false|string||
|&emsp;&emsp;&emsp;&emsp;resumeContent|简历内容||false|string||
|&emsp;&emsp;&emsp;&emsp;school|学校||false|string||
|&emsp;&emsp;&emsp;&emsp;updateBy|更新人||false|string||
|&emsp;&emsp;&emsp;&emsp;updateTime|更新日期||false|string||
|&emsp;&emsp;sex|性别||false|string||
|&emsp;&emsp;studentKind|考生类别||false|string||
|&emsp;&emsp;studentName|姓名||false|string||
|&emsp;&emsp;updateBy|更新人||false|string||
|&emsp;&emsp;updateTime|更新日期||false|string(date-time)||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«string»|
|201|Created||
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|string||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": "",
	"success": true,
	"timestamp": 0
}
```


## 学生信息-编辑


**接口地址**:`/nnzk/student/studentInfo/edit`


**请求方式**:`PUT`


**请求数据类型**:`application/json`


**响应数据类型**:`*/*`


**接口描述**:<p>学生信息-编辑</p>



**请求示例**:


```javascript
{
  "address": "",
  "archiveCode": "",
  "birth": "",
  "className": "",
  "createBy": "",
  "createTime": "",
  "delFlag": 0,
  "familyList": [
    {
      "archiveCode": "",
      "createBy": "",
      "createTime": "",
      "delFlag": 0,
      "householdAddress": "",
      "id": "",
      "numbers": "",
      "phone": "",
      "updateBy": "",
      "updateTime": "",
      "withConnection": "",
      "workPlace": ""
    }
  ],
  "finishSchoolCode": "",
  "graduateDate": "",
  "homePlace": "",
  "id": "",
  "identityCode": "",
  "isAreaStudent": 0,
  "isMilitary": 0,
  "nationCode": "",
  "phoneCode": "",
  "photosList": [
    {
      "archiveCode": "",
      "createBy": "",
      "createTime": "",
      "delFlag": 0,
      "id": "",
      "picture": "",
      "updateBy": "",
      "updateTime": ""
    }
  ],
  "polity": "",
  "postCode": "",
  "priseHistory": "",
  "resumeList": [
    {
      "archiveCode": "",
      "beginTime": "",
      "createBy": "",
      "createTime": "",
      "delFlag": 0,
      "endTime": "",
      "id": "",
      "resumeContent": "",
      "school": "",
      "updateBy": "",
      "updateTime": ""
    }
  ],
  "sex": "",
  "studentKind": "",
  "studentName": "",
  "updateBy": "",
  "updateTime": ""
}
```


**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|studentInfoPage|学生信息|body|true|student_infoPage对象|student_infoPage对象|
|&emsp;&emsp;address|现住地址||false|string||
|&emsp;&emsp;archiveCode|准考证号||false|string||
|&emsp;&emsp;birth|出生年月||false|string(date-time)||
|&emsp;&emsp;className|班级||false|string||
|&emsp;&emsp;createBy|创建人||false|string||
|&emsp;&emsp;createTime|创建日期||false|string(date-time)||
|&emsp;&emsp;delFlag|删除标识||false|integer(int32)||
|&emsp;&emsp;familyList|学生家庭表||false|array|family对象|
|&emsp;&emsp;&emsp;&emsp;archiveCode|准考证号||false|string||
|&emsp;&emsp;&emsp;&emsp;createBy|创建人||false|string||
|&emsp;&emsp;&emsp;&emsp;createTime|创建日期||false|string||
|&emsp;&emsp;&emsp;&emsp;delFlag|删除标识||false|integer||
|&emsp;&emsp;&emsp;&emsp;householdAddress|住址||false|string||
|&emsp;&emsp;&emsp;&emsp;id|主键||false|string||
|&emsp;&emsp;&emsp;&emsp;numbers|姓名||false|string||
|&emsp;&emsp;&emsp;&emsp;phone|联系电话||false|string||
|&emsp;&emsp;&emsp;&emsp;updateBy|更新人||false|string||
|&emsp;&emsp;&emsp;&emsp;updateTime|更新日期||false|string||
|&emsp;&emsp;&emsp;&emsp;withConnection|关系||false|string||
|&emsp;&emsp;&emsp;&emsp;workPlace|工作地点||false|string||
|&emsp;&emsp;finishSchoolCode|毕业学校||false|string||
|&emsp;&emsp;graduateDate|毕业时间||false|string(date-time)||
|&emsp;&emsp;homePlace|户口地址||false|string||
|&emsp;&emsp;id|主键||false|string||
|&emsp;&emsp;identityCode|身份证号||false|string||
|&emsp;&emsp;isAreaStudent|地段生||false|integer(int32)||
|&emsp;&emsp;isMilitary|优抚对象||false|integer(int32)||
|&emsp;&emsp;nationCode|民族||false|string||
|&emsp;&emsp;phoneCode|电话||false|string||
|&emsp;&emsp;photosList|照片||false|array|photos对象|
|&emsp;&emsp;&emsp;&emsp;archiveCode|准考证号||false|string||
|&emsp;&emsp;&emsp;&emsp;createBy|创建人||false|string||
|&emsp;&emsp;&emsp;&emsp;createTime|创建日期||false|string||
|&emsp;&emsp;&emsp;&emsp;delFlag|删除标识||false|integer||
|&emsp;&emsp;&emsp;&emsp;id|主键||false|string||
|&emsp;&emsp;&emsp;&emsp;picture|照片||false|string||
|&emsp;&emsp;&emsp;&emsp;updateBy|更新人||false|string||
|&emsp;&emsp;&emsp;&emsp;updateTime|更新日期||false|string||
|&emsp;&emsp;polity|政治面貌||false|string||
|&emsp;&emsp;postCode|邮政编码||false|string||
|&emsp;&emsp;priseHistory|历史荣誉||false|string||
|&emsp;&emsp;resumeList|简历||false|array|resume对象|
|&emsp;&emsp;&emsp;&emsp;archiveCode|准考证号||false|string||
|&emsp;&emsp;&emsp;&emsp;beginTime|开始时间||false|string||
|&emsp;&emsp;&emsp;&emsp;createBy|创建人||false|string||
|&emsp;&emsp;&emsp;&emsp;createTime|创建日期||false|string||
|&emsp;&emsp;&emsp;&emsp;delFlag|删除标识||false|integer||
|&emsp;&emsp;&emsp;&emsp;endTime|结束时间||false|string||
|&emsp;&emsp;&emsp;&emsp;id|主键||false|string||
|&emsp;&emsp;&emsp;&emsp;resumeContent|简历内容||false|string||
|&emsp;&emsp;&emsp;&emsp;school|学校||false|string||
|&emsp;&emsp;&emsp;&emsp;updateBy|更新人||false|string||
|&emsp;&emsp;&emsp;&emsp;updateTime|更新日期||false|string||
|&emsp;&emsp;sex|性别||false|string||
|&emsp;&emsp;studentKind|考生类别||false|string||
|&emsp;&emsp;studentName|姓名||false|string||
|&emsp;&emsp;updateBy|更新人||false|string||
|&emsp;&emsp;updateTime|更新日期||false|string(date-time)||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«string»|
|201|Created||
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|string||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": "",
	"success": true,
	"timestamp": 0
}
```


## 学生信息-登录后查询学生信息


**接口地址**:`/nnzk/student/studentInfo/getStudentInfoByToken`


**请求方式**:`GET`


**请求数据类型**:`application/x-www-form-urlencoded`


**响应数据类型**:`*/*`


**接口描述**:<p>学生信息-登录后查询学生信息</p>



**请求参数**:


暂无


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«student_info对象»|
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|student_info对象|student_info对象|
|&emsp;&emsp;address|现住地址|string||
|&emsp;&emsp;archiveCode|准考证号|string||
|&emsp;&emsp;birth|出生年月|string(date-time)||
|&emsp;&emsp;className|班级|string||
|&emsp;&emsp;createBy|创建人|string||
|&emsp;&emsp;createTime|创建日期|string(date-time)||
|&emsp;&emsp;delFlag|删除标识|integer(int32)||
|&emsp;&emsp;finishSchoolCode|毕业学校|string||
|&emsp;&emsp;graduateDate|毕业时间|string(date-time)||
|&emsp;&emsp;homePlace|户口地址|string||
|&emsp;&emsp;id|主键|string||
|&emsp;&emsp;identityCode|身份证号|string||
|&emsp;&emsp;isAreaStudent|地段生|integer(int32)||
|&emsp;&emsp;isDeadLock|是否冻结|integer(int32)||
|&emsp;&emsp;isLock|是否锁定|integer(int32)||
|&emsp;&emsp;isMilitary|优抚对象|integer(int32)||
|&emsp;&emsp;nationCode|民族|string||
|&emsp;&emsp;opinion|评语|string||
|&emsp;&emsp;phoneCode|电话|string||
|&emsp;&emsp;polity|政治面貌|string||
|&emsp;&emsp;postCode|邮政编码|string||
|&emsp;&emsp;priseHistory|历史荣誉|string||
|&emsp;&emsp;sex|性别|string||
|&emsp;&emsp;studentKind|考生类别|string||
|&emsp;&emsp;studentName|姓名|string||
|&emsp;&emsp;updateBy|更新人|string||
|&emsp;&emsp;updateTime|更新日期|string(date-time)||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": {
		"address": "",
		"archiveCode": "",
		"birth": "",
		"className": "",
		"createBy": "",
		"createTime": "",
		"delFlag": 0,
		"finishSchoolCode": "",
		"graduateDate": "",
		"homePlace": "",
		"id": "",
		"identityCode": "",
		"isAreaStudent": 0,
		"isDeadLock": 0,
		"isLock": 0,
		"isMilitary": 0,
		"nationCode": "",
		"opinion": "",
		"phoneCode": "",
		"polity": "",
		"postCode": "",
		"priseHistory": "",
		"sex": "",
		"studentKind": "",
		"studentName": "",
		"updateBy": "",
		"updateTime": ""
	},
	"success": true,
	"timestamp": 0
}
```


## 学生信息-登录后查询学生成绩


**接口地址**:`/nnzk/student/studentInfo/getStudentScoreByToken`


**请求方式**:`GET`


**请求数据类型**:`application/x-www-form-urlencoded`


**响应数据类型**:`*/*`


**接口描述**:<p>学生信息-登录后查询学生成绩</p>



**请求参数**:


暂无


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«QueryStuScoreByTokenDTO»|
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|QueryStuScoreByTokenDTO|QueryStuScoreByTokenDTO|
|&emsp;&emsp;addingScore|照顾分|string||
|&emsp;&emsp;archiveCode|准考证号|string||
|&emsp;&emsp;chineseLevel|语文|string||
|&emsp;&emsp;chymistLevel|化学|string||
|&emsp;&emsp;combinedScore|组合分|string||
|&emsp;&emsp;diathesis|综合素质|string||
|&emsp;&emsp;englishLevel|英语|string||
|&emsp;&emsp;experiment|实验|string||
|&emsp;&emsp;mathLevel|数学|string||
|&emsp;&emsp;orderCode|排序码|number||
|&emsp;&emsp;physicalEduLevel|体育|string||
|&emsp;&emsp;physicsLevel|物理|string||
|&emsp;&emsp;politicsLevel|政史|string||
|&emsp;&emsp;queryTime|查询时间|string(date-time)||
|&emsp;&emsp;scoreMd5|成绩校验码|string||
|&emsp;&emsp;sumScore|总分|string||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": {
		"addingScore": "",
		"archiveCode": "",
		"chineseLevel": "",
		"chymistLevel": "",
		"combinedScore": "",
		"diathesis": "",
		"englishLevel": "",
		"experiment": "",
		"mathLevel": "",
		"orderCode": 0,
		"physicalEduLevel": "",
		"physicsLevel": "",
		"politicsLevel": "",
		"queryTime": "",
		"scoreMd5": "",
		"sumScore": ""
	},
	"success": true,
	"timestamp": 0
}
```


## 学生信息-分页列表查询


**接口地址**:`/nnzk/student/studentInfo/list`


**请求方式**:`GET`


**请求数据类型**:`application/x-www-form-urlencoded`


**响应数据类型**:`*/*`


**接口描述**:<p>学生信息-分页列表查询</p>



**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|address|现住地址|query|false|string||
|archiveCode|准考证号|query|false|string||
|birth|出生年月|query|false|string(date-time)||
|className|班级|query|false|string||
|createBy|创建人|query|false|string||
|createTime|创建日期|query|false|string(date-time)||
|delFlag|删除标识|query|false|integer(int32)||
|finishSchoolCode|毕业学校|query|false|string||
|graduateDate|毕业时间|query|false|string(date-time)||
|homePlace|户口地址|query|false|string||
|id|主键|query|false|string||
|identityCode|身份证号|query|false|string||
|isAreaStudent|地段生|query|false|integer(int32)||
|isDeadLock|是否冻结|query|false|integer(int32)||
|isLock|是否锁定|query|false|integer(int32)||
|isMilitary|优抚对象|query|false|integer(int32)||
|nationCode|民族|query|false|string||
|opinion|评语|query|false|string||
|pageNo|pageNo|query|false|integer(int32)||
|pageSize|pageSize|query|false|integer(int32)||
|phoneCode|电话|query|false|string||
|polity|政治面貌|query|false|string||
|postCode|邮政编码|query|false|string||
|priseHistory|历史荣誉|query|false|string||
|sex|性别|query|false|string||
|studentKind|考生类别|query|false|string||
|studentName|姓名|query|false|string||
|updateBy|更新人|query|false|string||
|updateTime|更新日期|query|false|string(date-time)||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«IPage«student_info对象»»|
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|IPage«student_info对象»|IPage«student_info对象»|
|&emsp;&emsp;current||integer(int64)||
|&emsp;&emsp;pages||integer(int64)||
|&emsp;&emsp;records||array|student_info对象|
|&emsp;&emsp;&emsp;&emsp;address|现住地址|string||
|&emsp;&emsp;&emsp;&emsp;archiveCode|准考证号|string||
|&emsp;&emsp;&emsp;&emsp;birth|出生年月|string||
|&emsp;&emsp;&emsp;&emsp;className|班级|string||
|&emsp;&emsp;&emsp;&emsp;createBy|创建人|string||
|&emsp;&emsp;&emsp;&emsp;createTime|创建日期|string||
|&emsp;&emsp;&emsp;&emsp;delFlag|删除标识|integer||
|&emsp;&emsp;&emsp;&emsp;finishSchoolCode|毕业学校|string||
|&emsp;&emsp;&emsp;&emsp;graduateDate|毕业时间|string||
|&emsp;&emsp;&emsp;&emsp;homePlace|户口地址|string||
|&emsp;&emsp;&emsp;&emsp;id|主键|string||
|&emsp;&emsp;&emsp;&emsp;identityCode|身份证号|string||
|&emsp;&emsp;&emsp;&emsp;isAreaStudent|地段生|integer||
|&emsp;&emsp;&emsp;&emsp;isDeadLock|是否冻结|integer||
|&emsp;&emsp;&emsp;&emsp;isLock|是否锁定|integer||
|&emsp;&emsp;&emsp;&emsp;isMilitary|优抚对象|integer||
|&emsp;&emsp;&emsp;&emsp;nationCode|民族|string||
|&emsp;&emsp;&emsp;&emsp;opinion|评语|string||
|&emsp;&emsp;&emsp;&emsp;phoneCode|电话|string||
|&emsp;&emsp;&emsp;&emsp;polity|政治面貌|string||
|&emsp;&emsp;&emsp;&emsp;postCode|邮政编码|string||
|&emsp;&emsp;&emsp;&emsp;priseHistory|历史荣誉|string||
|&emsp;&emsp;&emsp;&emsp;sex|性别|string||
|&emsp;&emsp;&emsp;&emsp;studentKind|考生类别|string||
|&emsp;&emsp;&emsp;&emsp;studentName|姓名|string||
|&emsp;&emsp;&emsp;&emsp;updateBy|更新人|string||
|&emsp;&emsp;&emsp;&emsp;updateTime|更新日期|string||
|&emsp;&emsp;size||integer(int64)||
|&emsp;&emsp;total||integer(int64)||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": {
		"current": 0,
		"pages": 0,
		"records": [
			{
				"address": "",
				"archiveCode": "",
				"birth": "",
				"className": "",
				"createBy": "",
				"createTime": "",
				"delFlag": 0,
				"finishSchoolCode": "",
				"graduateDate": "",
				"homePlace": "",
				"id": "",
				"identityCode": "",
				"isAreaStudent": 0,
				"isDeadLock": 0,
				"isLock": 0,
				"isMilitary": 0,
				"nationCode": "",
				"opinion": "",
				"phoneCode": "",
				"polity": "",
				"postCode": "",
				"priseHistory": "",
				"sex": "",
				"studentKind": "",
				"studentName": "",
				"updateBy": "",
				"updateTime": ""
			}
		],
		"size": 0,
		"total": 0
	},
	"success": true,
	"timestamp": 0
}
```


## 学生信息-通过准考证号查询


**接口地址**:`/nnzk/student/studentInfo/queryByArchiveCode`


**请求方式**:`GET`


**请求数据类型**:`application/x-www-form-urlencoded`


**响应数据类型**:`*/*`


**接口描述**:<p>学生信息-通过准考证号查询</p>



**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|archiveCode|archiveCode|query|true|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«StudentInfoDTO»|
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|StudentInfoDTO|StudentInfoDTO|
|&emsp;&emsp;address|现住地址|string||
|&emsp;&emsp;archiveCode|准考证号|string||
|&emsp;&emsp;birth|出生年月|string(date-time)||
|&emsp;&emsp;className|班级|string||
|&emsp;&emsp;createBy|创建人|string||
|&emsp;&emsp;createTime|创建日期|string(date-time)||
|&emsp;&emsp;delFlag|删除标识|integer(int32)||
|&emsp;&emsp;finishSchoolCode|毕业学校|string||
|&emsp;&emsp;finishSchoolName|毕业学校名称-县份学生专用|string||
|&emsp;&emsp;graduateDate|毕业时间|string(date-time)||
|&emsp;&emsp;homePlace|户口地址|string||
|&emsp;&emsp;id|主键|string||
|&emsp;&emsp;identityCode|身份证号|string||
|&emsp;&emsp;isAreaStudent|地段生|integer(int32)||
|&emsp;&emsp;isDeadLock|是否冻结|integer(int32)||
|&emsp;&emsp;isLock|是否锁定|integer(int32)||
|&emsp;&emsp;isMilitary|优抚对象|integer(int32)||
|&emsp;&emsp;nationCode|民族|string||
|&emsp;&emsp;opinion|评语|string||
|&emsp;&emsp;phoneCode|电话|string||
|&emsp;&emsp;polity|政治面貌|string||
|&emsp;&emsp;postCode|邮政编码|string||
|&emsp;&emsp;priseHistory|历史荣誉|string||
|&emsp;&emsp;sex|性别|string||
|&emsp;&emsp;studentKind|考生类别|string||
|&emsp;&emsp;studentName|姓名|string||
|&emsp;&emsp;updateBy|更新人|string||
|&emsp;&emsp;updateTime|更新日期|string(date-time)||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": {
		"address": "",
		"archiveCode": "",
		"birth": "",
		"className": "",
		"createBy": "",
		"createTime": "",
		"delFlag": 0,
		"finishSchoolCode": "",
		"finishSchoolName": "",
		"graduateDate": "",
		"homePlace": "",
		"id": "",
		"identityCode": "",
		"isAreaStudent": 0,
		"isDeadLock": 0,
		"isLock": 0,
		"isMilitary": 0,
		"nationCode": "",
		"opinion": "",
		"phoneCode": "",
		"polity": "",
		"postCode": "",
		"priseHistory": "",
		"sex": "",
		"studentKind": "",
		"studentName": "",
		"updateBy": "",
		"updateTime": ""
	},
	"success": true,
	"timestamp": 0
}
```


## 学生信息-通过id查询


**接口地址**:`/nnzk/student/studentInfo/queryById`


**请求方式**:`GET`


**请求数据类型**:`application/x-www-form-urlencoded`


**响应数据类型**:`*/*`


**接口描述**:<p>学生信息-通过id查询</p>



**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|id|id|query|true|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«student_info对象»|
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|student_info对象|student_info对象|
|&emsp;&emsp;address|现住地址|string||
|&emsp;&emsp;archiveCode|准考证号|string||
|&emsp;&emsp;birth|出生年月|string(date-time)||
|&emsp;&emsp;className|班级|string||
|&emsp;&emsp;createBy|创建人|string||
|&emsp;&emsp;createTime|创建日期|string(date-time)||
|&emsp;&emsp;delFlag|删除标识|integer(int32)||
|&emsp;&emsp;finishSchoolCode|毕业学校|string||
|&emsp;&emsp;graduateDate|毕业时间|string(date-time)||
|&emsp;&emsp;homePlace|户口地址|string||
|&emsp;&emsp;id|主键|string||
|&emsp;&emsp;identityCode|身份证号|string||
|&emsp;&emsp;isAreaStudent|地段生|integer(int32)||
|&emsp;&emsp;isDeadLock|是否冻结|integer(int32)||
|&emsp;&emsp;isLock|是否锁定|integer(int32)||
|&emsp;&emsp;isMilitary|优抚对象|integer(int32)||
|&emsp;&emsp;nationCode|民族|string||
|&emsp;&emsp;opinion|评语|string||
|&emsp;&emsp;phoneCode|电话|string||
|&emsp;&emsp;polity|政治面貌|string||
|&emsp;&emsp;postCode|邮政编码|string||
|&emsp;&emsp;priseHistory|历史荣誉|string||
|&emsp;&emsp;sex|性别|string||
|&emsp;&emsp;studentKind|考生类别|string||
|&emsp;&emsp;studentName|姓名|string||
|&emsp;&emsp;updateBy|更新人|string||
|&emsp;&emsp;updateTime|更新日期|string(date-time)||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": {
		"address": "",
		"archiveCode": "",
		"birth": "",
		"className": "",
		"createBy": "",
		"createTime": "",
		"delFlag": 0,
		"finishSchoolCode": "",
		"graduateDate": "",
		"homePlace": "",
		"id": "",
		"identityCode": "",
		"isAreaStudent": 0,
		"isDeadLock": 0,
		"isLock": 0,
		"isMilitary": 0,
		"nationCode": "",
		"opinion": "",
		"phoneCode": "",
		"polity": "",
		"postCode": "",
		"priseHistory": "",
		"sex": "",
		"studentKind": "",
		"studentName": "",
		"updateBy": "",
		"updateTime": ""
	},
	"success": true,
	"timestamp": 0
}
```


## 学生家庭表主表ID查询


**接口地址**:`/nnzk/student/studentInfo/queryFamilyByMainId`


**请求方式**:`GET`


**请求数据类型**:`application/x-www-form-urlencoded`


**响应数据类型**:`*/*`


**接口描述**:<p>学生家庭表-通主表ID查询</p>



**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|archiveCode|archiveCode|query|true|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«List«family对象»»|
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|array|family对象|
|&emsp;&emsp;archiveCode|准考证号|string||
|&emsp;&emsp;createBy|创建人|string||
|&emsp;&emsp;createTime|创建日期|string(date-time)||
|&emsp;&emsp;delFlag|删除标识|integer(int32)||
|&emsp;&emsp;householdAddress|住址|string||
|&emsp;&emsp;id|主键|string||
|&emsp;&emsp;numbers|姓名|string||
|&emsp;&emsp;phone|联系电话|string||
|&emsp;&emsp;updateBy|更新人|string||
|&emsp;&emsp;updateTime|更新日期|string(date-time)||
|&emsp;&emsp;withConnection|关系|string||
|&emsp;&emsp;workPlace|工作地点|string||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": [
		{
			"archiveCode": "",
			"createBy": "",
			"createTime": "",
			"delFlag": 0,
			"householdAddress": "",
			"id": "",
			"numbers": "",
			"phone": "",
			"updateBy": "",
			"updateTime": "",
			"withConnection": "",
			"workPlace": ""
		}
	],
	"success": true,
	"timestamp": 0
}
```


## 照片表主表ID查询


**接口地址**:`/nnzk/student/studentInfo/queryPhotosByMainId`


**请求方式**:`GET`


**请求数据类型**:`application/x-www-form-urlencoded`


**响应数据类型**:`*/*`


**接口描述**:<p>照片表-通主表ID查询</p>



**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|archiveCode|archiveCode|query|true|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«List«photos对象»»|
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|array|photos对象|
|&emsp;&emsp;archiveCode|准考证号|string||
|&emsp;&emsp;createBy|创建人|string||
|&emsp;&emsp;createTime|创建日期|string(date-time)||
|&emsp;&emsp;delFlag|删除标识|integer(int32)||
|&emsp;&emsp;id|主键|string||
|&emsp;&emsp;picture|照片|string||
|&emsp;&emsp;updateBy|更新人|string||
|&emsp;&emsp;updateTime|更新日期|string(date-time)||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": [
		{
			"archiveCode": "",
			"createBy": "",
			"createTime": "",
			"delFlag": 0,
			"id": "",
			"picture": "",
			"updateBy": "",
			"updateTime": ""
		}
	],
	"success": true,
	"timestamp": 0
}
```


## 简历表主表ID查询


**接口地址**:`/nnzk/student/studentInfo/queryResumeByMainId`


**请求方式**:`GET`


**请求数据类型**:`application/x-www-form-urlencoded`


**响应数据类型**:`*/*`


**接口描述**:<p>简历表-通主表ID查询</p>



**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|archiveCode|archiveCode|query|true|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«List«resume对象»»|
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|array|resume对象|
|&emsp;&emsp;archiveCode|准考证号|string||
|&emsp;&emsp;beginTime|开始时间|string(date-time)||
|&emsp;&emsp;createBy|创建人|string||
|&emsp;&emsp;createTime|创建日期|string(date-time)||
|&emsp;&emsp;delFlag|删除标识|integer(int32)||
|&emsp;&emsp;endTime|结束时间|string(date-time)||
|&emsp;&emsp;id|主键|string||
|&emsp;&emsp;resumeContent|简历内容|string||
|&emsp;&emsp;school|学校|string||
|&emsp;&emsp;updateBy|更新人|string||
|&emsp;&emsp;updateTime|更新日期|string(date-time)||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": [
		{
			"archiveCode": "",
			"beginTime": "",
			"createBy": "",
			"createTime": "",
			"delFlag": 0,
			"endTime": "",
			"id": "",
			"resumeContent": "",
			"school": "",
			"updateBy": "",
			"updateTime": ""
		}
	],
	"success": true,
	"timestamp": 0
}
```


# 学生信息维护


## 学生信息维护-新增学生档案


**接口地址**:`/nnzk/studentInfoManage/addStudent`


**请求方式**:`POST`


**请求数据类型**:`application/json`


**响应数据类型**:`*/*`


**接口描述**:<p>学生信息维护-新增学生档案</p>



**请求示例**:


```javascript
{
  "address": "",
  "archiveCode": "",
  "birth": "",
  "className": "",
  "createBy": "",
  "createTime": "",
  "delFlag": 0,
  "familyList": [
    {
      "archiveCode": "",
      "createBy": "",
      "createTime": "",
      "delFlag": 0,
      "householdAddress": "",
      "id": "",
      "numbers": "",
      "phone": "",
      "updateBy": "",
      "updateTime": "",
      "withConnection": "",
      "workPlace": ""
    }
  ],
  "finishSchoolCode": "",
  "graduateDate": "",
  "homePlace": "",
  "id": "",
  "identityCode": "",
  "isAreaStudent": 0,
  "isMilitary": 0,
  "nationCode": "",
  "phoneCode": "",
  "photosList": [
    {
      "archiveCode": "",
      "createBy": "",
      "createTime": "",
      "delFlag": 0,
      "id": "",
      "picture": "",
      "updateBy": "",
      "updateTime": ""
    }
  ],
  "polity": "",
  "postCode": "",
  "priseHistory": "",
  "resumeList": [
    {
      "archiveCode": "",
      "beginTime": "",
      "createBy": "",
      "createTime": "",
      "delFlag": 0,
      "endTime": "",
      "id": "",
      "resumeContent": "",
      "school": "",
      "updateBy": "",
      "updateTime": ""
    }
  ],
  "sex": "",
  "studentKind": "",
  "studentName": "",
  "updateBy": "",
  "updateTime": ""
}
```


**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|studentInfoPage|学生信息|body|true|student_infoPage对象|student_infoPage对象|
|&emsp;&emsp;address|现住地址||false|string||
|&emsp;&emsp;archiveCode|准考证号||false|string||
|&emsp;&emsp;birth|出生年月||false|string(date-time)||
|&emsp;&emsp;className|班级||false|string||
|&emsp;&emsp;createBy|创建人||false|string||
|&emsp;&emsp;createTime|创建日期||false|string(date-time)||
|&emsp;&emsp;delFlag|删除标识||false|integer(int32)||
|&emsp;&emsp;familyList|学生家庭表||false|array|family对象|
|&emsp;&emsp;&emsp;&emsp;archiveCode|准考证号||false|string||
|&emsp;&emsp;&emsp;&emsp;createBy|创建人||false|string||
|&emsp;&emsp;&emsp;&emsp;createTime|创建日期||false|string||
|&emsp;&emsp;&emsp;&emsp;delFlag|删除标识||false|integer||
|&emsp;&emsp;&emsp;&emsp;householdAddress|住址||false|string||
|&emsp;&emsp;&emsp;&emsp;id|主键||false|string||
|&emsp;&emsp;&emsp;&emsp;numbers|姓名||false|string||
|&emsp;&emsp;&emsp;&emsp;phone|联系电话||false|string||
|&emsp;&emsp;&emsp;&emsp;updateBy|更新人||false|string||
|&emsp;&emsp;&emsp;&emsp;updateTime|更新日期||false|string||
|&emsp;&emsp;&emsp;&emsp;withConnection|关系||false|string||
|&emsp;&emsp;&emsp;&emsp;workPlace|工作地点||false|string||
|&emsp;&emsp;finishSchoolCode|毕业学校||false|string||
|&emsp;&emsp;graduateDate|毕业时间||false|string(date-time)||
|&emsp;&emsp;homePlace|户口地址||false|string||
|&emsp;&emsp;id|主键||false|string||
|&emsp;&emsp;identityCode|身份证号||false|string||
|&emsp;&emsp;isAreaStudent|地段生||false|integer(int32)||
|&emsp;&emsp;isMilitary|优抚对象||false|integer(int32)||
|&emsp;&emsp;nationCode|民族||false|string||
|&emsp;&emsp;phoneCode|电话||false|string||
|&emsp;&emsp;photosList|照片||false|array|photos对象|
|&emsp;&emsp;&emsp;&emsp;archiveCode|准考证号||false|string||
|&emsp;&emsp;&emsp;&emsp;createBy|创建人||false|string||
|&emsp;&emsp;&emsp;&emsp;createTime|创建日期||false|string||
|&emsp;&emsp;&emsp;&emsp;delFlag|删除标识||false|integer||
|&emsp;&emsp;&emsp;&emsp;id|主键||false|string||
|&emsp;&emsp;&emsp;&emsp;picture|照片||false|string||
|&emsp;&emsp;&emsp;&emsp;updateBy|更新人||false|string||
|&emsp;&emsp;&emsp;&emsp;updateTime|更新日期||false|string||
|&emsp;&emsp;polity|政治面貌||false|string||
|&emsp;&emsp;postCode|邮政编码||false|string||
|&emsp;&emsp;priseHistory|历史荣誉||false|string||
|&emsp;&emsp;resumeList|简历||false|array|resume对象|
|&emsp;&emsp;&emsp;&emsp;archiveCode|准考证号||false|string||
|&emsp;&emsp;&emsp;&emsp;beginTime|开始时间||false|string||
|&emsp;&emsp;&emsp;&emsp;createBy|创建人||false|string||
|&emsp;&emsp;&emsp;&emsp;createTime|创建日期||false|string||
|&emsp;&emsp;&emsp;&emsp;delFlag|删除标识||false|integer||
|&emsp;&emsp;&emsp;&emsp;endTime|结束时间||false|string||
|&emsp;&emsp;&emsp;&emsp;id|主键||false|string||
|&emsp;&emsp;&emsp;&emsp;resumeContent|简历内容||false|string||
|&emsp;&emsp;&emsp;&emsp;school|学校||false|string||
|&emsp;&emsp;&emsp;&emsp;updateBy|更新人||false|string||
|&emsp;&emsp;&emsp;&emsp;updateTime|更新日期||false|string||
|&emsp;&emsp;sex|性别||false|string||
|&emsp;&emsp;studentKind|考生类别||false|string||
|&emsp;&emsp;studentName|姓名||false|string||
|&emsp;&emsp;updateBy|更新人||false|string||
|&emsp;&emsp;updateTime|更新日期||false|string(date-time)||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«string»|
|201|Created||
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|string||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": "",
	"success": true,
	"timestamp": 0
}
```


## 学生信息维护-获取学生全部信息


**接口地址**:`/nnzk/studentInfoManage/allStudentInfo`


**请求方式**:`GET`


**请求数据类型**:`application/x-www-form-urlencoded`


**响应数据类型**:`*/*`


**接口描述**:<p>学生信息维护-获取学生全部信息</p>



**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|archiveCode|archiveCode|query|true|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«StudentInfoManageVO»|
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|StudentInfoManageVO|StudentInfoManageVO|
|&emsp;&emsp;asCityOthersMatedVO|是否已本市其他录取|AsCityOthersMatedVO|AsCityOthersMatedVO|
|&emsp;&emsp;&emsp;&emsp;commander|委托人|string||
|&emsp;&emsp;&emsp;&emsp;connector|联系单位或联系人|string||
|&emsp;&emsp;&emsp;&emsp;isCityOthersMated|是否本市其他录取|integer||
|&emsp;&emsp;stuInfo|学生信息|StuInfoVO|StuInfoVO|
|&emsp;&emsp;&emsp;&emsp;address|现住地址|string||
|&emsp;&emsp;&emsp;&emsp;archiveCode|准考证号|string||
|&emsp;&emsp;&emsp;&emsp;finishSchoolCode|毕业学校|string||
|&emsp;&emsp;&emsp;&emsp;graduateDate|毕业时间|string||
|&emsp;&emsp;&emsp;&emsp;id|主键|string||
|&emsp;&emsp;&emsp;&emsp;identityCode|身份证号|string||
|&emsp;&emsp;&emsp;&emsp;isAreaStudent|地段生|integer||
|&emsp;&emsp;&emsp;&emsp;isDeadLock|是否冻结|integer||
|&emsp;&emsp;&emsp;&emsp;isMilitary|优抚对象|integer||
|&emsp;&emsp;&emsp;&emsp;nationCode|民族|string||
|&emsp;&emsp;&emsp;&emsp;opinion|评语|string||
|&emsp;&emsp;&emsp;&emsp;phoneCode|电话|string||
|&emsp;&emsp;&emsp;&emsp;polity|政治面貌|string||
|&emsp;&emsp;&emsp;&emsp;postCode|邮政编码|string||
|&emsp;&emsp;&emsp;&emsp;sex|性别|string||
|&emsp;&emsp;&emsp;&emsp;studentKind|考生类别|string||
|&emsp;&emsp;&emsp;&emsp;studentName|姓名|string||
|&emsp;&emsp;stuMatedInfo|学生报名信息|StuMatedInfoVO|StuMatedInfoVO|
|&emsp;&emsp;&emsp;&emsp;archiveCode|准考证号|string||
|&emsp;&emsp;&emsp;&emsp;fillTime|填报时间|string||
|&emsp;&emsp;&emsp;&emsp;highSchoolCode|报名高中|string||
|&emsp;&emsp;&emsp;&emsp;id|主键|string||
|&emsp;&emsp;&emsp;&emsp;isLock|是否锁定|integer||
|&emsp;&emsp;&emsp;&emsp;isLodging|是否住宿|integer||
|&emsp;&emsp;&emsp;&emsp;matriculateStatus|录取状态|integer||
|&emsp;&emsp;&emsp;&emsp;matriculateTime|录取时间|string||
|&emsp;&emsp;&emsp;&emsp;matriculateType|录取类型|string||
|&emsp;&emsp;&emsp;&emsp;remarkOfMatriculate|录取说明|string||
|&emsp;&emsp;&emsp;&emsp;signUpType|报名类型|string||
|&emsp;&emsp;stuMatedTimeAndSchool|学生已录取的录取学校、时间、类型|StuMatedTimeAndSchoolVO|StuMatedTimeAndSchoolVO|
|&emsp;&emsp;&emsp;&emsp;archiveCode|准考证号|string||
|&emsp;&emsp;&emsp;&emsp;matriculateTime|录取时间|string||
|&emsp;&emsp;&emsp;&emsp;matriculateType|录取类型|string||
|&emsp;&emsp;&emsp;&emsp;schoolName|录取学校|string||
|&emsp;&emsp;&emsp;&emsp;studentName|学生姓名|string||
|&emsp;&emsp;stuOperateHistorys|关于该学生的操作历史|array|StuOperateHistoryVO|
|&emsp;&emsp;&emsp;&emsp;account|账号|string||
|&emsp;&emsp;&emsp;&emsp;archiveCode|准考证号|string||
|&emsp;&emsp;&emsp;&emsp;id|主键|string||
|&emsp;&emsp;&emsp;&emsp;operateDatetime|操作时间|string||
|&emsp;&emsp;&emsp;&emsp;operateKind|操作类型|string||
|&emsp;&emsp;&emsp;&emsp;operateLog|操作日志|string||
|&emsp;&emsp;stuScore|学生成绩|StuScoreVO|StuScoreVO|
|&emsp;&emsp;&emsp;&emsp;archiveCode|准考证号|string||
|&emsp;&emsp;&emsp;&emsp;chineseLevel|语文|string||
|&emsp;&emsp;&emsp;&emsp;chymistLevel|化学|string||
|&emsp;&emsp;&emsp;&emsp;combinedScore|组合分|string||
|&emsp;&emsp;&emsp;&emsp;diathesis|综合素质|string||
|&emsp;&emsp;&emsp;&emsp;englishLevel|英语|string||
|&emsp;&emsp;&emsp;&emsp;experiment|实验|string||
|&emsp;&emsp;&emsp;&emsp;id|主键|string||
|&emsp;&emsp;&emsp;&emsp;mathLevel|数学|string||
|&emsp;&emsp;&emsp;&emsp;orderCode|排序码|number||
|&emsp;&emsp;&emsp;&emsp;physicsLevel|物理|string||
|&emsp;&emsp;&emsp;&emsp;politicsLevel|政史|string||
|&emsp;&emsp;&emsp;&emsp;sumScore|总分|string||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": {
		"asCityOthersMatedVO": {
			"commander": "",
			"connector": "",
			"isCityOthersMated": 0
		},
		"stuInfo": {
			"address": "",
			"archiveCode": "",
			"finishSchoolCode": "",
			"graduateDate": "",
			"id": "",
			"identityCode": "",
			"isAreaStudent": 0,
			"isDeadLock": 0,
			"isMilitary": 0,
			"nationCode": "",
			"opinion": "",
			"phoneCode": "",
			"polity": "",
			"postCode": "",
			"sex": "",
			"studentKind": "",
			"studentName": ""
		},
		"stuMatedInfo": {
			"archiveCode": "",
			"fillTime": "",
			"highSchoolCode": "",
			"id": "",
			"isLock": 0,
			"isLodging": 0,
			"matriculateStatus": 0,
			"matriculateTime": "",
			"matriculateType": "",
			"remarkOfMatriculate": "",
			"signUpType": ""
		},
		"stuMatedTimeAndSchool": {
			"archiveCode": "",
			"matriculateTime": "",
			"matriculateType": "",
			"schoolName": "",
			"studentName": ""
		},
		"stuOperateHistorys": [
			{
				"account": "",
				"archiveCode": "",
				"id": "",
				"operateDatetime": "",
				"operateKind": "",
				"operateLog": ""
			}
		],
		"stuScore": {
			"archiveCode": "",
			"chineseLevel": "",
			"chymistLevel": "",
			"combinedScore": "",
			"diathesis": "",
			"englishLevel": "",
			"experiment": "",
			"id": "",
			"mathLevel": "",
			"orderCode": 0,
			"physicsLevel": "",
			"politicsLevel": "",
			"sumScore": ""
		}
	},
	"success": true,
	"timestamp": 0
}
```


## 学生信息维护-生成所有学生排序码


**接口地址**:`/nnzk/studentInfoManage/buildAllOrderCode`


**请求方式**:`POST`


**请求数据类型**:`application/json`


**响应数据类型**:`*/*`


**接口描述**:<p>学生信息维护-生成所有学生排序码</p>



**请求参数**:


暂无


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«string»|
|201|Created||
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|string||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": "",
	"success": true,
	"timestamp": 0
}
```


## 学生信息维护-生成单个学生排序码


**接口地址**:`/nnzk/studentInfoManage/buildOneOrderCodeByArchiveCode`


**请求方式**:`POST`


**请求数据类型**:`application/json`


**响应数据类型**:`*/*`


**接口描述**:<p>学生信息维护-生成单个学生排序码</p>



**请求示例**:


```javascript
{
  "archiveCode": "",
  "studentName": ""
}
```


**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|input|input|body|true|QueryStuInfoDTO|QueryStuInfoDTO|
|&emsp;&emsp;archiveCode|准考证号||false|string||
|&emsp;&emsp;studentName|姓名||false|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«string»|
|201|Created||
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|string||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": "",
	"success": true,
	"timestamp": 0
}
```


## 学生信息维护-密码取准考证后六位


**接口地址**:`/nnzk/studentInfoManage/changeStuPasswordByArchiveCode`


**请求方式**:`POST`


**请求数据类型**:`application/json`


**响应数据类型**:`*/*`


**接口描述**:<p>学生信息维护-密码取准考证后六位</p>



**请求示例**:


```javascript
{
  "archiveCode": "",
  "studentName": ""
}
```


**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|input|input|body|true|QueryStuInfoDTO|QueryStuInfoDTO|
|&emsp;&emsp;archiveCode|准考证号||false|string||
|&emsp;&emsp;studentName|姓名||false|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«string»|
|201|Created||
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|string||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": "",
	"success": true,
	"timestamp": 0
}
```


## 学生信息维护-密码取身份证后六位


**接口地址**:`/nnzk/studentInfoManage/changeStuPasswordById`


**请求方式**:`POST`


**请求数据类型**:`application/json`


**响应数据类型**:`*/*`


**接口描述**:<p>学生信息维护-密码取身份证后六位</p>



**请求示例**:


```javascript
{
  "archiveCode": "",
  "studentName": ""
}
```


**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|input|input|body|true|QueryStuInfoDTO|QueryStuInfoDTO|
|&emsp;&emsp;archiveCode|准考证号||false|string||
|&emsp;&emsp;studentName|姓名||false|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«string»|
|201|Created||
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|string||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": "",
	"success": true,
	"timestamp": 0
}
```


## 学生信息维护-根据输入的密码修改


**接口地址**:`/nnzk/studentInfoManage/changeStuPasswordByInput`


**请求方式**:`POST`


**请求数据类型**:`application/json`


**响应数据类型**:`*/*`


**接口描述**:<p>学生信息维护-根据输入的密码修改</p>



**请求示例**:


```javascript
{
  "archiveCode": "",
  "newPassword": ""
}
```


**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|input|input|body|true|ChangeStuPasswordDTO|ChangeStuPasswordDTO|
|&emsp;&emsp;archiveCode|准考证号||false|string||
|&emsp;&emsp;newPassword|输入的密码||false|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«string»|
|201|Created||
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|string||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": "",
	"success": true,
	"timestamp": 0
}
```


## 学生信息维护-冻结考生


**接口地址**:`/nnzk/studentInfoManage/freezeStudent`


**请求方式**:`POST`


**请求数据类型**:`application/json`


**响应数据类型**:`*/*`


**接口描述**:<p>学生信息维护-冻结考生</p>



**请求示例**:


```javascript
{
  "archiveCode": "",
  "studentName": ""
}
```


**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|input|input|body|true|QueryStuInfoDTO|QueryStuInfoDTO|
|&emsp;&emsp;archiveCode|准考证号||false|string||
|&emsp;&emsp;studentName|姓名||false|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«string»|
|201|Created||
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|string||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": "",
	"success": true,
	"timestamp": 0
}
```


## 学生信息维护-由成绩获取成绩排序码和组合分


**接口地址**:`/nnzk/studentInfoManage/getCombinedScoreAndOrderCode`


**请求方式**:`GET`


**请求数据类型**:`application/x-www-form-urlencoded`


**响应数据类型**:`*/*`


**接口描述**:<p>学生信息维护-由成绩获取成绩排序码和组合分</p>



**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|chineseLevel|语文|query|false|string||
|chymistLevel|化学|query|false|string||
|englishLevel|英语|query|false|string||
|mathLevel|数学|query|false|string||
|physicsLevel|物理|query|false|string||
|politicsLevel|政史|query|false|string||
|sumScore|总分|query|false|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«OrderCodeAndCombinedScoreVO»|
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|OrderCodeAndCombinedScoreVO|OrderCodeAndCombinedScoreVO|
|&emsp;&emsp;combinedScore|组合分|string||
|&emsp;&emsp;orderCode|成绩排序码|string||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": {
		"combinedScore": "",
		"orderCode": ""
	},
	"success": true,
	"timestamp": 0
}
```


## 学生信息维护-准考证号或姓名查询


**接口地址**:`/nnzk/studentInfoManage/getStuByCodeOrName`


**请求方式**:`GET`


**请求数据类型**:`application/x-www-form-urlencoded`


**响应数据类型**:`*/*`


**接口描述**:<p>学生信息维护-准考证号或姓名查询</p>



**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|archiveCode|准考证号|query|false|string||
|studentName|姓名|query|false|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«List«ArchiveCodeAndNameVO»»|
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|array|ArchiveCodeAndNameVO|
|&emsp;&emsp;archiveCode|准考证号|string||
|&emsp;&emsp;studentName|姓名|string||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": [
		{
			"archiveCode": "",
			"studentName": ""
		}
	],
	"success": true,
	"timestamp": 0
}
```


## 学生信息维护-打印数据


**接口地址**:`/nnzk/studentInfoManage/print`


**请求方式**:`GET`


**请求数据类型**:`application/x-www-form-urlencoded`


**响应数据类型**:`*/*`


**接口描述**:<p>学生信息维护-打印数据</p>



**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|ddlPrivilegeClass|特招班类型（国际班、民族班、外地生班。。）|query|false|string||
|highSchoolCode|录取学校代码|query|false|string||
|matBeginTime|录取时间范围（开始）|query|false|string(date-time)||
|matEndTime|录取时间（结束）|query|false|string(date-time)||
|matType|录取类型|query|false|string||
|selectedArchiveCode|选择打印的单个准考证号|query|false|string||
|selectedArchiveCodeList|选择打印的准考证号数组|query|false|array|string|


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|OrdMatAndPriRegPrintOutputDTO|
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|count|总条数|integer(int32)|integer(int32)|
|data|学生列表|array|OrdMatAndPriRegPrintDTO|
|&emsp;&emsp;archiveCode|准考证号|string||
|&emsp;&emsp;chineseLevel|语文|string||
|&emsp;&emsp;chymistLevel|化学|string||
|&emsp;&emsp;diathesis|综合素质|string||
|&emsp;&emsp;englishLevel|英语|string||
|&emsp;&emsp;experiment|实验|string||
|&emsp;&emsp;finishSchoolName|毕业学校|string||
|&emsp;&emsp;highSchoolName|录取学校|string||
|&emsp;&emsp;mathLevel|数学|string||
|&emsp;&emsp;matriculateType|录取类型|string||
|&emsp;&emsp;physicsLevel|物理|string||
|&emsp;&emsp;politicsLevel|政史|string||
|&emsp;&emsp;serialNum|序号|integer(int64)||
|&emsp;&emsp;sex|性别|string||
|&emsp;&emsp;studentName|学生姓名|string||
|&emsp;&emsp;sumScore|总分|string||
|total|总页数|integer(int32)|integer(int32)|


**响应示例**:
```javascript
{
	"count": 0,
	"data": [
		{
			"archiveCode": "",
			"chineseLevel": "",
			"chymistLevel": "",
			"diathesis": "",
			"englishLevel": "",
			"experiment": "",
			"finishSchoolName": "",
			"highSchoolName": "",
			"mathLevel": "",
			"matriculateType": "",
			"physicsLevel": "",
			"politicsLevel": "",
			"serialNum": 0,
			"sex": "",
			"studentName": "",
			"sumScore": ""
		}
	],
	"total": 0
}
```


## 学生信息维护-打印新转入证明数据


**接口地址**:`/nnzk/studentInfoManage/printChangeArCodeInfo`


**请求方式**:`GET`


**请求数据类型**:`application/x-www-form-urlencoded`


**响应数据类型**:`*/*`


**接口描述**:<p>学生信息维护-打印新转入证明数据</p>



**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|archiveCode|archiveCode|query|false|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|ChangeArCodeInfoOutputDTO|
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|count|总条数|integer(int32)|integer(int32)|
|data|学生列表|array|ChangeArCodeInfoDTO|
|&emsp;&emsp;newArchiveCode|新准考证号|string||
|&emsp;&emsp;oldArchiveCdoe|旧准考证号|string||
|&emsp;&emsp;studentName|学生姓名|string||
|total|总页数|integer(int32)|integer(int32)|


**响应示例**:
```javascript
{
	"count": 0,
	"data": [
		{
			"newArchiveCode": "",
			"oldArchiveCdoe": "",
			"studentName": ""
		}
	],
	"total": 0
}
```


## 学生信息维护-解除冻结考生


**接口地址**:`/nnzk/studentInfoManage/unfreezeStudent`


**请求方式**:`POST`


**请求数据类型**:`application/json`


**响应数据类型**:`*/*`


**接口描述**:<p>学生信息维护-解除冻结考生</p>



**请求示例**:


```javascript
{
  "archiveCode": "",
  "studentName": ""
}
```


**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|input|input|body|true|QueryStuInfoDTO|QueryStuInfoDTO|
|&emsp;&emsp;archiveCode|准考证号||false|string||
|&emsp;&emsp;studentName|姓名||false|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«string»|
|201|Created||
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|string||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": "",
	"success": true,
	"timestamp": 0
}
```


## 学生信息维护-退录操作


**接口地址**:`/nnzk/studentInfoManage/updateMatriculateOut`


**请求方式**:`POST`


**请求数据类型**:`application/json`


**响应数据类型**:`*/*`


**接口描述**:<p>学生信息维护-退录操作</p>



**请求示例**:


```javascript
{
  "archiveCode": "",
  "isLock": 0
}
```


**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|input|input|body|true|MatriculateOutDTO|MatriculateOutDTO|
|&emsp;&emsp;archiveCode|准考证号||false|string||
|&emsp;&emsp;isLock|是否锁定||false|integer(int32)||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«string»|
|201|Created||
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|string||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": "",
	"success": true,
	"timestamp": 0
}
```


## 学生信息维护-保存学生修改信息


**接口地址**:`/nnzk/studentInfoManage/updateStuAllInfo`


**请求方式**:`POST`


**请求数据类型**:`application/json`


**响应数据类型**:`*/*`


**接口描述**:<p>学生信息维护-保存学生修改信息</p>



**请求示例**:


```javascript
{
  "asCityOthersMatedVO": {
    "commander": "",
    "connector": "",
    "isCityOthersMated": 0
  },
  "oldArchiveCode": "",
  "stuInfo": {
    "address": "",
    "archiveCode": "",
    "finishSchoolCode": "",
    "graduateDate": "",
    "id": "",
    "identityCode": "",
    "isAreaStudent": 0,
    "isDeadLock": 0,
    "isMilitary": 0,
    "nationCode": "",
    "opinion": "",
    "phoneCode": "",
    "polity": "",
    "postCode": "",
    "sex": "",
    "studentKind": "",
    "studentName": ""
  },
  "stuMatedInfo": {
    "archiveCode": "",
    "fillTime": "",
    "highSchoolCode": "",
    "id": "",
    "isLock": 0,
    "isLodging": 0,
    "matriculateStatus": 0,
    "matriculateTime": "",
    "matriculateType": "",
    "remarkOfMatriculate": "",
    "signUpType": ""
  },
  "stuScore": {
    "archiveCode": "",
    "chineseLevel": "",
    "chymistLevel": "",
    "combinedScore": "",
    "diathesis": "",
    "englishLevel": "",
    "experiment": "",
    "id": "",
    "mathLevel": "",
    "orderCode": 0,
    "physicsLevel": "",
    "politicsLevel": "",
    "sumScore": ""
  }
}
```


**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|input|input|body|true|UpdateStuInfoManageDTO|UpdateStuInfoManageDTO|
|&emsp;&emsp;asCityOthersMatedVO|是否已本市其他录取||false|AsCityOthersMatedVO|AsCityOthersMatedVO|
|&emsp;&emsp;&emsp;&emsp;commander|委托人||false|string||
|&emsp;&emsp;&emsp;&emsp;connector|联系单位或联系人||false|string||
|&emsp;&emsp;&emsp;&emsp;isCityOthersMated|是否本市其他录取||false|integer||
|&emsp;&emsp;oldArchiveCode|原学生准考证||false|string||
|&emsp;&emsp;stuInfo|学生信息||false|StuInfoVO|StuInfoVO|
|&emsp;&emsp;&emsp;&emsp;address|现住地址||false|string||
|&emsp;&emsp;&emsp;&emsp;archiveCode|准考证号||false|string||
|&emsp;&emsp;&emsp;&emsp;finishSchoolCode|毕业学校||false|string||
|&emsp;&emsp;&emsp;&emsp;graduateDate|毕业时间||false|string||
|&emsp;&emsp;&emsp;&emsp;id|主键||false|string||
|&emsp;&emsp;&emsp;&emsp;identityCode|身份证号||false|string||
|&emsp;&emsp;&emsp;&emsp;isAreaStudent|地段生||false|integer||
|&emsp;&emsp;&emsp;&emsp;isDeadLock|是否冻结||false|integer||
|&emsp;&emsp;&emsp;&emsp;isMilitary|优抚对象||false|integer||
|&emsp;&emsp;&emsp;&emsp;nationCode|民族||false|string||
|&emsp;&emsp;&emsp;&emsp;opinion|评语||false|string||
|&emsp;&emsp;&emsp;&emsp;phoneCode|电话||false|string||
|&emsp;&emsp;&emsp;&emsp;polity|政治面貌||false|string||
|&emsp;&emsp;&emsp;&emsp;postCode|邮政编码||false|string||
|&emsp;&emsp;&emsp;&emsp;sex|性别||false|string||
|&emsp;&emsp;&emsp;&emsp;studentKind|考生类别||false|string||
|&emsp;&emsp;&emsp;&emsp;studentName|姓名||false|string||
|&emsp;&emsp;stuMatedInfo|学生报名信息||false|StuMatedInfoVO|StuMatedInfoVO|
|&emsp;&emsp;&emsp;&emsp;archiveCode|准考证号||false|string||
|&emsp;&emsp;&emsp;&emsp;fillTime|填报时间||false|string||
|&emsp;&emsp;&emsp;&emsp;highSchoolCode|报名高中||false|string||
|&emsp;&emsp;&emsp;&emsp;id|主键||false|string||
|&emsp;&emsp;&emsp;&emsp;isLock|是否锁定||false|integer||
|&emsp;&emsp;&emsp;&emsp;isLodging|是否住宿||false|integer||
|&emsp;&emsp;&emsp;&emsp;matriculateStatus|录取状态||false|integer||
|&emsp;&emsp;&emsp;&emsp;matriculateTime|录取时间||false|string||
|&emsp;&emsp;&emsp;&emsp;matriculateType|录取类型||false|string||
|&emsp;&emsp;&emsp;&emsp;remarkOfMatriculate|录取说明||false|string||
|&emsp;&emsp;&emsp;&emsp;signUpType|报名类型||false|string||
|&emsp;&emsp;stuScore|学生成绩||false|StuScoreVO|StuScoreVO|
|&emsp;&emsp;&emsp;&emsp;archiveCode|准考证号||false|string||
|&emsp;&emsp;&emsp;&emsp;chineseLevel|语文||false|string||
|&emsp;&emsp;&emsp;&emsp;chymistLevel|化学||false|string||
|&emsp;&emsp;&emsp;&emsp;combinedScore|组合分||false|string||
|&emsp;&emsp;&emsp;&emsp;diathesis|综合素质||false|string||
|&emsp;&emsp;&emsp;&emsp;englishLevel|英语||false|string||
|&emsp;&emsp;&emsp;&emsp;experiment|实验||false|string||
|&emsp;&emsp;&emsp;&emsp;id|主键||false|string||
|&emsp;&emsp;&emsp;&emsp;mathLevel|数学||false|string||
|&emsp;&emsp;&emsp;&emsp;orderCode|排序码||false|number||
|&emsp;&emsp;&emsp;&emsp;physicsLevel|物理||false|string||
|&emsp;&emsp;&emsp;&emsp;politicsLevel|政史||false|string||
|&emsp;&emsp;&emsp;&emsp;sumScore|总分||false|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«List«ArchiveCodeAndNameVO»»|
|201|Created||
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|array|ArchiveCodeAndNameVO|
|&emsp;&emsp;archiveCode|准考证号|string||
|&emsp;&emsp;studentName|姓名|string||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": [
		{
			"archiveCode": "",
			"studentName": ""
		}
	],
	"success": true,
	"timestamp": 0
}
```


# 学生成绩表


## 学生成绩表-添加


**接口地址**:`/nnzk/student/studentScore/add`


**请求方式**:`POST`


**请求数据类型**:`application/json`


**响应数据类型**:`*/*`


**接口描述**:<p>学生成绩表-添加</p>



**请求示例**:


```javascript
{
  "addingScore": "",
  "archiveCode": "",
  "chineseLevel": "",
  "chymistLevel": "",
  "combinedScore": "",
  "createBy": "",
  "createTime": "",
  "delFlag": 0,
  "diathesis": "",
  "englishLevel": "",
  "experiment": "",
  "id": "",
  "mathLevel": "",
  "orderCode": 0,
  "physicalEduLevel": "",
  "physicsLevel": "",
  "politicsLevel": "",
  "sumScore": "",
  "updateBy": "",
  "updateTime": ""
}
```


**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|studentScore|学生成绩表|body|true|student_score对象|student_score对象|
|&emsp;&emsp;addingScore|照顾分||false|string||
|&emsp;&emsp;archiveCode|准考证号||false|string||
|&emsp;&emsp;chineseLevel|语文||false|string||
|&emsp;&emsp;chymistLevel|化学||false|string||
|&emsp;&emsp;combinedScore|组合分||false|string||
|&emsp;&emsp;createBy|创建人||false|string||
|&emsp;&emsp;createTime|创建日期||false|string(date-time)||
|&emsp;&emsp;delFlag|删除标识||false|integer(int32)||
|&emsp;&emsp;diathesis|综合素质||false|string||
|&emsp;&emsp;englishLevel|英语||false|string||
|&emsp;&emsp;experiment|实验||false|string||
|&emsp;&emsp;id|主键||false|string||
|&emsp;&emsp;mathLevel|数学||false|string||
|&emsp;&emsp;orderCode|排序码||false|number||
|&emsp;&emsp;physicalEduLevel|体育||false|string||
|&emsp;&emsp;physicsLevel|物理||false|string||
|&emsp;&emsp;politicsLevel|政史||false|string||
|&emsp;&emsp;sumScore|总分||false|string||
|&emsp;&emsp;updateBy|更新人||false|string||
|&emsp;&emsp;updateTime|更新日期||false|string(date-time)||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«string»|
|201|Created||
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|string||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": "",
	"success": true,
	"timestamp": 0
}
```


## 学生成绩表-通过id删除


**接口地址**:`/nnzk/student/studentScore/delete`


**请求方式**:`DELETE`


**请求数据类型**:`application/x-www-form-urlencoded`


**响应数据类型**:`*/*`


**接口描述**:<p>学生成绩表-通过id删除</p>



**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|id|id|query|true|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«string»|
|204|No Content||
|401|Unauthorized||
|403|Forbidden||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|string||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": "",
	"success": true,
	"timestamp": 0
}
```


## 学生成绩表-批量删除


**接口地址**:`/nnzk/student/studentScore/deleteBatch`


**请求方式**:`DELETE`


**请求数据类型**:`application/x-www-form-urlencoded`


**响应数据类型**:`*/*`


**接口描述**:<p>学生成绩表-批量删除</p>



**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|ids|ids|query|true|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«string»|
|204|No Content||
|401|Unauthorized||
|403|Forbidden||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|string||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": "",
	"success": true,
	"timestamp": 0
}
```


## 学生成绩表-编辑


**接口地址**:`/nnzk/student/studentScore/edit`


**请求方式**:`POST`


**请求数据类型**:`application/json`


**响应数据类型**:`*/*`


**接口描述**:<p>学生成绩表-编辑</p>



**请求示例**:


```javascript
{
  "addingScore": "",
  "archiveCode": "",
  "chineseLevel": "",
  "chymistLevel": "",
  "combinedScore": "",
  "createBy": "",
  "createTime": "",
  "delFlag": 0,
  "diathesis": "",
  "englishLevel": "",
  "experiment": "",
  "id": "",
  "mathLevel": "",
  "orderCode": 0,
  "physicalEduLevel": "",
  "physicsLevel": "",
  "politicsLevel": "",
  "sumScore": "",
  "updateBy": "",
  "updateTime": ""
}
```


**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|studentScore|学生成绩表|body|true|student_score对象|student_score对象|
|&emsp;&emsp;addingScore|照顾分||false|string||
|&emsp;&emsp;archiveCode|准考证号||false|string||
|&emsp;&emsp;chineseLevel|语文||false|string||
|&emsp;&emsp;chymistLevel|化学||false|string||
|&emsp;&emsp;combinedScore|组合分||false|string||
|&emsp;&emsp;createBy|创建人||false|string||
|&emsp;&emsp;createTime|创建日期||false|string(date-time)||
|&emsp;&emsp;delFlag|删除标识||false|integer(int32)||
|&emsp;&emsp;diathesis|综合素质||false|string||
|&emsp;&emsp;englishLevel|英语||false|string||
|&emsp;&emsp;experiment|实验||false|string||
|&emsp;&emsp;id|主键||false|string||
|&emsp;&emsp;mathLevel|数学||false|string||
|&emsp;&emsp;orderCode|排序码||false|number||
|&emsp;&emsp;physicalEduLevel|体育||false|string||
|&emsp;&emsp;physicsLevel|物理||false|string||
|&emsp;&emsp;politicsLevel|政史||false|string||
|&emsp;&emsp;sumScore|总分||false|string||
|&emsp;&emsp;updateBy|更新人||false|string||
|&emsp;&emsp;updateTime|更新日期||false|string(date-time)||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«string»|
|201|Created||
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|string||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": "",
	"success": true,
	"timestamp": 0
}
```


## 学生成绩表-编辑


**接口地址**:`/nnzk/student/studentScore/edit`


**请求方式**:`PUT`


**请求数据类型**:`application/json`


**响应数据类型**:`*/*`


**接口描述**:<p>学生成绩表-编辑</p>



**请求示例**:


```javascript
{
  "addingScore": "",
  "archiveCode": "",
  "chineseLevel": "",
  "chymistLevel": "",
  "combinedScore": "",
  "createBy": "",
  "createTime": "",
  "delFlag": 0,
  "diathesis": "",
  "englishLevel": "",
  "experiment": "",
  "id": "",
  "mathLevel": "",
  "orderCode": 0,
  "physicalEduLevel": "",
  "physicsLevel": "",
  "politicsLevel": "",
  "sumScore": "",
  "updateBy": "",
  "updateTime": ""
}
```


**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|studentScore|学生成绩表|body|true|student_score对象|student_score对象|
|&emsp;&emsp;addingScore|照顾分||false|string||
|&emsp;&emsp;archiveCode|准考证号||false|string||
|&emsp;&emsp;chineseLevel|语文||false|string||
|&emsp;&emsp;chymistLevel|化学||false|string||
|&emsp;&emsp;combinedScore|组合分||false|string||
|&emsp;&emsp;createBy|创建人||false|string||
|&emsp;&emsp;createTime|创建日期||false|string(date-time)||
|&emsp;&emsp;delFlag|删除标识||false|integer(int32)||
|&emsp;&emsp;diathesis|综合素质||false|string||
|&emsp;&emsp;englishLevel|英语||false|string||
|&emsp;&emsp;experiment|实验||false|string||
|&emsp;&emsp;id|主键||false|string||
|&emsp;&emsp;mathLevel|数学||false|string||
|&emsp;&emsp;orderCode|排序码||false|number||
|&emsp;&emsp;physicalEduLevel|体育||false|string||
|&emsp;&emsp;physicsLevel|物理||false|string||
|&emsp;&emsp;politicsLevel|政史||false|string||
|&emsp;&emsp;sumScore|总分||false|string||
|&emsp;&emsp;updateBy|更新人||false|string||
|&emsp;&emsp;updateTime|更新日期||false|string(date-time)||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«string»|
|201|Created||
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|string||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": "",
	"success": true,
	"timestamp": 0
}
```


## 学生成绩表-导出


**接口地址**:`/nnzk/student/studentScore/exportXls`


**请求方式**:`GET`


**请求数据类型**:`application/x-www-form-urlencoded`


**响应数据类型**:`*/*`


**接口描述**:<p>学生成绩表-导出</p>



**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|archiveCode|准考证号|query|true|string||
|chineseLevel|语文|query|true|string||
|chymistLevel|化学|query|true|string||
|combinedScore|组合分|query|true|string||
|diathesis|综合素质|query|true|string||
|englishLevel|英语|query|true|string||
|experiment|实验|query|true|string||
|mathLevel|数学|query|true|string||
|physicsLevel|物理|query|true|string||
|politicsLevel|政史|query|true|string||
|sumScore|总分|query|true|string||
|addingScore|照顾分|query|false|string||
|createBy|创建人|query|false|string||
|createTime|创建日期|query|false|string(date-time)||
|delFlag|删除标识|query|false|integer(int32)||
|id|主键|query|false|string||
|orderCode|排序码|query|false|number||
|physicalEduLevel|体育|query|false|string||
|updateBy|更新人|query|false|string||
|updateTime|更新日期|query|false|string(date-time)||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|ModelAndView|
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|empty||boolean||
|model||object||
|modelMap||object||
|reference||boolean||
|status|可用值:ACCEPTED,ALREADY_REPORTED,BAD_GATEWAY,BAD_REQUEST,BANDWIDTH_LIMIT_EXCEEDED,CHECKPOINT,CONFLICT,CONTINUE,CREATED,DESTINATION_LOCKED,EXPECTATION_FAILED,FAILED_DEPENDENCY,FORBIDDEN,FOUND,GATEWAY_TIMEOUT,GONE,HTTP_VERSION_NOT_SUPPORTED,IM_USED,INSUFFICIENT_SPACE_ON_RESOURCE,INSUFFICIENT_STORAGE,INTERNAL_SERVER_ERROR,I_AM_A_TEAPOT,LENGTH_REQUIRED,LOCKED,LOOP_DETECTED,METHOD_FAILURE,METHOD_NOT_ALLOWED,MOVED_PERMANENTLY,MOVED_TEMPORARILY,MULTIPLE_CHOICES,MULTI_STATUS,NETWORK_AUTHENTICATION_REQUIRED,NON_AUTHORITATIVE_INFORMATION,NOT_ACCEPTABLE,NOT_EXTENDED,NOT_FOUND,NOT_IMPLEMENTED,NOT_MODIFIED,NO_CONTENT,OK,PARTIAL_CONTENT,PAYLOAD_TOO_LARGE,PAYMENT_REQUIRED,PERMANENT_REDIRECT,PRECONDITION_FAILED,PRECONDITION_REQUIRED,PROCESSING,PROXY_AUTHENTICATION_REQUIRED,REQUESTED_RANGE_NOT_SATISFIABLE,REQUEST_ENTITY_TOO_LARGE,REQUEST_HEADER_FIELDS_TOO_LARGE,REQUEST_TIMEOUT,REQUEST_URI_TOO_LONG,RESET_CONTENT,SEE_OTHER,SERVICE_UNAVAILABLE,SWITCHING_PROTOCOLS,TEMPORARY_REDIRECT,TOO_EARLY,TOO_MANY_REQUESTS,UNAUTHORIZED,UNAVAILABLE_FOR_LEGAL_REASONS,UNPROCESSABLE_ENTITY,UNSUPPORTED_MEDIA_TYPE,UPGRADE_REQUIRED,URI_TOO_LONG,USE_PROXY,VARIANT_ALSO_NEGOTIATES|string||
|view||View|View|
|&emsp;&emsp;contentType||string||
|viewName||string||


**响应示例**:
```javascript
{
	"empty": true,
	"model": {},
	"modelMap": {},
	"reference": true,
	"status": "",
	"view": {
		"contentType": ""
	},
	"viewName": ""
}
```


## 学生成绩表-导出


**接口地址**:`/nnzk/student/studentScore/exportXls`


**请求方式**:`POST`


**请求数据类型**:`application/json`


**响应数据类型**:`*/*`


**接口描述**:<p>学生成绩表-导出</p>



**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|archiveCode|准考证号|query|true|string||
|chineseLevel|语文|query|true|string||
|chymistLevel|化学|query|true|string||
|combinedScore|组合分|query|true|string||
|diathesis|综合素质|query|true|string||
|englishLevel|英语|query|true|string||
|experiment|实验|query|true|string||
|mathLevel|数学|query|true|string||
|physicsLevel|物理|query|true|string||
|politicsLevel|政史|query|true|string||
|sumScore|总分|query|true|string||
|addingScore|照顾分|query|false|string||
|createBy|创建人|query|false|string||
|createTime|创建日期|query|false|string(date-time)||
|delFlag|删除标识|query|false|integer(int32)||
|id|主键|query|false|string||
|orderCode|排序码|query|false|number||
|physicalEduLevel|体育|query|false|string||
|updateBy|更新人|query|false|string||
|updateTime|更新日期|query|false|string(date-time)||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|ModelAndView|
|201|Created||
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|empty||boolean||
|model||object||
|modelMap||object||
|reference||boolean||
|status|可用值:ACCEPTED,ALREADY_REPORTED,BAD_GATEWAY,BAD_REQUEST,BANDWIDTH_LIMIT_EXCEEDED,CHECKPOINT,CONFLICT,CONTINUE,CREATED,DESTINATION_LOCKED,EXPECTATION_FAILED,FAILED_DEPENDENCY,FORBIDDEN,FOUND,GATEWAY_TIMEOUT,GONE,HTTP_VERSION_NOT_SUPPORTED,IM_USED,INSUFFICIENT_SPACE_ON_RESOURCE,INSUFFICIENT_STORAGE,INTERNAL_SERVER_ERROR,I_AM_A_TEAPOT,LENGTH_REQUIRED,LOCKED,LOOP_DETECTED,METHOD_FAILURE,METHOD_NOT_ALLOWED,MOVED_PERMANENTLY,MOVED_TEMPORARILY,MULTIPLE_CHOICES,MULTI_STATUS,NETWORK_AUTHENTICATION_REQUIRED,NON_AUTHORITATIVE_INFORMATION,NOT_ACCEPTABLE,NOT_EXTENDED,NOT_FOUND,NOT_IMPLEMENTED,NOT_MODIFIED,NO_CONTENT,OK,PARTIAL_CONTENT,PAYLOAD_TOO_LARGE,PAYMENT_REQUIRED,PERMANENT_REDIRECT,PRECONDITION_FAILED,PRECONDITION_REQUIRED,PROCESSING,PROXY_AUTHENTICATION_REQUIRED,REQUESTED_RANGE_NOT_SATISFIABLE,REQUEST_ENTITY_TOO_LARGE,REQUEST_HEADER_FIELDS_TOO_LARGE,REQUEST_TIMEOUT,REQUEST_URI_TOO_LONG,RESET_CONTENT,SEE_OTHER,SERVICE_UNAVAILABLE,SWITCHING_PROTOCOLS,TEMPORARY_REDIRECT,TOO_EARLY,TOO_MANY_REQUESTS,UNAUTHORIZED,UNAVAILABLE_FOR_LEGAL_REASONS,UNPROCESSABLE_ENTITY,UNSUPPORTED_MEDIA_TYPE,UPGRADE_REQUIRED,URI_TOO_LONG,USE_PROXY,VARIANT_ALSO_NEGOTIATES|string||
|view||View|View|
|&emsp;&emsp;contentType||string||
|viewName||string||


**响应示例**:
```javascript
{
	"empty": true,
	"model": {},
	"modelMap": {},
	"reference": true,
	"status": "",
	"view": {
		"contentType": ""
	},
	"viewName": ""
}
```


## 学生成绩表-导出


**接口地址**:`/nnzk/student/studentScore/exportXls`


**请求方式**:`PUT`


**请求数据类型**:`application/json`


**响应数据类型**:`*/*`


**接口描述**:<p>学生成绩表-导出</p>



**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|archiveCode|准考证号|query|true|string||
|chineseLevel|语文|query|true|string||
|chymistLevel|化学|query|true|string||
|combinedScore|组合分|query|true|string||
|diathesis|综合素质|query|true|string||
|englishLevel|英语|query|true|string||
|experiment|实验|query|true|string||
|mathLevel|数学|query|true|string||
|physicsLevel|物理|query|true|string||
|politicsLevel|政史|query|true|string||
|sumScore|总分|query|true|string||
|addingScore|照顾分|query|false|string||
|createBy|创建人|query|false|string||
|createTime|创建日期|query|false|string(date-time)||
|delFlag|删除标识|query|false|integer(int32)||
|id|主键|query|false|string||
|orderCode|排序码|query|false|number||
|physicalEduLevel|体育|query|false|string||
|updateBy|更新人|query|false|string||
|updateTime|更新日期|query|false|string(date-time)||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|ModelAndView|
|201|Created||
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|empty||boolean||
|model||object||
|modelMap||object||
|reference||boolean||
|status|可用值:ACCEPTED,ALREADY_REPORTED,BAD_GATEWAY,BAD_REQUEST,BANDWIDTH_LIMIT_EXCEEDED,CHECKPOINT,CONFLICT,CONTINUE,CREATED,DESTINATION_LOCKED,EXPECTATION_FAILED,FAILED_DEPENDENCY,FORBIDDEN,FOUND,GATEWAY_TIMEOUT,GONE,HTTP_VERSION_NOT_SUPPORTED,IM_USED,INSUFFICIENT_SPACE_ON_RESOURCE,INSUFFICIENT_STORAGE,INTERNAL_SERVER_ERROR,I_AM_A_TEAPOT,LENGTH_REQUIRED,LOCKED,LOOP_DETECTED,METHOD_FAILURE,METHOD_NOT_ALLOWED,MOVED_PERMANENTLY,MOVED_TEMPORARILY,MULTIPLE_CHOICES,MULTI_STATUS,NETWORK_AUTHENTICATION_REQUIRED,NON_AUTHORITATIVE_INFORMATION,NOT_ACCEPTABLE,NOT_EXTENDED,NOT_FOUND,NOT_IMPLEMENTED,NOT_MODIFIED,NO_CONTENT,OK,PARTIAL_CONTENT,PAYLOAD_TOO_LARGE,PAYMENT_REQUIRED,PERMANENT_REDIRECT,PRECONDITION_FAILED,PRECONDITION_REQUIRED,PROCESSING,PROXY_AUTHENTICATION_REQUIRED,REQUESTED_RANGE_NOT_SATISFIABLE,REQUEST_ENTITY_TOO_LARGE,REQUEST_HEADER_FIELDS_TOO_LARGE,REQUEST_TIMEOUT,REQUEST_URI_TOO_LONG,RESET_CONTENT,SEE_OTHER,SERVICE_UNAVAILABLE,SWITCHING_PROTOCOLS,TEMPORARY_REDIRECT,TOO_EARLY,TOO_MANY_REQUESTS,UNAUTHORIZED,UNAVAILABLE_FOR_LEGAL_REASONS,UNPROCESSABLE_ENTITY,UNSUPPORTED_MEDIA_TYPE,UPGRADE_REQUIRED,URI_TOO_LONG,USE_PROXY,VARIANT_ALSO_NEGOTIATES|string||
|view||View|View|
|&emsp;&emsp;contentType||string||
|viewName||string||


**响应示例**:
```javascript
{
	"empty": true,
	"model": {},
	"modelMap": {},
	"reference": true,
	"status": "",
	"view": {
		"contentType": ""
	},
	"viewName": ""
}
```


## 学生成绩表-导出


**接口地址**:`/nnzk/student/studentScore/exportXls`


**请求方式**:`DELETE`


**请求数据类型**:`application/x-www-form-urlencoded`


**响应数据类型**:`*/*`


**接口描述**:<p>学生成绩表-导出</p>



**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|archiveCode|准考证号|query|true|string||
|chineseLevel|语文|query|true|string||
|chymistLevel|化学|query|true|string||
|combinedScore|组合分|query|true|string||
|diathesis|综合素质|query|true|string||
|englishLevel|英语|query|true|string||
|experiment|实验|query|true|string||
|mathLevel|数学|query|true|string||
|physicsLevel|物理|query|true|string||
|politicsLevel|政史|query|true|string||
|sumScore|总分|query|true|string||
|addingScore|照顾分|query|false|string||
|createBy|创建人|query|false|string||
|createTime|创建日期|query|false|string(date-time)||
|delFlag|删除标识|query|false|integer(int32)||
|id|主键|query|false|string||
|orderCode|排序码|query|false|number||
|physicalEduLevel|体育|query|false|string||
|updateBy|更新人|query|false|string||
|updateTime|更新日期|query|false|string(date-time)||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|ModelAndView|
|204|No Content||
|401|Unauthorized||
|403|Forbidden||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|empty||boolean||
|model||object||
|modelMap||object||
|reference||boolean||
|status|可用值:ACCEPTED,ALREADY_REPORTED,BAD_GATEWAY,BAD_REQUEST,BANDWIDTH_LIMIT_EXCEEDED,CHECKPOINT,CONFLICT,CONTINUE,CREATED,DESTINATION_LOCKED,EXPECTATION_FAILED,FAILED_DEPENDENCY,FORBIDDEN,FOUND,GATEWAY_TIMEOUT,GONE,HTTP_VERSION_NOT_SUPPORTED,IM_USED,INSUFFICIENT_SPACE_ON_RESOURCE,INSUFFICIENT_STORAGE,INTERNAL_SERVER_ERROR,I_AM_A_TEAPOT,LENGTH_REQUIRED,LOCKED,LOOP_DETECTED,METHOD_FAILURE,METHOD_NOT_ALLOWED,MOVED_PERMANENTLY,MOVED_TEMPORARILY,MULTIPLE_CHOICES,MULTI_STATUS,NETWORK_AUTHENTICATION_REQUIRED,NON_AUTHORITATIVE_INFORMATION,NOT_ACCEPTABLE,NOT_EXTENDED,NOT_FOUND,NOT_IMPLEMENTED,NOT_MODIFIED,NO_CONTENT,OK,PARTIAL_CONTENT,PAYLOAD_TOO_LARGE,PAYMENT_REQUIRED,PERMANENT_REDIRECT,PRECONDITION_FAILED,PRECONDITION_REQUIRED,PROCESSING,PROXY_AUTHENTICATION_REQUIRED,REQUESTED_RANGE_NOT_SATISFIABLE,REQUEST_ENTITY_TOO_LARGE,REQUEST_HEADER_FIELDS_TOO_LARGE,REQUEST_TIMEOUT,REQUEST_URI_TOO_LONG,RESET_CONTENT,SEE_OTHER,SERVICE_UNAVAILABLE,SWITCHING_PROTOCOLS,TEMPORARY_REDIRECT,TOO_EARLY,TOO_MANY_REQUESTS,UNAUTHORIZED,UNAVAILABLE_FOR_LEGAL_REASONS,UNPROCESSABLE_ENTITY,UNSUPPORTED_MEDIA_TYPE,UPGRADE_REQUIRED,URI_TOO_LONG,USE_PROXY,VARIANT_ALSO_NEGOTIATES|string||
|view||View|View|
|&emsp;&emsp;contentType||string||
|viewName||string||


**响应示例**:
```javascript
{
	"empty": true,
	"model": {},
	"modelMap": {},
	"reference": true,
	"status": "",
	"view": {
		"contentType": ""
	},
	"viewName": ""
}
```


## 学生成绩表-导出


**接口地址**:`/nnzk/student/studentScore/exportXls`


**请求方式**:`PATCH`


**请求数据类型**:`application/json`


**响应数据类型**:`*/*`


**接口描述**:<p>学生成绩表-导出</p>



**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|archiveCode|准考证号|query|true|string||
|chineseLevel|语文|query|true|string||
|chymistLevel|化学|query|true|string||
|combinedScore|组合分|query|true|string||
|diathesis|综合素质|query|true|string||
|englishLevel|英语|query|true|string||
|experiment|实验|query|true|string||
|mathLevel|数学|query|true|string||
|physicsLevel|物理|query|true|string||
|politicsLevel|政史|query|true|string||
|sumScore|总分|query|true|string||
|addingScore|照顾分|query|false|string||
|createBy|创建人|query|false|string||
|createTime|创建日期|query|false|string(date-time)||
|delFlag|删除标识|query|false|integer(int32)||
|id|主键|query|false|string||
|orderCode|排序码|query|false|number||
|physicalEduLevel|体育|query|false|string||
|updateBy|更新人|query|false|string||
|updateTime|更新日期|query|false|string(date-time)||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|ModelAndView|
|204|No Content||
|401|Unauthorized||
|403|Forbidden||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|empty||boolean||
|model||object||
|modelMap||object||
|reference||boolean||
|status|可用值:ACCEPTED,ALREADY_REPORTED,BAD_GATEWAY,BAD_REQUEST,BANDWIDTH_LIMIT_EXCEEDED,CHECKPOINT,CONFLICT,CONTINUE,CREATED,DESTINATION_LOCKED,EXPECTATION_FAILED,FAILED_DEPENDENCY,FORBIDDEN,FOUND,GATEWAY_TIMEOUT,GONE,HTTP_VERSION_NOT_SUPPORTED,IM_USED,INSUFFICIENT_SPACE_ON_RESOURCE,INSUFFICIENT_STORAGE,INTERNAL_SERVER_ERROR,I_AM_A_TEAPOT,LENGTH_REQUIRED,LOCKED,LOOP_DETECTED,METHOD_FAILURE,METHOD_NOT_ALLOWED,MOVED_PERMANENTLY,MOVED_TEMPORARILY,MULTIPLE_CHOICES,MULTI_STATUS,NETWORK_AUTHENTICATION_REQUIRED,NON_AUTHORITATIVE_INFORMATION,NOT_ACCEPTABLE,NOT_EXTENDED,NOT_FOUND,NOT_IMPLEMENTED,NOT_MODIFIED,NO_CONTENT,OK,PARTIAL_CONTENT,PAYLOAD_TOO_LARGE,PAYMENT_REQUIRED,PERMANENT_REDIRECT,PRECONDITION_FAILED,PRECONDITION_REQUIRED,PROCESSING,PROXY_AUTHENTICATION_REQUIRED,REQUESTED_RANGE_NOT_SATISFIABLE,REQUEST_ENTITY_TOO_LARGE,REQUEST_HEADER_FIELDS_TOO_LARGE,REQUEST_TIMEOUT,REQUEST_URI_TOO_LONG,RESET_CONTENT,SEE_OTHER,SERVICE_UNAVAILABLE,SWITCHING_PROTOCOLS,TEMPORARY_REDIRECT,TOO_EARLY,TOO_MANY_REQUESTS,UNAUTHORIZED,UNAVAILABLE_FOR_LEGAL_REASONS,UNPROCESSABLE_ENTITY,UNSUPPORTED_MEDIA_TYPE,UPGRADE_REQUIRED,URI_TOO_LONG,USE_PROXY,VARIANT_ALSO_NEGOTIATES|string||
|view||View|View|
|&emsp;&emsp;contentType||string||
|viewName||string||


**响应示例**:
```javascript
{
	"empty": true,
	"model": {},
	"modelMap": {},
	"reference": true,
	"status": "",
	"view": {
		"contentType": ""
	},
	"viewName": ""
}
```


## 学生成绩表-导出


**接口地址**:`/nnzk/student/studentScore/exportXls`


**请求方式**:`OPTIONS`


**请求数据类型**:`application/json`


**响应数据类型**:`*/*`


**接口描述**:<p>学生成绩表-导出</p>



**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|archiveCode|准考证号|query|true|string||
|chineseLevel|语文|query|true|string||
|chymistLevel|化学|query|true|string||
|combinedScore|组合分|query|true|string||
|diathesis|综合素质|query|true|string||
|englishLevel|英语|query|true|string||
|experiment|实验|query|true|string||
|mathLevel|数学|query|true|string||
|physicsLevel|物理|query|true|string||
|politicsLevel|政史|query|true|string||
|sumScore|总分|query|true|string||
|addingScore|照顾分|query|false|string||
|createBy|创建人|query|false|string||
|createTime|创建日期|query|false|string(date-time)||
|delFlag|删除标识|query|false|integer(int32)||
|id|主键|query|false|string||
|orderCode|排序码|query|false|number||
|physicalEduLevel|体育|query|false|string||
|updateBy|更新人|query|false|string||
|updateTime|更新日期|query|false|string(date-time)||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|ModelAndView|
|204|No Content||
|401|Unauthorized||
|403|Forbidden||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|empty||boolean||
|model||object||
|modelMap||object||
|reference||boolean||
|status|可用值:ACCEPTED,ALREADY_REPORTED,BAD_GATEWAY,BAD_REQUEST,BANDWIDTH_LIMIT_EXCEEDED,CHECKPOINT,CONFLICT,CONTINUE,CREATED,DESTINATION_LOCKED,EXPECTATION_FAILED,FAILED_DEPENDENCY,FORBIDDEN,FOUND,GATEWAY_TIMEOUT,GONE,HTTP_VERSION_NOT_SUPPORTED,IM_USED,INSUFFICIENT_SPACE_ON_RESOURCE,INSUFFICIENT_STORAGE,INTERNAL_SERVER_ERROR,I_AM_A_TEAPOT,LENGTH_REQUIRED,LOCKED,LOOP_DETECTED,METHOD_FAILURE,METHOD_NOT_ALLOWED,MOVED_PERMANENTLY,MOVED_TEMPORARILY,MULTIPLE_CHOICES,MULTI_STATUS,NETWORK_AUTHENTICATION_REQUIRED,NON_AUTHORITATIVE_INFORMATION,NOT_ACCEPTABLE,NOT_EXTENDED,NOT_FOUND,NOT_IMPLEMENTED,NOT_MODIFIED,NO_CONTENT,OK,PARTIAL_CONTENT,PAYLOAD_TOO_LARGE,PAYMENT_REQUIRED,PERMANENT_REDIRECT,PRECONDITION_FAILED,PRECONDITION_REQUIRED,PROCESSING,PROXY_AUTHENTICATION_REQUIRED,REQUESTED_RANGE_NOT_SATISFIABLE,REQUEST_ENTITY_TOO_LARGE,REQUEST_HEADER_FIELDS_TOO_LARGE,REQUEST_TIMEOUT,REQUEST_URI_TOO_LONG,RESET_CONTENT,SEE_OTHER,SERVICE_UNAVAILABLE,SWITCHING_PROTOCOLS,TEMPORARY_REDIRECT,TOO_EARLY,TOO_MANY_REQUESTS,UNAUTHORIZED,UNAVAILABLE_FOR_LEGAL_REASONS,UNPROCESSABLE_ENTITY,UNSUPPORTED_MEDIA_TYPE,UPGRADE_REQUIRED,URI_TOO_LONG,USE_PROXY,VARIANT_ALSO_NEGOTIATES|string||
|view||View|View|
|&emsp;&emsp;contentType||string||
|viewName||string||


**响应示例**:
```javascript
{
	"empty": true,
	"model": {},
	"modelMap": {},
	"reference": true,
	"status": "",
	"view": {
		"contentType": ""
	},
	"viewName": ""
}
```


## 学生成绩表-导出


**接口地址**:`/nnzk/student/studentScore/exportXls`


**请求方式**:`HEAD`


**请求数据类型**:`application/json`


**响应数据类型**:`*/*`


**接口描述**:<p>学生成绩表-导出</p>



**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|archiveCode|准考证号|query|true|string||
|chineseLevel|语文|query|true|string||
|chymistLevel|化学|query|true|string||
|combinedScore|组合分|query|true|string||
|diathesis|综合素质|query|true|string||
|englishLevel|英语|query|true|string||
|experiment|实验|query|true|string||
|mathLevel|数学|query|true|string||
|physicsLevel|物理|query|true|string||
|politicsLevel|政史|query|true|string||
|sumScore|总分|query|true|string||
|addingScore|照顾分|query|false|string||
|createBy|创建人|query|false|string||
|createTime|创建日期|query|false|string(date-time)||
|delFlag|删除标识|query|false|integer(int32)||
|id|主键|query|false|string||
|orderCode|排序码|query|false|number||
|physicalEduLevel|体育|query|false|string||
|updateBy|更新人|query|false|string||
|updateTime|更新日期|query|false|string(date-time)||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|ModelAndView|
|204|No Content||
|401|Unauthorized||
|403|Forbidden||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|empty||boolean||
|model||object||
|modelMap||object||
|reference||boolean||
|status|可用值:ACCEPTED,ALREADY_REPORTED,BAD_GATEWAY,BAD_REQUEST,BANDWIDTH_LIMIT_EXCEEDED,CHECKPOINT,CONFLICT,CONTINUE,CREATED,DESTINATION_LOCKED,EXPECTATION_FAILED,FAILED_DEPENDENCY,FORBIDDEN,FOUND,GATEWAY_TIMEOUT,GONE,HTTP_VERSION_NOT_SUPPORTED,IM_USED,INSUFFICIENT_SPACE_ON_RESOURCE,INSUFFICIENT_STORAGE,INTERNAL_SERVER_ERROR,I_AM_A_TEAPOT,LENGTH_REQUIRED,LOCKED,LOOP_DETECTED,METHOD_FAILURE,METHOD_NOT_ALLOWED,MOVED_PERMANENTLY,MOVED_TEMPORARILY,MULTIPLE_CHOICES,MULTI_STATUS,NETWORK_AUTHENTICATION_REQUIRED,NON_AUTHORITATIVE_INFORMATION,NOT_ACCEPTABLE,NOT_EXTENDED,NOT_FOUND,NOT_IMPLEMENTED,NOT_MODIFIED,NO_CONTENT,OK,PARTIAL_CONTENT,PAYLOAD_TOO_LARGE,PAYMENT_REQUIRED,PERMANENT_REDIRECT,PRECONDITION_FAILED,PRECONDITION_REQUIRED,PROCESSING,PROXY_AUTHENTICATION_REQUIRED,REQUESTED_RANGE_NOT_SATISFIABLE,REQUEST_ENTITY_TOO_LARGE,REQUEST_HEADER_FIELDS_TOO_LARGE,REQUEST_TIMEOUT,REQUEST_URI_TOO_LONG,RESET_CONTENT,SEE_OTHER,SERVICE_UNAVAILABLE,SWITCHING_PROTOCOLS,TEMPORARY_REDIRECT,TOO_EARLY,TOO_MANY_REQUESTS,UNAUTHORIZED,UNAVAILABLE_FOR_LEGAL_REASONS,UNPROCESSABLE_ENTITY,UNSUPPORTED_MEDIA_TYPE,UPGRADE_REQUIRED,URI_TOO_LONG,USE_PROXY,VARIANT_ALSO_NEGOTIATES|string||
|view||View|View|
|&emsp;&emsp;contentType||string||
|viewName||string||


**响应示例**:
```javascript
{
	"empty": true,
	"model": {},
	"modelMap": {},
	"reference": true,
	"status": "",
	"view": {
		"contentType": ""
	},
	"viewName": ""
}
```


## 学生成绩表-导入


**接口地址**:`/nnzk/student/studentScore/importExcel`


**请求方式**:`POST`


**请求数据类型**:`application/json`


**响应数据类型**:`*/*`


**接口描述**:<p>学生成绩表-导入</p>



**请求参数**:


暂无


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«object»|
|201|Created||
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|object||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": {},
	"success": true,
	"timestamp": 0
}
```


## 学生成绩表-分页列表查询


**接口地址**:`/nnzk/student/studentScore/list`


**请求方式**:`GET`


**请求数据类型**:`application/x-www-form-urlencoded`


**响应数据类型**:`*/*`


**接口描述**:<p>学生成绩表-分页列表查询</p>



**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|archiveCode|准考证号|query|true|string||
|chineseLevel|语文|query|true|string||
|chymistLevel|化学|query|true|string||
|combinedScore|组合分|query|true|string||
|diathesis|综合素质|query|true|string||
|englishLevel|英语|query|true|string||
|experiment|实验|query|true|string||
|mathLevel|数学|query|true|string||
|physicsLevel|物理|query|true|string||
|politicsLevel|政史|query|true|string||
|sumScore|总分|query|true|string||
|addingScore|照顾分|query|false|string||
|createBy|创建人|query|false|string||
|createTime|创建日期|query|false|string(date-time)||
|delFlag|删除标识|query|false|integer(int32)||
|id|主键|query|false|string||
|orderCode|排序码|query|false|number||
|pageNo|pageNo|query|false|integer(int32)||
|pageSize|pageSize|query|false|integer(int32)||
|physicalEduLevel|体育|query|false|string||
|updateBy|更新人|query|false|string||
|updateTime|更新日期|query|false|string(date-time)||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«IPage«student_score对象»»|
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|IPage«student_score对象»|IPage«student_score对象»|
|&emsp;&emsp;current||integer(int64)||
|&emsp;&emsp;pages||integer(int64)||
|&emsp;&emsp;records||array|student_score对象|
|&emsp;&emsp;&emsp;&emsp;addingScore|照顾分|string||
|&emsp;&emsp;&emsp;&emsp;archiveCode|准考证号|string||
|&emsp;&emsp;&emsp;&emsp;chineseLevel|语文|string||
|&emsp;&emsp;&emsp;&emsp;chymistLevel|化学|string||
|&emsp;&emsp;&emsp;&emsp;combinedScore|组合分|string||
|&emsp;&emsp;&emsp;&emsp;createBy|创建人|string||
|&emsp;&emsp;&emsp;&emsp;createTime|创建日期|string||
|&emsp;&emsp;&emsp;&emsp;delFlag|删除标识|integer||
|&emsp;&emsp;&emsp;&emsp;diathesis|综合素质|string||
|&emsp;&emsp;&emsp;&emsp;englishLevel|英语|string||
|&emsp;&emsp;&emsp;&emsp;experiment|实验|string||
|&emsp;&emsp;&emsp;&emsp;id|主键|string||
|&emsp;&emsp;&emsp;&emsp;mathLevel|数学|string||
|&emsp;&emsp;&emsp;&emsp;orderCode|排序码|number||
|&emsp;&emsp;&emsp;&emsp;physicalEduLevel|体育|string||
|&emsp;&emsp;&emsp;&emsp;physicsLevel|物理|string||
|&emsp;&emsp;&emsp;&emsp;politicsLevel|政史|string||
|&emsp;&emsp;&emsp;&emsp;sumScore|总分|string||
|&emsp;&emsp;&emsp;&emsp;updateBy|更新人|string||
|&emsp;&emsp;&emsp;&emsp;updateTime|更新日期|string||
|&emsp;&emsp;size||integer(int64)||
|&emsp;&emsp;total||integer(int64)||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": {
		"current": 0,
		"pages": 0,
		"records": [
			{
				"addingScore": "",
				"archiveCode": "",
				"chineseLevel": "",
				"chymistLevel": "",
				"combinedScore": "",
				"createBy": "",
				"createTime": "",
				"delFlag": 0,
				"diathesis": "",
				"englishLevel": "",
				"experiment": "",
				"id": "",
				"mathLevel": "",
				"orderCode": 0,
				"physicalEduLevel": "",
				"physicsLevel": "",
				"politicsLevel": "",
				"sumScore": "",
				"updateBy": "",
				"updateTime": ""
			}
		],
		"size": 0,
		"total": 0
	},
	"success": true,
	"timestamp": 0
}
```


## 学生成绩表-通过准考证号查询


**接口地址**:`/nnzk/student/studentScore/queryByArchiveCode`


**请求方式**:`GET`


**请求数据类型**:`application/x-www-form-urlencoded`


**响应数据类型**:`*/*`


**接口描述**:<p>学生成绩表-通过准考证号查询</p>



**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|archiveCode|archiveCode|query|true|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«student_score对象»|
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|student_score对象|student_score对象|
|&emsp;&emsp;addingScore|照顾分|string||
|&emsp;&emsp;archiveCode|准考证号|string||
|&emsp;&emsp;chineseLevel|语文|string||
|&emsp;&emsp;chymistLevel|化学|string||
|&emsp;&emsp;combinedScore|组合分|string||
|&emsp;&emsp;createBy|创建人|string||
|&emsp;&emsp;createTime|创建日期|string(date-time)||
|&emsp;&emsp;delFlag|删除标识|integer(int32)||
|&emsp;&emsp;diathesis|综合素质|string||
|&emsp;&emsp;englishLevel|英语|string||
|&emsp;&emsp;experiment|实验|string||
|&emsp;&emsp;id|主键|string||
|&emsp;&emsp;mathLevel|数学|string||
|&emsp;&emsp;orderCode|排序码|number||
|&emsp;&emsp;physicalEduLevel|体育|string||
|&emsp;&emsp;physicsLevel|物理|string||
|&emsp;&emsp;politicsLevel|政史|string||
|&emsp;&emsp;sumScore|总分|string||
|&emsp;&emsp;updateBy|更新人|string||
|&emsp;&emsp;updateTime|更新日期|string(date-time)||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": {
		"addingScore": "",
		"archiveCode": "",
		"chineseLevel": "",
		"chymistLevel": "",
		"combinedScore": "",
		"createBy": "",
		"createTime": "",
		"delFlag": 0,
		"diathesis": "",
		"englishLevel": "",
		"experiment": "",
		"id": "",
		"mathLevel": "",
		"orderCode": 0,
		"physicalEduLevel": "",
		"physicsLevel": "",
		"politicsLevel": "",
		"sumScore": "",
		"updateBy": "",
		"updateTime": ""
	},
	"success": true,
	"timestamp": 0
}
```


## 学生成绩表-通过id查询


**接口地址**:`/nnzk/student/studentScore/queryById`


**请求方式**:`GET`


**请求数据类型**:`application/x-www-form-urlencoded`


**响应数据类型**:`*/*`


**接口描述**:<p>学生成绩表-通过id查询</p>



**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|id|id|query|true|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«student_score对象»|
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|student_score对象|student_score对象|
|&emsp;&emsp;addingScore|照顾分|string||
|&emsp;&emsp;archiveCode|准考证号|string||
|&emsp;&emsp;chineseLevel|语文|string||
|&emsp;&emsp;chymistLevel|化学|string||
|&emsp;&emsp;combinedScore|组合分|string||
|&emsp;&emsp;createBy|创建人|string||
|&emsp;&emsp;createTime|创建日期|string(date-time)||
|&emsp;&emsp;delFlag|删除标识|integer(int32)||
|&emsp;&emsp;diathesis|综合素质|string||
|&emsp;&emsp;englishLevel|英语|string||
|&emsp;&emsp;experiment|实验|string||
|&emsp;&emsp;id|主键|string||
|&emsp;&emsp;mathLevel|数学|string||
|&emsp;&emsp;orderCode|排序码|number||
|&emsp;&emsp;physicalEduLevel|体育|string||
|&emsp;&emsp;physicsLevel|物理|string||
|&emsp;&emsp;politicsLevel|政史|string||
|&emsp;&emsp;sumScore|总分|string||
|&emsp;&emsp;updateBy|更新人|string||
|&emsp;&emsp;updateTime|更新日期|string(date-time)||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": {
		"addingScore": "",
		"archiveCode": "",
		"chineseLevel": "",
		"chymistLevel": "",
		"combinedScore": "",
		"createBy": "",
		"createTime": "",
		"delFlag": 0,
		"diathesis": "",
		"englishLevel": "",
		"experiment": "",
		"id": "",
		"mathLevel": "",
		"orderCode": 0,
		"physicalEduLevel": "",
		"physicsLevel": "",
		"politicsLevel": "",
		"sumScore": "",
		"updateBy": "",
		"updateTime": ""
	},
	"success": true,
	"timestamp": 0
}
```


# 学生端公示信息


## 获取初中学校的定向名额使用信息


**接口地址**:`/nnzk/publicityInfor/getMiddleSchoolDirectionalList`


**请求方式**:`GET`


**请求数据类型**:`application/x-www-form-urlencoded`


**响应数据类型**:`*/*`


**接口描述**:<p>获取初中学校的定向名额使用信息</p>



**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|finishSchoolCode|finishSchoolCode|query|true|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«MiddleSchooldirectionalVO»|
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|MiddleSchooldirectionalVO|MiddleSchooldirectionalVO|
|&emsp;&emsp;firstList||array|MidSchoolDirDataDTO|
|&emsp;&emsp;&emsp;&emsp;chineseLevel|语文|string||
|&emsp;&emsp;&emsp;&emsp;chymistLevel|化学|string||
|&emsp;&emsp;&emsp;&emsp;combinedScore|组合分|string||
|&emsp;&emsp;&emsp;&emsp;diathesis|综合素质|string||
|&emsp;&emsp;&emsp;&emsp;englishLevel|英语|string||
|&emsp;&emsp;&emsp;&emsp;experiment|实验|string||
|&emsp;&emsp;&emsp;&emsp;finishSchoolName|毕业学校|string||
|&emsp;&emsp;&emsp;&emsp;mathLevel|数学|string||
|&emsp;&emsp;&emsp;&emsp;orderCode|排序码|number||
|&emsp;&emsp;&emsp;&emsp;physicalEduLevel|体育|string||
|&emsp;&emsp;&emsp;&emsp;physicsLevel|物理|string||
|&emsp;&emsp;&emsp;&emsp;politicsLevel|政史|string||
|&emsp;&emsp;&emsp;&emsp;runtime|运算时间|string||
|&emsp;&emsp;&emsp;&emsp;serial|本校排名|integer||
|&emsp;&emsp;&emsp;&emsp;signupSchoolName|报名高中|string||
|&emsp;&emsp;&emsp;&emsp;sumScore|总分|string||
|&emsp;&emsp;&emsp;&emsp;tempOrder|排名|integer||
|&emsp;&emsp;firstPlan||integer(int32)||
|&emsp;&emsp;firstSchools||array|string|
|&emsp;&emsp;firstUsed||integer(int32)||
|&emsp;&emsp;runTime||string(date-time)||
|&emsp;&emsp;secondList||array|MidSchoolDirDataDTO|
|&emsp;&emsp;&emsp;&emsp;chineseLevel|语文|string||
|&emsp;&emsp;&emsp;&emsp;chymistLevel|化学|string||
|&emsp;&emsp;&emsp;&emsp;combinedScore|组合分|string||
|&emsp;&emsp;&emsp;&emsp;diathesis|综合素质|string||
|&emsp;&emsp;&emsp;&emsp;englishLevel|英语|string||
|&emsp;&emsp;&emsp;&emsp;experiment|实验|string||
|&emsp;&emsp;&emsp;&emsp;finishSchoolName|毕业学校|string||
|&emsp;&emsp;&emsp;&emsp;mathLevel|数学|string||
|&emsp;&emsp;&emsp;&emsp;orderCode|排序码|number||
|&emsp;&emsp;&emsp;&emsp;physicalEduLevel|体育|string||
|&emsp;&emsp;&emsp;&emsp;physicsLevel|物理|string||
|&emsp;&emsp;&emsp;&emsp;politicsLevel|政史|string||
|&emsp;&emsp;&emsp;&emsp;runtime|运算时间|string||
|&emsp;&emsp;&emsp;&emsp;serial|本校排名|integer||
|&emsp;&emsp;&emsp;&emsp;signupSchoolName|报名高中|string||
|&emsp;&emsp;&emsp;&emsp;sumScore|总分|string||
|&emsp;&emsp;&emsp;&emsp;tempOrder|排名|integer||
|&emsp;&emsp;secondPlan||integer(int32)||
|&emsp;&emsp;secondSchools||array|string|
|&emsp;&emsp;secondUsed||integer(int32)||
|&emsp;&emsp;secondarySchool||string||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": {
		"firstList": [
			{
				"chineseLevel": "",
				"chymistLevel": "",
				"combinedScore": "",
				"diathesis": "",
				"englishLevel": "",
				"experiment": "",
				"finishSchoolName": "",
				"mathLevel": "",
				"orderCode": 0,
				"physicalEduLevel": "",
				"physicsLevel": "",
				"politicsLevel": "",
				"runtime": "",
				"serial": 0,
				"signupSchoolName": "",
				"sumScore": "",
				"tempOrder": 0
			}
		],
		"firstPlan": 0,
		"firstSchools": [],
		"firstUsed": 0,
		"runTime": "",
		"secondList": [
			{
				"chineseLevel": "",
				"chymistLevel": "",
				"combinedScore": "",
				"diathesis": "",
				"englishLevel": "",
				"experiment": "",
				"finishSchoolName": "",
				"mathLevel": "",
				"orderCode": 0,
				"physicalEduLevel": "",
				"physicsLevel": "",
				"politicsLevel": "",
				"runtime": "",
				"serial": 0,
				"signupSchoolName": "",
				"sumScore": "",
				"tempOrder": 0
			}
		],
		"secondPlan": 0,
		"secondSchools": [],
		"secondUsed": 0,
		"secondarySchool": ""
	},
	"success": true,
	"timestamp": 0
}
```


## 获取普高招生进度


**接口地址**:`/nnzk/publicityInfor/getProgress`


**请求方式**:`GET`


**请求数据类型**:`application/x-www-form-urlencoded`


**响应数据类型**:`*/*`


**接口描述**:<p>获取普高招生进度</p>



**请求参数**:


暂无


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«SignupProgressDTO»|
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|SignupProgressDTO|SignupProgressDTO|
|&emsp;&emsp;progress||array|ProgressDTO|
|&emsp;&emsp;&emsp;&emsp;guideNum||string||
|&emsp;&emsp;&emsp;&emsp;instNum||string||
|&emsp;&emsp;&emsp;&emsp;schoolCode||string||
|&emsp;&emsp;&emsp;&emsp;schoolName||string||
|&emsp;&emsp;&emsp;&emsp;signupNum||string||
|&emsp;&emsp;&emsp;&emsp;status||string||
|&emsp;&emsp;&emsp;&emsp;statusName||string||
|&emsp;&emsp;runTime||string(date-time)||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": {
		"progress": [
			{
				"guideNum": "",
				"instNum": "",
				"schoolCode": "",
				"schoolName": "",
				"signupNum": "",
				"status": "",
				"statusName": ""
			}
		],
		"runTime": ""
	},
	"success": true,
	"timestamp": 0
}
```


## 获取普高报名公示


**接口地址**:`/nnzk/publicityInfor/getPublicity`


**请求方式**:`GET`


**请求数据类型**:`application/x-www-form-urlencoded`


**响应数据类型**:`*/*`


**接口描述**:<p>获取普高报名公示</p>



**请求参数**:


暂无


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«BmgsMainDTO»|
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|BmgsMainDTO|BmgsMainDTO|
|&emsp;&emsp;bmgs_main||array|BmgsSchDTO|
|&emsp;&emsp;&emsp;&emsp;alterLevel||string||
|&emsp;&emsp;&emsp;&emsp;alterPlan||string||
|&emsp;&emsp;&emsp;&emsp;dirLevel||string||
|&emsp;&emsp;&emsp;&emsp;dirPlan||string||
|&emsp;&emsp;&emsp;&emsp;guideLevel||string||
|&emsp;&emsp;&emsp;&emsp;guidePlan||string||
|&emsp;&emsp;&emsp;&emsp;instLevel||string||
|&emsp;&emsp;&emsp;&emsp;instPlan||string||
|&emsp;&emsp;&emsp;&emsp;schoolCode||string||
|&emsp;&emsp;&emsp;&emsp;schoolName||string||
|&emsp;&emsp;&emsp;&emsp;status||string||
|&emsp;&emsp;runTime||string||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": {
		"bmgs_main": [
			{
				"alterLevel": "",
				"alterPlan": "",
				"dirLevel": "",
				"dirPlan": "",
				"guideLevel": "",
				"guidePlan": "",
				"instLevel": "",
				"instPlan": "",
				"schoolCode": "",
				"schoolName": "",
				"status": ""
			}
		],
		"runTime": ""
	},
	"success": true,
	"timestamp": 0
}
```


## 获取普高报名公示详情


**接口地址**:`/nnzk/publicityInfor/getPublicityDetail`


**请求方式**:`GET`


**请求数据类型**:`application/x-www-form-urlencoded`


**响应数据类型**:`*/*`


**接口描述**:<p>获取普高报名公示详情</p>



**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|schoolCode|schoolCode|query|true|string||
|status|status|query|true|string||
|type|type|query|true|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«BmgsDetailDTO»|
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|BmgsDetailDTO|BmgsDetailDTO|
|&emsp;&emsp;lists||array|ScoreAndOrderDTO|
|&emsp;&emsp;&emsp;&emsp;chineseLevel||string||
|&emsp;&emsp;&emsp;&emsp;chymistLevel||string||
|&emsp;&emsp;&emsp;&emsp;combinedScore||string||
|&emsp;&emsp;&emsp;&emsp;englishLevel||string||
|&emsp;&emsp;&emsp;&emsp;experiment||string||
|&emsp;&emsp;&emsp;&emsp;mathLevel||string||
|&emsp;&emsp;&emsp;&emsp;order||string||
|&emsp;&emsp;&emsp;&emsp;physicsLevel||string||
|&emsp;&emsp;&emsp;&emsp;politicsLevel||string||
|&emsp;&emsp;&emsp;&emsp;serial||string||
|&emsp;&emsp;&emsp;&emsp;sumScore||string||
|&emsp;&emsp;runTime||string||
|&emsp;&emsp;schoolCode||string||
|&emsp;&emsp;schoolName||string||
|&emsp;&emsp;type||string||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": {
		"lists": [
			{
				"chineseLevel": "",
				"chymistLevel": "",
				"combinedScore": "",
				"englishLevel": "",
				"experiment": "",
				"mathLevel": "",
				"order": "",
				"physicsLevel": "",
				"politicsLevel": "",
				"serial": "",
				"sumScore": ""
			}
		],
		"runTime": "",
		"schoolCode": "",
		"schoolName": "",
		"type": ""
	},
	"success": true,
	"timestamp": 0
}
```


## 获取指定高中学校的统计信息


**接口地址**:`/nnzk/publicityInfor/getSinglePublicity`


**请求方式**:`GET`


**请求数据类型**:`application/x-www-form-urlencoded`


**响应数据类型**:`*/*`


**接口描述**:<p>获取指定高中学校的统计信息</p>



**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|highSchoolCode|highSchoolCode|query|true|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«BmgsSchDTO»|
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|BmgsSchDTO|BmgsSchDTO|
|&emsp;&emsp;alterLevel||string||
|&emsp;&emsp;alterPlan||string||
|&emsp;&emsp;dirLevel||string||
|&emsp;&emsp;dirPlan||string||
|&emsp;&emsp;guideLevel||string||
|&emsp;&emsp;guidePlan||string||
|&emsp;&emsp;instLevel||string||
|&emsp;&emsp;instPlan||string||
|&emsp;&emsp;schoolCode||string||
|&emsp;&emsp;schoolName||string||
|&emsp;&emsp;status||string||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": {
		"alterLevel": "",
		"alterPlan": "",
		"dirLevel": "",
		"dirPlan": "",
		"guideLevel": "",
		"guidePlan": "",
		"instLevel": "",
		"instPlan": "",
		"schoolCode": "",
		"schoolName": "",
		"status": ""
	},
	"success": true,
	"timestamp": 0
}
```


# 定向校验


## 定向校验-导出数据


**接口地址**:`/nnzk/sign/verifyDir/exportListXls`


**请求方式**:`GET`


**请求数据类型**:`application/x-www-form-urlencoded`


**响应数据类型**:`*/*`


**接口描述**:<p>定向校验-导出数据</p>



**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|areaCode|所属区域|query|false|string||
|dataGroupId|导出“查询”或“全部校验”的数据，1-查询，2-全部校验|query|false|integer(int32)||
|finishSchoolCode|毕业学校代码|query|false|string||
|HGroupCode||query|false|string||
|highSchoolCode|高中学校代码|query|false|string||
|limitNum|显示数据数|query|false|integer(int32)||
|MGroupCode||query|false|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|ModelAndView|
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|empty||boolean||
|model||object||
|modelMap||object||
|reference||boolean||
|status|可用值:ACCEPTED,ALREADY_REPORTED,BAD_GATEWAY,BAD_REQUEST,BANDWIDTH_LIMIT_EXCEEDED,CHECKPOINT,CONFLICT,CONTINUE,CREATED,DESTINATION_LOCKED,EXPECTATION_FAILED,FAILED_DEPENDENCY,FORBIDDEN,FOUND,GATEWAY_TIMEOUT,GONE,HTTP_VERSION_NOT_SUPPORTED,IM_USED,INSUFFICIENT_SPACE_ON_RESOURCE,INSUFFICIENT_STORAGE,INTERNAL_SERVER_ERROR,I_AM_A_TEAPOT,LENGTH_REQUIRED,LOCKED,LOOP_DETECTED,METHOD_FAILURE,METHOD_NOT_ALLOWED,MOVED_PERMANENTLY,MOVED_TEMPORARILY,MULTIPLE_CHOICES,MULTI_STATUS,NETWORK_AUTHENTICATION_REQUIRED,NON_AUTHORITATIVE_INFORMATION,NOT_ACCEPTABLE,NOT_EXTENDED,NOT_FOUND,NOT_IMPLEMENTED,NOT_MODIFIED,NO_CONTENT,OK,PARTIAL_CONTENT,PAYLOAD_TOO_LARGE,PAYMENT_REQUIRED,PERMANENT_REDIRECT,PRECONDITION_FAILED,PRECONDITION_REQUIRED,PROCESSING,PROXY_AUTHENTICATION_REQUIRED,REQUESTED_RANGE_NOT_SATISFIABLE,REQUEST_ENTITY_TOO_LARGE,REQUEST_HEADER_FIELDS_TOO_LARGE,REQUEST_TIMEOUT,REQUEST_URI_TOO_LONG,RESET_CONTENT,SEE_OTHER,SERVICE_UNAVAILABLE,SWITCHING_PROTOCOLS,TEMPORARY_REDIRECT,TOO_EARLY,TOO_MANY_REQUESTS,UNAUTHORIZED,UNAVAILABLE_FOR_LEGAL_REASONS,UNPROCESSABLE_ENTITY,UNSUPPORTED_MEDIA_TYPE,UPGRADE_REQUIRED,URI_TOO_LONG,USE_PROXY,VARIANT_ALSO_NEGOTIATES|string||
|view||View|View|
|&emsp;&emsp;contentType||string||
|viewName||string||


**响应示例**:
```javascript
{
	"empty": true,
	"model": {},
	"modelMap": {},
	"reference": true,
	"status": "",
	"view": {
		"contentType": ""
	},
	"viewName": ""
}
```


## 定向校验-毕业学校


**接口地址**:`/nnzk/sign/verifyDir/finishSchoolList`


**请求方式**:`GET`


**请求数据类型**:`application/x-www-form-urlencoded`


**响应数据类型**:`*/*`


**接口描述**:<p>定向校验-毕业学校</p>



**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|groupCode|groupCode|query|false|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«List«SchoolCodeAndNameDTO»»|
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|array|SchoolCodeAndNameDTO|
|&emsp;&emsp;schoolCode|学校代码|string||
|&emsp;&emsp;schoolName|学校名称|string||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": [
		{
			"schoolCode": "",
			"schoolName": ""
		}
	],
	"success": true,
	"timestamp": 0
}
```


## 定向校验-指定范围示范性高中


**接口地址**:`/nnzk/sign/verifyDir/highSchoolList`


**请求方式**:`GET`


**请求数据类型**:`application/x-www-form-urlencoded`


**响应数据类型**:`*/*`


**接口描述**:<p>定向校验-指定范围示范性高中</p>



**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|groupCode|groupCode|query|false|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«List«SchoolCodeAndNameDTO»»|
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|array|SchoolCodeAndNameDTO|
|&emsp;&emsp;schoolCode|学校代码|string||
|&emsp;&emsp;schoolName|学校名称|string||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": [
		{
			"schoolCode": "",
			"schoolName": ""
		}
	],
	"success": true,
	"timestamp": 0
}
```


## 定向校验-打印


**接口地址**:`/nnzk/sign/verifyDir/print`


**请求方式**:`GET`


**请求数据类型**:`application/x-www-form-urlencoded`


**响应数据类型**:`*/*`


**接口描述**:<p>常规录取-打印</p>



**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|areaCode|所属区域|query|false|string||
|dataGroupId|导出“查询”或“全部校验”的数据，1-查询，2-全部校验|query|false|integer(int32)||
|finishSchoolCode|毕业学校代码|query|false|string||
|HGroupCode||query|false|string||
|highSchoolCode|高中学校代码|query|false|string||
|limitNum|显示数据数|query|false|integer(int32)||
|MGroupCode||query|false|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|VerifyDirPrintOutputDTO|
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|count|总条数|integer(int32)|integer(int32)|
|data|数据列表|array|VerifyDirPrintDTO|
|&emsp;&emsp;archiveCode|准考证号|string||
|&emsp;&emsp;calculateType|入围情况|string||
|&emsp;&emsp;chineseLevel|语文成绩|string||
|&emsp;&emsp;chymistLevel|化学成绩|string||
|&emsp;&emsp;combinedscoreLevel|定向线|string||
|&emsp;&emsp;combinedscoreStudent|学生成绩|string||
|&emsp;&emsp;directionalNum|定向计划数|integer(int32)||
|&emsp;&emsp;directionalReason|定向不入围原因|string||
|&emsp;&emsp;englishLevel|英语成绩|string||
|&emsp;&emsp;finishSchoolName|毕业学校|string||
|&emsp;&emsp;isAreaStudent|是否地段生|integer(int32)||
|&emsp;&emsp;mathLevel|数学成绩|string||
|&emsp;&emsp;matriculateStatus|录取状态|integer(int32)||
|&emsp;&emsp;matriculateType|录取类型|string||
|&emsp;&emsp;orderCode|排序码_考生|string||
|&emsp;&emsp;ordercodeLevel|排序码_定向线|string||
|&emsp;&emsp;physicsLevel|物理成绩|string||
|&emsp;&emsp;politicsLevel|政史成绩|string||
|&emsp;&emsp;schoolName|报考学校|string||
|&emsp;&emsp;serialNum|序号|integer(int32)||
|&emsp;&emsp;sex|性别|string||
|&emsp;&emsp;signUpType|报考类型|string||
|&emsp;&emsp;studentName|姓名|string||
|&emsp;&emsp;usednum|已用定向数|integer(int32)||
|total|总页数|integer(int32)|integer(int32)|


**响应示例**:
```javascript
{
	"count": 0,
	"data": [
		{
			"archiveCode": "",
			"calculateType": "",
			"chineseLevel": "",
			"chymistLevel": "",
			"combinedscoreLevel": "",
			"combinedscoreStudent": "",
			"directionalNum": 0,
			"directionalReason": "",
			"englishLevel": "",
			"finishSchoolName": "",
			"isAreaStudent": 0,
			"mathLevel": "",
			"matriculateStatus": 0,
			"matriculateType": "",
			"orderCode": "",
			"ordercodeLevel": "",
			"physicsLevel": "",
			"politicsLevel": "",
			"schoolName": "",
			"serialNum": 0,
			"sex": "",
			"signUpType": "",
			"studentName": "",
			"usednum": 0
		}
	],
	"total": 0
}
```


## 定向校验-校验全部


**接口地址**:`/nnzk/sign/verifyDir/verifyAllDir`


**请求方式**:`GET`


**请求数据类型**:`application/x-www-form-urlencoded`


**响应数据类型**:`*/*`


**接口描述**:<p>定向校验-校验全部</p>



**请求参数**:


暂无


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«List«VerifyDirVO»»|
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|array|VerifyDirVO|
|&emsp;&emsp;archiveCode|准考证号|string||
|&emsp;&emsp;calculateType|入围情况|string||
|&emsp;&emsp;chineseLevel|语文成绩|string||
|&emsp;&emsp;chymistLevel|化学成绩|string||
|&emsp;&emsp;combinedscoreLevel|定向线|string||
|&emsp;&emsp;combinedscoreStudent|学生成绩|string||
|&emsp;&emsp;directionalNum|定向计划数|integer(int32)||
|&emsp;&emsp;directionalReason|定向不入围原因|string||
|&emsp;&emsp;englishLevel|英语成绩|string||
|&emsp;&emsp;finishSchoolName|毕业学校|string||
|&emsp;&emsp;highSchoolCode||string||
|&emsp;&emsp;isAreaStudent|是否地段生|integer(int32)||
|&emsp;&emsp;mathLevel|数学成绩|string||
|&emsp;&emsp;matriculateStatus|录取状态|integer(int32)||
|&emsp;&emsp;matriculateType|录取类型|string||
|&emsp;&emsp;mgroupCode||string||
|&emsp;&emsp;orderCode|排序码_考生|string||
|&emsp;&emsp;ordercodeLevel|排序码_定向线|string||
|&emsp;&emsp;physicsLevel|物理成绩|string||
|&emsp;&emsp;politicsLevel|政史成绩|string||
|&emsp;&emsp;schoolName|报考学校|string||
|&emsp;&emsp;serialNum|序号|integer(int32)||
|&emsp;&emsp;sex|性别|string||
|&emsp;&emsp;signUpType|报考类型|string||
|&emsp;&emsp;studentName|姓名|string||
|&emsp;&emsp;usednum|已用定向数|integer(int32)||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": [
		{
			"archiveCode": "",
			"calculateType": "",
			"chineseLevel": "",
			"chymistLevel": "",
			"combinedscoreLevel": "",
			"combinedscoreStudent": "",
			"directionalNum": 0,
			"directionalReason": "",
			"englishLevel": "",
			"finishSchoolName": "",
			"highSchoolCode": "",
			"isAreaStudent": 0,
			"mathLevel": "",
			"matriculateStatus": 0,
			"matriculateType": "",
			"mgroupCode": "",
			"orderCode": "",
			"ordercodeLevel": "",
			"physicsLevel": "",
			"politicsLevel": "",
			"schoolName": "",
			"serialNum": 0,
			"sex": "",
			"signUpType": "",
			"studentName": "",
			"usednum": 0
		}
	],
	"success": true,
	"timestamp": 0
}
```


## 定向校验-查询


**接口地址**:`/nnzk/sign/verifyDir/verifyDirQuery`


**请求方式**:`GET`


**请求数据类型**:`application/x-www-form-urlencoded`


**响应数据类型**:`*/*`


**接口描述**:<p>定向校验-查询</p>



**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|areaCode|所属区域|query|false|string||
|dataGroupId|导出“查询”或“全部校验”的数据，1-查询，2-全部校验|query|false|integer(int32)||
|finishSchoolCode|毕业学校代码|query|false|string||
|HGroupCode||query|false|string||
|highSchoolCode|高中学校代码|query|false|string||
|limitNum|显示数据数|query|false|integer(int32)||
|MGroupCode||query|false|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«List«VerifyDirVO»»|
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|array|VerifyDirVO|
|&emsp;&emsp;archiveCode|准考证号|string||
|&emsp;&emsp;calculateType|入围情况|string||
|&emsp;&emsp;chineseLevel|语文成绩|string||
|&emsp;&emsp;chymistLevel|化学成绩|string||
|&emsp;&emsp;combinedscoreLevel|定向线|string||
|&emsp;&emsp;combinedscoreStudent|学生成绩|string||
|&emsp;&emsp;directionalNum|定向计划数|integer(int32)||
|&emsp;&emsp;directionalReason|定向不入围原因|string||
|&emsp;&emsp;englishLevel|英语成绩|string||
|&emsp;&emsp;finishSchoolName|毕业学校|string||
|&emsp;&emsp;highSchoolCode||string||
|&emsp;&emsp;isAreaStudent|是否地段生|integer(int32)||
|&emsp;&emsp;mathLevel|数学成绩|string||
|&emsp;&emsp;matriculateStatus|录取状态|integer(int32)||
|&emsp;&emsp;matriculateType|录取类型|string||
|&emsp;&emsp;mgroupCode||string||
|&emsp;&emsp;orderCode|排序码_考生|string||
|&emsp;&emsp;ordercodeLevel|排序码_定向线|string||
|&emsp;&emsp;physicsLevel|物理成绩|string||
|&emsp;&emsp;politicsLevel|政史成绩|string||
|&emsp;&emsp;schoolName|报考学校|string||
|&emsp;&emsp;serialNum|序号|integer(int32)||
|&emsp;&emsp;sex|性别|string||
|&emsp;&emsp;signUpType|报考类型|string||
|&emsp;&emsp;studentName|姓名|string||
|&emsp;&emsp;usednum|已用定向数|integer(int32)||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": [
		{
			"archiveCode": "",
			"calculateType": "",
			"chineseLevel": "",
			"chymistLevel": "",
			"combinedscoreLevel": "",
			"combinedscoreStudent": "",
			"directionalNum": 0,
			"directionalReason": "",
			"englishLevel": "",
			"finishSchoolName": "",
			"highSchoolCode": "",
			"isAreaStudent": 0,
			"mathLevel": "",
			"matriculateStatus": 0,
			"matriculateType": "",
			"mgroupCode": "",
			"orderCode": "",
			"ordercodeLevel": "",
			"physicsLevel": "",
			"politicsLevel": "",
			"schoolName": "",
			"serialNum": 0,
			"sex": "",
			"signUpType": "",
			"studentName": "",
			"usednum": 0
		}
	],
	"success": true,
	"timestamp": 0
}
```


# 定向计划表


## 定向计划表-添加


**接口地址**:`/nnzk/rule/directionalPlan/add`


**请求方式**:`POST`


**请求数据类型**:`application/json`


**响应数据类型**:`*/*`


**接口描述**:<p>定向计划表-添加</p>



**请求示例**:


```javascript
{
  "createBy": "",
  "createTime": "",
  "delFlag": 0,
  "directionalNum": 0,
  "hgroupCode": "",
  "id": "",
  "mgroupCode": "",
  "updateBy": "",
  "updateTime": ""
}
```


**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|directionalPlan|定向计划表|body|true|directional_plan对象|directional_plan对象|
|&emsp;&emsp;createBy|创建人||false|string||
|&emsp;&emsp;createTime|创建日期||false|string(date-time)||
|&emsp;&emsp;delFlag|删除标识||false|integer(int32)||
|&emsp;&emsp;directionalNum|定向计划数||false|integer(int32)||
|&emsp;&emsp;hgroupCode|高中组||false|string||
|&emsp;&emsp;id|主键||false|string||
|&emsp;&emsp;mgroupCode|初中组||false|string||
|&emsp;&emsp;updateBy|更新人||false|string||
|&emsp;&emsp;updateTime|更新日期||false|string(date-time)||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«string»|
|201|Created||
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|string||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": "",
	"success": true,
	"timestamp": 0
}
```


## 定向配额-添加关联


**接口地址**:`/nnzk/rule/directionalPlan/addRelated`


**请求方式**:`POST`


**请求数据类型**:`application/json`


**响应数据类型**:`*/*`


**接口描述**:<p>定向配额-添加关联</p>



**请求示例**:


```javascript
{
  "hgroupCode": "",
  "mgroupCodeList": []
}
```


**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|input|input|body|true|AddOrRemoveRelatedDTO|AddOrRemoveRelatedDTO|
|&emsp;&emsp;hgroupCode|高中组代码||false|string||
|&emsp;&emsp;mgroupCodeList|||false|array|string|


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«string»|
|201|Created||
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|string||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": "",
	"success": true,
	"timestamp": 0
}
```


## 定向配额-批量更新定向配额数


**接口地址**:`/nnzk/rule/directionalPlan/batchUpdateDirNum`


**请求方式**:`POST`


**请求数据类型**:`application/json`


**响应数据类型**:`*/*`


**接口描述**:<p>定向配额-批量更新定向配额数</p>



**请求示例**:


```javascript
{
  "updateDirNumDTOList": [
    {
      "directionalNum": 0,
      "hgroupCode": "",
      "mgroupCode": ""
    }
  ]
}
```


**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|input|input|body|true|BatchUpdateDirNumDTO|BatchUpdateDirNumDTO|
|&emsp;&emsp;updateDirNumDTOList|||false|array|UpdateDirNumDTO|
|&emsp;&emsp;&emsp;&emsp;directionalNum|定向计划数||false|integer||
|&emsp;&emsp;&emsp;&emsp;hgroupCode|高中组代码||false|string||
|&emsp;&emsp;&emsp;&emsp;mgroupCode|||false|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«string»|
|201|Created||
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|string||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": "",
	"success": true,
	"timestamp": 0
}
```


## 定向计划表-通过id删除


**接口地址**:`/nnzk/rule/directionalPlan/delete`


**请求方式**:`DELETE`


**请求数据类型**:`application/x-www-form-urlencoded`


**响应数据类型**:`*/*`


**接口描述**:<p>定向计划表-通过id删除</p>



**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|id|id|query|true|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«string»|
|204|No Content||
|401|Unauthorized||
|403|Forbidden||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|string||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": "",
	"success": true,
	"timestamp": 0
}
```


## 定向计划表-批量删除


**接口地址**:`/nnzk/rule/directionalPlan/deleteBatch`


**请求方式**:`DELETE`


**请求数据类型**:`application/x-www-form-urlencoded`


**响应数据类型**:`*/*`


**接口描述**:<p>定向计划表-批量删除</p>



**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|ids|ids|query|true|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«string»|
|204|No Content||
|401|Unauthorized||
|403|Forbidden||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|string||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": "",
	"success": true,
	"timestamp": 0
}
```


## 定向计划表-编辑


**接口地址**:`/nnzk/rule/directionalPlan/edit`


**请求方式**:`POST`


**请求数据类型**:`application/json`


**响应数据类型**:`*/*`


**接口描述**:<p>定向计划表-编辑</p>



**请求示例**:


```javascript
{
  "createBy": "",
  "createTime": "",
  "delFlag": 0,
  "directionalNum": 0,
  "hgroupCode": "",
  "id": "",
  "mgroupCode": "",
  "updateBy": "",
  "updateTime": ""
}
```


**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|directionalPlan|定向计划表|body|true|directional_plan对象|directional_plan对象|
|&emsp;&emsp;createBy|创建人||false|string||
|&emsp;&emsp;createTime|创建日期||false|string(date-time)||
|&emsp;&emsp;delFlag|删除标识||false|integer(int32)||
|&emsp;&emsp;directionalNum|定向计划数||false|integer(int32)||
|&emsp;&emsp;hgroupCode|高中组||false|string||
|&emsp;&emsp;id|主键||false|string||
|&emsp;&emsp;mgroupCode|初中组||false|string||
|&emsp;&emsp;updateBy|更新人||false|string||
|&emsp;&emsp;updateTime|更新日期||false|string(date-time)||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«string»|
|201|Created||
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|string||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": "",
	"success": true,
	"timestamp": 0
}
```


## 定向计划表-编辑


**接口地址**:`/nnzk/rule/directionalPlan/edit`


**请求方式**:`PUT`


**请求数据类型**:`application/json`


**响应数据类型**:`*/*`


**接口描述**:<p>定向计划表-编辑</p>



**请求示例**:


```javascript
{
  "createBy": "",
  "createTime": "",
  "delFlag": 0,
  "directionalNum": 0,
  "hgroupCode": "",
  "id": "",
  "mgroupCode": "",
  "updateBy": "",
  "updateTime": ""
}
```


**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|directionalPlan|定向计划表|body|true|directional_plan对象|directional_plan对象|
|&emsp;&emsp;createBy|创建人||false|string||
|&emsp;&emsp;createTime|创建日期||false|string(date-time)||
|&emsp;&emsp;delFlag|删除标识||false|integer(int32)||
|&emsp;&emsp;directionalNum|定向计划数||false|integer(int32)||
|&emsp;&emsp;hgroupCode|高中组||false|string||
|&emsp;&emsp;id|主键||false|string||
|&emsp;&emsp;mgroupCode|初中组||false|string||
|&emsp;&emsp;updateBy|更新人||false|string||
|&emsp;&emsp;updateTime|更新日期||false|string(date-time)||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«string»|
|201|Created||
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|string||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": "",
	"success": true,
	"timestamp": 0
}
```


## 定向配额-定向配额结果一览


**接口地址**:`/nnzk/rule/directionalPlan/getDirectionPlanResult`


**请求方式**:`GET`


**请求数据类型**:`application/x-www-form-urlencoded`


**响应数据类型**:`*/*`


**接口描述**:<p>定向配额-定向配额结果一览</p>



**请求参数**:


暂无


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«List«DirectionPlanResultVO»»|
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|array|DirectionPlanResultVO|
|&emsp;&emsp;areaCode|所属县区|string||
|&emsp;&emsp;directionPlanVOList|初中关联定向配额|array|DirectionPlanVO|
|&emsp;&emsp;&emsp;&emsp;directionalNum|定向计划数|integer||
|&emsp;&emsp;&emsp;&emsp;hgroupCode|高中组|string||
|&emsp;&emsp;&emsp;&emsp;mgroupCode|初中组|string||
|&emsp;&emsp;groupCode|初中分组编码|string||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": [
		{
			"areaCode": "",
			"directionPlanVOList": [
				{
					"directionalNum": 0,
					"hgroupCode": "",
					"mgroupCode": ""
				}
			],
			"groupCode": ""
		}
	],
	"success": true,
	"timestamp": 0
}
```


## 定向配额-获取高中组


**接口地址**:`/nnzk/rule/directionalPlan/getHighSchoolGroup`


**请求方式**:`GET`


**请求数据类型**:`application/x-www-form-urlencoded`


**响应数据类型**:`*/*`


**接口描述**:<p>定向配额-获取高中组</p>



**请求参数**:


暂无


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«List«GroupBaseVO»»|
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|array|GroupBaseVO|
|&emsp;&emsp;areaCode|所属县区|string||
|&emsp;&emsp;groupCode|分组编码|string||
|&emsp;&emsp;groupName|分组名称|string||
|&emsp;&emsp;groupType|分组类型(初中组、高中组)|string||
|&emsp;&emsp;id|主键|string||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": [
		{
			"areaCode": "",
			"groupCode": "",
			"groupName": "",
			"groupType": "",
			"id": ""
		}
	],
	"success": true,
	"timestamp": 0
}
```


## 定向配额-由高中组获取关联定向配额的初中组


**接口地址**:`/nnzk/rule/directionalPlan/getRelatedMGroupByHGroupCode`


**请求方式**:`GET`


**请求数据类型**:`application/x-www-form-urlencoded`


**响应数据类型**:`*/*`


**接口描述**:<p>定向配额-由高中组获取关联定向配额的初中组</p>



**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|hGroupCode|hGroupCode|query|true|string||
|areaCode|areaCode|query|false|string||
|groupName|groupName|query|false|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«List«RelatedMSchoolGroupVO»»|
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|array|RelatedMSchoolGroupVO|
|&emsp;&emsp;areaCode|所属县区|string||
|&emsp;&emsp;directionalNum|定向计划数|integer(int32)||
|&emsp;&emsp;groupCode|分组编码|string||
|&emsp;&emsp;schoolOfMGroup|初中组成员|array|SchoolOfGroupVO|
|&emsp;&emsp;&emsp;&emsp;areaCode|所属县区|string||
|&emsp;&emsp;&emsp;&emsp;schoolCode|学校代码|string||
|&emsp;&emsp;&emsp;&emsp;schoolName|学校名称|string||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": [
		{
			"areaCode": "",
			"directionalNum": 0,
			"groupCode": "",
			"schoolOfMGroup": [
				{
					"areaCode": "",
					"schoolCode": "",
					"schoolName": ""
				}
			]
		}
	],
	"success": true,
	"timestamp": 0
}
```


## 定向配额-由高中组获取未关联定向配额的初中组


**接口地址**:`/nnzk/rule/directionalPlan/getUnRelatedMGroupByHGroupCode`


**请求方式**:`GET`


**请求数据类型**:`application/x-www-form-urlencoded`


**响应数据类型**:`*/*`


**接口描述**:<p>定向配额-由高中组获取未关联定向配额的初中组</p>



**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|hGroupCode|hGroupCode|query|true|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«List«RelatedMSchoolGroupVO»»|
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|array|RelatedMSchoolGroupVO|
|&emsp;&emsp;areaCode|所属县区|string||
|&emsp;&emsp;directionalNum|定向计划数|integer(int32)||
|&emsp;&emsp;groupCode|分组编码|string||
|&emsp;&emsp;schoolOfMGroup|初中组成员|array|SchoolOfGroupVO|
|&emsp;&emsp;&emsp;&emsp;areaCode|所属县区|string||
|&emsp;&emsp;&emsp;&emsp;schoolCode|学校代码|string||
|&emsp;&emsp;&emsp;&emsp;schoolName|学校名称|string||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": [
		{
			"areaCode": "",
			"directionalNum": 0,
			"groupCode": "",
			"schoolOfMGroup": [
				{
					"areaCode": "",
					"schoolCode": "",
					"schoolName": ""
				}
			]
		}
	],
	"success": true,
	"timestamp": 0
}
```


## 定向计划表-分页列表查询


**接口地址**:`/nnzk/rule/directionalPlan/list`


**请求方式**:`GET`


**请求数据类型**:`application/x-www-form-urlencoded`


**响应数据类型**:`*/*`


**接口描述**:<p>定向计划表-分页列表查询</p>



**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|hgroupCode|高中组|query|true|string||
|mgroupCode|初中组|query|true|string||
|createBy|创建人|query|false|string||
|createTime|创建日期|query|false|string(date-time)||
|delFlag|删除标识|query|false|integer(int32)||
|directionalNum|定向计划数|query|false|integer(int32)||
|id|主键|query|false|string||
|pageNo|pageNo|query|false|integer(int32)||
|pageSize|pageSize|query|false|integer(int32)||
|updateBy|更新人|query|false|string||
|updateTime|更新日期|query|false|string(date-time)||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«IPage«directional_plan对象»»|
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|IPage«directional_plan对象»|IPage«directional_plan对象»|
|&emsp;&emsp;current||integer(int64)||
|&emsp;&emsp;pages||integer(int64)||
|&emsp;&emsp;records||array|directional_plan对象|
|&emsp;&emsp;&emsp;&emsp;createBy|创建人|string||
|&emsp;&emsp;&emsp;&emsp;createTime|创建日期|string||
|&emsp;&emsp;&emsp;&emsp;delFlag|删除标识|integer||
|&emsp;&emsp;&emsp;&emsp;directionalNum|定向计划数|integer||
|&emsp;&emsp;&emsp;&emsp;hgroupCode|高中组|string||
|&emsp;&emsp;&emsp;&emsp;id|主键|string||
|&emsp;&emsp;&emsp;&emsp;mgroupCode|初中组|string||
|&emsp;&emsp;&emsp;&emsp;updateBy|更新人|string||
|&emsp;&emsp;&emsp;&emsp;updateTime|更新日期|string||
|&emsp;&emsp;size||integer(int64)||
|&emsp;&emsp;total||integer(int64)||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": {
		"current": 0,
		"pages": 0,
		"records": [
			{
				"createBy": "",
				"createTime": "",
				"delFlag": 0,
				"directionalNum": 0,
				"hgroupCode": "",
				"id": "",
				"mgroupCode": "",
				"updateBy": "",
				"updateTime": ""
			}
		],
		"size": 0,
		"total": 0
	},
	"success": true,
	"timestamp": 0
}
```


## 定向计划表-通过id查询


**接口地址**:`/nnzk/rule/directionalPlan/queryById`


**请求方式**:`GET`


**请求数据类型**:`application/x-www-form-urlencoded`


**响应数据类型**:`*/*`


**接口描述**:<p>定向计划表-通过id查询</p>



**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|id|id|query|true|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«directional_plan对象»|
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|directional_plan对象|directional_plan对象|
|&emsp;&emsp;createBy|创建人|string||
|&emsp;&emsp;createTime|创建日期|string(date-time)||
|&emsp;&emsp;delFlag|删除标识|integer(int32)||
|&emsp;&emsp;directionalNum|定向计划数|integer(int32)||
|&emsp;&emsp;hgroupCode|高中组|string||
|&emsp;&emsp;id|主键|string||
|&emsp;&emsp;mgroupCode|初中组|string||
|&emsp;&emsp;updateBy|更新人|string||
|&emsp;&emsp;updateTime|更新日期|string(date-time)||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": {
		"createBy": "",
		"createTime": "",
		"delFlag": 0,
		"directionalNum": 0,
		"hgroupCode": "",
		"id": "",
		"mgroupCode": "",
		"updateBy": "",
		"updateTime": ""
	},
	"success": true,
	"timestamp": 0
}
```


## 定向配额-移除关联


**接口地址**:`/nnzk/rule/directionalPlan/removeRelated`


**请求方式**:`POST`


**请求数据类型**:`application/json`


**响应数据类型**:`*/*`


**接口描述**:<p>定向配额-移除关联</p>



**请求示例**:


```javascript
{
  "hgroupCode": "",
  "mgroupCodeList": []
}
```


**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|input|input|body|true|AddOrRemoveRelatedDTO|AddOrRemoveRelatedDTO|
|&emsp;&emsp;hgroupCode|高中组代码||false|string||
|&emsp;&emsp;mgroupCodeList|||false|array|string|


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«string»|
|201|Created||
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|string||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": "",
	"success": true,
	"timestamp": 0
}
```


## 定向配额-更新定向配额数


**接口地址**:`/nnzk/rule/directionalPlan/updateDirNum`


**请求方式**:`POST`


**请求数据类型**:`application/json`


**响应数据类型**:`*/*`


**接口描述**:<p>定向配额-更新定向配额数</p>



**请求示例**:


```javascript
{
  "directionalNum": 0,
  "hgroupCode": "",
  "mgroupCode": ""
}
```


**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|input|input|body|true|UpdateDirNumDTO|UpdateDirNumDTO|
|&emsp;&emsp;directionalNum|定向计划数||false|integer(int32)||
|&emsp;&emsp;hgroupCode|高中组代码||false|string||
|&emsp;&emsp;mgroupCode|||false|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«string»|
|201|Created||
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|string||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": "",
	"success": true,
	"timestamp": 0
}
```


# 定时任务接口


## 停止定时任务


**接口地址**:`/nnzk/sys/quartzJob/pause`


**请求方式**:`GET`


**请求数据类型**:`application/x-www-form-urlencoded`


**响应数据类型**:`*/*`


**接口描述**:


**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|id|id|query|true|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«object»|
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|object||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": {},
	"success": true,
	"timestamp": 0
}
```


## 启动定时任务


**接口地址**:`/nnzk/sys/quartzJob/resume`


**请求方式**:`GET`


**请求数据类型**:`application/x-www-form-urlencoded`


**响应数据类型**:`*/*`


**接口描述**:


**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|id|id|query|true|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«object»|
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|object||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": {},
	"success": true,
	"timestamp": 0
}
```


# 成绩分布表


## 成绩分布表-添加


**接口地址**:`/nnzk/base/scoreDistribution/add`


**请求方式**:`POST`


**请求数据类型**:`application/json`


**响应数据类型**:`*/*`


**接口描述**:<p>成绩分布表-添加</p>



**请求示例**:


```javascript
{
  "createBy": "",
  "createTime": "",
  "delFlag": 0,
  "id": "",
  "ideNo": 0,
  "remark": "",
  "score": "",
  "studentqty": 0,
  "updateBy": "",
  "updateTime": ""
}
```


**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|scoreDistribution|成绩分布表|body|true|score_distribution对象|score_distribution对象|
|&emsp;&emsp;createBy|创建人||false|string||
|&emsp;&emsp;createTime|创建日期||false|string(date-time)||
|&emsp;&emsp;delFlag|删除标识||false|integer(int32)||
|&emsp;&emsp;id|主键||false|string||
|&emsp;&emsp;ideNo|排名||false|integer(int32)||
|&emsp;&emsp;remark|说明||false|string||
|&emsp;&emsp;score|成绩||false|string||
|&emsp;&emsp;studentqty|学生人数||false|integer(int32)||
|&emsp;&emsp;updateBy|更新人||false|string||
|&emsp;&emsp;updateTime|更新日期||false|string(date-time)||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«string»|
|201|Created||
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|string||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": "",
	"success": true,
	"timestamp": 0
}
```


## 成绩分布表-通过id删除


**接口地址**:`/nnzk/base/scoreDistribution/delete`


**请求方式**:`DELETE`


**请求数据类型**:`application/x-www-form-urlencoded`


**响应数据类型**:`*/*`


**接口描述**:<p>成绩分布表-通过id删除</p>



**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|id|id|query|true|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«string»|
|204|No Content||
|401|Unauthorized||
|403|Forbidden||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|string||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": "",
	"success": true,
	"timestamp": 0
}
```


## 成绩分布表-批量删除


**接口地址**:`/nnzk/base/scoreDistribution/deleteBatch`


**请求方式**:`DELETE`


**请求数据类型**:`application/x-www-form-urlencoded`


**响应数据类型**:`*/*`


**接口描述**:<p>成绩分布表-批量删除</p>



**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|ids|ids|query|true|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«string»|
|204|No Content||
|401|Unauthorized||
|403|Forbidden||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|string||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": "",
	"success": true,
	"timestamp": 0
}
```


## 成绩分布表-编辑


**接口地址**:`/nnzk/base/scoreDistribution/edit`


**请求方式**:`POST`


**请求数据类型**:`application/json`


**响应数据类型**:`*/*`


**接口描述**:<p>成绩分布表-编辑</p>



**请求示例**:


```javascript
{
  "createBy": "",
  "createTime": "",
  "delFlag": 0,
  "id": "",
  "ideNo": 0,
  "remark": "",
  "score": "",
  "studentqty": 0,
  "updateBy": "",
  "updateTime": ""
}
```


**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|scoreDistribution|成绩分布表|body|true|score_distribution对象|score_distribution对象|
|&emsp;&emsp;createBy|创建人||false|string||
|&emsp;&emsp;createTime|创建日期||false|string(date-time)||
|&emsp;&emsp;delFlag|删除标识||false|integer(int32)||
|&emsp;&emsp;id|主键||false|string||
|&emsp;&emsp;ideNo|排名||false|integer(int32)||
|&emsp;&emsp;remark|说明||false|string||
|&emsp;&emsp;score|成绩||false|string||
|&emsp;&emsp;studentqty|学生人数||false|integer(int32)||
|&emsp;&emsp;updateBy|更新人||false|string||
|&emsp;&emsp;updateTime|更新日期||false|string(date-time)||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«string»|
|201|Created||
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|string||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": "",
	"success": true,
	"timestamp": 0
}
```


## 成绩分布表-编辑


**接口地址**:`/nnzk/base/scoreDistribution/edit`


**请求方式**:`PUT`


**请求数据类型**:`application/json`


**响应数据类型**:`*/*`


**接口描述**:<p>成绩分布表-编辑</p>



**请求示例**:


```javascript
{
  "createBy": "",
  "createTime": "",
  "delFlag": 0,
  "id": "",
  "ideNo": 0,
  "remark": "",
  "score": "",
  "studentqty": 0,
  "updateBy": "",
  "updateTime": ""
}
```


**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|scoreDistribution|成绩分布表|body|true|score_distribution对象|score_distribution对象|
|&emsp;&emsp;createBy|创建人||false|string||
|&emsp;&emsp;createTime|创建日期||false|string(date-time)||
|&emsp;&emsp;delFlag|删除标识||false|integer(int32)||
|&emsp;&emsp;id|主键||false|string||
|&emsp;&emsp;ideNo|排名||false|integer(int32)||
|&emsp;&emsp;remark|说明||false|string||
|&emsp;&emsp;score|成绩||false|string||
|&emsp;&emsp;studentqty|学生人数||false|integer(int32)||
|&emsp;&emsp;updateBy|更新人||false|string||
|&emsp;&emsp;updateTime|更新日期||false|string(date-time)||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«string»|
|201|Created||
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|string||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": "",
	"success": true,
	"timestamp": 0
}
```


## 成绩分布表-初始化


**接口地址**:`/nnzk/base/scoreDistribution/initialize`


**请求方式**:`PUT`


**请求数据类型**:`application/json`


**响应数据类型**:`*/*`


**接口描述**:<p>成绩分布表-初始化</p>



**请求参数**:


暂无


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«string»|
|201|Created||
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|string||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": "",
	"success": true,
	"timestamp": 0
}
```


## 成绩分布表-分页列表查询


**接口地址**:`/nnzk/base/scoreDistribution/list`


**请求方式**:`GET`


**请求数据类型**:`application/x-www-form-urlencoded`


**响应数据类型**:`*/*`


**接口描述**:<p>成绩分布表-分页列表查询</p>



**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|createBy|创建人|query|false|string||
|createTime|创建日期|query|false|string(date-time)||
|delFlag|删除标识|query|false|integer(int32)||
|id|主键|query|false|string||
|ideNo|排名|query|false|integer(int32)||
|pageNo|pageNo|query|false|integer(int32)||
|pageSize|pageSize|query|false|integer(int32)||
|remark|说明|query|false|string||
|score|成绩|query|false|string||
|studentqty|学生人数|query|false|integer(int32)||
|updateBy|更新人|query|false|string||
|updateTime|更新日期|query|false|string(date-time)||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«IPage«score_distribution对象»»|
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|IPage«score_distribution对象»|IPage«score_distribution对象»|
|&emsp;&emsp;current||integer(int64)||
|&emsp;&emsp;pages||integer(int64)||
|&emsp;&emsp;records||array|score_distribution对象|
|&emsp;&emsp;&emsp;&emsp;createBy|创建人|string||
|&emsp;&emsp;&emsp;&emsp;createTime|创建日期|string||
|&emsp;&emsp;&emsp;&emsp;delFlag|删除标识|integer||
|&emsp;&emsp;&emsp;&emsp;id|主键|string||
|&emsp;&emsp;&emsp;&emsp;ideNo|排名|integer||
|&emsp;&emsp;&emsp;&emsp;remark|说明|string||
|&emsp;&emsp;&emsp;&emsp;score|成绩|string||
|&emsp;&emsp;&emsp;&emsp;studentqty|学生人数|integer||
|&emsp;&emsp;&emsp;&emsp;updateBy|更新人|string||
|&emsp;&emsp;&emsp;&emsp;updateTime|更新日期|string||
|&emsp;&emsp;size||integer(int64)||
|&emsp;&emsp;total||integer(int64)||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": {
		"current": 0,
		"pages": 0,
		"records": [
			{
				"createBy": "",
				"createTime": "",
				"delFlag": 0,
				"id": "",
				"ideNo": 0,
				"remark": "",
				"score": "",
				"studentqty": 0,
				"updateBy": "",
				"updateTime": ""
			}
		],
		"size": 0,
		"total": 0
	},
	"success": true,
	"timestamp": 0
}
```


## 成绩分布表-通过id查询


**接口地址**:`/nnzk/base/scoreDistribution/queryById`


**请求方式**:`GET`


**请求数据类型**:`application/x-www-form-urlencoded`


**响应数据类型**:`*/*`


**接口描述**:<p>成绩分布表-通过id查询</p>



**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|id|id|query|true|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«score_distribution对象»|
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|score_distribution对象|score_distribution对象|
|&emsp;&emsp;createBy|创建人|string||
|&emsp;&emsp;createTime|创建日期|string(date-time)||
|&emsp;&emsp;delFlag|删除标识|integer(int32)||
|&emsp;&emsp;id|主键|string||
|&emsp;&emsp;ideNo|排名|integer(int32)||
|&emsp;&emsp;remark|说明|string||
|&emsp;&emsp;score|成绩|string||
|&emsp;&emsp;studentqty|学生人数|integer(int32)||
|&emsp;&emsp;updateBy|更新人|string||
|&emsp;&emsp;updateTime|更新日期|string(date-time)||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": {
		"createBy": "",
		"createTime": "",
		"delFlag": 0,
		"id": "",
		"ideNo": 0,
		"remark": "",
		"score": "",
		"studentqty": 0,
		"updateBy": "",
		"updateTime": ""
	},
	"success": true,
	"timestamp": 0
}
```


## 学校简介表-学生端成绩分布列表


**接口地址**:`/nnzk/base/scoreDistribution/studentWebList`


**请求方式**:`GET`


**请求数据类型**:`application/x-www-form-urlencoded`


**响应数据类型**:`*/*`


**接口描述**:<p>学校简介表-学生端成绩分布列表</p>



**请求参数**:


暂无


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«List«ScoreDistributionVO»»|
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|array|ScoreDistributionVO|
|&emsp;&emsp;id|主键|string||
|&emsp;&emsp;ideNo|排名|integer(int32)||
|&emsp;&emsp;remark|说明|string||
|&emsp;&emsp;score|成绩|string||
|&emsp;&emsp;studentqty|学生人数|integer(int32)||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": [
		{
			"id": "",
			"ideNo": 0,
			"remark": "",
			"score": "",
			"studentqty": 0
		}
	],
	"success": true,
	"timestamp": 0
}
```


# 报名规则


## 报名规则-添加


**接口地址**:`/nnzk/rule/ruleOfSignUp/add`


**请求方式**:`POST`


**请求数据类型**:`application/json`


**响应数据类型**:`*/*`


**接口描述**:<p>报名规则-添加</p>



**请求示例**:


```javascript
{
  "createBy": "",
  "createTime": "",
  "delFlag": 0,
  "directionalPlanNum": 0,
  "displayInfo": "",
  "enClaim": 0,
  "enGuide": 0,
  "enInstruction": 0,
  "enLodging": 0,
  "guideCombinedScore": "",
  "guidePhysicalEdu": "",
  "guidePlanNum": 0,
  "guideRemarkScore": "",
  "guideScoreLevel": "",
  "guideSingelSubject": "",
  "guideSumScore": "",
  "highSchoolCode": "",
  "id": "",
  "instructionCombinedScore": "",
  "instructionPhysicalEdu": "",
  "instructionPlanNum": 0,
  "instructionRemarkScore": "",
  "instructionScoreLevel": "",
  "instructionSingelSubject": "",
  "instructionSumScore": "",
  "lodgingInfo": "",
  "phaseId": "",
  "phaseIdBak": "",
  "specplanNum": 0,
  "status": "",
  "updateBy": "",
  "updateTime": ""
}
```


**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|ruleOfSignUp|报名规则|body|true|rule_of_sign_up对象|rule_of_sign_up对象|
|&emsp;&emsp;createBy|创建人||false|string||
|&emsp;&emsp;createTime|创建日期||false|string(date-time)||
|&emsp;&emsp;delFlag|删除标识||false|integer(int32)||
|&emsp;&emsp;directionalPlanNum|定向指标||false|integer(int32)||
|&emsp;&emsp;displayInfo|公示信息||false|string||
|&emsp;&emsp;enClaim|允许公示||false|integer(int32)||
|&emsp;&emsp;enGuide|可报指导||false|integer(int32)||
|&emsp;&emsp;enInstruction|可报指令||false|integer(int32)||
|&emsp;&emsp;enLodging|可住宿||false|integer(int32)||
|&emsp;&emsp;guideCombinedScore|指导组合分||false|string||
|&emsp;&emsp;guidePhysicalEdu|指导实验||false|string||
|&emsp;&emsp;guidePlanNum|拟招人数||false|integer(int32)||
|&emsp;&emsp;guideRemarkScore|综合素质||false|string||
|&emsp;&emsp;guideScoreLevel|指导分数线(组合分)||false|string||
|&emsp;&emsp;guideSingelSubject|指导单科限制||false|string||
|&emsp;&emsp;guideSumScore|指导总分||false|string||
|&emsp;&emsp;highSchoolCode|(高中)学校代码||false|string||
|&emsp;&emsp;id|主键||false|string||
|&emsp;&emsp;instructionCombinedScore|组合分||false|string||
|&emsp;&emsp;instructionPhysicalEdu|实验||false|string||
|&emsp;&emsp;instructionPlanNum|拟招人数||false|integer(int32)||
|&emsp;&emsp;instructionRemarkScore|综合素质||false|string||
|&emsp;&emsp;instructionScoreLevel|指导分数线(组合分)||false|string||
|&emsp;&emsp;instructionSingelSubject|单科限制||false|string||
|&emsp;&emsp;instructionSumScore|总分||false|string||
|&emsp;&emsp;lodgingInfo|内宿信息||false|string||
|&emsp;&emsp;phaseId|时段名称||false|string||
|&emsp;&emsp;phaseIdBak|时段名称||false|string||
|&emsp;&emsp;specplanNum|特长生拟招人数||false|integer(int32)||
|&emsp;&emsp;status|报名状态||false|string||
|&emsp;&emsp;updateBy|更新人||false|string||
|&emsp;&emsp;updateTime|更新日期||false|string(date-time)||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«string»|
|201|Created||
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|string||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": "",
	"success": true,
	"timestamp": 0
}
```


## 报名规则-批量修改字段值


**接口地址**:`/nnzk/rule/ruleOfSignUp/batchUpdateField`


**请求方式**:`POST`


**请求数据类型**:`application/json`


**响应数据类型**:`*/*`


**接口描述**:<p>报名规则-批量修改字段值</p>



**请求示例**:


```javascript
{
  "enClaim": 0,
  "enGuide": 0,
  "enInstruction": 0,
  "enLodging": 0,
  "schoolCodes": [],
  "status": ""
}
```


**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|input|input|body|true|BatchUpdateROSFieldDTO|BatchUpdateROSFieldDTO|
|&emsp;&emsp;enClaim|是否允许公示||false|integer(int32)||
|&emsp;&emsp;enGuide|是否可报指导||false|integer(int32)||
|&emsp;&emsp;enInstruction|是否可报指令||false|integer(int32)||
|&emsp;&emsp;enLodging|是否可住宿||false|integer(int32)||
|&emsp;&emsp;schoolCodes|||false|array|string|
|&emsp;&emsp;status|报名状态||false|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«string»|
|201|Created||
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|string||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": "",
	"success": true,
	"timestamp": 0
}
```


## 报名规则-通过id删除


**接口地址**:`/nnzk/rule/ruleOfSignUp/delete`


**请求方式**:`DELETE`


**请求数据类型**:`application/x-www-form-urlencoded`


**响应数据类型**:`*/*`


**接口描述**:<p>报名规则-通过id删除</p>



**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|id|id|query|true|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«string»|
|204|No Content||
|401|Unauthorized||
|403|Forbidden||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|string||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": "",
	"success": true,
	"timestamp": 0
}
```


## 报名规则-批量删除


**接口地址**:`/nnzk/rule/ruleOfSignUp/deleteBatch`


**请求方式**:`DELETE`


**请求数据类型**:`application/x-www-form-urlencoded`


**响应数据类型**:`*/*`


**接口描述**:<p>报名规则-批量删除</p>



**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|ids|ids|query|true|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«string»|
|204|No Content||
|401|Unauthorized||
|403|Forbidden||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|string||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": "",
	"success": true,
	"timestamp": 0
}
```


## 报名规则-编辑


**接口地址**:`/nnzk/rule/ruleOfSignUp/edit`


**请求方式**:`POST`


**请求数据类型**:`application/json`


**响应数据类型**:`*/*`


**接口描述**:<p>报名规则-编辑</p>



**请求示例**:


```javascript
{
  "createBy": "",
  "createTime": "",
  "delFlag": 0,
  "directionalPlanNum": 0,
  "displayInfo": "",
  "enClaim": 0,
  "enGuide": 0,
  "enInstruction": 0,
  "enLodging": 0,
  "guideCombinedScore": "",
  "guidePhysicalEdu": "",
  "guidePlanNum": 0,
  "guideRemarkScore": "",
  "guideScoreLevel": "",
  "guideSingelSubject": "",
  "guideSumScore": "",
  "highSchoolCode": "",
  "id": "",
  "instructionCombinedScore": "",
  "instructionPhysicalEdu": "",
  "instructionPlanNum": 0,
  "instructionRemarkScore": "",
  "instructionScoreLevel": "",
  "instructionSingelSubject": "",
  "instructionSumScore": "",
  "lodgingInfo": "",
  "phaseId": "",
  "phaseIdBak": "",
  "specplanNum": 0,
  "status": "",
  "updateBy": "",
  "updateTime": ""
}
```


**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|ruleOfSignUp|报名规则|body|true|rule_of_sign_up对象|rule_of_sign_up对象|
|&emsp;&emsp;createBy|创建人||false|string||
|&emsp;&emsp;createTime|创建日期||false|string(date-time)||
|&emsp;&emsp;delFlag|删除标识||false|integer(int32)||
|&emsp;&emsp;directionalPlanNum|定向指标||false|integer(int32)||
|&emsp;&emsp;displayInfo|公示信息||false|string||
|&emsp;&emsp;enClaim|允许公示||false|integer(int32)||
|&emsp;&emsp;enGuide|可报指导||false|integer(int32)||
|&emsp;&emsp;enInstruction|可报指令||false|integer(int32)||
|&emsp;&emsp;enLodging|可住宿||false|integer(int32)||
|&emsp;&emsp;guideCombinedScore|指导组合分||false|string||
|&emsp;&emsp;guidePhysicalEdu|指导实验||false|string||
|&emsp;&emsp;guidePlanNum|拟招人数||false|integer(int32)||
|&emsp;&emsp;guideRemarkScore|综合素质||false|string||
|&emsp;&emsp;guideScoreLevel|指导分数线(组合分)||false|string||
|&emsp;&emsp;guideSingelSubject|指导单科限制||false|string||
|&emsp;&emsp;guideSumScore|指导总分||false|string||
|&emsp;&emsp;highSchoolCode|(高中)学校代码||false|string||
|&emsp;&emsp;id|主键||false|string||
|&emsp;&emsp;instructionCombinedScore|组合分||false|string||
|&emsp;&emsp;instructionPhysicalEdu|实验||false|string||
|&emsp;&emsp;instructionPlanNum|拟招人数||false|integer(int32)||
|&emsp;&emsp;instructionRemarkScore|综合素质||false|string||
|&emsp;&emsp;instructionScoreLevel|指导分数线(组合分)||false|string||
|&emsp;&emsp;instructionSingelSubject|单科限制||false|string||
|&emsp;&emsp;instructionSumScore|总分||false|string||
|&emsp;&emsp;lodgingInfo|内宿信息||false|string||
|&emsp;&emsp;phaseId|时段名称||false|string||
|&emsp;&emsp;phaseIdBak|时段名称||false|string||
|&emsp;&emsp;specplanNum|特长生拟招人数||false|integer(int32)||
|&emsp;&emsp;status|报名状态||false|string||
|&emsp;&emsp;updateBy|更新人||false|string||
|&emsp;&emsp;updateTime|更新日期||false|string(date-time)||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«string»|
|201|Created||
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|string||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": "",
	"success": true,
	"timestamp": 0
}
```


## 报名规则-编辑


**接口地址**:`/nnzk/rule/ruleOfSignUp/edit`


**请求方式**:`PUT`


**请求数据类型**:`application/json`


**响应数据类型**:`*/*`


**接口描述**:<p>报名规则-编辑</p>



**请求示例**:


```javascript
{
  "createBy": "",
  "createTime": "",
  "delFlag": 0,
  "directionalPlanNum": 0,
  "displayInfo": "",
  "enClaim": 0,
  "enGuide": 0,
  "enInstruction": 0,
  "enLodging": 0,
  "guideCombinedScore": "",
  "guidePhysicalEdu": "",
  "guidePlanNum": 0,
  "guideRemarkScore": "",
  "guideScoreLevel": "",
  "guideSingelSubject": "",
  "guideSumScore": "",
  "highSchoolCode": "",
  "id": "",
  "instructionCombinedScore": "",
  "instructionPhysicalEdu": "",
  "instructionPlanNum": 0,
  "instructionRemarkScore": "",
  "instructionScoreLevel": "",
  "instructionSingelSubject": "",
  "instructionSumScore": "",
  "lodgingInfo": "",
  "phaseId": "",
  "phaseIdBak": "",
  "specplanNum": 0,
  "status": "",
  "updateBy": "",
  "updateTime": ""
}
```


**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|ruleOfSignUp|报名规则|body|true|rule_of_sign_up对象|rule_of_sign_up对象|
|&emsp;&emsp;createBy|创建人||false|string||
|&emsp;&emsp;createTime|创建日期||false|string(date-time)||
|&emsp;&emsp;delFlag|删除标识||false|integer(int32)||
|&emsp;&emsp;directionalPlanNum|定向指标||false|integer(int32)||
|&emsp;&emsp;displayInfo|公示信息||false|string||
|&emsp;&emsp;enClaim|允许公示||false|integer(int32)||
|&emsp;&emsp;enGuide|可报指导||false|integer(int32)||
|&emsp;&emsp;enInstruction|可报指令||false|integer(int32)||
|&emsp;&emsp;enLodging|可住宿||false|integer(int32)||
|&emsp;&emsp;guideCombinedScore|指导组合分||false|string||
|&emsp;&emsp;guidePhysicalEdu|指导实验||false|string||
|&emsp;&emsp;guidePlanNum|拟招人数||false|integer(int32)||
|&emsp;&emsp;guideRemarkScore|综合素质||false|string||
|&emsp;&emsp;guideScoreLevel|指导分数线(组合分)||false|string||
|&emsp;&emsp;guideSingelSubject|指导单科限制||false|string||
|&emsp;&emsp;guideSumScore|指导总分||false|string||
|&emsp;&emsp;highSchoolCode|(高中)学校代码||false|string||
|&emsp;&emsp;id|主键||false|string||
|&emsp;&emsp;instructionCombinedScore|组合分||false|string||
|&emsp;&emsp;instructionPhysicalEdu|实验||false|string||
|&emsp;&emsp;instructionPlanNum|拟招人数||false|integer(int32)||
|&emsp;&emsp;instructionRemarkScore|综合素质||false|string||
|&emsp;&emsp;instructionScoreLevel|指导分数线(组合分)||false|string||
|&emsp;&emsp;instructionSingelSubject|单科限制||false|string||
|&emsp;&emsp;instructionSumScore|总分||false|string||
|&emsp;&emsp;lodgingInfo|内宿信息||false|string||
|&emsp;&emsp;phaseId|时段名称||false|string||
|&emsp;&emsp;phaseIdBak|时段名称||false|string||
|&emsp;&emsp;specplanNum|特长生拟招人数||false|integer(int32)||
|&emsp;&emsp;status|报名状态||false|string||
|&emsp;&emsp;updateBy|更新人||false|string||
|&emsp;&emsp;updateTime|更新日期||false|string(date-time)||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«string»|
|201|Created||
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|string||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": "",
	"success": true,
	"timestamp": 0
}
```


## 报名规则-列表查询


**接口地址**:`/nnzk/rule/ruleOfSignUp/list`


**请求方式**:`GET`


**请求数据类型**:`application/x-www-form-urlencoded`


**响应数据类型**:`*/*`


**接口描述**:<p>报名规则-列表查询</p>



**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|enClaim|允许公示|query|false|integer(int32)||
|enGuide|可报指导|query|false|integer(int32)||
|enInstruction|可报指令|query|false|integer(int32)||
|enLodging|可住宿|query|false|integer(int32)||
|hgroupCode|高中分组|query|false|string||
|schoolType|学校类型|query|false|integer(int32)||
|status|报名状态|query|false|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«List«RuleOfSignUpVO»»|
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|array|RuleOfSignUpVO|
|&emsp;&emsp;belongRegion|所属区域|string||
|&emsp;&emsp;directionalPlanNum|定向指标|integer(int32)||
|&emsp;&emsp;dispOrder|填报时的显示顺序|integer(int32)||
|&emsp;&emsp;displayInfo|公示信息|string||
|&emsp;&emsp;enClaim|允许公示|integer(int32)||
|&emsp;&emsp;enGuide|可报指导|integer(int32)||
|&emsp;&emsp;enInstruction|可报指令|integer(int32)||
|&emsp;&emsp;enLodging|可住宿|integer(int32)||
|&emsp;&emsp;guideCombinedScore|指导组合分|string||
|&emsp;&emsp;guidePhysicalEdu|指导实验|string||
|&emsp;&emsp;guidePlanNum|拟招人数|integer(int32)||
|&emsp;&emsp;guideRemarkScore|综合素质|string||
|&emsp;&emsp;guideScoreLevel|指导分数线(组合分)|string||
|&emsp;&emsp;guideSingelSubject|指导单科限制|string||
|&emsp;&emsp;guideSumScore|指导总分|string||
|&emsp;&emsp;highSchoolCode|(高中)学校代码|string||
|&emsp;&emsp;id|主键|string||
|&emsp;&emsp;instructionCombinedScore|组合分|string||
|&emsp;&emsp;instructionPhysicalEdu|实验|string||
|&emsp;&emsp;instructionPlanNum|拟招人数|integer(int32)||
|&emsp;&emsp;instructionRemarkScore|综合素质|string||
|&emsp;&emsp;instructionScoreLevel|指导分数线(组合分)|string||
|&emsp;&emsp;instructionSingelSubject|单科限制|string||
|&emsp;&emsp;instructionSumScore|总分|string||
|&emsp;&emsp;isCurrentPhase|当前时段|integer(int32)||
|&emsp;&emsp;lodgingInfo|内宿信息|string||
|&emsp;&emsp;phaseId|时段名称|string||
|&emsp;&emsp;schoolType|学校类型|integer(int32)||
|&emsp;&emsp;specplanNum|特长生拟招人数|integer(int32)||
|&emsp;&emsp;status|报名状态|string||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": [
		{
			"belongRegion": "",
			"directionalPlanNum": 0,
			"dispOrder": 0,
			"displayInfo": "",
			"enClaim": 0,
			"enGuide": 0,
			"enInstruction": 0,
			"enLodging": 0,
			"guideCombinedScore": "",
			"guidePhysicalEdu": "",
			"guidePlanNum": 0,
			"guideRemarkScore": "",
			"guideScoreLevel": "",
			"guideSingelSubject": "",
			"guideSumScore": "",
			"highSchoolCode": "",
			"id": "",
			"instructionCombinedScore": "",
			"instructionPhysicalEdu": "",
			"instructionPlanNum": 0,
			"instructionRemarkScore": "",
			"instructionScoreLevel": "",
			"instructionSingelSubject": "",
			"instructionSumScore": "",
			"isCurrentPhase": 0,
			"lodgingInfo": "",
			"phaseId": "",
			"schoolType": 0,
			"specplanNum": 0,
			"status": ""
		}
	],
	"success": true,
	"timestamp": 0
}
```


## 报名规则-通过id查询


**接口地址**:`/nnzk/rule/ruleOfSignUp/queryById`


**请求方式**:`GET`


**请求数据类型**:`application/x-www-form-urlencoded`


**响应数据类型**:`*/*`


**接口描述**:<p>报名规则-通过id查询</p>



**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|id|id|query|true|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«rule_of_sign_up对象»|
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|rule_of_sign_up对象|rule_of_sign_up对象|
|&emsp;&emsp;createBy|创建人|string||
|&emsp;&emsp;createTime|创建日期|string(date-time)||
|&emsp;&emsp;delFlag|删除标识|integer(int32)||
|&emsp;&emsp;directionalPlanNum|定向指标|integer(int32)||
|&emsp;&emsp;displayInfo|公示信息|string||
|&emsp;&emsp;enClaim|允许公示|integer(int32)||
|&emsp;&emsp;enGuide|可报指导|integer(int32)||
|&emsp;&emsp;enInstruction|可报指令|integer(int32)||
|&emsp;&emsp;enLodging|可住宿|integer(int32)||
|&emsp;&emsp;guideCombinedScore|指导组合分|string||
|&emsp;&emsp;guidePhysicalEdu|指导实验|string||
|&emsp;&emsp;guidePlanNum|拟招人数|integer(int32)||
|&emsp;&emsp;guideRemarkScore|综合素质|string||
|&emsp;&emsp;guideScoreLevel|指导分数线(组合分)|string||
|&emsp;&emsp;guideSingelSubject|指导单科限制|string||
|&emsp;&emsp;guideSumScore|指导总分|string||
|&emsp;&emsp;highSchoolCode|(高中)学校代码|string||
|&emsp;&emsp;id|主键|string||
|&emsp;&emsp;instructionCombinedScore|组合分|string||
|&emsp;&emsp;instructionPhysicalEdu|实验|string||
|&emsp;&emsp;instructionPlanNum|拟招人数|integer(int32)||
|&emsp;&emsp;instructionRemarkScore|综合素质|string||
|&emsp;&emsp;instructionScoreLevel|指导分数线(组合分)|string||
|&emsp;&emsp;instructionSingelSubject|单科限制|string||
|&emsp;&emsp;instructionSumScore|总分|string||
|&emsp;&emsp;lodgingInfo|内宿信息|string||
|&emsp;&emsp;phaseId|时段名称|string||
|&emsp;&emsp;phaseIdBak|时段名称|string||
|&emsp;&emsp;specplanNum|特长生拟招人数|integer(int32)||
|&emsp;&emsp;status|报名状态|string||
|&emsp;&emsp;updateBy|更新人|string||
|&emsp;&emsp;updateTime|更新日期|string(date-time)||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": {
		"createBy": "",
		"createTime": "",
		"delFlag": 0,
		"directionalPlanNum": 0,
		"displayInfo": "",
		"enClaim": 0,
		"enGuide": 0,
		"enInstruction": 0,
		"enLodging": 0,
		"guideCombinedScore": "",
		"guidePhysicalEdu": "",
		"guidePlanNum": 0,
		"guideRemarkScore": "",
		"guideScoreLevel": "",
		"guideSingelSubject": "",
		"guideSumScore": "",
		"highSchoolCode": "",
		"id": "",
		"instructionCombinedScore": "",
		"instructionPhysicalEdu": "",
		"instructionPlanNum": 0,
		"instructionRemarkScore": "",
		"instructionScoreLevel": "",
		"instructionSingelSubject": "",
		"instructionSumScore": "",
		"lodgingInfo": "",
		"phaseId": "",
		"phaseIdBak": "",
		"specplanNum": 0,
		"status": "",
		"updateBy": "",
		"updateTime": ""
	},
	"success": true,
	"timestamp": 0
}
```


# 报表脚本


## 报表脚本-添加


**接口地址**:`/nnzk/base/reportScript/add`


**请求方式**:`POST`


**请求数据类型**:`application/json`


**响应数据类型**:`*/*`


**接口描述**:<p>报表脚本-添加</p>



**请求示例**:


```javascript
{
  "id": "",
  "name": "",
  "script": "",
  "scriptGroup": ""
}
```


**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|reportScript|报表脚本|body|true|report_script对象|report_script对象|
|&emsp;&emsp;id|主键||false|string||
|&emsp;&emsp;name|报表名称||false|string||
|&emsp;&emsp;script|取数脚本||false|string||
|&emsp;&emsp;scriptGroup|隶属组群||false|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«string»|
|201|Created||
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|string||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": "",
	"success": true,
	"timestamp": 0
}
```


## 报表脚本-通过id删除


**接口地址**:`/nnzk/base/reportScript/delete`


**请求方式**:`DELETE`


**请求数据类型**:`application/x-www-form-urlencoded`


**响应数据类型**:`*/*`


**接口描述**:<p>报表脚本-通过id删除</p>



**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|id|id|query|true|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«string»|
|204|No Content||
|401|Unauthorized||
|403|Forbidden||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|string||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": "",
	"success": true,
	"timestamp": 0
}
```


## 报表脚本-批量删除


**接口地址**:`/nnzk/base/reportScript/deleteBatch`


**请求方式**:`DELETE`


**请求数据类型**:`application/x-www-form-urlencoded`


**响应数据类型**:`*/*`


**接口描述**:<p>报表脚本-批量删除</p>



**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|ids|ids|query|true|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«string»|
|204|No Content||
|401|Unauthorized||
|403|Forbidden||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|string||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": "",
	"success": true,
	"timestamp": 0
}
```


## 报表脚本-编辑


**接口地址**:`/nnzk/base/reportScript/edit`


**请求方式**:`POST`


**请求数据类型**:`application/json`


**响应数据类型**:`*/*`


**接口描述**:<p>报表脚本-编辑</p>



**请求示例**:


```javascript
{
  "id": "",
  "name": "",
  "script": "",
  "scriptGroup": ""
}
```


**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|reportScript|报表脚本|body|true|report_script对象|report_script对象|
|&emsp;&emsp;id|主键||false|string||
|&emsp;&emsp;name|报表名称||false|string||
|&emsp;&emsp;script|取数脚本||false|string||
|&emsp;&emsp;scriptGroup|隶属组群||false|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«string»|
|201|Created||
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|string||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": "",
	"success": true,
	"timestamp": 0
}
```


## 报表脚本-编辑


**接口地址**:`/nnzk/base/reportScript/edit`


**请求方式**:`PUT`


**请求数据类型**:`application/json`


**响应数据类型**:`*/*`


**接口描述**:<p>报表脚本-编辑</p>



**请求示例**:


```javascript
{
  "id": "",
  "name": "",
  "script": "",
  "scriptGroup": ""
}
```


**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|reportScript|报表脚本|body|true|report_script对象|report_script对象|
|&emsp;&emsp;id|主键||false|string||
|&emsp;&emsp;name|报表名称||false|string||
|&emsp;&emsp;script|取数脚本||false|string||
|&emsp;&emsp;scriptGroup|隶属组群||false|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«string»|
|201|Created||
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|string||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": "",
	"success": true,
	"timestamp": 0
}
```


## 报表脚本-分页列表查询


**接口地址**:`/nnzk/base/reportScript/list`


**请求方式**:`GET`


**请求数据类型**:`application/x-www-form-urlencoded`


**响应数据类型**:`*/*`


**接口描述**:<p>报表脚本-分页列表查询</p>



**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|id|主键|query|false|string||
|name|报表名称|query|false|string||
|pageNo|pageNo|query|false|integer(int32)||
|pageSize|pageSize|query|false|integer(int32)||
|script|取数脚本|query|false|string||
|scriptGroup|隶属组群|query|false|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«IPage«report_script对象»»|
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|IPage«report_script对象»|IPage«report_script对象»|
|&emsp;&emsp;current||integer(int64)||
|&emsp;&emsp;pages||integer(int64)||
|&emsp;&emsp;records||array|report_script对象|
|&emsp;&emsp;&emsp;&emsp;id|主键|string||
|&emsp;&emsp;&emsp;&emsp;name|报表名称|string||
|&emsp;&emsp;&emsp;&emsp;script|取数脚本|string||
|&emsp;&emsp;&emsp;&emsp;scriptGroup|隶属组群|string||
|&emsp;&emsp;size||integer(int64)||
|&emsp;&emsp;total||integer(int64)||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": {
		"current": 0,
		"pages": 0,
		"records": [
			{
				"id": "",
				"name": "",
				"script": "",
				"scriptGroup": ""
			}
		],
		"size": 0,
		"total": 0
	},
	"success": true,
	"timestamp": 0
}
```


## 报表脚本-通过id查询


**接口地址**:`/nnzk/base/reportScript/queryById`


**请求方式**:`GET`


**请求数据类型**:`application/x-www-form-urlencoded`


**响应数据类型**:`*/*`


**接口描述**:<p>报表脚本-通过id查询</p>



**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|id|id|query|true|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«report_script对象»|
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|report_script对象|report_script对象|
|&emsp;&emsp;id|主键|string||
|&emsp;&emsp;name|报表名称|string||
|&emsp;&emsp;script|取数脚本|string||
|&emsp;&emsp;scriptGroup|隶属组群|string||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": {
		"id": "",
		"name": "",
		"script": "",
		"scriptGroup": ""
	},
	"success": true,
	"timestamp": 0
}
```


# 拖拽WebSocket测试


## 测试拖拽组件更新


**接口地址**:`/nnzk/drag/websocket/sendData`


**请求方式**:`POST`


**请求数据类型**:`application/json`


**响应数据类型**:`*/*`


**接口描述**:<p>测试拖拽组件更新</p>



**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|chartId|chartId|query|false|string||
|data|data|query|false|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«string»|
|201|Created||
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|string||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": "",
	"success": true,
	"timestamp": 0
}
```


# 招办端补录


## 招办端补录-关闭民办学校补录权限


**接口地址**:`/nnzk/alter/admissionsOffice/closePermission`


**请求方式**:`PUT`


**请求数据类型**:`application/json`


**响应数据类型**:`*/*`


**接口描述**:<p>招办端补录-关闭民办学校补录权限</p>



**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|id|id|query|true|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«string»|
|201|Created||
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|string||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": "",
	"success": true,
	"timestamp": 0
}
```


## 招办端补录-开启民办学校补录权限


**接口地址**:`/nnzk/alter/admissionsOffice/enablePermission`


**请求方式**:`PUT`


**请求数据类型**:`application/json`


**响应数据类型**:`*/*`


**接口描述**:<p>招办端补录-开启民办学校补录权限</p>



**请求示例**:


```javascript
{
  "admissionsNumber": 0,
  "enrollmentPlan": 0,
  "giveUpAdmissionsNumber": 0,
  "id": "",
  "introduceName": "",
  "isGiveUpAdmission": 0,
  "isNeedAudit": 0,
  "isOpenReview": 0,
  "makeUpNumber": 0,
  "supplementFrequency": 0,
  "supplementNumber": 0
}
```


**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|input|input|body|true|HighSchoolEditDTO|HighSchoolEditDTO|
|&emsp;&emsp;admissionsNumber|录取人数||false|integer(int32)||
|&emsp;&emsp;enrollmentPlan|招生计划数||false|integer(int32)||
|&emsp;&emsp;giveUpAdmissionsNumber|放弃录取人数||false|integer(int32)||
|&emsp;&emsp;id|主键id||false|string||
|&emsp;&emsp;introduceName|介绍名称||false|string||
|&emsp;&emsp;isGiveUpAdmission|开放放弃补录||false|integer(int32)||
|&emsp;&emsp;isNeedAudit|是否需要审核||false|integer(int32)||
|&emsp;&emsp;isOpenReview|是否开放补录||false|integer(int32)||
|&emsp;&emsp;makeUpNumber|补录人数||false|integer(int32)||
|&emsp;&emsp;supplementFrequency|补录次数||false|integer(int32)||
|&emsp;&emsp;supplementNumber|增补计划数||false|integer(int32)||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«string»|
|201|Created||
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|string||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": "",
	"success": true,
	"timestamp": 0
}
```


## 招办端补录-退回补录申请


**接口地址**:`/nnzk/alter/admissionsOffice/failedMakeUpApplication`


**请求方式**:`POST`


**请求数据类型**:`application/json`


**响应数据类型**:`*/*`


**接口描述**:<p>招办端补录-退回补录申请</p>



**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|id|id|query|true|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«string»|
|201|Created||
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|string||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": "",
	"success": true,
	"timestamp": 0
}
```


## 招办端补录-获取民办学校列表


**接口地址**:`/nnzk/alter/admissionsOffice/getPrivateHighSchoolList`


**请求方式**:`GET`


**请求数据类型**:`application/x-www-form-urlencoded`


**响应数据类型**:`*/*`


**接口描述**:<p>招办端补录-获取民办学校列表</p>



**请求参数**:


暂无


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«List«PrivateHighSchoolDTO»»|
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|array|PrivateHighSchoolDTO|
|&emsp;&emsp;admissionsNumber|录取人数|integer(int32)||
|&emsp;&emsp;awaitAdmissionsNumber|待确认录取人数|integer(int32)||
|&emsp;&emsp;awaitRecordNumber|待备案人数|integer(int32)||
|&emsp;&emsp;enrollmentPlan|招生计划数|integer(int32)||
|&emsp;&emsp;giveUpAdmissionsNumber|放弃录取人数|integer(int32)||
|&emsp;&emsp;haveStudent|实际录取人数|integer(int32)||
|&emsp;&emsp;id|主键id|string||
|&emsp;&emsp;isGiveUpAdmission|开放放弃补录|integer(int32)||
|&emsp;&emsp;isNeedAudit|是否需要审核|integer(int32)||
|&emsp;&emsp;isOpenReview|是否开放补录|integer(int32)||
|&emsp;&emsp;makeUpNumber|补录人数|integer(int32)||
|&emsp;&emsp;recordNumber|备案人数|integer(int32)||
|&emsp;&emsp;schoolName|学校名称|string||
|&emsp;&emsp;supplementFrequency|补录次数|integer(int32)||
|&emsp;&emsp;supplementNumber|增补计划数|integer(int32)||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": [
		{
			"admissionsNumber": 0,
			"awaitAdmissionsNumber": 0,
			"awaitRecordNumber": 0,
			"enrollmentPlan": 0,
			"giveUpAdmissionsNumber": 0,
			"haveStudent": 0,
			"id": "",
			"isGiveUpAdmission": 0,
			"isNeedAudit": 0,
			"isOpenReview": 0,
			"makeUpNumber": 0,
			"recordNumber": 0,
			"schoolName": "",
			"supplementFrequency": 0,
			"supplementNumber": 0
		}
	],
	"success": true,
	"timestamp": 0
}
```


## 招办端补录-同意补录申请


**接口地址**:`/nnzk/alter/admissionsOffice/passMakeUpApplication`


**请求方式**:`POST`


**请求数据类型**:`application/json`


**响应数据类型**:`*/*`


**接口描述**:<p>招办端补录-同意补录申请</p>



**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|id|id|query|true|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«string»|
|201|Created||
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|string||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": "",
	"success": true,
	"timestamp": 0
}
```


# 招生时段表


## 招生时段表-添加


**接口地址**:`/nnzk/base/periodOfEnrollment/add`


**请求方式**:`POST`


**请求数据类型**:`application/json`


**响应数据类型**:`*/*`


**接口描述**:<p>招生时段表-添加</p>



**请求示例**:


```javascript
{
  "admNotes": "",
  "admPeriod": "",
  "admPermission": "",
  "admQueryPermission": "",
  "admWorkContent": "",
  "createBy": "",
  "createTime": "",
  "dayNum": 0,
  "delFlag": 0,
  "id": "",
  "registNotes": "",
  "registPeriod": "",
  "registPermission": "",
  "registQueryPermission": "",
  "registWorkContent": "",
  "updateBy": "",
  "updateTime": ""
}
```


**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|periodOfEnrollment|招生时段表|body|true|period_of_enrollment对象|period_of_enrollment对象|
|&emsp;&emsp;admNotes|录取注意||false|string||
|&emsp;&emsp;admPeriod|录取时段||false|string||
|&emsp;&emsp;admPermission|录取权限||false|string||
|&emsp;&emsp;admQueryPermission|录取查询权限||false|string||
|&emsp;&emsp;admWorkContent|录取招生工作内容||false|string||
|&emsp;&emsp;createBy|创建人||false|string||
|&emsp;&emsp;createTime|创建日期||false|string(date-time)||
|&emsp;&emsp;dayNum|天数||false|integer(int32)||
|&emsp;&emsp;delFlag|删除标识||false|integer(int32)||
|&emsp;&emsp;id|主键||false|string||
|&emsp;&emsp;registNotes|报名注意||false|string||
|&emsp;&emsp;registPeriod|报名时段||false|string||
|&emsp;&emsp;registPermission|报名权限||false|string||
|&emsp;&emsp;registQueryPermission|报名查询权限||false|string||
|&emsp;&emsp;registWorkContent|报名招生工作内容||false|string||
|&emsp;&emsp;updateBy|更新人||false|string||
|&emsp;&emsp;updateTime|更新日期||false|string(date-time)||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«string»|
|201|Created||
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|string||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": "",
	"success": true,
	"timestamp": 0
}
```


## 招生时段表-通过id删除


**接口地址**:`/nnzk/base/periodOfEnrollment/delete`


**请求方式**:`DELETE`


**请求数据类型**:`application/x-www-form-urlencoded`


**响应数据类型**:`*/*`


**接口描述**:<p>招生时段表-通过id删除</p>



**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|id|id|query|true|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«string»|
|204|No Content||
|401|Unauthorized||
|403|Forbidden||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|string||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": "",
	"success": true,
	"timestamp": 0
}
```


## 招生时段表-批量删除


**接口地址**:`/nnzk/base/periodOfEnrollment/deleteBatch`


**请求方式**:`DELETE`


**请求数据类型**:`application/x-www-form-urlencoded`


**响应数据类型**:`*/*`


**接口描述**:<p>招生时段表-批量删除</p>



**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|ids|ids|query|true|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«string»|
|204|No Content||
|401|Unauthorized||
|403|Forbidden||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|string||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": "",
	"success": true,
	"timestamp": 0
}
```


## 招生时段表-编辑


**接口地址**:`/nnzk/base/periodOfEnrollment/edit`


**请求方式**:`POST`


**请求数据类型**:`application/json`


**响应数据类型**:`*/*`


**接口描述**:<p>招生时段表-编辑</p>



**请求示例**:


```javascript
{
  "admNotes": "",
  "admPeriod": "",
  "admPermission": "",
  "admQueryPermission": "",
  "admWorkContent": "",
  "createBy": "",
  "createTime": "",
  "dayNum": 0,
  "delFlag": 0,
  "id": "",
  "registNotes": "",
  "registPeriod": "",
  "registPermission": "",
  "registQueryPermission": "",
  "registWorkContent": "",
  "updateBy": "",
  "updateTime": ""
}
```


**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|periodOfEnrollment|招生时段表|body|true|period_of_enrollment对象|period_of_enrollment对象|
|&emsp;&emsp;admNotes|录取注意||false|string||
|&emsp;&emsp;admPeriod|录取时段||false|string||
|&emsp;&emsp;admPermission|录取权限||false|string||
|&emsp;&emsp;admQueryPermission|录取查询权限||false|string||
|&emsp;&emsp;admWorkContent|录取招生工作内容||false|string||
|&emsp;&emsp;createBy|创建人||false|string||
|&emsp;&emsp;createTime|创建日期||false|string(date-time)||
|&emsp;&emsp;dayNum|天数||false|integer(int32)||
|&emsp;&emsp;delFlag|删除标识||false|integer(int32)||
|&emsp;&emsp;id|主键||false|string||
|&emsp;&emsp;registNotes|报名注意||false|string||
|&emsp;&emsp;registPeriod|报名时段||false|string||
|&emsp;&emsp;registPermission|报名权限||false|string||
|&emsp;&emsp;registQueryPermission|报名查询权限||false|string||
|&emsp;&emsp;registWorkContent|报名招生工作内容||false|string||
|&emsp;&emsp;updateBy|更新人||false|string||
|&emsp;&emsp;updateTime|更新日期||false|string(date-time)||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«string»|
|201|Created||
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|string||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": "",
	"success": true,
	"timestamp": 0
}
```


## 招生时段表-编辑


**接口地址**:`/nnzk/base/periodOfEnrollment/edit`


**请求方式**:`PUT`


**请求数据类型**:`application/json`


**响应数据类型**:`*/*`


**接口描述**:<p>招生时段表-编辑</p>



**请求示例**:


```javascript
{
  "admNotes": "",
  "admPeriod": "",
  "admPermission": "",
  "admQueryPermission": "",
  "admWorkContent": "",
  "createBy": "",
  "createTime": "",
  "dayNum": 0,
  "delFlag": 0,
  "id": "",
  "registNotes": "",
  "registPeriod": "",
  "registPermission": "",
  "registQueryPermission": "",
  "registWorkContent": "",
  "updateBy": "",
  "updateTime": ""
}
```


**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|periodOfEnrollment|招生时段表|body|true|period_of_enrollment对象|period_of_enrollment对象|
|&emsp;&emsp;admNotes|录取注意||false|string||
|&emsp;&emsp;admPeriod|录取时段||false|string||
|&emsp;&emsp;admPermission|录取权限||false|string||
|&emsp;&emsp;admQueryPermission|录取查询权限||false|string||
|&emsp;&emsp;admWorkContent|录取招生工作内容||false|string||
|&emsp;&emsp;createBy|创建人||false|string||
|&emsp;&emsp;createTime|创建日期||false|string(date-time)||
|&emsp;&emsp;dayNum|天数||false|integer(int32)||
|&emsp;&emsp;delFlag|删除标识||false|integer(int32)||
|&emsp;&emsp;id|主键||false|string||
|&emsp;&emsp;registNotes|报名注意||false|string||
|&emsp;&emsp;registPeriod|报名时段||false|string||
|&emsp;&emsp;registPermission|报名权限||false|string||
|&emsp;&emsp;registQueryPermission|报名查询权限||false|string||
|&emsp;&emsp;registWorkContent|报名招生工作内容||false|string||
|&emsp;&emsp;updateBy|更新人||false|string||
|&emsp;&emsp;updateTime|更新日期||false|string(date-time)||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«string»|
|201|Created||
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|string||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": "",
	"success": true,
	"timestamp": 0
}
```


## 招生时段表-分页列表查询


**接口地址**:`/nnzk/base/periodOfEnrollment/list`


**请求方式**:`GET`


**请求数据类型**:`application/x-www-form-urlencoded`


**响应数据类型**:`*/*`


**接口描述**:<p>招生时段表-分页列表查询</p>



**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|admNotes|录取注意|query|true|string||
|admPeriod|录取时段|query|true|string||
|admPermission|录取权限|query|true|string||
|admQueryPermission|录取查询权限|query|true|string||
|admWorkContent|录取招生工作内容|query|true|string||
|dayNum|天数|query|true|integer(int32)||
|registNotes|报名注意|query|true|string||
|registPeriod|报名时段|query|true|string||
|registPermission|报名权限|query|true|string||
|registQueryPermission|报名查询权限|query|true|string||
|registWorkContent|报名招生工作内容|query|true|string||
|createBy|创建人|query|false|string||
|createTime|创建日期|query|false|string(date-time)||
|delFlag|删除标识|query|false|integer(int32)||
|id|主键|query|false|string||
|pageNo|pageNo|query|false|integer(int32)||
|pageSize|pageSize|query|false|integer(int32)||
|updateBy|更新人|query|false|string||
|updateTime|更新日期|query|false|string(date-time)||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«IPage«period_of_enrollment对象»»|
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|IPage«period_of_enrollment对象»|IPage«period_of_enrollment对象»|
|&emsp;&emsp;current||integer(int64)||
|&emsp;&emsp;pages||integer(int64)||
|&emsp;&emsp;records||array|period_of_enrollment对象|
|&emsp;&emsp;&emsp;&emsp;admNotes|录取注意|string||
|&emsp;&emsp;&emsp;&emsp;admPeriod|录取时段|string||
|&emsp;&emsp;&emsp;&emsp;admPermission|录取权限|string||
|&emsp;&emsp;&emsp;&emsp;admQueryPermission|录取查询权限|string||
|&emsp;&emsp;&emsp;&emsp;admWorkContent|录取招生工作内容|string||
|&emsp;&emsp;&emsp;&emsp;createBy|创建人|string||
|&emsp;&emsp;&emsp;&emsp;createTime|创建日期|string||
|&emsp;&emsp;&emsp;&emsp;dayNum|天数|integer||
|&emsp;&emsp;&emsp;&emsp;delFlag|删除标识|integer||
|&emsp;&emsp;&emsp;&emsp;id|主键|string||
|&emsp;&emsp;&emsp;&emsp;registNotes|报名注意|string||
|&emsp;&emsp;&emsp;&emsp;registPeriod|报名时段|string||
|&emsp;&emsp;&emsp;&emsp;registPermission|报名权限|string||
|&emsp;&emsp;&emsp;&emsp;registQueryPermission|报名查询权限|string||
|&emsp;&emsp;&emsp;&emsp;registWorkContent|报名招生工作内容|string||
|&emsp;&emsp;&emsp;&emsp;updateBy|更新人|string||
|&emsp;&emsp;&emsp;&emsp;updateTime|更新日期|string||
|&emsp;&emsp;size||integer(int64)||
|&emsp;&emsp;total||integer(int64)||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": {
		"current": 0,
		"pages": 0,
		"records": [
			{
				"admNotes": "",
				"admPeriod": "",
				"admPermission": "",
				"admQueryPermission": "",
				"admWorkContent": "",
				"createBy": "",
				"createTime": "",
				"dayNum": 0,
				"delFlag": 0,
				"id": "",
				"registNotes": "",
				"registPeriod": "",
				"registPermission": "",
				"registQueryPermission": "",
				"registWorkContent": "",
				"updateBy": "",
				"updateTime": ""
			}
		],
		"size": 0,
		"total": 0
	},
	"success": true,
	"timestamp": 0
}
```


## 招生时段表-学生端列表


**接口地址**:`/nnzk/base/periodOfEnrollment/periodOfEnrollmentList`


**请求方式**:`GET`


**请求数据类型**:`application/x-www-form-urlencoded`


**响应数据类型**:`*/*`


**接口描述**:<p>招生时段表-学生端列表</p>



**请求参数**:


暂无


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«List«PeriodOfEnrollmentVO»»|
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|array|PeriodOfEnrollmentVO|
|&emsp;&emsp;admNotes|录取注意|string||
|&emsp;&emsp;admPeriod|录取时段|string||
|&emsp;&emsp;admPermission|录取权限|string||
|&emsp;&emsp;admQueryPermission|录取查询权限|string||
|&emsp;&emsp;admWorkContent|录取招生工作内容|string||
|&emsp;&emsp;dayNum|天数|integer(int32)||
|&emsp;&emsp;id|主键|string||
|&emsp;&emsp;registNotes|报名注意|string||
|&emsp;&emsp;registPeriod|报名时段|string||
|&emsp;&emsp;registPermission|报名权限|string||
|&emsp;&emsp;registQueryPermission|报名查询权限|string||
|&emsp;&emsp;registWorkContent|报名招生工作内容|string||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": [
		{
			"admNotes": "",
			"admPeriod": "",
			"admPermission": "",
			"admQueryPermission": "",
			"admWorkContent": "",
			"dayNum": 0,
			"id": "",
			"registNotes": "",
			"registPeriod": "",
			"registPermission": "",
			"registQueryPermission": "",
			"registWorkContent": ""
		}
	],
	"success": true,
	"timestamp": 0
}
```


## 招生时段表-通过id查询


**接口地址**:`/nnzk/base/periodOfEnrollment/queryById`


**请求方式**:`GET`


**请求数据类型**:`application/x-www-form-urlencoded`


**响应数据类型**:`*/*`


**接口描述**:<p>招生时段表-通过id查询</p>



**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|id|id|query|true|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«period_of_enrollment对象»|
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|period_of_enrollment对象|period_of_enrollment对象|
|&emsp;&emsp;admNotes|录取注意|string||
|&emsp;&emsp;admPeriod|录取时段|string||
|&emsp;&emsp;admPermission|录取权限|string||
|&emsp;&emsp;admQueryPermission|录取查询权限|string||
|&emsp;&emsp;admWorkContent|录取招生工作内容|string||
|&emsp;&emsp;createBy|创建人|string||
|&emsp;&emsp;createTime|创建日期|string(date-time)||
|&emsp;&emsp;dayNum|天数|integer(int32)||
|&emsp;&emsp;delFlag|删除标识|integer(int32)||
|&emsp;&emsp;id|主键|string||
|&emsp;&emsp;registNotes|报名注意|string||
|&emsp;&emsp;registPeriod|报名时段|string||
|&emsp;&emsp;registPermission|报名权限|string||
|&emsp;&emsp;registQueryPermission|报名查询权限|string||
|&emsp;&emsp;registWorkContent|报名招生工作内容|string||
|&emsp;&emsp;updateBy|更新人|string||
|&emsp;&emsp;updateTime|更新日期|string(date-time)||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": {
		"admNotes": "",
		"admPeriod": "",
		"admPermission": "",
		"admQueryPermission": "",
		"admWorkContent": "",
		"createBy": "",
		"createTime": "",
		"dayNum": 0,
		"delFlag": 0,
		"id": "",
		"registNotes": "",
		"registPeriod": "",
		"registPermission": "",
		"registQueryPermission": "",
		"registWorkContent": "",
		"updateBy": "",
		"updateTime": ""
	},
	"success": true,
	"timestamp": 0
}
```


# 操作历史表


## 操作历史表-添加


**接口地址**:`/nnzk/studentLog/operationHistory/add`


**请求方式**:`POST`


**请求数据类型**:`application/json`


**响应数据类型**:`*/*`


**接口描述**:<p>操作历史表-添加</p>



**请求示例**:


```javascript
{
  "account": "",
  "archiveCode": "",
  "createBy": "",
  "createTime": "",
  "delFlag": 0,
  "id": "",
  "ip": "",
  "isStudentSelf": 0,
  "operateDatetime": "",
  "operateKind": "",
  "operateLog": "",
  "schoolCode": "",
  "schoolName": "",
  "signUpType": "",
  "updateBy": "",
  "updateTime": "",
  "winNo": ""
}
```


**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|operationHistory|操作历史表|body|true|operation_history对象|operation_history对象|
|&emsp;&emsp;account|账号||false|string||
|&emsp;&emsp;archiveCode|准考证号||false|string||
|&emsp;&emsp;createBy|创建人||false|string||
|&emsp;&emsp;createTime|创建日期||false|string(date-time)||
|&emsp;&emsp;delFlag|删除标识||false|integer(int32)||
|&emsp;&emsp;id|主键||false|string||
|&emsp;&emsp;ip|网络IP||false|string||
|&emsp;&emsp;isStudentSelf|学生本人||false|integer(int32)||
|&emsp;&emsp;operateDatetime|操作时间||false|string(date-time)||
|&emsp;&emsp;operateKind|操作类型||false|string||
|&emsp;&emsp;operateLog|操作日志||false|string||
|&emsp;&emsp;schoolCode|报名高中学校代码||false|string||
|&emsp;&emsp;schoolName|报名高中学校名称||false|string||
|&emsp;&emsp;signUpType|报名类型||false|string||
|&emsp;&emsp;updateBy|更新人||false|string||
|&emsp;&emsp;updateTime|更新日期||false|string(date-time)||
|&emsp;&emsp;winNo|平台端||false|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«string»|
|201|Created||
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|string||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": "",
	"success": true,
	"timestamp": 0
}
```


## 操作历史表-通过id删除


**接口地址**:`/nnzk/studentLog/operationHistory/delete`


**请求方式**:`DELETE`


**请求数据类型**:`application/x-www-form-urlencoded`


**响应数据类型**:`*/*`


**接口描述**:<p>操作历史表-通过id删除</p>



**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|id|id|query|true|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«string»|
|204|No Content||
|401|Unauthorized||
|403|Forbidden||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|string||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": "",
	"success": true,
	"timestamp": 0
}
```


## 操作历史表-批量删除


**接口地址**:`/nnzk/studentLog/operationHistory/deleteBatch`


**请求方式**:`DELETE`


**请求数据类型**:`application/x-www-form-urlencoded`


**响应数据类型**:`*/*`


**接口描述**:<p>操作历史表-批量删除</p>



**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|ids|ids|query|true|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«string»|
|204|No Content||
|401|Unauthorized||
|403|Forbidden||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|string||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": "",
	"success": true,
	"timestamp": 0
}
```


## 操作历史表-编辑


**接口地址**:`/nnzk/studentLog/operationHistory/edit`


**请求方式**:`POST`


**请求数据类型**:`application/json`


**响应数据类型**:`*/*`


**接口描述**:<p>操作历史表-编辑</p>



**请求示例**:


```javascript
{
  "account": "",
  "archiveCode": "",
  "createBy": "",
  "createTime": "",
  "delFlag": 0,
  "id": "",
  "ip": "",
  "isStudentSelf": 0,
  "operateDatetime": "",
  "operateKind": "",
  "operateLog": "",
  "schoolCode": "",
  "schoolName": "",
  "signUpType": "",
  "updateBy": "",
  "updateTime": "",
  "winNo": ""
}
```


**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|operationHistory|操作历史表|body|true|operation_history对象|operation_history对象|
|&emsp;&emsp;account|账号||false|string||
|&emsp;&emsp;archiveCode|准考证号||false|string||
|&emsp;&emsp;createBy|创建人||false|string||
|&emsp;&emsp;createTime|创建日期||false|string(date-time)||
|&emsp;&emsp;delFlag|删除标识||false|integer(int32)||
|&emsp;&emsp;id|主键||false|string||
|&emsp;&emsp;ip|网络IP||false|string||
|&emsp;&emsp;isStudentSelf|学生本人||false|integer(int32)||
|&emsp;&emsp;operateDatetime|操作时间||false|string(date-time)||
|&emsp;&emsp;operateKind|操作类型||false|string||
|&emsp;&emsp;operateLog|操作日志||false|string||
|&emsp;&emsp;schoolCode|报名高中学校代码||false|string||
|&emsp;&emsp;schoolName|报名高中学校名称||false|string||
|&emsp;&emsp;signUpType|报名类型||false|string||
|&emsp;&emsp;updateBy|更新人||false|string||
|&emsp;&emsp;updateTime|更新日期||false|string(date-time)||
|&emsp;&emsp;winNo|平台端||false|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«string»|
|201|Created||
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|string||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": "",
	"success": true,
	"timestamp": 0
}
```


## 操作历史表-编辑


**接口地址**:`/nnzk/studentLog/operationHistory/edit`


**请求方式**:`PUT`


**请求数据类型**:`application/json`


**响应数据类型**:`*/*`


**接口描述**:<p>操作历史表-编辑</p>



**请求示例**:


```javascript
{
  "account": "",
  "archiveCode": "",
  "createBy": "",
  "createTime": "",
  "delFlag": 0,
  "id": "",
  "ip": "",
  "isStudentSelf": 0,
  "operateDatetime": "",
  "operateKind": "",
  "operateLog": "",
  "schoolCode": "",
  "schoolName": "",
  "signUpType": "",
  "updateBy": "",
  "updateTime": "",
  "winNo": ""
}
```


**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|operationHistory|操作历史表|body|true|operation_history对象|operation_history对象|
|&emsp;&emsp;account|账号||false|string||
|&emsp;&emsp;archiveCode|准考证号||false|string||
|&emsp;&emsp;createBy|创建人||false|string||
|&emsp;&emsp;createTime|创建日期||false|string(date-time)||
|&emsp;&emsp;delFlag|删除标识||false|integer(int32)||
|&emsp;&emsp;id|主键||false|string||
|&emsp;&emsp;ip|网络IP||false|string||
|&emsp;&emsp;isStudentSelf|学生本人||false|integer(int32)||
|&emsp;&emsp;operateDatetime|操作时间||false|string(date-time)||
|&emsp;&emsp;operateKind|操作类型||false|string||
|&emsp;&emsp;operateLog|操作日志||false|string||
|&emsp;&emsp;schoolCode|报名高中学校代码||false|string||
|&emsp;&emsp;schoolName|报名高中学校名称||false|string||
|&emsp;&emsp;signUpType|报名类型||false|string||
|&emsp;&emsp;updateBy|更新人||false|string||
|&emsp;&emsp;updateTime|更新日期||false|string(date-time)||
|&emsp;&emsp;winNo|平台端||false|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«string»|
|201|Created||
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|string||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": "",
	"success": true,
	"timestamp": 0
}
```


## 操作历史表-分页列表查询


**接口地址**:`/nnzk/studentLog/operationHistory/list`


**请求方式**:`GET`


**请求数据类型**:`application/x-www-form-urlencoded`


**响应数据类型**:`*/*`


**接口描述**:<p>操作历史表-分页列表查询</p>



**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|account|账号|query|false|string||
|archiveCode|准考证号|query|false|string||
|createBy|创建人|query|false|string||
|createTime|创建日期|query|false|string(date-time)||
|delFlag|删除标识|query|false|integer(int32)||
|id|主键|query|false|string||
|ip|网络IP|query|false|string||
|isStudentSelf|学生本人|query|false|integer(int32)||
|operateDatetime|操作时间|query|false|string(date-time)||
|operateKind|操作类型|query|false|string||
|operateLog|操作日志|query|false|string||
|pageNo|pageNo|query|false|integer(int32)||
|pageSize|pageSize|query|false|integer(int32)||
|schoolCode|报名高中学校代码|query|false|string||
|schoolName|报名高中学校名称|query|false|string||
|signUpType|报名类型|query|false|string||
|updateBy|更新人|query|false|string||
|updateTime|更新日期|query|false|string(date-time)||
|winNo|平台端|query|false|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«IPage«operation_history对象»»|
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|IPage«operation_history对象»|IPage«operation_history对象»|
|&emsp;&emsp;current||integer(int64)||
|&emsp;&emsp;pages||integer(int64)||
|&emsp;&emsp;records||array|operation_history对象|
|&emsp;&emsp;&emsp;&emsp;account|账号|string||
|&emsp;&emsp;&emsp;&emsp;archiveCode|准考证号|string||
|&emsp;&emsp;&emsp;&emsp;createBy|创建人|string||
|&emsp;&emsp;&emsp;&emsp;createTime|创建日期|string||
|&emsp;&emsp;&emsp;&emsp;delFlag|删除标识|integer||
|&emsp;&emsp;&emsp;&emsp;id|主键|string||
|&emsp;&emsp;&emsp;&emsp;ip|网络IP|string||
|&emsp;&emsp;&emsp;&emsp;isStudentSelf|学生本人|integer||
|&emsp;&emsp;&emsp;&emsp;operateDatetime|操作时间|string||
|&emsp;&emsp;&emsp;&emsp;operateKind|操作类型|string||
|&emsp;&emsp;&emsp;&emsp;operateLog|操作日志|string||
|&emsp;&emsp;&emsp;&emsp;schoolCode|报名高中学校代码|string||
|&emsp;&emsp;&emsp;&emsp;schoolName|报名高中学校名称|string||
|&emsp;&emsp;&emsp;&emsp;signUpType|报名类型|string||
|&emsp;&emsp;&emsp;&emsp;updateBy|更新人|string||
|&emsp;&emsp;&emsp;&emsp;updateTime|更新日期|string||
|&emsp;&emsp;&emsp;&emsp;winNo|平台端|string||
|&emsp;&emsp;size||integer(int64)||
|&emsp;&emsp;total||integer(int64)||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": {
		"current": 0,
		"pages": 0,
		"records": [
			{
				"account": "",
				"archiveCode": "",
				"createBy": "",
				"createTime": "",
				"delFlag": 0,
				"id": "",
				"ip": "",
				"isStudentSelf": 0,
				"operateDatetime": "",
				"operateKind": "",
				"operateLog": "",
				"schoolCode": "",
				"schoolName": "",
				"signUpType": "",
				"updateBy": "",
				"updateTime": "",
				"winNo": ""
			}
		],
		"size": 0,
		"total": 0
	},
	"success": true,
	"timestamp": 0
}
```


## 操作历史表-通过id查询


**接口地址**:`/nnzk/studentLog/operationHistory/queryById`


**请求方式**:`GET`


**请求数据类型**:`application/x-www-form-urlencoded`


**响应数据类型**:`*/*`


**接口描述**:<p>操作历史表-通过id查询</p>



**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|id|id|query|true|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«operation_history对象»|
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|operation_history对象|operation_history对象|
|&emsp;&emsp;account|账号|string||
|&emsp;&emsp;archiveCode|准考证号|string||
|&emsp;&emsp;createBy|创建人|string||
|&emsp;&emsp;createTime|创建日期|string(date-time)||
|&emsp;&emsp;delFlag|删除标识|integer(int32)||
|&emsp;&emsp;id|主键|string||
|&emsp;&emsp;ip|网络IP|string||
|&emsp;&emsp;isStudentSelf|学生本人|integer(int32)||
|&emsp;&emsp;operateDatetime|操作时间|string(date-time)||
|&emsp;&emsp;operateKind|操作类型|string||
|&emsp;&emsp;operateLog|操作日志|string||
|&emsp;&emsp;schoolCode|报名高中学校代码|string||
|&emsp;&emsp;schoolName|报名高中学校名称|string||
|&emsp;&emsp;signUpType|报名类型|string||
|&emsp;&emsp;updateBy|更新人|string||
|&emsp;&emsp;updateTime|更新日期|string(date-time)||
|&emsp;&emsp;winNo|平台端|string||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": {
		"account": "",
		"archiveCode": "",
		"createBy": "",
		"createTime": "",
		"delFlag": 0,
		"id": "",
		"ip": "",
		"isStudentSelf": 0,
		"operateDatetime": "",
		"operateKind": "",
		"operateLog": "",
		"schoolCode": "",
		"schoolName": "",
		"signUpType": "",
		"updateBy": "",
		"updateTime": "",
		"winNo": ""
	},
	"success": true,
	"timestamp": 0
}
```


## 操作历史表-学生个人历史列表


**接口地址**:`/nnzk/studentLog/operationHistory/studentList`


**请求方式**:`GET`


**请求数据类型**:`application/x-www-form-urlencoded`


**响应数据类型**:`*/*`


**接口描述**:<p>操作历史表-学生个人历史列表</p>



**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|pageNo|pageNo|query|false|integer(int32)||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«IPage«operation_history对象»»|
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|IPage«operation_history对象»|IPage«operation_history对象»|
|&emsp;&emsp;current||integer(int64)||
|&emsp;&emsp;pages||integer(int64)||
|&emsp;&emsp;records||array|operation_history对象|
|&emsp;&emsp;&emsp;&emsp;account|账号|string||
|&emsp;&emsp;&emsp;&emsp;archiveCode|准考证号|string||
|&emsp;&emsp;&emsp;&emsp;createBy|创建人|string||
|&emsp;&emsp;&emsp;&emsp;createTime|创建日期|string||
|&emsp;&emsp;&emsp;&emsp;delFlag|删除标识|integer||
|&emsp;&emsp;&emsp;&emsp;id|主键|string||
|&emsp;&emsp;&emsp;&emsp;ip|网络IP|string||
|&emsp;&emsp;&emsp;&emsp;isStudentSelf|学生本人|integer||
|&emsp;&emsp;&emsp;&emsp;operateDatetime|操作时间|string||
|&emsp;&emsp;&emsp;&emsp;operateKind|操作类型|string||
|&emsp;&emsp;&emsp;&emsp;operateLog|操作日志|string||
|&emsp;&emsp;&emsp;&emsp;schoolCode|报名高中学校代码|string||
|&emsp;&emsp;&emsp;&emsp;schoolName|报名高中学校名称|string||
|&emsp;&emsp;&emsp;&emsp;signUpType|报名类型|string||
|&emsp;&emsp;&emsp;&emsp;updateBy|更新人|string||
|&emsp;&emsp;&emsp;&emsp;updateTime|更新日期|string||
|&emsp;&emsp;&emsp;&emsp;winNo|平台端|string||
|&emsp;&emsp;size||integer(int64)||
|&emsp;&emsp;total||integer(int64)||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": {
		"current": 0,
		"pages": 0,
		"records": [
			{
				"account": "",
				"archiveCode": "",
				"createBy": "",
				"createTime": "",
				"delFlag": 0,
				"id": "",
				"ip": "",
				"isStudentSelf": 0,
				"operateDatetime": "",
				"operateKind": "",
				"operateLog": "",
				"schoolCode": "",
				"schoolName": "",
				"signUpType": "",
				"updateBy": "",
				"updateTime": "",
				"winNo": ""
			}
		],
		"size": 0,
		"total": 0
	},
	"success": true,
	"timestamp": 0
}
```


# 操作指南视频


## 获取后端视频流


**接口地址**:`/nnzk/video/getVideo`


**请求方式**:`GET`


**请求数据类型**:`application/x-www-form-urlencoded`


**响应数据类型**:`*/*`


**接口描述**:<p>获取后端视频流</p>



**请求参数**:


暂无


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK||
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


暂无


**响应示例**:
```javascript

```


## 上传


**接口地址**:`/nnzk/video/uploadVideo`


**请求方式**:`POST`


**请求数据类型**:`multipart/form-data`


**响应数据类型**:`*/*`


**接口描述**:<p>上传</p>



**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|file|file|body|true|string||
|SavePath|SavePath|query|true|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«string»|
|201|Created||
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|string||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": "",
	"success": true,
	"timestamp": 0
}
```


# 数据字典


## 字典重复校验接口


**接口地址**:`/nnzk/sys/dictItem/dictItemCheck`


**请求方式**:`GET`


**请求数据类型**:`application/x-www-form-urlencoded`


**响应数据类型**:`*/*`


**接口描述**:


**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|createBy||query|false|string||
|createTime||query|false|string(date-time)||
|description||query|false|string||
|dictId||query|false|string||
|id||query|false|string||
|itemText||query|false|string||
|itemValue||query|false|string||
|sortOrder||query|false|integer(int32)||
|status||query|false|integer(int32)||
|updateBy||query|false|string||
|updateTime||query|false|string(date-time)||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«object»|
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|object||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": {},
	"success": true,
	"timestamp": 0
}
```


# 数据源表


## 数据源表-添加


**接口地址**:`/nnzk/drag/onlDragDataSource/add`


**请求方式**:`POST`


**请求数据类型**:`application/json`


**响应数据类型**:`*/*`


**接口描述**:<p>数据源表-添加</p>



**请求示例**:


```javascript
{
  "code": "",
  "connectTimes": 0,
  "createBy": "",
  "createTime": "",
  "dbDriver": "",
  "dbPassword": "",
  "dbType": "",
  "dbUrl": "",
  "dbUsername": "",
  "id": "",
  "name": "",
  "remark": "",
  "reportId": "",
  "type": "",
  "updateBy": "",
  "updateTime": ""
}
```


**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|param0|param0|body|true|OnlDragDataSource|OnlDragDataSource|
|&emsp;&emsp;code|编码||false|string||
|&emsp;&emsp;connectTimes|连接失败次数||false|integer(int32)||
|&emsp;&emsp;createBy|创建人||false|string||
|&emsp;&emsp;createTime|创建日期||false|string(date-time)||
|&emsp;&emsp;dbDriver|驱动类||false|string||
|&emsp;&emsp;dbPassword|密码||false|string||
|&emsp;&emsp;dbType|数据库类型||false|string||
|&emsp;&emsp;dbUrl|数据源地址||false|string||
|&emsp;&emsp;dbUsername|用户名||false|string||
|&emsp;&emsp;id|id||false|string||
|&emsp;&emsp;name|数据源名称||false|string||
|&emsp;&emsp;remark|备注||false|string||
|&emsp;&emsp;reportId|报表_id||false|string||
|&emsp;&emsp;type|类型(report:报表;drag:仪表盘)||false|string||
|&emsp;&emsp;updateBy|更新人||false|string||
|&emsp;&emsp;updateTime|更新日期||false|string(date-time)||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«object»|
|201|Created||
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|object||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": {},
	"success": true,
	"timestamp": 0
}
```


## 数据源表-通过id删除


**接口地址**:`/nnzk/drag/onlDragDataSource/delete`


**请求方式**:`DELETE`


**请求数据类型**:`application/x-www-form-urlencoded`


**响应数据类型**:`*/*`


**接口描述**:<p>数据源表-通过id删除</p>



**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|id|id|query|true|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«object»|
|204|No Content||
|401|Unauthorized||
|403|Forbidden||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|object||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": {},
	"success": true,
	"timestamp": 0
}
```


## 数据源表-批量删除


**接口地址**:`/nnzk/drag/onlDragDataSource/deleteBatch`


**请求方式**:`DELETE`


**请求数据类型**:`application/x-www-form-urlencoded`


**响应数据类型**:`*/*`


**接口描述**:<p>数据源表-批量删除</p>



**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|ids|ids|query|true|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«object»|
|204|No Content||
|401|Unauthorized||
|403|Forbidden||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|object||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": {},
	"success": true,
	"timestamp": 0
}
```


## 数据源表-编辑


**接口地址**:`/nnzk/drag/onlDragDataSource/edit`


**请求方式**:`POST`


**请求数据类型**:`application/json`


**响应数据类型**:`*/*`


**接口描述**:<p>数据源表-编辑</p>



**请求示例**:


```javascript
{
  "code": "",
  "connectTimes": 0,
  "createBy": "",
  "createTime": "",
  "dbDriver": "",
  "dbPassword": "",
  "dbType": "",
  "dbUrl": "",
  "dbUsername": "",
  "id": "",
  "name": "",
  "remark": "",
  "reportId": "",
  "type": "",
  "updateBy": "",
  "updateTime": ""
}
```


**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|param0|param0|body|true|OnlDragDataSource|OnlDragDataSource|
|&emsp;&emsp;code|编码||false|string||
|&emsp;&emsp;connectTimes|连接失败次数||false|integer(int32)||
|&emsp;&emsp;createBy|创建人||false|string||
|&emsp;&emsp;createTime|创建日期||false|string(date-time)||
|&emsp;&emsp;dbDriver|驱动类||false|string||
|&emsp;&emsp;dbPassword|密码||false|string||
|&emsp;&emsp;dbType|数据库类型||false|string||
|&emsp;&emsp;dbUrl|数据源地址||false|string||
|&emsp;&emsp;dbUsername|用户名||false|string||
|&emsp;&emsp;id|id||false|string||
|&emsp;&emsp;name|数据源名称||false|string||
|&emsp;&emsp;remark|备注||false|string||
|&emsp;&emsp;reportId|报表_id||false|string||
|&emsp;&emsp;type|类型(report:报表;drag:仪表盘)||false|string||
|&emsp;&emsp;updateBy|更新人||false|string||
|&emsp;&emsp;updateTime|更新日期||false|string(date-time)||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«object»|
|201|Created||
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|object||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": {},
	"success": true,
	"timestamp": 0
}
```


## 数据源表-编辑


**接口地址**:`/nnzk/drag/onlDragDataSource/edit`


**请求方式**:`PUT`


**请求数据类型**:`application/json`


**响应数据类型**:`*/*`


**接口描述**:<p>数据源表-编辑</p>



**请求示例**:


```javascript
{
  "code": "",
  "connectTimes": 0,
  "createBy": "",
  "createTime": "",
  "dbDriver": "",
  "dbPassword": "",
  "dbType": "",
  "dbUrl": "",
  "dbUsername": "",
  "id": "",
  "name": "",
  "remark": "",
  "reportId": "",
  "type": "",
  "updateBy": "",
  "updateTime": ""
}
```


**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|param0|param0|body|true|OnlDragDataSource|OnlDragDataSource|
|&emsp;&emsp;code|编码||false|string||
|&emsp;&emsp;connectTimes|连接失败次数||false|integer(int32)||
|&emsp;&emsp;createBy|创建人||false|string||
|&emsp;&emsp;createTime|创建日期||false|string(date-time)||
|&emsp;&emsp;dbDriver|驱动类||false|string||
|&emsp;&emsp;dbPassword|密码||false|string||
|&emsp;&emsp;dbType|数据库类型||false|string||
|&emsp;&emsp;dbUrl|数据源地址||false|string||
|&emsp;&emsp;dbUsername|用户名||false|string||
|&emsp;&emsp;id|id||false|string||
|&emsp;&emsp;name|数据源名称||false|string||
|&emsp;&emsp;remark|备注||false|string||
|&emsp;&emsp;reportId|报表_id||false|string||
|&emsp;&emsp;type|类型(report:报表;drag:仪表盘)||false|string||
|&emsp;&emsp;updateBy|更新人||false|string||
|&emsp;&emsp;updateTime|更新日期||false|string(date-time)||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«object»|
|201|Created||
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|object||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": {},
	"success": true,
	"timestamp": 0
}
```


## 数据源表-分页列表查询


**接口地址**:`/nnzk/drag/onlDragDataSource/list`


**请求方式**:`GET`


**请求数据类型**:`application/x-www-form-urlencoded`


**响应数据类型**:`*/*`


**接口描述**:<p>数据源表-分页列表查询</p>



**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|code|编码|query|false|string||
|connectTimes|连接失败次数|query|false|integer(int32)||
|createBy|创建人|query|false|string||
|createTime|创建日期|query|false|string(date-time)||
|dbDriver|驱动类|query|false|string||
|dbPassword|密码|query|false|string||
|dbType|数据库类型|query|false|string||
|dbUrl|数据源地址|query|false|string||
|dbUsername|用户名|query|false|string||
|id|id|query|false|string||
|name|数据源名称|query|false|string||
|pageNo|pageNo|query|false|integer(int32)||
|pageSize|pageSize|query|false|integer(int32)||
|remark|备注|query|false|string||
|reportId|报表_id|query|false|string||
|type|类型(report:报表;drag:仪表盘)|query|false|string||
|updateBy|更新人|query|false|string||
|updateTime|更新日期|query|false|string(date-time)||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«object»|
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|object||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": {},
	"success": true,
	"timestamp": 0
}
```


## 数据源表-通过id查询


**接口地址**:`/nnzk/drag/onlDragDataSource/queryById`


**请求方式**:`GET`


**请求数据类型**:`application/x-www-form-urlencoded`


**响应数据类型**:`*/*`


**接口描述**:<p>数据源表-通过id查询</p>



**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|id|id|query|true|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«object»|
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|object||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": {},
	"success": true,
	"timestamp": 0
}
```


# 数据集参数表


## 数据集参数表-添加


**接口地址**:`/nnzk/drag/onlDragDatasetParam/add`


**请求方式**:`POST`


**请求数据类型**:`application/json`


**响应数据类型**:`*/*`


**接口描述**:<p>数据集参数表-添加</p>



**请求示例**:


```javascript
{
  "createBy": "",
  "createTime": "",
  "dictCode": "",
  "headId": "",
  "id": "",
  "izSearch": 0,
  "orderNum": 0,
  "paramName": "",
  "paramTxt": "",
  "paramValue": "",
  "searchMode": 0,
  "updateBy": "",
  "updateTime": "",
  "widgetType": ""
}
```


**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|param0|数据集参数表|body|true|onl_drag_dataset_param对象|onl_drag_dataset_param对象|
|&emsp;&emsp;createBy|创建人登录名称||false|string||
|&emsp;&emsp;createTime|创建日期||false|string(date-time)||
|&emsp;&emsp;dictCode|字典||false|string||
|&emsp;&emsp;headId|动态报表ID||false|string||
|&emsp;&emsp;id|id||false|string||
|&emsp;&emsp;izSearch|查询标识0否1是 默认0||false|integer(int32)||
|&emsp;&emsp;orderNum|排序||false|integer(int32)||
|&emsp;&emsp;paramName|参数字段||false|string||
|&emsp;&emsp;paramTxt|参数文本||false|string||
|&emsp;&emsp;paramValue|参数默认值||false|string||
|&emsp;&emsp;searchMode|查询模式1简单2范围||false|integer(int32)||
|&emsp;&emsp;updateBy|更新人登录名称||false|string||
|&emsp;&emsp;updateTime|更新日期||false|string(date-time)||
|&emsp;&emsp;widgetType|查询控件类型||false|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«object»|
|201|Created||
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|object||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": {},
	"success": true,
	"timestamp": 0
}
```


## 数据集参数表-通过id删除


**接口地址**:`/nnzk/drag/onlDragDatasetParam/delete`


**请求方式**:`DELETE`


**请求数据类型**:`application/x-www-form-urlencoded`


**响应数据类型**:`*/*`


**接口描述**:<p>数据集参数表-通过id删除</p>



**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|id|id|query|true|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«object»|
|204|No Content||
|401|Unauthorized||
|403|Forbidden||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|object||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": {},
	"success": true,
	"timestamp": 0
}
```


## 数据集参数表-批量删除


**接口地址**:`/nnzk/drag/onlDragDatasetParam/deleteBatch`


**请求方式**:`DELETE`


**请求数据类型**:`application/x-www-form-urlencoded`


**响应数据类型**:`*/*`


**接口描述**:<p>数据集参数表-批量删除</p>



**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|ids|ids|query|true|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«object»|
|204|No Content||
|401|Unauthorized||
|403|Forbidden||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|object||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": {},
	"success": true,
	"timestamp": 0
}
```


## 数据集参数表-编辑


**接口地址**:`/nnzk/drag/onlDragDatasetParam/edit`


**请求方式**:`POST`


**请求数据类型**:`application/json`


**响应数据类型**:`*/*`


**接口描述**:<p>数据集参数表-编辑</p>



**请求示例**:


```javascript
{
  "createBy": "",
  "createTime": "",
  "dictCode": "",
  "headId": "",
  "id": "",
  "izSearch": 0,
  "orderNum": 0,
  "paramName": "",
  "paramTxt": "",
  "paramValue": "",
  "searchMode": 0,
  "updateBy": "",
  "updateTime": "",
  "widgetType": ""
}
```


**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|param0|数据集参数表|body|true|onl_drag_dataset_param对象|onl_drag_dataset_param对象|
|&emsp;&emsp;createBy|创建人登录名称||false|string||
|&emsp;&emsp;createTime|创建日期||false|string(date-time)||
|&emsp;&emsp;dictCode|字典||false|string||
|&emsp;&emsp;headId|动态报表ID||false|string||
|&emsp;&emsp;id|id||false|string||
|&emsp;&emsp;izSearch|查询标识0否1是 默认0||false|integer(int32)||
|&emsp;&emsp;orderNum|排序||false|integer(int32)||
|&emsp;&emsp;paramName|参数字段||false|string||
|&emsp;&emsp;paramTxt|参数文本||false|string||
|&emsp;&emsp;paramValue|参数默认值||false|string||
|&emsp;&emsp;searchMode|查询模式1简单2范围||false|integer(int32)||
|&emsp;&emsp;updateBy|更新人登录名称||false|string||
|&emsp;&emsp;updateTime|更新日期||false|string(date-time)||
|&emsp;&emsp;widgetType|查询控件类型||false|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«object»|
|201|Created||
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|object||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": {},
	"success": true,
	"timestamp": 0
}
```


## 数据集参数表-编辑


**接口地址**:`/nnzk/drag/onlDragDatasetParam/edit`


**请求方式**:`PUT`


**请求数据类型**:`application/json`


**响应数据类型**:`*/*`


**接口描述**:<p>数据集参数表-编辑</p>



**请求示例**:


```javascript
{
  "createBy": "",
  "createTime": "",
  "dictCode": "",
  "headId": "",
  "id": "",
  "izSearch": 0,
  "orderNum": 0,
  "paramName": "",
  "paramTxt": "",
  "paramValue": "",
  "searchMode": 0,
  "updateBy": "",
  "updateTime": "",
  "widgetType": ""
}
```


**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|param0|数据集参数表|body|true|onl_drag_dataset_param对象|onl_drag_dataset_param对象|
|&emsp;&emsp;createBy|创建人登录名称||false|string||
|&emsp;&emsp;createTime|创建日期||false|string(date-time)||
|&emsp;&emsp;dictCode|字典||false|string||
|&emsp;&emsp;headId|动态报表ID||false|string||
|&emsp;&emsp;id|id||false|string||
|&emsp;&emsp;izSearch|查询标识0否1是 默认0||false|integer(int32)||
|&emsp;&emsp;orderNum|排序||false|integer(int32)||
|&emsp;&emsp;paramName|参数字段||false|string||
|&emsp;&emsp;paramTxt|参数文本||false|string||
|&emsp;&emsp;paramValue|参数默认值||false|string||
|&emsp;&emsp;searchMode|查询模式1简单2范围||false|integer(int32)||
|&emsp;&emsp;updateBy|更新人登录名称||false|string||
|&emsp;&emsp;updateTime|更新日期||false|string(date-time)||
|&emsp;&emsp;widgetType|查询控件类型||false|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«object»|
|201|Created||
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|object||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": {},
	"success": true,
	"timestamp": 0
}
```


## 数据集参数表-分页列表查询


**接口地址**:`/nnzk/drag/onlDragDatasetParam/list`


**请求方式**:`GET`


**请求数据类型**:`application/x-www-form-urlencoded`


**响应数据类型**:`*/*`


**接口描述**:<p>数据集参数表-分页列表查询</p>



**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|createBy|创建人登录名称|query|false|string||
|createTime|创建日期|query|false|string(date-time)||
|dictCode|字典|query|false|string||
|headId|动态报表ID|query|false|string||
|id|id|query|false|string||
|izSearch|查询标识0否1是 默认0|query|false|integer(int32)||
|orderNum|排序|query|false|integer(int32)||
|pageNo|pageNo|query|false|integer(int32)||
|pageSize|pageSize|query|false|integer(int32)||
|paramName|参数字段|query|false|string||
|paramTxt|参数文本|query|false|string||
|paramValue|参数默认值|query|false|string||
|searchMode|查询模式1简单2范围|query|false|integer(int32)||
|updateBy|更新人登录名称|query|false|string||
|updateTime|更新日期|query|false|string(date-time)||
|widgetType|查询控件类型|query|false|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«object»|
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|object||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": {},
	"success": true,
	"timestamp": 0
}
```


## 数据集参数表-通过id查询


**接口地址**:`/nnzk/drag/onlDragDatasetParam/queryById`


**请求方式**:`GET`


**请求数据类型**:`application/x-www-form-urlencoded`


**响应数据类型**:`*/*`


**接口描述**:<p>数据集参数表-通过id查询</p>



**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|id|id|query|true|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«object»|
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|object||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": {},
	"success": true,
	"timestamp": 0
}
```


# 时段信息表


## 时段信息表-添加


**接口地址**:`/nnzk/rule/phaseInfo/add`


**请求方式**:`POST`


**请求数据类型**:`application/json`


**响应数据类型**:`*/*`


**接口描述**:<p>时段信息表-添加</p>



**请求示例**:


```javascript
{
  "beginDate": "",
  "beginTime": "",
  "createBy": "",
  "createTime": "",
  "delFlag": 0,
  "endTime": "",
  "id": "",
  "isCurrentPhase": 0,
  "isMatPhase": 0,
  "phaseName": "",
  "remark": "",
  "stopSignupTime": "",
  "updateBy": "",
  "updateTime": ""
}
```


**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|phaseInfo|时段信息表|body|true|phase_info对象|phase_info对象|
|&emsp;&emsp;beginDate|开始日期||false|string(date-time)||
|&emsp;&emsp;beginTime|开始时间||false|string||
|&emsp;&emsp;createBy|创建人||false|string||
|&emsp;&emsp;createTime|创建日期||false|string(date-time)||
|&emsp;&emsp;delFlag|删除标识||false|integer(int32)||
|&emsp;&emsp;endTime|结束时间||false|string||
|&emsp;&emsp;id|主键||false|string||
|&emsp;&emsp;isCurrentPhase|当前时段||false|integer(int32)||
|&emsp;&emsp;isMatPhase|录取时段||false|integer(int32)||
|&emsp;&emsp;phaseName|时段名称||false|string||
|&emsp;&emsp;remark|说明||false|string||
|&emsp;&emsp;stopSignupTime|停止报名时间||false|string(date-time)||
|&emsp;&emsp;updateBy|更新人||false|string||
|&emsp;&emsp;updateTime|更新日期||false|string(date-time)||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«string»|
|201|Created||
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|string||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": "",
	"success": true,
	"timestamp": 0
}
```


## 时段信息表-通过id删除


**接口地址**:`/nnzk/rule/phaseInfo/delete`


**请求方式**:`DELETE`


**请求数据类型**:`application/x-www-form-urlencoded`


**响应数据类型**:`*/*`


**接口描述**:<p>时段信息表-通过id删除</p>



**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|id|id|query|true|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«string»|
|204|No Content||
|401|Unauthorized||
|403|Forbidden||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|string||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": "",
	"success": true,
	"timestamp": 0
}
```


## 时段信息表-批量删除


**接口地址**:`/nnzk/rule/phaseInfo/deleteBatch`


**请求方式**:`DELETE`


**请求数据类型**:`application/x-www-form-urlencoded`


**响应数据类型**:`*/*`


**接口描述**:<p>时段信息表-批量删除</p>



**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|ids|ids|query|true|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«string»|
|204|No Content||
|401|Unauthorized||
|403|Forbidden||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|string||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": "",
	"success": true,
	"timestamp": 0
}
```


## 时段信息表-编辑


**接口地址**:`/nnzk/rule/phaseInfo/edit`


**请求方式**:`POST`


**请求数据类型**:`application/json`


**响应数据类型**:`*/*`


**接口描述**:<p>时段信息表-编辑</p>



**请求示例**:


```javascript
{
  "beginDate": "",
  "beginTime": "",
  "createBy": "",
  "createTime": "",
  "delFlag": 0,
  "endTime": "",
  "id": "",
  "isCurrentPhase": 0,
  "isMatPhase": 0,
  "phaseName": "",
  "remark": "",
  "stopSignupTime": "",
  "updateBy": "",
  "updateTime": ""
}
```


**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|phaseInfo|时段信息表|body|true|phase_info对象|phase_info对象|
|&emsp;&emsp;beginDate|开始日期||false|string(date-time)||
|&emsp;&emsp;beginTime|开始时间||false|string||
|&emsp;&emsp;createBy|创建人||false|string||
|&emsp;&emsp;createTime|创建日期||false|string(date-time)||
|&emsp;&emsp;delFlag|删除标识||false|integer(int32)||
|&emsp;&emsp;endTime|结束时间||false|string||
|&emsp;&emsp;id|主键||false|string||
|&emsp;&emsp;isCurrentPhase|当前时段||false|integer(int32)||
|&emsp;&emsp;isMatPhase|录取时段||false|integer(int32)||
|&emsp;&emsp;phaseName|时段名称||false|string||
|&emsp;&emsp;remark|说明||false|string||
|&emsp;&emsp;stopSignupTime|停止报名时间||false|string(date-time)||
|&emsp;&emsp;updateBy|更新人||false|string||
|&emsp;&emsp;updateTime|更新日期||false|string(date-time)||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«string»|
|201|Created||
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|string||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": "",
	"success": true,
	"timestamp": 0
}
```


## 时段信息表-编辑


**接口地址**:`/nnzk/rule/phaseInfo/edit`


**请求方式**:`PUT`


**请求数据类型**:`application/json`


**响应数据类型**:`*/*`


**接口描述**:<p>时段信息表-编辑</p>



**请求示例**:


```javascript
{
  "beginDate": "",
  "beginTime": "",
  "createBy": "",
  "createTime": "",
  "delFlag": 0,
  "endTime": "",
  "id": "",
  "isCurrentPhase": 0,
  "isMatPhase": 0,
  "phaseName": "",
  "remark": "",
  "stopSignupTime": "",
  "updateBy": "",
  "updateTime": ""
}
```


**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|phaseInfo|时段信息表|body|true|phase_info对象|phase_info对象|
|&emsp;&emsp;beginDate|开始日期||false|string(date-time)||
|&emsp;&emsp;beginTime|开始时间||false|string||
|&emsp;&emsp;createBy|创建人||false|string||
|&emsp;&emsp;createTime|创建日期||false|string(date-time)||
|&emsp;&emsp;delFlag|删除标识||false|integer(int32)||
|&emsp;&emsp;endTime|结束时间||false|string||
|&emsp;&emsp;id|主键||false|string||
|&emsp;&emsp;isCurrentPhase|当前时段||false|integer(int32)||
|&emsp;&emsp;isMatPhase|录取时段||false|integer(int32)||
|&emsp;&emsp;phaseName|时段名称||false|string||
|&emsp;&emsp;remark|说明||false|string||
|&emsp;&emsp;stopSignupTime|停止报名时间||false|string(date-time)||
|&emsp;&emsp;updateBy|更新人||false|string||
|&emsp;&emsp;updateTime|更新日期||false|string(date-time)||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«string»|
|201|Created||
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|string||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": "",
	"success": true,
	"timestamp": 0
}
```


## 时段信息表-获取剩余时间戳


**接口地址**:`/nnzk/rule/phaseInfo/getTimestamp`


**请求方式**:`GET`


**请求数据类型**:`application/x-www-form-urlencoded`


**响应数据类型**:`*/*`


**接口描述**:<p>时段信息表-获取剩余时间戳</p>



**请求参数**:


暂无


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«PhaseInfoResultVO»|
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|PhaseInfoResultVO|PhaseInfoResultVO|
|&emsp;&emsp;message|消息描述|string||
|&emsp;&emsp;result|报名是否开放|boolean||
|&emsp;&emsp;value|剩余时间（秒数）|integer(int64)||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": {
		"message": "",
		"result": true,
		"value": 0
	},
	"success": true,
	"timestamp": 0
}
```


## 时段信息表-分页列表查询


**接口地址**:`/nnzk/rule/phaseInfo/list`


**请求方式**:`GET`


**请求数据类型**:`application/x-www-form-urlencoded`


**响应数据类型**:`*/*`


**接口描述**:<p>时段信息表-分页列表查询</p>



**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|beginDate|开始日期|query|true|string(date-time)||
|beginTime|开始时间|query|true|string||
|endTime|结束时间|query|true|string||
|isCurrentPhase|当前时段|query|true|integer(int32)||
|isMatPhase|录取时段|query|true|integer(int32)||
|phaseName|时段名称|query|true|string||
|stopSignupTime|停止报名时间|query|true|string(date-time)||
|createBy|创建人|query|false|string||
|createTime|创建日期|query|false|string(date-time)||
|delFlag|删除标识|query|false|integer(int32)||
|id|主键|query|false|string||
|pageNo|pageNo|query|false|integer(int32)||
|pageSize|pageSize|query|false|integer(int32)||
|remark|说明|query|false|string||
|updateBy|更新人|query|false|string||
|updateTime|更新日期|query|false|string(date-time)||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«IPage«phase_info对象»»|
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|IPage«phase_info对象»|IPage«phase_info对象»|
|&emsp;&emsp;current||integer(int64)||
|&emsp;&emsp;pages||integer(int64)||
|&emsp;&emsp;records||array|phase_info对象|
|&emsp;&emsp;&emsp;&emsp;beginDate|开始日期|string||
|&emsp;&emsp;&emsp;&emsp;beginTime|开始时间|string||
|&emsp;&emsp;&emsp;&emsp;createBy|创建人|string||
|&emsp;&emsp;&emsp;&emsp;createTime|创建日期|string||
|&emsp;&emsp;&emsp;&emsp;delFlag|删除标识|integer||
|&emsp;&emsp;&emsp;&emsp;endTime|结束时间|string||
|&emsp;&emsp;&emsp;&emsp;id|主键|string||
|&emsp;&emsp;&emsp;&emsp;isCurrentPhase|当前时段|integer||
|&emsp;&emsp;&emsp;&emsp;isMatPhase|录取时段|integer||
|&emsp;&emsp;&emsp;&emsp;phaseName|时段名称|string||
|&emsp;&emsp;&emsp;&emsp;remark|说明|string||
|&emsp;&emsp;&emsp;&emsp;stopSignupTime|停止报名时间|string||
|&emsp;&emsp;&emsp;&emsp;updateBy|更新人|string||
|&emsp;&emsp;&emsp;&emsp;updateTime|更新日期|string||
|&emsp;&emsp;size||integer(int64)||
|&emsp;&emsp;total||integer(int64)||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": {
		"current": 0,
		"pages": 0,
		"records": [
			{
				"beginDate": "",
				"beginTime": "",
				"createBy": "",
				"createTime": "",
				"delFlag": 0,
				"endTime": "",
				"id": "",
				"isCurrentPhase": 0,
				"isMatPhase": 0,
				"phaseName": "",
				"remark": "",
				"stopSignupTime": "",
				"updateBy": "",
				"updateTime": ""
			}
		],
		"size": 0,
		"total": 0
	},
	"success": true,
	"timestamp": 0
}
```


## 时段信息表-通过id查询


**接口地址**:`/nnzk/rule/phaseInfo/queryById`


**请求方式**:`GET`


**请求数据类型**:`application/x-www-form-urlencoded`


**响应数据类型**:`*/*`


**接口描述**:<p>时段信息表-通过id查询</p>



**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|id|id|query|true|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«phase_info对象»|
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|phase_info对象|phase_info对象|
|&emsp;&emsp;beginDate|开始日期|string(date-time)||
|&emsp;&emsp;beginTime|开始时间|string||
|&emsp;&emsp;createBy|创建人|string||
|&emsp;&emsp;createTime|创建日期|string(date-time)||
|&emsp;&emsp;delFlag|删除标识|integer(int32)||
|&emsp;&emsp;endTime|结束时间|string||
|&emsp;&emsp;id|主键|string||
|&emsp;&emsp;isCurrentPhase|当前时段|integer(int32)||
|&emsp;&emsp;isMatPhase|录取时段|integer(int32)||
|&emsp;&emsp;phaseName|时段名称|string||
|&emsp;&emsp;remark|说明|string||
|&emsp;&emsp;stopSignupTime|停止报名时间|string(date-time)||
|&emsp;&emsp;updateBy|更新人|string||
|&emsp;&emsp;updateTime|更新日期|string(date-time)||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": {
		"beginDate": "",
		"beginTime": "",
		"createBy": "",
		"createTime": "",
		"delFlag": 0,
		"endTime": "",
		"id": "",
		"isCurrentPhase": 0,
		"isMatPhase": 0,
		"phaseName": "",
		"remark": "",
		"stopSignupTime": "",
		"updateBy": "",
		"updateTime": ""
	},
	"success": true,
	"timestamp": 0
}
```


# 普通高中报名


## 常规录取-定向核查


**接口地址**:`/nnzk/matriculate/ordinary/dirCheck`


**请求方式**:`GET`


**请求数据类型**:`application/x-www-form-urlencoded`


**响应数据类型**:`*/*`


**接口描述**:<p>常规录取-定向核查</p>



**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|finishSchoolCode|finishSchoolCode|query|true|string||
|highSchoolCode|highSchoolCode|query|true|string||
|isShowGuide|isShowGuide|query|true|integer(int32)||
|isShowInst|isShowInst|query|true|integer(int32)||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«DirCheckResultVO»|
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|DirCheckResultVO|DirCheckResultVO|
|&emsp;&emsp;currentMgroupDirPlanNum|当前初中组定向配额数|integer(int32)||
|&emsp;&emsp;dirCheckLevelList|高中组学校定向线列表|array|DirCheckLevelVO|
|&emsp;&emsp;&emsp;&emsp;alterLevel|补录线|string||
|&emsp;&emsp;&emsp;&emsp;dirLevel|定向线|string||
|&emsp;&emsp;&emsp;&emsp;schoolName|高中学校|string||
|&emsp;&emsp;dirCheckList|定向核查信息列表|array|DirCheckVO|
|&emsp;&emsp;&emsp;&emsp;archiveCode|准考证号|string||
|&emsp;&emsp;&emsp;&emsp;calculateType|计算类型|string||
|&emsp;&emsp;&emsp;&emsp;chineseLevel|语文|string||
|&emsp;&emsp;&emsp;&emsp;chymistLevel|化学|string||
|&emsp;&emsp;&emsp;&emsp;className|班级|string||
|&emsp;&emsp;&emsp;&emsp;combinedScore|组合分|string||
|&emsp;&emsp;&emsp;&emsp;directionalReason|未入围定向原因|string||
|&emsp;&emsp;&emsp;&emsp;englishLevel|英语|string||
|&emsp;&emsp;&emsp;&emsp;finishSchoolCode|毕业学校代码|string||
|&emsp;&emsp;&emsp;&emsp;finishSchoolName|毕业学校名称|string||
|&emsp;&emsp;&emsp;&emsp;isAreaStudent|是否地段生|integer||
|&emsp;&emsp;&emsp;&emsp;isMilitary|是否优抚|integer||
|&emsp;&emsp;&emsp;&emsp;mathLevel|数学|string||
|&emsp;&emsp;&emsp;&emsp;matriculateStatus|录取状态|integer||
|&emsp;&emsp;&emsp;&emsp;matriculateType|录取类型|string||
|&emsp;&emsp;&emsp;&emsp;orderCode|成绩排序码|string||
|&emsp;&emsp;&emsp;&emsp;physicsLevel|物理|string||
|&emsp;&emsp;&emsp;&emsp;politicsLevel|政史|string||
|&emsp;&emsp;&emsp;&emsp;serialNum|序号|integer||
|&emsp;&emsp;&emsp;&emsp;shortName|报考学校|string||
|&emsp;&emsp;&emsp;&emsp;signUpType|报名类型|string||
|&emsp;&emsp;&emsp;&emsp;studentName|学生姓名|string||
|&emsp;&emsp;&emsp;&emsp;sumScore|总分|string||
|&emsp;&emsp;realDirAboveNum|定向实际入围数|integer(int32)||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": {
		"currentMgroupDirPlanNum": 0,
		"dirCheckLevelList": [
			{
				"alterLevel": "",
				"dirLevel": "",
				"schoolName": ""
			}
		],
		"dirCheckList": [
			{
				"archiveCode": "",
				"calculateType": "",
				"chineseLevel": "",
				"chymistLevel": "",
				"className": "",
				"combinedScore": "",
				"directionalReason": "",
				"englishLevel": "",
				"finishSchoolCode": "",
				"finishSchoolName": "",
				"isAreaStudent": 0,
				"isMilitary": 0,
				"mathLevel": "",
				"matriculateStatus": 0,
				"matriculateType": "",
				"orderCode": "",
				"physicsLevel": "",
				"politicsLevel": "",
				"serialNum": 0,
				"shortName": "",
				"signUpType": "",
				"studentName": "",
				"sumScore": ""
			}
		],
		"realDirAboveNum": 0
	},
	"success": true,
	"timestamp": 0
}
```


## 常规录取-录取


**接口地址**:`/nnzk/matriculate/ordinary/doMatriculate`


**请求方式**:`POST`


**请求数据类型**:`application/json`


**响应数据类型**:`*/*`


**接口描述**:<p>常规录取-录取</p>



**请求示例**:


```javascript
{
  "archiveCodes": [],
  "matriculateType": ""
}
```


**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|input|input|body|true|OrdinaryMatAndUnMatDTO|OrdinaryMatAndUnMatDTO|
|&emsp;&emsp;archiveCodes|准考证号数组||false|array|string|
|&emsp;&emsp;matriculateType|录取类型||false|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«int»|
|201|Created||
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|integer(int32)|integer(int32)|
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": 0,
	"success": true,
	"timestamp": 0
}
```


## 常规录取-列表


**接口地址**:`/nnzk/matriculate/ordinary/list`


**请求方式**:`GET`


**请求数据类型**:`application/x-www-form-urlencoded`


**响应数据类型**:`*/*`


**接口描述**:<p>常规录取-列表</p>



**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|isOnlyShowMatriculated|仅显示已录取|query|true|boolean||
|isOnlyShowOnline|仅显示上线名单|query|true|boolean||
|isRealTimeData|实时数据|query|true|boolean||
|signUpType|报考类型|query|true|string||
|highSchoolCode|录取学校|query|false|string||
|isCalculateDirection|计算定向使用名额|query|false|boolean||
|matEndTime|录取时间|query|false|string(date-time)||
|matStartTime|录取时间|query|false|string(date-time)||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«List«OrdinaryMatriculateList»»|
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|array|OrdinaryMatriculateList|
|&emsp;&emsp;archiveCode|准考证号|string||
|&emsp;&emsp;calculateType|运算类型|string||
|&emsp;&emsp;chineseLevel|语文|string||
|&emsp;&emsp;chymistLevel|化学|string||
|&emsp;&emsp;combinedScore|组合分|string||
|&emsp;&emsp;createTime|创建时间|string||
|&emsp;&emsp;diathesis|综合素质|string||
|&emsp;&emsp;dirNum|已用名额|integer(int32)||
|&emsp;&emsp;dirPlan|组配额数|integer(int32)||
|&emsp;&emsp;directionalReason|定向未入围原因|string||
|&emsp;&emsp;englishLevel|英语|string||
|&emsp;&emsp;experiment|实验|string||
|&emsp;&emsp;fillTime|填报时间|string||
|&emsp;&emsp;finishSchoolCode|毕业学校|string||
|&emsp;&emsp;highSchoolCode|高中学校代码|string||
|&emsp;&emsp;id|报名记录id|string||
|&emsp;&emsp;isAreaStudent|是否地段生|string||
|&emsp;&emsp;mathLevel|数学|string||
|&emsp;&emsp;matriculateStatus|录取状态|integer(int32)||
|&emsp;&emsp;matriculateTime|录取时间|string||
|&emsp;&emsp;matriculateType|录取类型|string||
|&emsp;&emsp;operator|操作人|string||
|&emsp;&emsp;physicalEduLevel|体育|string||
|&emsp;&emsp;physicsLevel|物理|string||
|&emsp;&emsp;politicsLevel|政史|string||
|&emsp;&emsp;runtime|运算时间|string||
|&emsp;&emsp;sc||string||
|&emsp;&emsp;sex|性别|string||
|&emsp;&emsp;signUpType|报考类型|string||
|&emsp;&emsp;sn||string||
|&emsp;&emsp;studentName|学生姓名|string||
|&emsp;&emsp;sumScore|总分|string||
|&emsp;&emsp;winNo|报名号|string||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": [
		{
			"archiveCode": "",
			"calculateType": "",
			"chineseLevel": "",
			"chymistLevel": "",
			"combinedScore": "",
			"createTime": "",
			"diathesis": "",
			"dirNum": 0,
			"dirPlan": 0,
			"directionalReason": "",
			"englishLevel": "",
			"experiment": "",
			"fillTime": "",
			"finishSchoolCode": "",
			"highSchoolCode": "",
			"id": "",
			"isAreaStudent": "",
			"mathLevel": "",
			"matriculateStatus": 0,
			"matriculateTime": "",
			"matriculateType": "",
			"operator": "",
			"physicalEduLevel": "",
			"physicsLevel": "",
			"politicsLevel": "",
			"runtime": "",
			"sc": "",
			"sex": "",
			"signUpType": "",
			"sn": "",
			"studentName": "",
			"sumScore": "",
			"winNo": ""
		}
	],
	"success": true,
	"timestamp": 0
}
```


## 常规录取-录取(军属)


**接口地址**:`/nnzk/matriculate/ordinary/matMilitary`


**请求方式**:`POST`


**请求数据类型**:`application/json`


**响应数据类型**:`*/*`


**接口描述**:<p>常规录取-录取(军属)</p>



**请求示例**:


```javascript
{
  "archiveCodes": [],
  "matriculateType": ""
}
```


**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|input|input|body|true|OrdinaryMatAndUnMatDTO|OrdinaryMatAndUnMatDTO|
|&emsp;&emsp;archiveCodes|准考证号数组||false|array|string|
|&emsp;&emsp;matriculateType|录取类型||false|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«int»|
|201|Created||
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|integer(int32)|integer(int32)|
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": 0,
	"success": true,
	"timestamp": 0
}
```


## 常规录取-打印通知数据


**接口地址**:`/nnzk/matriculate/ordinary/print`


**请求方式**:`GET`


**请求数据类型**:`application/x-www-form-urlencoded`


**响应数据类型**:`*/*`


**接口描述**:<p>常规录取-打印通知数据</p>



**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|ddlPrivilegeClass|特招班类型（国际班、民族班、外地生班。。）|query|false|string||
|highSchoolCode|录取学校代码|query|false|string||
|matBeginTime|录取时间范围（开始）|query|false|string(date-time)||
|matEndTime|录取时间（结束）|query|false|string(date-time)||
|matType|录取类型|query|false|string||
|selectedArchiveCode|选择打印的单个准考证号|query|false|string||
|selectedArchiveCodeList|选择打印的准考证号数组|query|false|array|string|


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|OrdMatAndPriRegPrintOutputDTO|
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|count|总条数|integer(int32)|integer(int32)|
|data|学生列表|array|OrdMatAndPriRegPrintDTO|
|&emsp;&emsp;archiveCode|准考证号|string||
|&emsp;&emsp;chineseLevel|语文|string||
|&emsp;&emsp;chymistLevel|化学|string||
|&emsp;&emsp;diathesis|综合素质|string||
|&emsp;&emsp;englishLevel|英语|string||
|&emsp;&emsp;experiment|实验|string||
|&emsp;&emsp;finishSchoolName|毕业学校|string||
|&emsp;&emsp;highSchoolName|录取学校|string||
|&emsp;&emsp;mathLevel|数学|string||
|&emsp;&emsp;matriculateType|录取类型|string||
|&emsp;&emsp;physicsLevel|物理|string||
|&emsp;&emsp;politicsLevel|政史|string||
|&emsp;&emsp;serialNum|序号|integer(int64)||
|&emsp;&emsp;sex|性别|string||
|&emsp;&emsp;studentName|学生姓名|string||
|&emsp;&emsp;sumScore|总分|string||
|total|总页数|integer(int32)|integer(int32)|


**响应示例**:
```javascript
{
	"count": 0,
	"data": [
		{
			"archiveCode": "",
			"chineseLevel": "",
			"chymistLevel": "",
			"diathesis": "",
			"englishLevel": "",
			"experiment": "",
			"finishSchoolName": "",
			"highSchoolName": "",
			"mathLevel": "",
			"matriculateType": "",
			"physicsLevel": "",
			"politicsLevel": "",
			"serialNum": 0,
			"sex": "",
			"studentName": "",
			"sumScore": ""
		}
	],
	"total": 0
}
```


## 常规录取-打印发榜数据


**接口地址**:`/nnzk/matriculate/ordinary/printList`


**请求方式**:`GET`


**请求数据类型**:`application/x-www-form-urlencoded`


**响应数据类型**:`*/*`


**接口描述**:<p>常规录取-打印发榜数据</p>



**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|ddlPrivilegeClass|特招班类型（国际班、民族班、外地生班。。）|query|false|string||
|highSchoolCode|录取学校代码|query|false|string||
|matBeginTime|录取时间范围（开始）|query|false|string(date-time)||
|matEndTime|录取时间（结束）|query|false|string(date-time)||
|matType|录取类型|query|false|string||
|selectedArchiveCode|选择打印的单个准考证号|query|false|string||
|selectedArchiveCodeList|选择打印的准考证号数组|query|false|array|string|


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|OrdMatAndPriRegPrintOutputDTO|
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|count|总条数|integer(int32)|integer(int32)|
|data|学生列表|array|OrdMatAndPriRegPrintDTO|
|&emsp;&emsp;archiveCode|准考证号|string||
|&emsp;&emsp;chineseLevel|语文|string||
|&emsp;&emsp;chymistLevel|化学|string||
|&emsp;&emsp;diathesis|综合素质|string||
|&emsp;&emsp;englishLevel|英语|string||
|&emsp;&emsp;experiment|实验|string||
|&emsp;&emsp;finishSchoolName|毕业学校|string||
|&emsp;&emsp;highSchoolName|录取学校|string||
|&emsp;&emsp;mathLevel|数学|string||
|&emsp;&emsp;matriculateType|录取类型|string||
|&emsp;&emsp;physicsLevel|物理|string||
|&emsp;&emsp;politicsLevel|政史|string||
|&emsp;&emsp;serialNum|序号|integer(int64)||
|&emsp;&emsp;sex|性别|string||
|&emsp;&emsp;studentName|学生姓名|string||
|&emsp;&emsp;sumScore|总分|string||
|total|总页数|integer(int32)|integer(int32)|


**响应示例**:
```javascript
{
	"count": 0,
	"data": [
		{
			"archiveCode": "",
			"chineseLevel": "",
			"chymistLevel": "",
			"diathesis": "",
			"englishLevel": "",
			"experiment": "",
			"finishSchoolName": "",
			"highSchoolName": "",
			"mathLevel": "",
			"matriculateType": "",
			"physicsLevel": "",
			"politicsLevel": "",
			"serialNum": 0,
			"sex": "",
			"studentName": "",
			"sumScore": ""
		}
	],
	"total": 0
}
```


## 常规录取-学校列表


**接口地址**:`/nnzk/matriculate/ordinary/schoolList`


**请求方式**:`GET`


**请求数据类型**:`application/x-www-form-urlencoded`


**响应数据类型**:`*/*`


**接口描述**:<p>常规录取-学校列表</p>



**请求参数**:


暂无


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«List«HighSchoolRuleDTO»»|
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|array|HighSchoolRuleDTO|
|&emsp;&emsp;directionalPlanNum||integer(int32)||
|&emsp;&emsp;guidePlanNum||integer(int32)||
|&emsp;&emsp;instructionPlanNum||integer(int32)||
|&emsp;&emsp;printName||string||
|&emsp;&emsp;schoolCode||string||
|&emsp;&emsp;schoolName||string||
|&emsp;&emsp;schoolType||string||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": [
		{
			"directionalPlanNum": 0,
			"guidePlanNum": 0,
			"instructionPlanNum": 0,
			"printName": "",
			"schoolCode": "",
			"schoolName": "",
			"schoolType": ""
		}
	],
	"success": true,
	"timestamp": 0
}
```


## 常规录取-学校统计数据


**接口地址**:`/nnzk/matriculate/ordinary/schoolStatistics`


**请求方式**:`GET`


**请求数据类型**:`application/x-www-form-urlencoded`


**响应数据类型**:`*/*`


**接口描述**:<p>常规录取-学校统计数据</p>



**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|schoolCode|schoolCode|query|true|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«school_statistics_data对象»|
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|school_statistics_data对象|school_statistics_data对象|
|&emsp;&emsp;aboveAlterLevel|补录入围人数|integer(int32)||
|&emsp;&emsp;aboveDirLevel|定向入围人数|integer(int32)||
|&emsp;&emsp;aboveGuideLevel|指导入围人数|integer(int32)||
|&emsp;&emsp;aboveInstLevel|指令入围人数|integer(int32)||
|&emsp;&emsp;alterAppose|补录并列人数|integer(int32)||
|&emsp;&emsp;alterLevel|补录等级线|string||
|&emsp;&emsp;alterOrderCode|补录成绩顺序号|string||
|&emsp;&emsp;dirAppose|定向并列人数|integer(int32)||
|&emsp;&emsp;dirLevel|定向等级线|string||
|&emsp;&emsp;dirOrderCode|定向成绩顺序号|string||
|&emsp;&emsp;dirPlan|定向计划数|integer(int32)||
|&emsp;&emsp;guideAppose|指导并列人数|integer(int32)||
|&emsp;&emsp;guideLevel|指导等级线|string||
|&emsp;&emsp;guideNum|指导报名数|integer(int32)||
|&emsp;&emsp;guideOrderCode|指导成绩顺序号|string||
|&emsp;&emsp;guidePlan|指导计划数|integer(int32)||
|&emsp;&emsp;hguideScore|指导最高分数|string||
|&emsp;&emsp;hinstScore|指令最高分数|string||
|&emsp;&emsp;hscore|最高分数|string||
|&emsp;&emsp;id|主键|string||
|&emsp;&emsp;instAppose|指令并列人数|integer(int32)||
|&emsp;&emsp;instLevel|指令等级线|string||
|&emsp;&emsp;instNum|指令报名数|integer(int32)||
|&emsp;&emsp;instOrderCode|指令成绩顺序号|string||
|&emsp;&emsp;instPlan|指令计划数|integer(int32)||
|&emsp;&emsp;lguideScore|指导最低分数|string||
|&emsp;&emsp;linstScore|指令最低分数|string||
|&emsp;&emsp;lscore|最低分数|string||
|&emsp;&emsp;runtime|运算时间|string(date-time)||
|&emsp;&emsp;schoolCode|学校代码|string||
|&emsp;&emsp;schoolName|学校名称|string||
|&emsp;&emsp;signupNum|报名人数|integer(int32)||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": {
		"aboveAlterLevel": 0,
		"aboveDirLevel": 0,
		"aboveGuideLevel": 0,
		"aboveInstLevel": 0,
		"alterAppose": 0,
		"alterLevel": "",
		"alterOrderCode": "",
		"dirAppose": 0,
		"dirLevel": "",
		"dirOrderCode": "",
		"dirPlan": 0,
		"guideAppose": 0,
		"guideLevel": "",
		"guideNum": 0,
		"guideOrderCode": "",
		"guidePlan": 0,
		"hguideScore": "",
		"hinstScore": "",
		"hscore": "",
		"id": "",
		"instAppose": 0,
		"instLevel": "",
		"instNum": 0,
		"instOrderCode": "",
		"instPlan": 0,
		"lguideScore": "",
		"linstScore": "",
		"lscore": "",
		"runtime": "",
		"schoolCode": "",
		"schoolName": "",
		"signupNum": 0
	},
	"success": true,
	"timestamp": 0
}
```


## 常规录取-取消录取(军属)


**接口地址**:`/nnzk/matriculate/ordinary/unMatMilitary`


**请求方式**:`POST`


**请求数据类型**:`application/json`


**响应数据类型**:`*/*`


**接口描述**:<p>常规录取-取消录取(军属)</p>



**请求示例**:


```javascript
{
  "archiveCodes": [],
  "matriculateType": ""
}
```


**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|input|input|body|true|OrdinaryMatAndUnMatDTO|OrdinaryMatAndUnMatDTO|
|&emsp;&emsp;archiveCodes|准考证号数组||false|array|string|
|&emsp;&emsp;matriculateType|录取类型||false|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«int»|
|201|Created||
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|integer(int32)|integer(int32)|
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": 0,
	"success": true,
	"timestamp": 0
}
```


## 常规录取-取消录取


**接口地址**:`/nnzk/matriculate/ordinary/unMatriculate`


**请求方式**:`POST`


**请求数据类型**:`application/json`


**响应数据类型**:`*/*`


**接口描述**:<p>常规录取-取消录取</p>



**请求示例**:


```javascript
{
  "archiveCodes": [],
  "matriculateType": ""
}
```


**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|input|input|body|true|OrdinaryMatAndUnMatDTO|OrdinaryMatAndUnMatDTO|
|&emsp;&emsp;archiveCodes|准考证号数组||false|array|string|
|&emsp;&emsp;matriculateType|录取类型||false|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«int»|
|201|Created||
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|integer(int32)|integer(int32)|
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": 0,
	"success": true,
	"timestamp": 0
}
```


## 普通高中报名-添加


**接口地址**:`/nnzk/sign/signAndMatriculate/add`


**请求方式**:`POST`


**请求数据类型**:`application/json`


**响应数据类型**:`*/*`


**接口描述**:<p>普通高中报名-添加</p>



**请求示例**:


```javascript
{
  "archiveCode": "",
  "batch": 0,
  "createBy": "",
  "createTime": "",
  "delFlag": 0,
  "fillTime": "",
  "highSchoolCode": "",
  "id": "",
  "isLodging": 0,
  "matriculateStatus": 0,
  "matriculateTime": "",
  "matriculateType": "",
  "newMatriculateStatus": 0,
  "operator": "",
  "remarkOfMatriculate": "",
  "signUpNo": "",
  "signUpType": "",
  "status": 0,
  "updateBy": "",
  "updateTime": "",
  "winNo": ""
}
```


**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|signAndMatriculate|普通高中报名|body|true|sign_and_matriculate对象|sign_and_matriculate对象|
|&emsp;&emsp;archiveCode|准考证号||false|string||
|&emsp;&emsp;batch|批次||false|integer(int32)||
|&emsp;&emsp;createBy|创建人||false|string||
|&emsp;&emsp;createTime|创建日期||false|string(date-time)||
|&emsp;&emsp;delFlag|删除标识||false|integer(int32)||
|&emsp;&emsp;fillTime|填报时间||false|string(date-time)||
|&emsp;&emsp;highSchoolCode|报名高中||false|string||
|&emsp;&emsp;id|主键||false|string||
|&emsp;&emsp;isLodging|是否住宿||false|integer(int32)||
|&emsp;&emsp;matriculateStatus|录取状态||false|integer(int32)||
|&emsp;&emsp;matriculateTime|录取时间||false|string(date-time)||
|&emsp;&emsp;matriculateType|录取类型||false|string||
|&emsp;&emsp;newMatriculateStatus|新录取状态||false|integer(int32)||
|&emsp;&emsp;operator|操作人||false|string||
|&emsp;&emsp;remarkOfMatriculate|录取说明||false|string||
|&emsp;&emsp;signUpNo|报名号||false|string||
|&emsp;&emsp;signUpType|报名类型||false|string||
|&emsp;&emsp;status|状态||false|integer(int32)||
|&emsp;&emsp;updateBy|更新人||false|string||
|&emsp;&emsp;updateTime|更新日期||false|string(date-time)||
|&emsp;&emsp;winNo|操作终端||false|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«string»|
|201|Created||
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|string||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": "",
	"success": true,
	"timestamp": 0
}
```


## 普通高中报名-注销志愿


**接口地址**:`/nnzk/sign/signAndMatriculate/cleanWish`


**请求方式**:`PUT`


**请求数据类型**:`application/json`


**响应数据类型**:`*/*`


**接口描述**:<p>普通高中报名-注销志愿</p>



**请求参数**:


暂无


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«string»|
|201|Created||
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|string||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": "",
	"success": true,
	"timestamp": 0
}
```


## 普通高中报名-通过id删除


**接口地址**:`/nnzk/sign/signAndMatriculate/delete`


**请求方式**:`DELETE`


**请求数据类型**:`application/x-www-form-urlencoded`


**响应数据类型**:`*/*`


**接口描述**:<p>普通高中报名-通过id删除</p>



**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|id|id|query|true|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«string»|
|204|No Content||
|401|Unauthorized||
|403|Forbidden||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|string||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": "",
	"success": true,
	"timestamp": 0
}
```


## 普通高中报名-批量删除


**接口地址**:`/nnzk/sign/signAndMatriculate/deleteBatch`


**请求方式**:`DELETE`


**请求数据类型**:`application/x-www-form-urlencoded`


**响应数据类型**:`*/*`


**接口描述**:<p>普通高中报名-批量删除</p>



**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|ids|ids|query|true|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«string»|
|204|No Content||
|401|Unauthorized||
|403|Forbidden||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|string||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": "",
	"success": true,
	"timestamp": 0
}
```


## 普通高中报名-编辑


**接口地址**:`/nnzk/sign/signAndMatriculate/edit`


**请求方式**:`POST`


**请求数据类型**:`application/json`


**响应数据类型**:`*/*`


**接口描述**:<p>普通高中报名-编辑</p>



**请求示例**:


```javascript
{
  "archiveCode": "",
  "batch": 0,
  "createBy": "",
  "createTime": "",
  "delFlag": 0,
  "fillTime": "",
  "highSchoolCode": "",
  "id": "",
  "isLodging": 0,
  "matriculateStatus": 0,
  "matriculateTime": "",
  "matriculateType": "",
  "newMatriculateStatus": 0,
  "operator": "",
  "remarkOfMatriculate": "",
  "signUpNo": "",
  "signUpType": "",
  "status": 0,
  "updateBy": "",
  "updateTime": "",
  "winNo": ""
}
```


**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|signAndMatriculate|普通高中报名|body|true|sign_and_matriculate对象|sign_and_matriculate对象|
|&emsp;&emsp;archiveCode|准考证号||false|string||
|&emsp;&emsp;batch|批次||false|integer(int32)||
|&emsp;&emsp;createBy|创建人||false|string||
|&emsp;&emsp;createTime|创建日期||false|string(date-time)||
|&emsp;&emsp;delFlag|删除标识||false|integer(int32)||
|&emsp;&emsp;fillTime|填报时间||false|string(date-time)||
|&emsp;&emsp;highSchoolCode|报名高中||false|string||
|&emsp;&emsp;id|主键||false|string||
|&emsp;&emsp;isLodging|是否住宿||false|integer(int32)||
|&emsp;&emsp;matriculateStatus|录取状态||false|integer(int32)||
|&emsp;&emsp;matriculateTime|录取时间||false|string(date-time)||
|&emsp;&emsp;matriculateType|录取类型||false|string||
|&emsp;&emsp;newMatriculateStatus|新录取状态||false|integer(int32)||
|&emsp;&emsp;operator|操作人||false|string||
|&emsp;&emsp;remarkOfMatriculate|录取说明||false|string||
|&emsp;&emsp;signUpNo|报名号||false|string||
|&emsp;&emsp;signUpType|报名类型||false|string||
|&emsp;&emsp;status|状态||false|integer(int32)||
|&emsp;&emsp;updateBy|更新人||false|string||
|&emsp;&emsp;updateTime|更新日期||false|string(date-time)||
|&emsp;&emsp;winNo|操作终端||false|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«string»|
|201|Created||
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|string||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": "",
	"success": true,
	"timestamp": 0
}
```


## 普通高中报名-编辑


**接口地址**:`/nnzk/sign/signAndMatriculate/edit`


**请求方式**:`PUT`


**请求数据类型**:`application/json`


**响应数据类型**:`*/*`


**接口描述**:<p>普通高中报名-编辑</p>



**请求示例**:


```javascript
{
  "archiveCode": "",
  "batch": 0,
  "createBy": "",
  "createTime": "",
  "delFlag": 0,
  "fillTime": "",
  "highSchoolCode": "",
  "id": "",
  "isLodging": 0,
  "matriculateStatus": 0,
  "matriculateTime": "",
  "matriculateType": "",
  "newMatriculateStatus": 0,
  "operator": "",
  "remarkOfMatriculate": "",
  "signUpNo": "",
  "signUpType": "",
  "status": 0,
  "updateBy": "",
  "updateTime": "",
  "winNo": ""
}
```


**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|signAndMatriculate|普通高中报名|body|true|sign_and_matriculate对象|sign_and_matriculate对象|
|&emsp;&emsp;archiveCode|准考证号||false|string||
|&emsp;&emsp;batch|批次||false|integer(int32)||
|&emsp;&emsp;createBy|创建人||false|string||
|&emsp;&emsp;createTime|创建日期||false|string(date-time)||
|&emsp;&emsp;delFlag|删除标识||false|integer(int32)||
|&emsp;&emsp;fillTime|填报时间||false|string(date-time)||
|&emsp;&emsp;highSchoolCode|报名高中||false|string||
|&emsp;&emsp;id|主键||false|string||
|&emsp;&emsp;isLodging|是否住宿||false|integer(int32)||
|&emsp;&emsp;matriculateStatus|录取状态||false|integer(int32)||
|&emsp;&emsp;matriculateTime|录取时间||false|string(date-time)||
|&emsp;&emsp;matriculateType|录取类型||false|string||
|&emsp;&emsp;newMatriculateStatus|新录取状态||false|integer(int32)||
|&emsp;&emsp;operator|操作人||false|string||
|&emsp;&emsp;remarkOfMatriculate|录取说明||false|string||
|&emsp;&emsp;signUpNo|报名号||false|string||
|&emsp;&emsp;signUpType|报名类型||false|string||
|&emsp;&emsp;status|状态||false|integer(int32)||
|&emsp;&emsp;updateBy|更新人||false|string||
|&emsp;&emsp;updateTime|更新日期||false|string(date-time)||
|&emsp;&emsp;winNo|操作终端||false|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«string»|
|201|Created||
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|string||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": "",
	"success": true,
	"timestamp": 0
}
```


## 普通高中报名-获取可填报的高中学校


**接口地址**:`/nnzk/sign/signAndMatriculate/getEnableSchool`


**请求方式**:`GET`


**请求数据类型**:`application/x-www-form-urlencoded`


**响应数据类型**:`*/*`


**接口描述**:<p>普通高中报名-获取可填报的高中学校</p>



**请求参数**:


暂无


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«List«EnableSchoolDTO»»|
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|array|EnableSchoolDTORes|
|&emsp;&emsp;beginTime|开始时间|string||
|&emsp;&emsp;canFill|允许填报|boolean||
|&emsp;&emsp;dispOrder|显示顺序|integer(int32)||
|&emsp;&emsp;enGuide|启用指导|integer(int32)||
|&emsp;&emsp;enInstruction|启用指令|integer(int32)||
|&emsp;&emsp;endTime|结束时间|string||
|&emsp;&emsp;lodgingInfo|住宿信息|string||
|&emsp;&emsp;privateOrder|什么顺序???|integer(int32)||
|&emsp;&emsp;reason|理由|string||
|&emsp;&emsp;schoolCode|学校代码|string||
|&emsp;&emsp;schoolCodeBlank||boolean||
|&emsp;&emsp;schoolName|学校名称|string||
|&emsp;&emsp;selectName|??|string||
|&emsp;&emsp;signType|可报考类型|string||
|&emsp;&emsp;signTypeGuide||boolean||
|&emsp;&emsp;signTypeInstructionAndGuide||boolean||
|&emsp;&emsp;status|状态|string||
|&emsp;&emsp;statusName|状态名称|string||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": [
		{
			"beginTime": "",
			"canFill": true,
			"dispOrder": 0,
			"enGuide": 0,
			"enInstruction": 0,
			"endTime": "",
			"lodgingInfo": "",
			"privateOrder": 0,
			"reason": "",
			"schoolCode": "",
			"schoolCodeBlank": true,
			"schoolName": "",
			"selectName": "",
			"signType": "",
			"signTypeGuide": true,
			"signTypeInstructionAndGuide": true,
			"status": "",
			"statusName": ""
		}
	],
	"success": true,
	"timestamp": 0
}
```


## 学校端-获取录取学生数据(学校录取名单)


**接口地址**:`/nnzk/sign/signAndMatriculate/getGzMatriculate`


**请求方式**:`GET`


**请求数据类型**:`application/x-www-form-urlencoded`


**响应数据类型**:`*/*`


**接口描述**:<p>学校端-获取录取学生数据(学校录取名单)</p>



**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|highSchoolCode|高中学校代码|query|true|string||
|matriculateType|录取类型|query|false|string||
|rangeEnd|按编号范围(结束)|query|false|integer(int32)||
|rangeStart|按编号范围(开始)|query|false|integer(int32)||
|searchByArchiveCode|按准考证号|query|false|string||
|selectBy|查询方式（全部/按准考证号/按编号范围）|query|false|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«GetGzMatriculateOutputDTO»|
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|GetGzMatriculateOutputDTO|GetGzMatriculateOutputDTO|
|&emsp;&emsp;apposeNum|？？|integer(int32)||
|&emsp;&emsp;highestScore|最高成绩|string||
|&emsp;&emsp;lowestScore|最低成绩|string||
|&emsp;&emsp;matriculateNum|记录总数|integer(int32)||
|&emsp;&emsp;proposedMatriculateNum|拟录取人数|integer(int32)||
|&emsp;&emsp;records|录取信息|array|MatriculateInfoDTO|
|&emsp;&emsp;&emsp;&emsp;archiveCode|准考证号|string||
|&emsp;&emsp;&emsp;&emsp;batch|?|integer||
|&emsp;&emsp;&emsp;&emsp;chineseLevel|语文|string||
|&emsp;&emsp;&emsp;&emsp;chymistLevel|化学|string||
|&emsp;&emsp;&emsp;&emsp;combinedScore|组合分|string||
|&emsp;&emsp;&emsp;&emsp;diathesis|综合素质|string||
|&emsp;&emsp;&emsp;&emsp;englishLevel|英语|string||
|&emsp;&emsp;&emsp;&emsp;experiment|实验|string||
|&emsp;&emsp;&emsp;&emsp;finishSchoolName|毕业学校|string||
|&emsp;&emsp;&emsp;&emsp;isAreaStudent|是否地段生|integer||
|&emsp;&emsp;&emsp;&emsp;mathLevel|数学|string||
|&emsp;&emsp;&emsp;&emsp;matriculateStatus|?|integer||
|&emsp;&emsp;&emsp;&emsp;matriculateType|录取类型|string||
|&emsp;&emsp;&emsp;&emsp;newMatriculateStatus|?|integer||
|&emsp;&emsp;&emsp;&emsp;order|?|integer||
|&emsp;&emsp;&emsp;&emsp;phoneCode|电话号码|string||
|&emsp;&emsp;&emsp;&emsp;physicsLevel|物理|string||
|&emsp;&emsp;&emsp;&emsp;politicsLevel|政史|string||
|&emsp;&emsp;&emsp;&emsp;printMatType|录取类型（用于打印）|string||
|&emsp;&emsp;&emsp;&emsp;schoolName|?|string||
|&emsp;&emsp;&emsp;&emsp;scoreOrder|成绩排序码|number||
|&emsp;&emsp;&emsp;&emsp;serialNum|序号|integer||
|&emsp;&emsp;&emsp;&emsp;sex|性别|string||
|&emsp;&emsp;&emsp;&emsp;signUpType|报考类型|integer||
|&emsp;&emsp;&emsp;&emsp;status|?|integer||
|&emsp;&emsp;&emsp;&emsp;studentFrom|?|string||
|&emsp;&emsp;&emsp;&emsp;studentName|学生姓名|string||
|&emsp;&emsp;&emsp;&emsp;sumScore|总分|string||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": {
		"apposeNum": 0,
		"highestScore": "",
		"lowestScore": "",
		"matriculateNum": 0,
		"proposedMatriculateNum": 0,
		"records": [
			{
				"archiveCode": "",
				"batch": 0,
				"chineseLevel": "",
				"chymistLevel": "",
				"combinedScore": "",
				"diathesis": "",
				"englishLevel": "",
				"experiment": "",
				"finishSchoolName": "",
				"isAreaStudent": 0,
				"mathLevel": "",
				"matriculateStatus": 0,
				"matriculateType": "",
				"newMatriculateStatus": 0,
				"order": 0,
				"phoneCode": "",
				"physicsLevel": "",
				"politicsLevel": "",
				"printMatType": "",
				"schoolName": "",
				"scoreOrder": 0,
				"serialNum": 0,
				"sex": "",
				"signUpType": 0,
				"status": 0,
				"studentFrom": "",
				"studentName": "",
				"sumScore": ""
			}
		]
	},
	"success": true,
	"timestamp": 0
}
```


## 学校端-获取学校录取名单打印数据


**接口地址**:`/nnzk/sign/signAndMatriculate/getGzMatriculatePrintData`


**请求方式**:`GET`


**请求数据类型**:`application/x-www-form-urlencoded`


**响应数据类型**:`*/*`


**接口描述**:<p>学校端-获取学校录取名单打印数据</p>



**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|highSchoolCode|高中学校代码|query|true|string||
|matriculateType|录取类型|query|false|string||
|rangeEnd|按编号范围(结束)|query|false|integer(int32)||
|rangeStart|按编号范围(开始)|query|false|integer(int32)||
|searchByArchiveCode|按准考证号|query|false|string||
|selectBy|查询方式（全部/按准考证号/按编号范围）|query|false|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|GzMatPrintOutputDTO|
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|count|总条数|integer(int32)|integer(int32)|
|data|学生列表|array|MatriculateInfoDTO|
|&emsp;&emsp;archiveCode|准考证号|string||
|&emsp;&emsp;batch|?|integer(int32)||
|&emsp;&emsp;chineseLevel|语文|string||
|&emsp;&emsp;chymistLevel|化学|string||
|&emsp;&emsp;combinedScore|组合分|string||
|&emsp;&emsp;diathesis|综合素质|string||
|&emsp;&emsp;englishLevel|英语|string||
|&emsp;&emsp;experiment|实验|string||
|&emsp;&emsp;finishSchoolName|毕业学校|string||
|&emsp;&emsp;isAreaStudent|是否地段生|integer(int32)||
|&emsp;&emsp;mathLevel|数学|string||
|&emsp;&emsp;matriculateStatus|?|integer(int32)||
|&emsp;&emsp;matriculateType|录取类型|string||
|&emsp;&emsp;newMatriculateStatus|?|integer(int32)||
|&emsp;&emsp;order|?|integer(int32)||
|&emsp;&emsp;phoneCode|电话号码|string||
|&emsp;&emsp;physicsLevel|物理|string||
|&emsp;&emsp;politicsLevel|政史|string||
|&emsp;&emsp;printMatType|录取类型（用于打印）|string||
|&emsp;&emsp;schoolName|?|string||
|&emsp;&emsp;scoreOrder|成绩排序码|number||
|&emsp;&emsp;serialNum|序号|integer(int32)||
|&emsp;&emsp;sex|性别|string||
|&emsp;&emsp;signUpType|报考类型|integer(int32)||
|&emsp;&emsp;status|?|integer(int32)||
|&emsp;&emsp;studentFrom|?|string||
|&emsp;&emsp;studentName|学生姓名|string||
|&emsp;&emsp;sumScore|总分|string||
|total|总页数|integer(int32)|integer(int32)|


**响应示例**:
```javascript
{
	"count": 0,
	"data": [
		{
			"archiveCode": "",
			"batch": 0,
			"chineseLevel": "",
			"chymistLevel": "",
			"combinedScore": "",
			"diathesis": "",
			"englishLevel": "",
			"experiment": "",
			"finishSchoolName": "",
			"isAreaStudent": 0,
			"mathLevel": "",
			"matriculateStatus": 0,
			"matriculateType": "",
			"newMatriculateStatus": 0,
			"order": 0,
			"phoneCode": "",
			"physicsLevel": "",
			"politicsLevel": "",
			"printMatType": "",
			"schoolName": "",
			"scoreOrder": 0,
			"serialNum": 0,
			"sex": "",
			"signUpType": 0,
			"status": 0,
			"studentFrom": "",
			"studentName": "",
			"sumScore": ""
		}
	],
	"total": 0
}
```


## 普通高中报名-报名情况查询学生信息列表


**接口地址**:`/nnzk/sign/signAndMatriculate/getGzSignInfoList`


**请求方式**:`GET`


**请求数据类型**:`application/x-www-form-urlencoded`


**响应数据类型**:`*/*`


**接口描述**:<p>普通高中报名-报名情况查询学生信息列表</p>



**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|archiveCode|准考证号|query|false|string||
|calculateType|入围类型|query|false|string||
|chineseLevel|语文|query|false|string||
|chymistLevel|化学|query|false|string||
|combinedScore|组合分|query|false|string||
|diathesis|综合素质|query|false|string||
|englishLevel|英语|query|false|string||
|experiment|实验|query|false|string||
|isAreaStudent|地段生|query|false|integer(int32)||
|mathLevel|数学|query|false|string||
|pageNo|pageNo|query|false|integer(int32)||
|pageSize|pageSize|query|false|integer(int32)||
|physicsLevel|物理|query|false|string||
|politicsLevel|政史|query|false|string||
|schoolCode|学校代码|query|false|string||
|schoolName|报考学校|query|false|string||
|scoreOrder|成绩排序码|query|false|number||
|sex|性别|query|false|string||
|signUpType|报考类型|query|false|string||
|studentName|学生姓名|query|false|string||
|sumScore|总分|query|false|string||
|tempOrder|排名|query|false|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«IPage«SignInfo»»|
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|IPage«SignInfo»|IPage«SignInfo»|
|&emsp;&emsp;current||integer(int64)||
|&emsp;&emsp;pages||integer(int64)||
|&emsp;&emsp;records||array|SignInfo|
|&emsp;&emsp;&emsp;&emsp;archiveCode|准考证号|string||
|&emsp;&emsp;&emsp;&emsp;calculateType|入围类型|string||
|&emsp;&emsp;&emsp;&emsp;chineseLevel|语文|string||
|&emsp;&emsp;&emsp;&emsp;chymistLevel|化学|string||
|&emsp;&emsp;&emsp;&emsp;combinedScore|组合分|string||
|&emsp;&emsp;&emsp;&emsp;diathesis|综合素质|string||
|&emsp;&emsp;&emsp;&emsp;englishLevel|英语|string||
|&emsp;&emsp;&emsp;&emsp;experiment|实验|string||
|&emsp;&emsp;&emsp;&emsp;isAreaStudent|地段生|integer||
|&emsp;&emsp;&emsp;&emsp;mathLevel|数学|string||
|&emsp;&emsp;&emsp;&emsp;physicsLevel|物理|string||
|&emsp;&emsp;&emsp;&emsp;politicsLevel|政史|string||
|&emsp;&emsp;&emsp;&emsp;schoolCode|学校代码|string||
|&emsp;&emsp;&emsp;&emsp;schoolName|报考学校|string||
|&emsp;&emsp;&emsp;&emsp;scoreOrder|成绩排序码|number||
|&emsp;&emsp;&emsp;&emsp;sex|性别|string||
|&emsp;&emsp;&emsp;&emsp;signUpType|报考类型|string||
|&emsp;&emsp;&emsp;&emsp;studentName|学生姓名|string||
|&emsp;&emsp;&emsp;&emsp;sumScore|总分|string||
|&emsp;&emsp;&emsp;&emsp;tempOrder|排名|string||
|&emsp;&emsp;size||integer(int64)||
|&emsp;&emsp;total||integer(int64)||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": {
		"current": 0,
		"pages": 0,
		"records": [
			{
				"archiveCode": "",
				"calculateType": "",
				"chineseLevel": "",
				"chymistLevel": "",
				"combinedScore": "",
				"diathesis": "",
				"englishLevel": "",
				"experiment": "",
				"isAreaStudent": 0,
				"mathLevel": "",
				"physicsLevel": "",
				"politicsLevel": "",
				"schoolCode": "",
				"schoolName": "",
				"scoreOrder": 0,
				"sex": "",
				"signUpType": "",
				"studentName": "",
				"sumScore": "",
				"tempOrder": ""
			}
		],
		"size": 0,
		"total": 0
	},
	"success": true,
	"timestamp": 0
}
```


## 普通高中报名-报名情况查询学校统计信息


**接口地址**:`/nnzk/sign/signAndMatriculate/getGzStatistics`


**请求方式**:`GET`


**请求数据类型**:`application/x-www-form-urlencoded`


**响应数据类型**:`*/*`


**接口描述**:<p>普通高中报名-报名情况查询学校统计信息</p>



**请求参数**:


暂无


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«GetGzStatisticsDTO»|
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|GetGzStatisticsDTO|GetGzStatisticsDTO|
|&emsp;&emsp;aboveAlterLevel|补录入围人数|integer(int32)||
|&emsp;&emsp;aboveDirLevel|定向入围人数|integer(int32)||
|&emsp;&emsp;aboveGuideLevel|指导入围人数|integer(int32)||
|&emsp;&emsp;aboveInstLevel|指令入围人数|integer(int32)||
|&emsp;&emsp;alterAppose|补录并列人数|integer(int32)||
|&emsp;&emsp;alterLevel|补录等级线|string||
|&emsp;&emsp;alterPlan|拟招补录数|integer(int32)||
|&emsp;&emsp;dirAppose|定向并列人数|integer(int32)||
|&emsp;&emsp;dirLevel|定向等级线|string||
|&emsp;&emsp;dirPlan|定向计划数|integer(int32)||
|&emsp;&emsp;guideAppose|指导并列人数|integer(int32)||
|&emsp;&emsp;guideLevel|指导等级线|string||
|&emsp;&emsp;guidePlan|指导计划数|integer(int32)||
|&emsp;&emsp;instAppose|指令并列人数|integer(int32)||
|&emsp;&emsp;instLevel|指令等级线|string||
|&emsp;&emsp;instNum|指令报名数|integer(int32)||
|&emsp;&emsp;instPlan|指令计划数|integer(int32)||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": {
		"aboveAlterLevel": 0,
		"aboveDirLevel": 0,
		"aboveGuideLevel": 0,
		"aboveInstLevel": 0,
		"alterAppose": 0,
		"alterLevel": "",
		"alterPlan": 0,
		"dirAppose": 0,
		"dirLevel": "",
		"dirPlan": 0,
		"guideAppose": 0,
		"guideLevel": "",
		"guidePlan": 0,
		"instAppose": 0,
		"instLevel": "",
		"instNum": 0,
		"instPlan": 0
	},
	"success": true,
	"timestamp": 0
}
```


## 普通高中报名-报名排名查询


**接口地址**:`/nnzk/sign/signAndMatriculate/getMatriculateInfo`


**请求方式**:`GET`


**请求数据类型**:`application/x-www-form-urlencoded`


**响应数据类型**:`*/*`


**接口描述**:<p>普通高中报名-报名排名查询</p>



**请求参数**:


暂无


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«StudentMatriculateInfoDTO»|
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|StudentMatriculateInfoDTO|StudentMatriculateInfoDTO|
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": {},
	"success": true,
	"timestamp": 0
}
```


## 普通高中报名-个人录取查询


**接口地址**:`/nnzk/sign/signAndMatriculate/getPersonalMat`


**请求方式**:`GET`


**请求数据类型**:`application/x-www-form-urlencoded`


**响应数据类型**:`*/*`


**接口描述**:<p>普通高中报名-个人录取查询</p>



**请求参数**:


暂无


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«PersonalSignInfo»|
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|PersonalSignInfo|PersonalSignInfo|
|&emsp;&emsp;matSchoolName||string||
|&emsp;&emsp;matriculateResult||string||
|&emsp;&emsp;matriculateTime||string(date-time)||
|&emsp;&emsp;studentType||string||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": {
		"matSchoolName": "",
		"matriculateResult": "",
		"matriculateTime": "",
		"studentType": ""
	},
	"success": true,
	"timestamp": 0
}
```


## 普通高中报名-个人报名查询


**接口地址**:`/nnzk/sign/signAndMatriculate/getStudentSignupInfo`


**请求方式**:`GET`


**请求数据类型**:`application/x-www-form-urlencoded`


**响应数据类型**:`*/*`


**接口描述**:<p>普通高中报名-个人报名查询</p>



**请求参数**:


暂无


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«StudentSignupInfoDTO»|
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|StudentSignupInfoDTO|StudentSignupInfoDTO|
|&emsp;&emsp;alterLevel|高中补录等级线|string||
|&emsp;&emsp;alterPlan|高中补录数|integer(int32)||
|&emsp;&emsp;alters|高中补录入围的等级排序码序列|string||
|&emsp;&emsp;archiveCode|准考证号|string||
|&emsp;&emsp;calculateType|入围类型|string||
|&emsp;&emsp;directionalLevel|高中定向等级线|string||
|&emsp;&emsp;directionalPlan|高中定向计划数|integer(int32)||
|&emsp;&emsp;directionals|高中定向入围的等级排序码序列|string||
|&emsp;&emsp;guideLevel|高中指导等级线|string||
|&emsp;&emsp;guidePlan|高中指导计划数|integer(int32)||
|&emsp;&emsp;guides|高中指导入围的等级排序码序列|string||
|&emsp;&emsp;highSchoolCode|高中学校编码|string||
|&emsp;&emsp;highSchoolName|高中学校名称|string||
|&emsp;&emsp;highSchoolStatus|高中学校状态|string||
|&emsp;&emsp;instructionLevel|高中指令等级线|string||
|&emsp;&emsp;instructionPlan|高中指令计划数|integer(int32)||
|&emsp;&emsp;instructions|高中指令入围的等级排序码序列|string||
|&emsp;&emsp;isMilitary|是否优抚对象|boolean||
|&emsp;&emsp;matriculateStatus|是否录取|boolean||
|&emsp;&emsp;maxList|各入围序列里的最大值|string||
|&emsp;&emsp;order|排名|integer(int32)||
|&emsp;&emsp;orderCode|等级排序码|string||
|&emsp;&emsp;runTime|运算时间|string(date-time)||
|&emsp;&emsp;signupType|报名类型|string||
|&emsp;&emsp;studentName|学生姓名|string||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": {
		"alterLevel": "",
		"alterPlan": 0,
		"alters": "",
		"archiveCode": "",
		"calculateType": "",
		"directionalLevel": "",
		"directionalPlan": 0,
		"directionals": "",
		"guideLevel": "",
		"guidePlan": 0,
		"guides": "",
		"highSchoolCode": "",
		"highSchoolName": "",
		"highSchoolStatus": "",
		"instructionLevel": "",
		"instructionPlan": 0,
		"instructions": "",
		"isMilitary": true,
		"matriculateStatus": true,
		"maxList": "",
		"order": 0,
		"orderCode": "",
		"runTime": "",
		"signupType": "",
		"studentName": ""
	},
	"success": true,
	"timestamp": 0
}
```


## 普通高中报名-分页列表查询


**接口地址**:`/nnzk/sign/signAndMatriculate/list`


**请求方式**:`GET`


**请求数据类型**:`application/x-www-form-urlencoded`


**响应数据类型**:`*/*`


**接口描述**:<p>普通高中报名-分页列表查询</p>



**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|archiveCode|准考证号|query|true|string||
|batch|批次|query|false|integer(int32)||
|createBy|创建人|query|false|string||
|createTime|创建日期|query|false|string(date-time)||
|delFlag|删除标识|query|false|integer(int32)||
|fillTime|填报时间|query|false|string(date-time)||
|highSchoolCode|报名高中|query|false|string||
|id|主键|query|false|string||
|isLodging|是否住宿|query|false|integer(int32)||
|matriculateStatus|录取状态|query|false|integer(int32)||
|matriculateTime|录取时间|query|false|string(date-time)||
|matriculateType|录取类型|query|false|string||
|newMatriculateStatus|新录取状态|query|false|integer(int32)||
|operator|操作人|query|false|string||
|pageNo|pageNo|query|false|integer(int32)||
|pageSize|pageSize|query|false|integer(int32)||
|remarkOfMatriculate|录取说明|query|false|string||
|signUpNo|报名号|query|false|string||
|signUpType|报名类型|query|false|string||
|status|状态|query|false|integer(int32)||
|updateBy|更新人|query|false|string||
|updateTime|更新日期|query|false|string(date-time)||
|winNo|操作终端|query|false|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«IPage«sign_and_matriculate对象»»|
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|IPage«sign_and_matriculate对象»|IPage«sign_and_matriculate对象»|
|&emsp;&emsp;current||integer(int64)||
|&emsp;&emsp;pages||integer(int64)||
|&emsp;&emsp;records||array|sign_and_matriculate对象|
|&emsp;&emsp;&emsp;&emsp;archiveCode|准考证号|string||
|&emsp;&emsp;&emsp;&emsp;batch|批次|integer||
|&emsp;&emsp;&emsp;&emsp;createBy|创建人|string||
|&emsp;&emsp;&emsp;&emsp;createTime|创建日期|string||
|&emsp;&emsp;&emsp;&emsp;delFlag|删除标识|integer||
|&emsp;&emsp;&emsp;&emsp;fillTime|填报时间|string||
|&emsp;&emsp;&emsp;&emsp;highSchoolCode|报名高中|string||
|&emsp;&emsp;&emsp;&emsp;id|主键|string||
|&emsp;&emsp;&emsp;&emsp;isLodging|是否住宿|integer||
|&emsp;&emsp;&emsp;&emsp;matriculateStatus|录取状态|integer||
|&emsp;&emsp;&emsp;&emsp;matriculateTime|录取时间|string||
|&emsp;&emsp;&emsp;&emsp;matriculateType|录取类型|string||
|&emsp;&emsp;&emsp;&emsp;newMatriculateStatus|新录取状态|integer||
|&emsp;&emsp;&emsp;&emsp;operator|操作人|string||
|&emsp;&emsp;&emsp;&emsp;remarkOfMatriculate|录取说明|string||
|&emsp;&emsp;&emsp;&emsp;signUpNo|报名号|string||
|&emsp;&emsp;&emsp;&emsp;signUpType|报名类型|string||
|&emsp;&emsp;&emsp;&emsp;status|状态|integer||
|&emsp;&emsp;&emsp;&emsp;updateBy|更新人|string||
|&emsp;&emsp;&emsp;&emsp;updateTime|更新日期|string||
|&emsp;&emsp;&emsp;&emsp;winNo|操作终端|string||
|&emsp;&emsp;size||integer(int64)||
|&emsp;&emsp;total||integer(int64)||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": {
		"current": 0,
		"pages": 0,
		"records": [
			{
				"archiveCode": "",
				"batch": 0,
				"createBy": "",
				"createTime": "",
				"delFlag": 0,
				"fillTime": "",
				"highSchoolCode": "",
				"id": "",
				"isLodging": 0,
				"matriculateStatus": 0,
				"matriculateTime": "",
				"matriculateType": "",
				"newMatriculateStatus": 0,
				"operator": "",
				"remarkOfMatriculate": "",
				"signUpNo": "",
				"signUpType": "",
				"status": 0,
				"updateBy": "",
				"updateTime": "",
				"winNo": ""
			}
		],
		"size": 0,
		"total": 0
	},
	"success": true,
	"timestamp": 0
}
```


## 普通高中报名-通过id查询


**接口地址**:`/nnzk/sign/signAndMatriculate/queryById`


**请求方式**:`GET`


**请求数据类型**:`application/x-www-form-urlencoded`


**响应数据类型**:`*/*`


**接口描述**:<p>普通高中报名-通过id查询</p>



**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|id|id|query|true|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«sign_and_matriculate对象»|
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|sign_and_matriculate对象|sign_and_matriculate对象|
|&emsp;&emsp;archiveCode|准考证号|string||
|&emsp;&emsp;batch|批次|integer(int32)||
|&emsp;&emsp;createBy|创建人|string||
|&emsp;&emsp;createTime|创建日期|string(date-time)||
|&emsp;&emsp;delFlag|删除标识|integer(int32)||
|&emsp;&emsp;fillTime|填报时间|string(date-time)||
|&emsp;&emsp;highSchoolCode|报名高中|string||
|&emsp;&emsp;id|主键|string||
|&emsp;&emsp;isLodging|是否住宿|integer(int32)||
|&emsp;&emsp;matriculateStatus|录取状态|integer(int32)||
|&emsp;&emsp;matriculateTime|录取时间|string(date-time)||
|&emsp;&emsp;matriculateType|录取类型|string||
|&emsp;&emsp;newMatriculateStatus|新录取状态|integer(int32)||
|&emsp;&emsp;operator|操作人|string||
|&emsp;&emsp;remarkOfMatriculate|录取说明|string||
|&emsp;&emsp;signUpNo|报名号|string||
|&emsp;&emsp;signUpType|报名类型|string||
|&emsp;&emsp;status|状态|integer(int32)||
|&emsp;&emsp;updateBy|更新人|string||
|&emsp;&emsp;updateTime|更新日期|string(date-time)||
|&emsp;&emsp;winNo|操作终端|string||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": {
		"archiveCode": "",
		"batch": 0,
		"createBy": "",
		"createTime": "",
		"delFlag": 0,
		"fillTime": "",
		"highSchoolCode": "",
		"id": "",
		"isLodging": 0,
		"matriculateStatus": 0,
		"matriculateTime": "",
		"matriculateType": "",
		"newMatriculateStatus": 0,
		"operator": "",
		"remarkOfMatriculate": "",
		"signUpNo": "",
		"signUpType": "",
		"status": 0,
		"updateBy": "",
		"updateTime": "",
		"winNo": ""
	},
	"success": true,
	"timestamp": 0
}
```


## 普通高中报名-保存志愿


**接口地址**:`/nnzk/sign/signAndMatriculate/saveWish`


**请求方式**:`POST`


**请求数据类型**:`application/json`


**响应数据类型**:`*/*`


**接口描述**:<p>普通高中报名-保存志愿</p>



**请求示例**:


```javascript
{
  "beginTime": "",
  "canFill": true,
  "dispOrder": 0,
  "enGuide": 0,
  "enInstruction": 0,
  "endTime": "",
  "lodgingInfo": "",
  "privateOrder": 0,
  "reason": "",
  "schoolCode": "",
  "schoolName": "",
  "selectName": "",
  "signType": "",
  "status": "",
  "statusName": ""
}
```


**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|enableSchoolDto|enableSchoolDto|body|true|EnableSchoolDTOReq|EnableSchoolDTOReq|
|&emsp;&emsp;beginTime|开始时间||false|string||
|&emsp;&emsp;canFill|允许填报||false|boolean||
|&emsp;&emsp;dispOrder|显示顺序||false|integer(int32)||
|&emsp;&emsp;enGuide|启用指导||false|integer(int32)||
|&emsp;&emsp;enInstruction|启用指令||false|integer(int32)||
|&emsp;&emsp;endTime|结束时间||false|string||
|&emsp;&emsp;lodgingInfo|住宿信息||false|string||
|&emsp;&emsp;privateOrder|什么顺序???||false|integer(int32)||
|&emsp;&emsp;reason|理由||false|string||
|&emsp;&emsp;schoolCode|学校代码||false|string||
|&emsp;&emsp;schoolName|学校名称||false|string||
|&emsp;&emsp;selectName|??||false|string||
|&emsp;&emsp;signType|可报考类型||false|string||
|&emsp;&emsp;status|状态||false|string||
|&emsp;&emsp;statusName|状态名称||false|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«string»|
|201|Created||
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|string||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": "",
	"success": true,
	"timestamp": 0
}
```


# 查询统计


## 统计总表


**接口地址**:`/nnzk/base/queryStatistics/ReportSchoolStatistic`


**请求方式**:`GET`


**请求数据类型**:`application/x-www-form-urlencoded`


**响应数据类型**:`*/*`


**接口描述**:<p>统计总表</p>



**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|schoolCodeList|schoolCodeList|query|false|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«List«school_statistics_data对象»»|
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|array|school_statistics_data对象|
|&emsp;&emsp;aboveAlterLevel|补录入围人数|integer(int32)||
|&emsp;&emsp;aboveDirLevel|定向入围人数|integer(int32)||
|&emsp;&emsp;aboveGuideLevel|指导入围人数|integer(int32)||
|&emsp;&emsp;aboveInstLevel|指令入围人数|integer(int32)||
|&emsp;&emsp;alterAppose|补录并列人数|integer(int32)||
|&emsp;&emsp;alterLevel|补录等级线|string||
|&emsp;&emsp;alterOrderCode|补录成绩顺序号|string||
|&emsp;&emsp;dirAppose|定向并列人数|integer(int32)||
|&emsp;&emsp;dirLevel|定向等级线|string||
|&emsp;&emsp;dirOrderCode|定向成绩顺序号|string||
|&emsp;&emsp;dirPlan|定向计划数|integer(int32)||
|&emsp;&emsp;guideAppose|指导并列人数|integer(int32)||
|&emsp;&emsp;guideLevel|指导等级线|string||
|&emsp;&emsp;guideNum|指导报名数|integer(int32)||
|&emsp;&emsp;guideOrderCode|指导成绩顺序号|string||
|&emsp;&emsp;guidePlan|指导计划数|integer(int32)||
|&emsp;&emsp;hguideScore|指导最高分数|string||
|&emsp;&emsp;hinstScore|指令最高分数|string||
|&emsp;&emsp;hscore|最高分数|string||
|&emsp;&emsp;id|主键|string||
|&emsp;&emsp;instAppose|指令并列人数|integer(int32)||
|&emsp;&emsp;instLevel|指令等级线|string||
|&emsp;&emsp;instNum|指令报名数|integer(int32)||
|&emsp;&emsp;instOrderCode|指令成绩顺序号|string||
|&emsp;&emsp;instPlan|指令计划数|integer(int32)||
|&emsp;&emsp;lguideScore|指导最低分数|string||
|&emsp;&emsp;linstScore|指令最低分数|string||
|&emsp;&emsp;lscore|最低分数|string||
|&emsp;&emsp;runtime|运算时间|string(date-time)||
|&emsp;&emsp;schoolCode|学校代码|string||
|&emsp;&emsp;schoolName|学校名称|string||
|&emsp;&emsp;signupNum|报名人数|integer(int32)||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": [
		{
			"aboveAlterLevel": 0,
			"aboveDirLevel": 0,
			"aboveGuideLevel": 0,
			"aboveInstLevel": 0,
			"alterAppose": 0,
			"alterLevel": "",
			"alterOrderCode": "",
			"dirAppose": 0,
			"dirLevel": "",
			"dirOrderCode": "",
			"dirPlan": 0,
			"guideAppose": 0,
			"guideLevel": "",
			"guideNum": 0,
			"guideOrderCode": "",
			"guidePlan": 0,
			"hguideScore": "",
			"hinstScore": "",
			"hscore": "",
			"id": "",
			"instAppose": 0,
			"instLevel": "",
			"instNum": 0,
			"instOrderCode": "",
			"instPlan": 0,
			"lguideScore": "",
			"linstScore": "",
			"lscore": "",
			"runtime": "",
			"schoolCode": "",
			"schoolName": "",
			"signupNum": 0
		}
	],
	"success": true,
	"timestamp": 0
}
```


## 统计总表-打印


**接口地址**:`/nnzk/base/queryStatistics/ReportSchoolStatisticPrint`


**请求方式**:`GET`


**请求数据类型**:`application/x-www-form-urlencoded`


**响应数据类型**:`*/*`


**接口描述**:<p>统计总表-打印</p>



**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|schoolCodeList|schoolCodeList|query|false|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|ReportSchoolStatisticPrintOutputDTO|
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|count|总条数|integer(int32)|integer(int32)|
|data|数据列表|array|school_statistics_data对象|
|&emsp;&emsp;aboveAlterLevel|补录入围人数|integer(int32)||
|&emsp;&emsp;aboveDirLevel|定向入围人数|integer(int32)||
|&emsp;&emsp;aboveGuideLevel|指导入围人数|integer(int32)||
|&emsp;&emsp;aboveInstLevel|指令入围人数|integer(int32)||
|&emsp;&emsp;alterAppose|补录并列人数|integer(int32)||
|&emsp;&emsp;alterLevel|补录等级线|string||
|&emsp;&emsp;alterOrderCode|补录成绩顺序号|string||
|&emsp;&emsp;dirAppose|定向并列人数|integer(int32)||
|&emsp;&emsp;dirLevel|定向等级线|string||
|&emsp;&emsp;dirOrderCode|定向成绩顺序号|string||
|&emsp;&emsp;dirPlan|定向计划数|integer(int32)||
|&emsp;&emsp;guideAppose|指导并列人数|integer(int32)||
|&emsp;&emsp;guideLevel|指导等级线|string||
|&emsp;&emsp;guideNum|指导报名数|integer(int32)||
|&emsp;&emsp;guideOrderCode|指导成绩顺序号|string||
|&emsp;&emsp;guidePlan|指导计划数|integer(int32)||
|&emsp;&emsp;hguideScore|指导最高分数|string||
|&emsp;&emsp;hinstScore|指令最高分数|string||
|&emsp;&emsp;hscore|最高分数|string||
|&emsp;&emsp;id|主键|string||
|&emsp;&emsp;instAppose|指令并列人数|integer(int32)||
|&emsp;&emsp;instLevel|指令等级线|string||
|&emsp;&emsp;instNum|指令报名数|integer(int32)||
|&emsp;&emsp;instOrderCode|指令成绩顺序号|string||
|&emsp;&emsp;instPlan|指令计划数|integer(int32)||
|&emsp;&emsp;lguideScore|指导最低分数|string||
|&emsp;&emsp;linstScore|指令最低分数|string||
|&emsp;&emsp;lscore|最低分数|string||
|&emsp;&emsp;runtime|运算时间|string(date-time)||
|&emsp;&emsp;schoolCode|学校代码|string||
|&emsp;&emsp;schoolName|学校名称|string||
|&emsp;&emsp;signupNum|报名人数|integer(int32)||
|total|总页数|integer(int32)|integer(int32)|


**响应示例**:
```javascript
{
	"count": 0,
	"data": [
		{
			"aboveAlterLevel": 0,
			"aboveDirLevel": 0,
			"aboveGuideLevel": 0,
			"aboveInstLevel": 0,
			"alterAppose": 0,
			"alterLevel": "",
			"alterOrderCode": "",
			"dirAppose": 0,
			"dirLevel": "",
			"dirOrderCode": "",
			"dirPlan": 0,
			"guideAppose": 0,
			"guideLevel": "",
			"guideNum": 0,
			"guideOrderCode": "",
			"guidePlan": 0,
			"hguideScore": "",
			"hinstScore": "",
			"hscore": "",
			"id": "",
			"instAppose": 0,
			"instLevel": "",
			"instNum": 0,
			"instOrderCode": "",
			"instPlan": 0,
			"lguideScore": "",
			"linstScore": "",
			"lscore": "",
			"runtime": "",
			"schoolCode": "",
			"schoolName": "",
			"signupNum": 0
		}
	],
	"total": 0
}
```


## 多项查询


**接口地址**:`/nnzk/base/queryStatistics/multiQuery`


**请求方式**:`GET`


**请求数据类型**:`application/x-www-form-urlencoded`


**响应数据类型**:`*/*`


**接口描述**:<p>多项查询</p>



**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|archiveCode|准考证号|query|false|string||
|areaCode|所属城区|query|false|string||
|className|班级|query|false|string||
|combinedScoreLower|组合成绩下界|query|false|string||
|combinedScoreUpper|组合成绩上界|query|false|string||
|dispNum|显示数|query|false|integer(int64)||
|finishSchoolCode|毕业学校代码|query|false|string||
|hgroupCode|高中组代码|query|false|string||
|isAreaStudent|是否地段生|query|false|integer(int32)||
|isMilitaryStudent|是否优抚对象|query|false|integer(int32)||
|keepDir|保留显示定向|query|false|integer(int32)||
|keepGuide|保留显示指导|query|false|integer(int32)||
|keepInst|保留显示指令|query|false|integer(int32)||
|keepMakeup|保留显示补录|query|false|integer(int32)||
|keepNotSelected|保留显示不入围|query|false|integer(int32)||
|matriculateStatus|录取状态|query|false|integer(int32)||
|matriculateTimeLower|录取时间下界|query|false|string(date-time)||
|matriculateTimeUpper|录取时间上界|query|false|string(date-time)||
|mgroupCode|初中组代码|query|false|string||
|schoolType|高中类型|query|false|integer(int32)||
|sex|性别|query|false|string||
|signupSchoolCode|报考学校|query|false|string||
|signupStatus|报名状态|query|false|integer(int32)||
|signupTimeLower|报名时间下界|query|false|string(date-time)||
|signupTimeUpper|报名时间上界|query|false|string(date-time)||
|signupType|报考类型|query|false|string||
|singleScore|主科单科不低于|query|false|string||
|studentName|姓名|query|false|string||
|sumScoreLower|总成绩下界|query|false|string||
|sumScoreUpper|总成绩上界|query|false|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«MultiQueryResultVO»|
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|MultiQueryResultVO|MultiQueryResultVO|
|&emsp;&emsp;highestScore|最高分|string||
|&emsp;&emsp;matInfos|学生信息|array|MultiQueryStuMatVO|
|&emsp;&emsp;&emsp;&emsp;archiveCode|准考证号|string||
|&emsp;&emsp;&emsp;&emsp;calculateType|入围情况|string||
|&emsp;&emsp;&emsp;&emsp;chineseLevel|语文|string||
|&emsp;&emsp;&emsp;&emsp;chymistLevel|化学|string||
|&emsp;&emsp;&emsp;&emsp;className|班级|string||
|&emsp;&emsp;&emsp;&emsp;combinedScore|组合分|string||
|&emsp;&emsp;&emsp;&emsp;diathesis|综合素质|string||
|&emsp;&emsp;&emsp;&emsp;englishLevel|英语|string||
|&emsp;&emsp;&emsp;&emsp;experiment|实验|string||
|&emsp;&emsp;&emsp;&emsp;fillTime|报名时间|string||
|&emsp;&emsp;&emsp;&emsp;finishSchoolName|毕业学校|string||
|&emsp;&emsp;&emsp;&emsp;isAreaStudent|是否地段生|integer||
|&emsp;&emsp;&emsp;&emsp;isMilitary|是否优抚对象|integer||
|&emsp;&emsp;&emsp;&emsp;mathLevel|数学|string||
|&emsp;&emsp;&emsp;&emsp;matriculateStatus|录取状态|integer||
|&emsp;&emsp;&emsp;&emsp;matriculateTime|录取时间|string||
|&emsp;&emsp;&emsp;&emsp;matriculateType|录取类型|string||
|&emsp;&emsp;&emsp;&emsp;operator|操作员|string||
|&emsp;&emsp;&emsp;&emsp;physicsLevel|物理|string||
|&emsp;&emsp;&emsp;&emsp;politicsLevel|政史|string||
|&emsp;&emsp;&emsp;&emsp;remarkOfMatriculate|录取说明|string||
|&emsp;&emsp;&emsp;&emsp;serialNum|序号|integer||
|&emsp;&emsp;&emsp;&emsp;serialNumOfType|类型序号|integer||
|&emsp;&emsp;&emsp;&emsp;sex|性别|string||
|&emsp;&emsp;&emsp;&emsp;signUpType|报考类型|string||
|&emsp;&emsp;&emsp;&emsp;signupSchoolName|报考学校|string||
|&emsp;&emsp;&emsp;&emsp;studentKind|考生类别|string||
|&emsp;&emsp;&emsp;&emsp;studentName|学生姓名|string||
|&emsp;&emsp;&emsp;&emsp;sumScore|总分|string||
|&emsp;&emsp;&emsp;&emsp;winNo|窗口号|string||
|&emsp;&emsp;minimumScore|最低分|string||
|&emsp;&emsp;totalNum|记录数|integer(int32)||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": {
		"highestScore": "",
		"matInfos": [
			{
				"archiveCode": "",
				"calculateType": "",
				"chineseLevel": "",
				"chymistLevel": "",
				"className": "",
				"combinedScore": "",
				"diathesis": "",
				"englishLevel": "",
				"experiment": "",
				"fillTime": "",
				"finishSchoolName": "",
				"isAreaStudent": 0,
				"isMilitary": 0,
				"mathLevel": "",
				"matriculateStatus": 0,
				"matriculateTime": "",
				"matriculateType": "",
				"operator": "",
				"physicsLevel": "",
				"politicsLevel": "",
				"remarkOfMatriculate": "",
				"serialNum": 0,
				"serialNumOfType": 0,
				"sex": "",
				"signUpType": "",
				"signupSchoolName": "",
				"studentKind": "",
				"studentName": "",
				"sumScore": "",
				"winNo": ""
			}
		],
		"minimumScore": "",
		"totalNum": 0
	},
	"success": true,
	"timestamp": 0
}
```


## 多项查询-打印


**接口地址**:`/nnzk/base/queryStatistics/multiQueryPrint`


**请求方式**:`GET`


**请求数据类型**:`application/x-www-form-urlencoded`


**响应数据类型**:`*/*`


**接口描述**:<p>多项查询-打印</p>



**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|archiveCode|准考证号|query|false|string||
|areaCode|所属城区|query|false|string||
|className|班级|query|false|string||
|combinedScoreLower|组合成绩下界|query|false|string||
|combinedScoreUpper|组合成绩上界|query|false|string||
|dispNum|显示数|query|false|integer(int64)||
|finishSchoolCode|毕业学校代码|query|false|string||
|hgroupCode|高中组代码|query|false|string||
|isAreaStudent|是否地段生|query|false|integer(int32)||
|isMilitaryStudent|是否优抚对象|query|false|integer(int32)||
|keepDir|保留显示定向|query|false|integer(int32)||
|keepGuide|保留显示指导|query|false|integer(int32)||
|keepInst|保留显示指令|query|false|integer(int32)||
|keepMakeup|保留显示补录|query|false|integer(int32)||
|keepNotSelected|保留显示不入围|query|false|integer(int32)||
|matriculateStatus|录取状态|query|false|integer(int32)||
|matriculateTimeLower|录取时间下界|query|false|string(date-time)||
|matriculateTimeUpper|录取时间上界|query|false|string(date-time)||
|mgroupCode|初中组代码|query|false|string||
|schoolType|高中类型|query|false|integer(int32)||
|sex|性别|query|false|string||
|signupSchoolCode|报考学校|query|false|string||
|signupStatus|报名状态|query|false|integer(int32)||
|signupTimeLower|报名时间下界|query|false|string(date-time)||
|signupTimeUpper|报名时间上界|query|false|string(date-time)||
|signupType|报考类型|query|false|string||
|singleScore|主科单科不低于|query|false|string||
|studentName|姓名|query|false|string||
|sumScoreLower|总成绩下界|query|false|string||
|sumScoreUpper|总成绩上界|query|false|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|MultiQueryPrintOutputDTO|
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|count|总条数|integer(int32)|integer(int32)|
|data|数据列表|array|MultiQueryStuMatVO|
|&emsp;&emsp;archiveCode|准考证号|string||
|&emsp;&emsp;calculateType|入围情况|string||
|&emsp;&emsp;chineseLevel|语文|string||
|&emsp;&emsp;chymistLevel|化学|string||
|&emsp;&emsp;className|班级|string||
|&emsp;&emsp;combinedScore|组合分|string||
|&emsp;&emsp;diathesis|综合素质|string||
|&emsp;&emsp;englishLevel|英语|string||
|&emsp;&emsp;experiment|实验|string||
|&emsp;&emsp;fillTime|报名时间|string(date-time)||
|&emsp;&emsp;finishSchoolName|毕业学校|string||
|&emsp;&emsp;isAreaStudent|是否地段生|integer(int32)||
|&emsp;&emsp;isMilitary|是否优抚对象|integer(int32)||
|&emsp;&emsp;mathLevel|数学|string||
|&emsp;&emsp;matriculateStatus|录取状态|integer(int32)||
|&emsp;&emsp;matriculateTime|录取时间|string(date-time)||
|&emsp;&emsp;matriculateType|录取类型|string||
|&emsp;&emsp;operator|操作员|string||
|&emsp;&emsp;physicsLevel|物理|string||
|&emsp;&emsp;politicsLevel|政史|string||
|&emsp;&emsp;remarkOfMatriculate|录取说明|string||
|&emsp;&emsp;serialNum|序号|integer(int32)||
|&emsp;&emsp;serialNumOfType|类型序号|integer(int32)||
|&emsp;&emsp;sex|性别|string||
|&emsp;&emsp;signUpType|报考类型|string||
|&emsp;&emsp;signupSchoolName|报考学校|string||
|&emsp;&emsp;studentKind|考生类别|string||
|&emsp;&emsp;studentName|学生姓名|string||
|&emsp;&emsp;sumScore|总分|string||
|&emsp;&emsp;winNo|窗口号|string||
|total|总页数|integer(int32)|integer(int32)|


**响应示例**:
```javascript
{
	"count": 0,
	"data": [
		{
			"archiveCode": "",
			"calculateType": "",
			"chineseLevel": "",
			"chymistLevel": "",
			"className": "",
			"combinedScore": "",
			"diathesis": "",
			"englishLevel": "",
			"experiment": "",
			"fillTime": "",
			"finishSchoolName": "",
			"isAreaStudent": 0,
			"isMilitary": 0,
			"mathLevel": "",
			"matriculateStatus": 0,
			"matriculateTime": "",
			"matriculateType": "",
			"operator": "",
			"physicsLevel": "",
			"politicsLevel": "",
			"remarkOfMatriculate": "",
			"serialNum": 0,
			"serialNumOfType": 0,
			"sex": "",
			"signUpType": "",
			"signupSchoolName": "",
			"studentKind": "",
			"studentName": "",
			"sumScore": "",
			"winNo": ""
		}
	],
	"total": 0
}
```


## 内录查询


**接口地址**:`/nnzk/base/queryStatistics/privilegeQuery`


**请求方式**:`GET`


**请求数据类型**:`application/x-www-form-urlencoded`


**响应数据类型**:`*/*`


**接口描述**:<p>内录查询</p>



**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|archiveCode|准考证号|query|false|string||
|commandType|登记类型|query|false|string||
|finishSchoolCode|毕业学校|query|false|string||
|matriculateStatus|录取状态|query|false|integer(int32)||
|regStatus|登记状态|query|false|string||
|sex|性别|query|false|string||
|signupSchoolCode|报考学校|query|false|string||
|studentName|学生姓名|query|false|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«List«PrivilegeQueryVO»»|
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|array|PrivilegeQueryVO|
|&emsp;&emsp;archiveCode|准考证号|string||
|&emsp;&emsp;chineseLevel|语文|string||
|&emsp;&emsp;chymistLevel|化学|string||
|&emsp;&emsp;combinedScore|组合分|string||
|&emsp;&emsp;commandType|推荐类型|string||
|&emsp;&emsp;commander|推荐人|string||
|&emsp;&emsp;commanderPhone|推荐人电话|string||
|&emsp;&emsp;connector|联系单位或联系人|string||
|&emsp;&emsp;diathesis|综合素质|string||
|&emsp;&emsp;englishLevel|英语|string||
|&emsp;&emsp;experiment|实验|string||
|&emsp;&emsp;finishSchoolName|毕业学校|string||
|&emsp;&emsp;guardian|监护人|string||
|&emsp;&emsp;guardianPhone|监护人电话|string||
|&emsp;&emsp;mathLevel|数学|string||
|&emsp;&emsp;matriculateStatus|录取状态|integer(int32)||
|&emsp;&emsp;matriculateTime|录取时间|string(date-time)||
|&emsp;&emsp;physicsLevel|物理|string||
|&emsp;&emsp;politicsLevel|政史|string||
|&emsp;&emsp;registTime|登记时间|string(date-time)||
|&emsp;&emsp;registeDept|登记部门|string||
|&emsp;&emsp;schoolName|报考学校|string||
|&emsp;&emsp;serialNum|序号|integer(int32)||
|&emsp;&emsp;sex|性别|string||
|&emsp;&emsp;studentName|姓名|string||
|&emsp;&emsp;sumScore|总分|string||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": [
		{
			"archiveCode": "",
			"chineseLevel": "",
			"chymistLevel": "",
			"combinedScore": "",
			"commandType": "",
			"commander": "",
			"commanderPhone": "",
			"connector": "",
			"diathesis": "",
			"englishLevel": "",
			"experiment": "",
			"finishSchoolName": "",
			"guardian": "",
			"guardianPhone": "",
			"mathLevel": "",
			"matriculateStatus": 0,
			"matriculateTime": "",
			"physicsLevel": "",
			"politicsLevel": "",
			"registTime": "",
			"registeDept": "",
			"schoolName": "",
			"serialNum": 0,
			"sex": "",
			"studentName": "",
			"sumScore": ""
		}
	],
	"success": true,
	"timestamp": 0
}
```


## 内录查询-打印


**接口地址**:`/nnzk/base/queryStatistics/privilegeQueryPrint`


**请求方式**:`GET`


**请求数据类型**:`application/x-www-form-urlencoded`


**响应数据类型**:`*/*`


**接口描述**:<p>内录查询-打印</p>



**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|archiveCode|准考证号|query|false|string||
|commandType|登记类型|query|false|string||
|finishSchoolCode|毕业学校|query|false|string||
|matriculateStatus|录取状态|query|false|integer(int32)||
|regStatus|登记状态|query|false|string||
|sex|性别|query|false|string||
|signupSchoolCode|报考学校|query|false|string||
|studentName|学生姓名|query|false|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|PrivilegeQueryPrintOutputDTO|
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|count|总条数|integer(int32)|integer(int32)|
|data|数据列表|array|PrivilegeQueryVO|
|&emsp;&emsp;archiveCode|准考证号|string||
|&emsp;&emsp;chineseLevel|语文|string||
|&emsp;&emsp;chymistLevel|化学|string||
|&emsp;&emsp;combinedScore|组合分|string||
|&emsp;&emsp;commandType|推荐类型|string||
|&emsp;&emsp;commander|推荐人|string||
|&emsp;&emsp;commanderPhone|推荐人电话|string||
|&emsp;&emsp;connector|联系单位或联系人|string||
|&emsp;&emsp;diathesis|综合素质|string||
|&emsp;&emsp;englishLevel|英语|string||
|&emsp;&emsp;experiment|实验|string||
|&emsp;&emsp;finishSchoolName|毕业学校|string||
|&emsp;&emsp;guardian|监护人|string||
|&emsp;&emsp;guardianPhone|监护人电话|string||
|&emsp;&emsp;mathLevel|数学|string||
|&emsp;&emsp;matriculateStatus|录取状态|integer(int32)||
|&emsp;&emsp;matriculateTime|录取时间|string(date-time)||
|&emsp;&emsp;physicsLevel|物理|string||
|&emsp;&emsp;politicsLevel|政史|string||
|&emsp;&emsp;registTime|登记时间|string(date-time)||
|&emsp;&emsp;registeDept|登记部门|string||
|&emsp;&emsp;schoolName|报考学校|string||
|&emsp;&emsp;serialNum|序号|integer(int32)||
|&emsp;&emsp;sex|性别|string||
|&emsp;&emsp;studentName|姓名|string||
|&emsp;&emsp;sumScore|总分|string||
|total|总页数|integer(int32)|integer(int32)|


**响应示例**:
```javascript
{
	"count": 0,
	"data": [
		{
			"archiveCode": "",
			"chineseLevel": "",
			"chymistLevel": "",
			"combinedScore": "",
			"commandType": "",
			"commander": "",
			"commanderPhone": "",
			"connector": "",
			"diathesis": "",
			"englishLevel": "",
			"experiment": "",
			"finishSchoolName": "",
			"guardian": "",
			"guardianPhone": "",
			"mathLevel": "",
			"matriculateStatus": 0,
			"matriculateTime": "",
			"physicsLevel": "",
			"politicsLevel": "",
			"registTime": "",
			"registeDept": "",
			"schoolName": "",
			"serialNum": 0,
			"sex": "",
			"studentName": "",
			"sumScore": ""
		}
	],
	"total": 0
}
```


## 统计报表一


**接口地址**:`/nnzk/base/queryStatistics/queryReportOne`


**请求方式**:`GET`


**请求数据类型**:`application/x-www-form-urlencoded`


**响应数据类型**:`*/*`


**接口描述**:<p>统计报表一</p>



**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|schoolCodeList|schoolCodeList|query|false|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«List«QueryStatisticsOneVO»»|
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|array|QueryStatisticsOneVO|
|&emsp;&emsp;allPlanNum|计划人数合计|integer(int32)||
|&emsp;&emsp;allRealNum|实际人数合计|integer(int32)||
|&emsp;&emsp;altLine|定向空余最低成绩|string||
|&emsp;&emsp;altPlanNum|定向空余空缺名额|integer(int32)||
|&emsp;&emsp;altRealNum|定向空余实际人数|integer(int32)||
|&emsp;&emsp;classNum|拟招班数|integer(int32)||
|&emsp;&emsp;dirLine|指令定向最低成绩|string||
|&emsp;&emsp;dirPlanNum|指令定向计划人数|integer(int32)||
|&emsp;&emsp;dirRealNum|指令定向实际人数|integer(int32)||
|&emsp;&emsp;guiLine|指导最低成绩|string||
|&emsp;&emsp;guiPlanNum|指导计划人数|integer(int32)||
|&emsp;&emsp;guiRealNum|指导实际人数|integer(int32)||
|&emsp;&emsp;insPlanNum|指令非定向计划人数|integer(int32)||
|&emsp;&emsp;insRealNum|指令非定向实际人数|integer(int32)||
|&emsp;&emsp;instLine|指令非定向最低成绩|string||
|&emsp;&emsp;schoolName|学校名称|string||
|&emsp;&emsp;serialNum|序号|integer(int32)||
|&emsp;&emsp;speLine|特长生最低成绩|string||
|&emsp;&emsp;spePlanNum|特长生计划人数|integer(int32)||
|&emsp;&emsp;speRealNum|特长生实际人数|integer(int32)||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": [
		{
			"allPlanNum": 0,
			"allRealNum": 0,
			"altLine": "",
			"altPlanNum": 0,
			"altRealNum": 0,
			"classNum": 0,
			"dirLine": "",
			"dirPlanNum": 0,
			"dirRealNum": 0,
			"guiLine": "",
			"guiPlanNum": 0,
			"guiRealNum": 0,
			"insPlanNum": 0,
			"insRealNum": 0,
			"instLine": "",
			"schoolName": "",
			"serialNum": 0,
			"speLine": "",
			"spePlanNum": 0,
			"speRealNum": 0
		}
	],
	"success": true,
	"timestamp": 0
}
```


## 统计报表一-打印


**接口地址**:`/nnzk/base/queryStatistics/queryReportOnePrint`


**请求方式**:`GET`


**请求数据类型**:`application/x-www-form-urlencoded`


**响应数据类型**:`*/*`


**接口描述**:<p>统计报表一-打印</p>



**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|schoolCodeList|schoolCodeList|query|false|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|QueryReportOnePrintOutputDTO|
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|count|总条数|integer(int32)|integer(int32)|
|data|数据列表|array|QueryStatisticsOneVO|
|&emsp;&emsp;allPlanNum|计划人数合计|integer(int32)||
|&emsp;&emsp;allRealNum|实际人数合计|integer(int32)||
|&emsp;&emsp;altLine|定向空余最低成绩|string||
|&emsp;&emsp;altPlanNum|定向空余空缺名额|integer(int32)||
|&emsp;&emsp;altRealNum|定向空余实际人数|integer(int32)||
|&emsp;&emsp;classNum|拟招班数|integer(int32)||
|&emsp;&emsp;dirLine|指令定向最低成绩|string||
|&emsp;&emsp;dirPlanNum|指令定向计划人数|integer(int32)||
|&emsp;&emsp;dirRealNum|指令定向实际人数|integer(int32)||
|&emsp;&emsp;guiLine|指导最低成绩|string||
|&emsp;&emsp;guiPlanNum|指导计划人数|integer(int32)||
|&emsp;&emsp;guiRealNum|指导实际人数|integer(int32)||
|&emsp;&emsp;insPlanNum|指令非定向计划人数|integer(int32)||
|&emsp;&emsp;insRealNum|指令非定向实际人数|integer(int32)||
|&emsp;&emsp;instLine|指令非定向最低成绩|string||
|&emsp;&emsp;schoolName|学校名称|string||
|&emsp;&emsp;serialNum|序号|integer(int32)||
|&emsp;&emsp;speLine|特长生最低成绩|string||
|&emsp;&emsp;spePlanNum|特长生计划人数|integer(int32)||
|&emsp;&emsp;speRealNum|特长生实际人数|integer(int32)||
|total|总页数|integer(int32)|integer(int32)|


**响应示例**:
```javascript
{
	"count": 0,
	"data": [
		{
			"allPlanNum": 0,
			"allRealNum": 0,
			"altLine": "",
			"altPlanNum": 0,
			"altRealNum": 0,
			"classNum": 0,
			"dirLine": "",
			"dirPlanNum": 0,
			"dirRealNum": 0,
			"guiLine": "",
			"guiPlanNum": 0,
			"guiRealNum": 0,
			"insPlanNum": 0,
			"insRealNum": 0,
			"instLine": "",
			"schoolName": "",
			"serialNum": 0,
			"speLine": "",
			"spePlanNum": 0,
			"speRealNum": 0
		}
	],
	"total": 0
}
```


## 统计报表三


**接口地址**:`/nnzk/base/queryStatistics/queryReportThree`


**请求方式**:`GET`


**请求数据类型**:`application/x-www-form-urlencoded`


**响应数据类型**:`*/*`


**接口描述**:<p>统计报表三</p>



**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|schoolCodeList|schoolCodeList|query|false|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«List«QueryStatisticsThreeVO»»|
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|array|QueryStatisticsThreeVO|
|&emsp;&emsp;altPlanNum|定向空余-空缺名额|integer(int32)||
|&emsp;&emsp;altRealNum|定向空余-实际人数|integer(int32)||
|&emsp;&emsp;classNum|拟招班数|integer(int32)||
|&emsp;&emsp;classNum2|合计-班额|string||
|&emsp;&emsp;dirPlanNum|指令定向-计划人数|integer(int32)||
|&emsp;&emsp;dirRealNum|指令定向-实际人数|integer(int32)||
|&emsp;&emsp;guiPlanNum|指导-计划人数|integer(int32)||
|&emsp;&emsp;guiRealNum|指导-实际人数|integer(int32)||
|&emsp;&emsp;innerRealNum|本市其他-实际录取|integer(int32)||
|&emsp;&emsp;insPlanNum|指令非定向-计划人数|integer(int32)||
|&emsp;&emsp;insRealNum|指令非定向-实际人数|integer(int32)||
|&emsp;&emsp;outlandRealNum|外地生-实际录取|integer(int32)||
|&emsp;&emsp;planAllNum|小计-计划人数|integer(int32)||
|&emsp;&emsp;realAllNum|小计-实际人数|integer(int32)||
|&emsp;&emsp;realAllNum2|合计-实际录取|integer(int32)||
|&emsp;&emsp;schoolCode|学校代码|string||
|&emsp;&emsp;schoolName|学生名称|string||
|&emsp;&emsp;serialNum|序号|integer(int32)||
|&emsp;&emsp;spePlanNum|特长生-计划人数|integer(int32)||
|&emsp;&emsp;speRealNum|特长生-实际人数|integer(int32)||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": [
		{
			"altPlanNum": 0,
			"altRealNum": 0,
			"classNum": 0,
			"classNum2": "",
			"dirPlanNum": 0,
			"dirRealNum": 0,
			"guiPlanNum": 0,
			"guiRealNum": 0,
			"innerRealNum": 0,
			"insPlanNum": 0,
			"insRealNum": 0,
			"outlandRealNum": 0,
			"planAllNum": 0,
			"realAllNum": 0,
			"realAllNum2": 0,
			"schoolCode": "",
			"schoolName": "",
			"serialNum": 0,
			"spePlanNum": 0,
			"speRealNum": 0
		}
	],
	"success": true,
	"timestamp": 0
}
```


## 统计报表三-打印


**接口地址**:`/nnzk/base/queryStatistics/queryReportThreePrint`


**请求方式**:`GET`


**请求数据类型**:`application/x-www-form-urlencoded`


**响应数据类型**:`*/*`


**接口描述**:<p>统计报表三-打印</p>



**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|schoolCodeList|schoolCodeList|query|false|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|QueryReportThreePrintOutputDTO|
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|count|总条数|integer(int32)|integer(int32)|
|data|数据列表|array|QueryStatisticsThreeVO|
|&emsp;&emsp;altPlanNum|定向空余-空缺名额|integer(int32)||
|&emsp;&emsp;altRealNum|定向空余-实际人数|integer(int32)||
|&emsp;&emsp;classNum|拟招班数|integer(int32)||
|&emsp;&emsp;classNum2|合计-班额|string||
|&emsp;&emsp;dirPlanNum|指令定向-计划人数|integer(int32)||
|&emsp;&emsp;dirRealNum|指令定向-实际人数|integer(int32)||
|&emsp;&emsp;guiPlanNum|指导-计划人数|integer(int32)||
|&emsp;&emsp;guiRealNum|指导-实际人数|integer(int32)||
|&emsp;&emsp;innerRealNum|本市其他-实际录取|integer(int32)||
|&emsp;&emsp;insPlanNum|指令非定向-计划人数|integer(int32)||
|&emsp;&emsp;insRealNum|指令非定向-实际人数|integer(int32)||
|&emsp;&emsp;outlandRealNum|外地生-实际录取|integer(int32)||
|&emsp;&emsp;planAllNum|小计-计划人数|integer(int32)||
|&emsp;&emsp;realAllNum|小计-实际人数|integer(int32)||
|&emsp;&emsp;realAllNum2|合计-实际录取|integer(int32)||
|&emsp;&emsp;schoolCode|学校代码|string||
|&emsp;&emsp;schoolName|学生名称|string||
|&emsp;&emsp;serialNum|序号|integer(int32)||
|&emsp;&emsp;spePlanNum|特长生-计划人数|integer(int32)||
|&emsp;&emsp;speRealNum|特长生-实际人数|integer(int32)||
|total|总页数|integer(int32)|integer(int32)|


**响应示例**:
```javascript
{
	"count": 0,
	"data": [
		{
			"altPlanNum": 0,
			"altRealNum": 0,
			"classNum": 0,
			"classNum2": "",
			"dirPlanNum": 0,
			"dirRealNum": 0,
			"guiPlanNum": 0,
			"guiRealNum": 0,
			"innerRealNum": 0,
			"insPlanNum": 0,
			"insRealNum": 0,
			"outlandRealNum": 0,
			"planAllNum": 0,
			"realAllNum": 0,
			"realAllNum2": 0,
			"schoolCode": "",
			"schoolName": "",
			"serialNum": 0,
			"spePlanNum": 0,
			"speRealNum": 0
		}
	],
	"total": 0
}
```


## 统计报表-登记


**接口地址**:`/nnzk/base/queryStatistics/reportOfReg`


**请求方式**:`GET`


**请求数据类型**:`application/x-www-form-urlencoded`


**响应数据类型**:`*/*`


**接口描述**:<p>统计报表-登记</p>



**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|schoolCodeList|schoolCodeList|query|false|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«List«ReportOfRegVO»»|
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|array|ReportOfRegVO|
|&emsp;&emsp;adjustNum|调剂数|integer(int32)||
|&emsp;&emsp;allNum|调剂名额情况-调剂招生空额|integer(int32)||
|&emsp;&emsp;classNum|班数|integer(int32)||
|&emsp;&emsp;disNum|调剂名额情况-可用空额|integer(int32)||
|&emsp;&emsp;gjb|学校特招-国际班|integer(int32)||
|&emsp;&emsp;hzb|学校特招-宏志班|integer(int32)||
|&emsp;&emsp;local|调剂名额情况-本市其他已用|integer(int32)||
|&emsp;&emsp;mzb|学校特招-民族班|integer(int32)||
|&emsp;&emsp;outland|调剂名额情况-外地生已用|integer(int32)||
|&emsp;&emsp;schoolCode|学校代码|string||
|&emsp;&emsp;schoolName|学校名称|string||
|&emsp;&emsp;serialNum|序号|integer(int32)||
|&emsp;&emsp;sumNum|调剂名额情况-小计|integer(int32)||
|&emsp;&emsp;wdb|学校特招-外地生班|integer(int32)||
|&emsp;&emsp;zzb|学校特招-珍珠班|integer(int32)||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": [
		{
			"adjustNum": 0,
			"allNum": 0,
			"classNum": 0,
			"disNum": 0,
			"gjb": 0,
			"hzb": 0,
			"local": 0,
			"mzb": 0,
			"outland": 0,
			"schoolCode": "",
			"schoolName": "",
			"serialNum": 0,
			"sumNum": 0,
			"wdb": 0,
			"zzb": 0
		}
	],
	"success": true,
	"timestamp": 0
}
```


## 统计报表-登记-打印


**接口地址**:`/nnzk/base/queryStatistics/reportOfRegPrint`


**请求方式**:`GET`


**请求数据类型**:`application/x-www-form-urlencoded`


**响应数据类型**:`*/*`


**接口描述**:<p>统计报表-登记-打印</p>



**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|schoolCodeList|schoolCodeList|query|false|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|ReportOfRegPrintOutputDTO|
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|count|总条数|integer(int32)|integer(int32)|
|data|数据列表|array|ReportOfRegVO|
|&emsp;&emsp;adjustNum|调剂数|integer(int32)||
|&emsp;&emsp;allNum|调剂名额情况-调剂招生空额|integer(int32)||
|&emsp;&emsp;classNum|班数|integer(int32)||
|&emsp;&emsp;disNum|调剂名额情况-可用空额|integer(int32)||
|&emsp;&emsp;gjb|学校特招-国际班|integer(int32)||
|&emsp;&emsp;hzb|学校特招-宏志班|integer(int32)||
|&emsp;&emsp;local|调剂名额情况-本市其他已用|integer(int32)||
|&emsp;&emsp;mzb|学校特招-民族班|integer(int32)||
|&emsp;&emsp;outland|调剂名额情况-外地生已用|integer(int32)||
|&emsp;&emsp;schoolCode|学校代码|string||
|&emsp;&emsp;schoolName|学校名称|string||
|&emsp;&emsp;serialNum|序号|integer(int32)||
|&emsp;&emsp;sumNum|调剂名额情况-小计|integer(int32)||
|&emsp;&emsp;wdb|学校特招-外地生班|integer(int32)||
|&emsp;&emsp;zzb|学校特招-珍珠班|integer(int32)||
|total|总页数|integer(int32)|integer(int32)|


**响应示例**:
```javascript
{
	"count": 0,
	"data": [
		{
			"adjustNum": 0,
			"allNum": 0,
			"classNum": 0,
			"disNum": 0,
			"gjb": 0,
			"hzb": 0,
			"local": 0,
			"mzb": 0,
			"outland": 0,
			"schoolCode": "",
			"schoolName": "",
			"serialNum": 0,
			"sumNum": 0,
			"wdb": 0,
			"zzb": 0
		}
	],
	"total": 0
}
```


## 导出名单


**接口地址**:`/nnzk/base/queryStatistics/schMatReport`


**请求方式**:`GET`


**请求数据类型**:`application/x-www-form-urlencoded`


**响应数据类型**:`*/*`


**接口描述**:<p>导出名单</p>



**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|schoolCode|schoolCode|query|true|string||
|removeFormalMat|removeFormalMat|query|false|boolean||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«List«HighSchoolMatReportVO»»|
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|array|HighSchoolMatReportVO|
|&emsp;&emsp;archiveCode|准考证号|string||
|&emsp;&emsp;chineseLevel|语文|string||
|&emsp;&emsp;chymistLevel|化学|string||
|&emsp;&emsp;combinedScore|组合分|string||
|&emsp;&emsp;englishLevel|英语|string||
|&emsp;&emsp;mathLevel|数学|string||
|&emsp;&emsp;matriculateStatus|是否录取|integer(int32)||
|&emsp;&emsp;matriculateType1|录取类型|string||
|&emsp;&emsp;physicsLevel|物理|string||
|&emsp;&emsp;politicsLevel|政史|string||
|&emsp;&emsp;schoolName|学校名称|string||
|&emsp;&emsp;serialNum|序号|integer(int32)||
|&emsp;&emsp;sex|性别|string||
|&emsp;&emsp;signUpType|报考类型|string||
|&emsp;&emsp;studentName|学生姓名|string||
|&emsp;&emsp;sum_score|总分|string||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": [
		{
			"archiveCode": "",
			"chineseLevel": "",
			"chymistLevel": "",
			"combinedScore": "",
			"englishLevel": "",
			"mathLevel": "",
			"matriculateStatus": 0,
			"matriculateType1": "",
			"physicsLevel": "",
			"politicsLevel": "",
			"schoolName": "",
			"serialNum": 0,
			"sex": "",
			"signUpType": "",
			"studentName": "",
			"sum_score": ""
		}
	],
	"success": true,
	"timestamp": 0
}
```


## 导出名单-打印


**接口地址**:`/nnzk/base/queryStatistics/schMatReportPrint`


**请求方式**:`GET`


**请求数据类型**:`application/x-www-form-urlencoded`


**响应数据类型**:`*/*`


**接口描述**:<p>导出名单-打印</p>



**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|schoolCode|schoolCode|query|true|string||
|removeFormalMat|removeFormalMat|query|false|boolean||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|SchMatReportPrintOutputDTO|
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|count|总条数|integer(int32)|integer(int32)|
|data|数据列表|array|HighSchoolMatReportVO|
|&emsp;&emsp;archiveCode|准考证号|string||
|&emsp;&emsp;chineseLevel|语文|string||
|&emsp;&emsp;chymistLevel|化学|string||
|&emsp;&emsp;combinedScore|组合分|string||
|&emsp;&emsp;englishLevel|英语|string||
|&emsp;&emsp;mathLevel|数学|string||
|&emsp;&emsp;matriculateStatus|是否录取|integer(int32)||
|&emsp;&emsp;matriculateType1|录取类型|string||
|&emsp;&emsp;physicsLevel|物理|string||
|&emsp;&emsp;politicsLevel|政史|string||
|&emsp;&emsp;schoolName|学校名称|string||
|&emsp;&emsp;serialNum|序号|integer(int32)||
|&emsp;&emsp;sex|性别|string||
|&emsp;&emsp;signUpType|报考类型|string||
|&emsp;&emsp;studentName|学生姓名|string||
|&emsp;&emsp;sum_score|总分|string||
|total|总页数|integer(int32)|integer(int32)|


**响应示例**:
```javascript
{
	"count": 0,
	"data": [
		{
			"archiveCode": "",
			"chineseLevel": "",
			"chymistLevel": "",
			"combinedScore": "",
			"englishLevel": "",
			"mathLevel": "",
			"matriculateStatus": 0,
			"matriculateType1": "",
			"physicsLevel": "",
			"politicsLevel": "",
			"schoolName": "",
			"serialNum": 0,
			"sex": "",
			"signUpType": "",
			"studentName": "",
			"sum_score": ""
		}
	],
	"total": 0
}
```


## 统计报表


**接口地址**:`/nnzk/base/queryStatistics/statisticReport`


**请求方式**:`GET`


**请求数据类型**:`application/x-www-form-urlencoded`


**响应数据类型**:`*/*`


**接口描述**:<p>统计报表</p>



**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|scriptName|scriptName|query|true|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«List«Map«string,object»»»|
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|array||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": [],
	"success": true,
	"timestamp": 0
}
```


## 统计报表-打印


**接口地址**:`/nnzk/base/queryStatistics/statisticReportPrint`


**请求方式**:`GET`


**请求数据类型**:`application/x-www-form-urlencoded`


**响应数据类型**:`*/*`


**接口描述**:<p>统计报表-打印</p>



**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|scriptName|scriptName|query|true|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|StatisticReportPrintOutputDTO|
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|count|总条数|integer(int32)|integer(int32)|
|data|数据列表|array||
|total|总页数|integer(int32)|integer(int32)|


**响应示例**:
```javascript
{
	"count": 0,
	"data": [],
	"total": 0
}
```


# 民办学校补录数据表


## 民办学校补录数据表-添加


**接口地址**:`/nnzk/alter/makeUpApplication/add`


**请求方式**:`POST`


**请求数据类型**:`application/json`


**响应数据类型**:`*/*`


**接口描述**:<p>民办学校补录数据表-添加</p>



**请求示例**:


```javascript
{
  "annexUrl": "",
  "applicationTime": "",
  "createBy": "",
  "createTime": "",
  "delFlag": 0,
  "id": "",
  "makeUpDataStatus": 0,
  "makeUpNum": 0,
  "makeUpPeopleNum": 0,
  "schoolCode": "",
  "schoolName": "",
  "updateBy": "",
  "updateTime": ""
}
```


**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|makeUpApplication|民办学校补录数据表|body|true|make_up_application对象|make_up_application对象|
|&emsp;&emsp;annexUrl|附件url||false|string||
|&emsp;&emsp;applicationTime|申请时间||false|string(date-time)||
|&emsp;&emsp;createBy|创建人||false|string||
|&emsp;&emsp;createTime|创建日期||false|string(date-time)||
|&emsp;&emsp;delFlag|删除标识||false|integer(int32)||
|&emsp;&emsp;id|主键||false|string||
|&emsp;&emsp;makeUpDataStatus|状态||false|integer(int32)||
|&emsp;&emsp;makeUpNum|补录次数||false|integer(int32)||
|&emsp;&emsp;makeUpPeopleNum|补录人数||false|integer(int32)||
|&emsp;&emsp;schoolCode|学校代码||false|string||
|&emsp;&emsp;schoolName|学校名称||false|string||
|&emsp;&emsp;updateBy|更新人||false|string||
|&emsp;&emsp;updateTime|更新日期||false|string(date-time)||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«string»|
|201|Created||
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|string||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": "",
	"success": true,
	"timestamp": 0
}
```


## 民办学校补录数据表-通过id删除


**接口地址**:`/nnzk/alter/makeUpApplication/delete`


**请求方式**:`DELETE`


**请求数据类型**:`application/x-www-form-urlencoded`


**响应数据类型**:`*/*`


**接口描述**:<p>民办学校补录数据表-通过id删除</p>



**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|id|id|query|true|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«string»|
|204|No Content||
|401|Unauthorized||
|403|Forbidden||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|string||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": "",
	"success": true,
	"timestamp": 0
}
```


## 民办学校补录数据表-批量删除


**接口地址**:`/nnzk/alter/makeUpApplication/deleteBatch`


**请求方式**:`DELETE`


**请求数据类型**:`application/x-www-form-urlencoded`


**响应数据类型**:`*/*`


**接口描述**:<p>民办学校补录数据表-批量删除</p>



**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|ids|ids|query|true|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«string»|
|204|No Content||
|401|Unauthorized||
|403|Forbidden||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|string||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": "",
	"success": true,
	"timestamp": 0
}
```


## 民办学校补录数据表-编辑


**接口地址**:`/nnzk/alter/makeUpApplication/edit`


**请求方式**:`POST`


**请求数据类型**:`application/json`


**响应数据类型**:`*/*`


**接口描述**:<p>民办学校补录数据表-编辑</p>



**请求示例**:


```javascript
{
  "annexUrl": "",
  "applicationTime": "",
  "createBy": "",
  "createTime": "",
  "delFlag": 0,
  "id": "",
  "makeUpDataStatus": 0,
  "makeUpNum": 0,
  "makeUpPeopleNum": 0,
  "schoolCode": "",
  "schoolName": "",
  "updateBy": "",
  "updateTime": ""
}
```


**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|makeUpApplication|民办学校补录数据表|body|true|make_up_application对象|make_up_application对象|
|&emsp;&emsp;annexUrl|附件url||false|string||
|&emsp;&emsp;applicationTime|申请时间||false|string(date-time)||
|&emsp;&emsp;createBy|创建人||false|string||
|&emsp;&emsp;createTime|创建日期||false|string(date-time)||
|&emsp;&emsp;delFlag|删除标识||false|integer(int32)||
|&emsp;&emsp;id|主键||false|string||
|&emsp;&emsp;makeUpDataStatus|状态||false|integer(int32)||
|&emsp;&emsp;makeUpNum|补录次数||false|integer(int32)||
|&emsp;&emsp;makeUpPeopleNum|补录人数||false|integer(int32)||
|&emsp;&emsp;schoolCode|学校代码||false|string||
|&emsp;&emsp;schoolName|学校名称||false|string||
|&emsp;&emsp;updateBy|更新人||false|string||
|&emsp;&emsp;updateTime|更新日期||false|string(date-time)||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«string»|
|201|Created||
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|string||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": "",
	"success": true,
	"timestamp": 0
}
```


## 民办学校补录数据表-编辑


**接口地址**:`/nnzk/alter/makeUpApplication/edit`


**请求方式**:`PUT`


**请求数据类型**:`application/json`


**响应数据类型**:`*/*`


**接口描述**:<p>民办学校补录数据表-编辑</p>



**请求示例**:


```javascript
{
  "annexUrl": "",
  "applicationTime": "",
  "createBy": "",
  "createTime": "",
  "delFlag": 0,
  "id": "",
  "makeUpDataStatus": 0,
  "makeUpNum": 0,
  "makeUpPeopleNum": 0,
  "schoolCode": "",
  "schoolName": "",
  "updateBy": "",
  "updateTime": ""
}
```


**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|makeUpApplication|民办学校补录数据表|body|true|make_up_application对象|make_up_application对象|
|&emsp;&emsp;annexUrl|附件url||false|string||
|&emsp;&emsp;applicationTime|申请时间||false|string(date-time)||
|&emsp;&emsp;createBy|创建人||false|string||
|&emsp;&emsp;createTime|创建日期||false|string(date-time)||
|&emsp;&emsp;delFlag|删除标识||false|integer(int32)||
|&emsp;&emsp;id|主键||false|string||
|&emsp;&emsp;makeUpDataStatus|状态||false|integer(int32)||
|&emsp;&emsp;makeUpNum|补录次数||false|integer(int32)||
|&emsp;&emsp;makeUpPeopleNum|补录人数||false|integer(int32)||
|&emsp;&emsp;schoolCode|学校代码||false|string||
|&emsp;&emsp;schoolName|学校名称||false|string||
|&emsp;&emsp;updateBy|更新人||false|string||
|&emsp;&emsp;updateTime|更新日期||false|string(date-time)||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«string»|
|201|Created||
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|string||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": "",
	"success": true,
	"timestamp": 0
}
```


## 民办学校补录数据表-分页列表查询


**接口地址**:`/nnzk/alter/makeUpApplication/list`


**请求方式**:`GET`


**请求数据类型**:`application/x-www-form-urlencoded`


**响应数据类型**:`*/*`


**接口描述**:<p>民办学校补录数据表-分页列表查询</p>



**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|annexUrl|附件url|query|false|string||
|applicationTime|申请时间|query|false|string(date-time)||
|createBy|创建人|query|false|string||
|createTime|创建日期|query|false|string(date-time)||
|delFlag|删除标识|query|false|integer(int32)||
|id|主键|query|false|string||
|makeUpDataStatus|状态|query|false|integer(int32)||
|makeUpNum|补录次数|query|false|integer(int32)||
|makeUpPeopleNum|补录人数|query|false|integer(int32)||
|pageNo|pageNo|query|false|integer(int32)||
|pageSize|pageSize|query|false|integer(int32)||
|schoolCode|学校代码|query|false|string||
|schoolName|学校名称|query|false|string||
|updateBy|更新人|query|false|string||
|updateTime|更新日期|query|false|string(date-time)||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«IPage«make_up_application对象»»|
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|IPage«make_up_application对象»|IPage«make_up_application对象»|
|&emsp;&emsp;current||integer(int64)||
|&emsp;&emsp;pages||integer(int64)||
|&emsp;&emsp;records||array|make_up_application对象|
|&emsp;&emsp;&emsp;&emsp;annexUrl|附件url|string||
|&emsp;&emsp;&emsp;&emsp;applicationTime|申请时间|string||
|&emsp;&emsp;&emsp;&emsp;createBy|创建人|string||
|&emsp;&emsp;&emsp;&emsp;createTime|创建日期|string||
|&emsp;&emsp;&emsp;&emsp;delFlag|删除标识|integer||
|&emsp;&emsp;&emsp;&emsp;id|主键|string||
|&emsp;&emsp;&emsp;&emsp;makeUpDataStatus|状态|integer||
|&emsp;&emsp;&emsp;&emsp;makeUpNum|补录次数|integer||
|&emsp;&emsp;&emsp;&emsp;makeUpPeopleNum|补录人数|integer||
|&emsp;&emsp;&emsp;&emsp;schoolCode|学校代码|string||
|&emsp;&emsp;&emsp;&emsp;schoolName|学校名称|string||
|&emsp;&emsp;&emsp;&emsp;updateBy|更新人|string||
|&emsp;&emsp;&emsp;&emsp;updateTime|更新日期|string||
|&emsp;&emsp;size||integer(int64)||
|&emsp;&emsp;total||integer(int64)||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": {
		"current": 0,
		"pages": 0,
		"records": [
			{
				"annexUrl": "",
				"applicationTime": "",
				"createBy": "",
				"createTime": "",
				"delFlag": 0,
				"id": "",
				"makeUpDataStatus": 0,
				"makeUpNum": 0,
				"makeUpPeopleNum": 0,
				"schoolCode": "",
				"schoolName": "",
				"updateBy": "",
				"updateTime": ""
			}
		],
		"size": 0,
		"total": 0
	},
	"success": true,
	"timestamp": 0
}
```


## 民办学校补录数据表-通过id查询


**接口地址**:`/nnzk/alter/makeUpApplication/queryById`


**请求方式**:`GET`


**请求数据类型**:`application/x-www-form-urlencoded`


**响应数据类型**:`*/*`


**接口描述**:<p>民办学校补录数据表-通过id查询</p>



**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|id|id|query|true|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«make_up_application对象»|
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|make_up_application对象|make_up_application对象|
|&emsp;&emsp;annexUrl|附件url|string||
|&emsp;&emsp;applicationTime|申请时间|string(date-time)||
|&emsp;&emsp;createBy|创建人|string||
|&emsp;&emsp;createTime|创建日期|string(date-time)||
|&emsp;&emsp;delFlag|删除标识|integer(int32)||
|&emsp;&emsp;id|主键|string||
|&emsp;&emsp;makeUpDataStatus|状态|integer(int32)||
|&emsp;&emsp;makeUpNum|补录次数|integer(int32)||
|&emsp;&emsp;makeUpPeopleNum|补录人数|integer(int32)||
|&emsp;&emsp;schoolCode|学校代码|string||
|&emsp;&emsp;schoolName|学校名称|string||
|&emsp;&emsp;updateBy|更新人|string||
|&emsp;&emsp;updateTime|更新日期|string(date-time)||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": {
		"annexUrl": "",
		"applicationTime": "",
		"createBy": "",
		"createTime": "",
		"delFlag": 0,
		"id": "",
		"makeUpDataStatus": 0,
		"makeUpNum": 0,
		"makeUpPeopleNum": 0,
		"schoolCode": "",
		"schoolName": "",
		"updateBy": "",
		"updateTime": ""
	},
	"success": true,
	"timestamp": 0
}
```


# 特招班


## 特招班-添加


**接口地址**:`/nnzk/PrivilegeClassSetting/privilegeClass/add`


**请求方式**:`POST`


**请求数据类型**:`application/json`


**响应数据类型**:`*/*`


**接口描述**:<p>特招班-添加</p>



**请求示例**:


```javascript
{
  "classId": "",
  "className": "",
  "createBy": "",
  "createTime": "",
  "dispOrder": "",
  "id": "",
  "matType": "",
  "studentType": "",
  "updateBy": "",
  "updateTime": ""
}
```


**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|privilegeClass|特招班|body|true|privilege_class对象|privilege_class对象|
|&emsp;&emsp;classId|编码||false|string||
|&emsp;&emsp;className|名称||false|string||
|&emsp;&emsp;createBy|创建人||false|string||
|&emsp;&emsp;createTime|创建日期||false|string(date-time)||
|&emsp;&emsp;dispOrder|排序码||false|string||
|&emsp;&emsp;id|主键||false|string||
|&emsp;&emsp;matType|录取类型||false|string||
|&emsp;&emsp;studentType|生源||false|string||
|&emsp;&emsp;updateBy|更新人||false|string||
|&emsp;&emsp;updateTime|更新日期||false|string(date-time)||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«string»|
|201|Created||
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|string||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": "",
	"success": true,
	"timestamp": 0
}
```


## 特招班-通过id删除


**接口地址**:`/nnzk/PrivilegeClassSetting/privilegeClass/delete`


**请求方式**:`DELETE`


**请求数据类型**:`application/x-www-form-urlencoded`


**响应数据类型**:`*/*`


**接口描述**:<p>特招班-通过id删除</p>



**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|id|id|query|true|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«string»|
|204|No Content||
|401|Unauthorized||
|403|Forbidden||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|string||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": "",
	"success": true,
	"timestamp": 0
}
```


## 特招班-批量删除


**接口地址**:`/nnzk/PrivilegeClassSetting/privilegeClass/deleteBatch`


**请求方式**:`DELETE`


**请求数据类型**:`application/x-www-form-urlencoded`


**响应数据类型**:`*/*`


**接口描述**:<p>特招班-批量删除</p>



**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|ids|ids|query|true|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«string»|
|204|No Content||
|401|Unauthorized||
|403|Forbidden||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|string||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": "",
	"success": true,
	"timestamp": 0
}
```


## 特招班-编辑


**接口地址**:`/nnzk/PrivilegeClassSetting/privilegeClass/edit`


**请求方式**:`POST`


**请求数据类型**:`application/json`


**响应数据类型**:`*/*`


**接口描述**:<p>特招班-编辑</p>



**请求示例**:


```javascript
{
  "classId": "",
  "className": "",
  "createBy": "",
  "createTime": "",
  "dispOrder": "",
  "id": "",
  "matType": "",
  "studentType": "",
  "updateBy": "",
  "updateTime": ""
}
```


**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|privilegeClass|特招班|body|true|privilege_class对象|privilege_class对象|
|&emsp;&emsp;classId|编码||false|string||
|&emsp;&emsp;className|名称||false|string||
|&emsp;&emsp;createBy|创建人||false|string||
|&emsp;&emsp;createTime|创建日期||false|string(date-time)||
|&emsp;&emsp;dispOrder|排序码||false|string||
|&emsp;&emsp;id|主键||false|string||
|&emsp;&emsp;matType|录取类型||false|string||
|&emsp;&emsp;studentType|生源||false|string||
|&emsp;&emsp;updateBy|更新人||false|string||
|&emsp;&emsp;updateTime|更新日期||false|string(date-time)||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«string»|
|201|Created||
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|string||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": "",
	"success": true,
	"timestamp": 0
}
```


## 特招班-编辑


**接口地址**:`/nnzk/PrivilegeClassSetting/privilegeClass/edit`


**请求方式**:`PUT`


**请求数据类型**:`application/json`


**响应数据类型**:`*/*`


**接口描述**:<p>特招班-编辑</p>



**请求示例**:


```javascript
{
  "classId": "",
  "className": "",
  "createBy": "",
  "createTime": "",
  "dispOrder": "",
  "id": "",
  "matType": "",
  "studentType": "",
  "updateBy": "",
  "updateTime": ""
}
```


**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|privilegeClass|特招班|body|true|privilege_class对象|privilege_class对象|
|&emsp;&emsp;classId|编码||false|string||
|&emsp;&emsp;className|名称||false|string||
|&emsp;&emsp;createBy|创建人||false|string||
|&emsp;&emsp;createTime|创建日期||false|string(date-time)||
|&emsp;&emsp;dispOrder|排序码||false|string||
|&emsp;&emsp;id|主键||false|string||
|&emsp;&emsp;matType|录取类型||false|string||
|&emsp;&emsp;studentType|生源||false|string||
|&emsp;&emsp;updateBy|更新人||false|string||
|&emsp;&emsp;updateTime|更新日期||false|string(date-time)||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«string»|
|201|Created||
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|string||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": "",
	"success": true,
	"timestamp": 0
}
```


## 特招班-分页列表查询


**接口地址**:`/nnzk/PrivilegeClassSetting/privilegeClass/list`


**请求方式**:`GET`


**请求数据类型**:`application/x-www-form-urlencoded`


**响应数据类型**:`*/*`


**接口描述**:<p>特招班-分页列表查询</p>



**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|classId|编码|query|false|string||
|className|名称|query|false|string||
|createBy|创建人|query|false|string||
|createTime|创建日期|query|false|string(date-time)||
|dispOrder|排序码|query|false|string||
|id|主键|query|false|string||
|matType|录取类型|query|false|string||
|pageNo|pageNo|query|false|integer(int32)||
|pageSize|pageSize|query|false|integer(int32)||
|studentType|生源|query|false|string||
|updateBy|更新人|query|false|string||
|updateTime|更新日期|query|false|string(date-time)||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«IPage«privilege_class对象»»|
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|IPage«privilege_class对象»|IPage«privilege_class对象»|
|&emsp;&emsp;current||integer(int64)||
|&emsp;&emsp;pages||integer(int64)||
|&emsp;&emsp;records||array|privilege_class对象|
|&emsp;&emsp;&emsp;&emsp;classId|编码|string||
|&emsp;&emsp;&emsp;&emsp;className|名称|string||
|&emsp;&emsp;&emsp;&emsp;createBy|创建人|string||
|&emsp;&emsp;&emsp;&emsp;createTime|创建日期|string||
|&emsp;&emsp;&emsp;&emsp;dispOrder|排序码|string||
|&emsp;&emsp;&emsp;&emsp;id|主键|string||
|&emsp;&emsp;&emsp;&emsp;matType|录取类型|string||
|&emsp;&emsp;&emsp;&emsp;studentType|生源|string||
|&emsp;&emsp;&emsp;&emsp;updateBy|更新人|string||
|&emsp;&emsp;&emsp;&emsp;updateTime|更新日期|string||
|&emsp;&emsp;size||integer(int64)||
|&emsp;&emsp;total||integer(int64)||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": {
		"current": 0,
		"pages": 0,
		"records": [
			{
				"classId": "",
				"className": "",
				"createBy": "",
				"createTime": "",
				"dispOrder": "",
				"id": "",
				"matType": "",
				"studentType": "",
				"updateBy": "",
				"updateTime": ""
			}
		],
		"size": 0,
		"total": 0
	},
	"success": true,
	"timestamp": 0
}
```


## 特招班-通过id查询


**接口地址**:`/nnzk/PrivilegeClassSetting/privilegeClass/queryById`


**请求方式**:`GET`


**请求数据类型**:`application/x-www-form-urlencoded`


**响应数据类型**:`*/*`


**接口描述**:<p>特招班-通过id查询</p>



**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|id|id|query|true|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«privilege_class对象»|
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|privilege_class对象|privilege_class对象|
|&emsp;&emsp;classId|编码|string||
|&emsp;&emsp;className|名称|string||
|&emsp;&emsp;createBy|创建人|string||
|&emsp;&emsp;createTime|创建日期|string(date-time)||
|&emsp;&emsp;dispOrder|排序码|string||
|&emsp;&emsp;id|主键|string||
|&emsp;&emsp;matType|录取类型|string||
|&emsp;&emsp;studentType|生源|string||
|&emsp;&emsp;updateBy|更新人|string||
|&emsp;&emsp;updateTime|更新日期|string(date-time)||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": {
		"classId": "",
		"className": "",
		"createBy": "",
		"createTime": "",
		"dispOrder": "",
		"id": "",
		"matType": "",
		"studentType": "",
		"updateBy": "",
		"updateTime": ""
	},
	"success": true,
	"timestamp": 0
}
```


# 特招班关联规则


## 特招班关联规则-添加


**接口地址**:`/nnzk/PrivilegeClassSetting/privilegeRule/add`


**请求方式**:`POST`


**请求数据类型**:`application/json`


**响应数据类型**:`*/*`


**接口描述**:<p>特招班关联规则-添加</p>



**请求示例**:


```javascript
{
  "classId": "",
  "createBy": "",
  "createTime": "",
  "highSchoolCode": "",
  "id": "",
  "signUpNum": 0,
  "updateBy": "",
  "updateTime": ""
}
```


**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|privilegeRule|特招班关联规则|body|true|privilege_rule对象|privilege_rule对象|
|&emsp;&emsp;classId|特招班编码||false|string||
|&emsp;&emsp;createBy|创建人||false|string||
|&emsp;&emsp;createTime|创建日期||false|string(date-time)||
|&emsp;&emsp;highSchoolCode|学校代码||false|string||
|&emsp;&emsp;id|主键||false|string||
|&emsp;&emsp;signUpNum|报名计划数||false|integer(int32)||
|&emsp;&emsp;updateBy|更新人||false|string||
|&emsp;&emsp;updateTime|更新日期||false|string(date-time)||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«string»|
|201|Created||
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|string||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": "",
	"success": true,
	"timestamp": 0
}
```


## 特招班关联规则-通过id删除


**接口地址**:`/nnzk/PrivilegeClassSetting/privilegeRule/delete`


**请求方式**:`DELETE`


**请求数据类型**:`application/x-www-form-urlencoded`


**响应数据类型**:`*/*`


**接口描述**:<p>特招班关联规则-通过id删除</p>



**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|id|id|query|true|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«string»|
|204|No Content||
|401|Unauthorized||
|403|Forbidden||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|string||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": "",
	"success": true,
	"timestamp": 0
}
```


## 特招班关联规则-批量删除


**接口地址**:`/nnzk/PrivilegeClassSetting/privilegeRule/deleteBatch`


**请求方式**:`DELETE`


**请求数据类型**:`application/x-www-form-urlencoded`


**响应数据类型**:`*/*`


**接口描述**:<p>特招班关联规则-批量删除</p>



**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|ids|ids|query|true|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«string»|
|204|No Content||
|401|Unauthorized||
|403|Forbidden||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|string||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": "",
	"success": true,
	"timestamp": 0
}
```


## 特招班关联规则-编辑


**接口地址**:`/nnzk/PrivilegeClassSetting/privilegeRule/edit`


**请求方式**:`POST`


**请求数据类型**:`application/json`


**响应数据类型**:`*/*`


**接口描述**:<p>特招班关联规则-编辑</p>



**请求示例**:


```javascript
{
  "classId": "",
  "createBy": "",
  "createTime": "",
  "highSchoolCode": "",
  "id": "",
  "signUpNum": 0,
  "updateBy": "",
  "updateTime": ""
}
```


**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|privilegeRule|特招班关联规则|body|true|privilege_rule对象|privilege_rule对象|
|&emsp;&emsp;classId|特招班编码||false|string||
|&emsp;&emsp;createBy|创建人||false|string||
|&emsp;&emsp;createTime|创建日期||false|string(date-time)||
|&emsp;&emsp;highSchoolCode|学校代码||false|string||
|&emsp;&emsp;id|主键||false|string||
|&emsp;&emsp;signUpNum|报名计划数||false|integer(int32)||
|&emsp;&emsp;updateBy|更新人||false|string||
|&emsp;&emsp;updateTime|更新日期||false|string(date-time)||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«string»|
|201|Created||
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|string||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": "",
	"success": true,
	"timestamp": 0
}
```


## 特招班关联规则-编辑


**接口地址**:`/nnzk/PrivilegeClassSetting/privilegeRule/edit`


**请求方式**:`PUT`


**请求数据类型**:`application/json`


**响应数据类型**:`*/*`


**接口描述**:<p>特招班关联规则-编辑</p>



**请求示例**:


```javascript
{
  "classId": "",
  "createBy": "",
  "createTime": "",
  "highSchoolCode": "",
  "id": "",
  "signUpNum": 0,
  "updateBy": "",
  "updateTime": ""
}
```


**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|privilegeRule|特招班关联规则|body|true|privilege_rule对象|privilege_rule对象|
|&emsp;&emsp;classId|特招班编码||false|string||
|&emsp;&emsp;createBy|创建人||false|string||
|&emsp;&emsp;createTime|创建日期||false|string(date-time)||
|&emsp;&emsp;highSchoolCode|学校代码||false|string||
|&emsp;&emsp;id|主键||false|string||
|&emsp;&emsp;signUpNum|报名计划数||false|integer(int32)||
|&emsp;&emsp;updateBy|更新人||false|string||
|&emsp;&emsp;updateTime|更新日期||false|string(date-time)||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«string»|
|201|Created||
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|string||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": "",
	"success": true,
	"timestamp": 0
}
```


## 特招班关联规则-分页列表查询


**接口地址**:`/nnzk/PrivilegeClassSetting/privilegeRule/list`


**请求方式**:`GET`


**请求数据类型**:`application/x-www-form-urlencoded`


**响应数据类型**:`*/*`


**接口描述**:<p>特招班关联规则-分页列表查询</p>



**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|classId|特招班编码|query|false|string||
|createBy|创建人|query|false|string||
|createTime|创建日期|query|false|string(date-time)||
|highSchoolCode|学校代码|query|false|string||
|id|主键|query|false|string||
|pageNo|pageNo|query|false|integer(int32)||
|pageSize|pageSize|query|false|integer(int32)||
|signUpNum|报名计划数|query|false|integer(int32)||
|updateBy|更新人|query|false|string||
|updateTime|更新日期|query|false|string(date-time)||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«IPage«privilege_rule对象»»|
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|IPage«privilege_rule对象»|IPage«privilege_rule对象»|
|&emsp;&emsp;current||integer(int64)||
|&emsp;&emsp;pages||integer(int64)||
|&emsp;&emsp;records||array|privilege_rule对象|
|&emsp;&emsp;&emsp;&emsp;classId|特招班编码|string||
|&emsp;&emsp;&emsp;&emsp;createBy|创建人|string||
|&emsp;&emsp;&emsp;&emsp;createTime|创建日期|string||
|&emsp;&emsp;&emsp;&emsp;highSchoolCode|学校代码|string||
|&emsp;&emsp;&emsp;&emsp;id|主键|string||
|&emsp;&emsp;&emsp;&emsp;signUpNum|报名计划数|integer||
|&emsp;&emsp;&emsp;&emsp;updateBy|更新人|string||
|&emsp;&emsp;&emsp;&emsp;updateTime|更新日期|string||
|&emsp;&emsp;size||integer(int64)||
|&emsp;&emsp;total||integer(int64)||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": {
		"current": 0,
		"pages": 0,
		"records": [
			{
				"classId": "",
				"createBy": "",
				"createTime": "",
				"highSchoolCode": "",
				"id": "",
				"signUpNum": 0,
				"updateBy": "",
				"updateTime": ""
			}
		],
		"size": 0,
		"total": 0
	},
	"success": true,
	"timestamp": 0
}
```


## 特招班关联规则-通过id查询


**接口地址**:`/nnzk/PrivilegeClassSetting/privilegeRule/queryById`


**请求方式**:`GET`


**请求数据类型**:`application/x-www-form-urlencoded`


**响应数据类型**:`*/*`


**接口描述**:<p>特招班关联规则-通过id查询</p>



**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|id|id|query|true|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«privilege_rule对象»|
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|privilege_rule对象|privilege_rule对象|
|&emsp;&emsp;classId|特招班编码|string||
|&emsp;&emsp;createBy|创建人|string||
|&emsp;&emsp;createTime|创建日期|string(date-time)||
|&emsp;&emsp;highSchoolCode|学校代码|string||
|&emsp;&emsp;id|主键|string||
|&emsp;&emsp;signUpNum|报名计划数|integer(int32)||
|&emsp;&emsp;updateBy|更新人|string||
|&emsp;&emsp;updateTime|更新日期|string(date-time)||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": {
		"classId": "",
		"createBy": "",
		"createTime": "",
		"highSchoolCode": "",
		"id": "",
		"signUpNum": 0,
		"updateBy": "",
		"updateTime": ""
	},
	"success": true,
	"timestamp": 0
}
```


# 特招设置


## 编辑特招班


**接口地址**:`/nnzk/PrivilegeClassSetting/setting/editPrivilegeClass`


**请求方式**:`POST`


**请求数据类型**:`application/json`


**响应数据类型**:`*/*`


**接口描述**:<p>编辑特招班</p>



**请求示例**:


```javascript
{
  "classId": "",
  "className": "",
  "dispOrder": "",
  "matType": "",
  "studentType": ""
}
```


**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|input|input|body|true|PrivilegeClassDTO|PrivilegeClassDTO|
|&emsp;&emsp;classId|编码||false|string||
|&emsp;&emsp;className|名称||false|string||
|&emsp;&emsp;dispOrder|排序码||false|string||
|&emsp;&emsp;matType|录取类型||false|string||
|&emsp;&emsp;studentType|生源||false|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«string»|
|201|Created||
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|string||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": "",
	"success": true,
	"timestamp": 0
}
```


## 特招设置-获取全部学校及其设置的特招班数


**接口地址**:`/nnzk/PrivilegeClassSetting/setting/getAllSchoolWithPriClass`


**请求方式**:`GET`


**请求数据类型**:`application/x-www-form-urlencoded`


**响应数据类型**:`*/*`


**接口描述**:<p>特招班关联规则-获取全部学校及其设置的特招班数</p>



**请求参数**:


暂无


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«List«SchoolPrivilegeRuleVO»»|
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|array|SchoolPrivilegeRuleVO|
|&emsp;&emsp;privilegeClassNum||integer(int32)||
|&emsp;&emsp;schoolCode||string||
|&emsp;&emsp;schoolName||string||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": [
		{
			"privilegeClassNum": 0,
			"schoolCode": "",
			"schoolName": ""
		}
	],
	"success": true,
	"timestamp": 0
}
```


## 特招设置-根据学校查询设置的特招班


**接口地址**:`/nnzk/PrivilegeClassSetting/setting/getPriClassBySchoolCode`


**请求方式**:`GET`


**请求数据类型**:`application/x-www-form-urlencoded`


**响应数据类型**:`*/*`


**接口描述**:<p>特招班-根据学校查询设置的特招班</p>



**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|schoolCode|schoolCode|query|false|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«List«PrivilegeClassVO»»|
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|array|PrivilegeClassVO|
|&emsp;&emsp;classId|编码|string||
|&emsp;&emsp;className|名称|string||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": [
		{
			"classId": "",
			"className": ""
		}
	],
	"success": true,
	"timestamp": 0
}
```


## 特招设置-根据学校获取其特招设置


**接口地址**:`/nnzk/PrivilegeClassSetting/setting/getPriRuleBySchoolCode`


**请求方式**:`GET`


**请求数据类型**:`application/x-www-form-urlencoded`


**响应数据类型**:`*/*`


**接口描述**:<p>特招班关联规则-根据学校获取其特招设置</p>



**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|schoolCode|schoolCode|query|true|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«List«PrivilegeClassSettingVO»»|
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|array|PrivilegeClassSettingVO|
|&emsp;&emsp;classId|特招班编码|string||
|&emsp;&emsp;className|特招班名称|string||
|&emsp;&emsp;dispOrder|排序码|string||
|&emsp;&emsp;highSchoolCode|学校代码|string||
|&emsp;&emsp;signUpNum|报名计划数|integer(int32)||
|&emsp;&emsp;studentType|生源|string||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": [
		{
			"classId": "",
			"className": "",
			"dispOrder": "",
			"highSchoolCode": "",
			"signUpNum": 0,
			"studentType": ""
		}
	],
	"success": true,
	"timestamp": 0
}
```


## 特招设置-保存设置


**接口地址**:`/nnzk/PrivilegeClassSetting/setting/save`


**请求方式**:`POST`


**请求数据类型**:`application/json`


**响应数据类型**:`*/*`


**接口描述**:<p>特招设置-保存设置</p>



**请求示例**:


```javascript
{
  "records": [
    {
      "classId": "",
      "className": "",
      "dispOrder": "",
      "highSchoolCode": "",
      "signUpNum": 0,
      "studentType": ""
    }
  ]
}
```


**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|input|input|body|true|PrivilegeClassSettingEditVO|PrivilegeClassSettingEditVO|
|&emsp;&emsp;records|||false|array|PrivilegeClassSettingVO|
|&emsp;&emsp;&emsp;&emsp;classId|特招班编码||false|string||
|&emsp;&emsp;&emsp;&emsp;className|特招班名称||false|string||
|&emsp;&emsp;&emsp;&emsp;dispOrder|排序码||false|string||
|&emsp;&emsp;&emsp;&emsp;highSchoolCode|学校代码||false|string||
|&emsp;&emsp;&emsp;&emsp;signUpNum|报名计划数||false|integer||
|&emsp;&emsp;&emsp;&emsp;studentType|生源||false|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«string»|
|201|Created||
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|string||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": "",
	"success": true,
	"timestamp": 0
}
```


# 用户登录


## 登录二维码


**接口地址**:`/nnzk/sys/getLoginQrcode`


**请求方式**:`GET`


**请求数据类型**:`application/x-www-form-urlencoded`


**响应数据类型**:`*/*`


**接口描述**:<p>登录二维码</p>



**请求参数**:


暂无


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«object»|
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|object||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": {},
	"success": true,
	"timestamp": 0
}
```


## 获取用户扫码后保存的token


**接口地址**:`/nnzk/sys/getQrcodeToken`


**请求方式**:`GET`


**请求数据类型**:`application/x-www-form-urlencoded`


**响应数据类型**:`*/*`


**接口描述**:<p>获取用户扫码后保存的token</p>



**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|qrcodeId|qrcodeId|query|true|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象|
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|object||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": {},
	"success": true,
	"timestamp": 0
}
```


## 登录接口


**接口地址**:`/nnzk/sys/login`


**请求方式**:`POST`


**请求数据类型**:`application/json`


**响应数据类型**:`*/*`


**接口描述**:


**请求示例**:


```javascript
{
  "captcha": "",
  "checkKey": "",
  "eighthGradeStuName": "",
  "password": "",
  "username": ""
}
```


**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|sysLoginModel|登录对象|body|true|登录对象|登录对象|
|&emsp;&emsp;captcha|验证码||false|string||
|&emsp;&emsp;checkKey|验证码key||false|string||
|&emsp;&emsp;eighthGradeStuName|八年级学生姓名（查询生地成绩专用）||false|string||
|&emsp;&emsp;password|密码||false|string||
|&emsp;&emsp;username|账号||false|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«JSONObject»|
|201|Created||
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|object||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": {},
	"success": true,
	"timestamp": 0
}
```


## 手机号登录接口


**接口地址**:`/nnzk/sys/phoneLogin`


**请求方式**:`POST`


**请求数据类型**:`application/json`


**响应数据类型**:`*/*`


**接口描述**:


**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|jsonObject|jsonObject|body|true|||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«JSONObject»|
|201|Created||
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|object||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": {},
	"success": true,
	"timestamp": 0
}
```


## 获取验证码


**接口地址**:`/nnzk/sys/randomImage/{key}`


**请求方式**:`GET`


**请求数据类型**:`application/x-www-form-urlencoded`


**响应数据类型**:`*/*`


**接口描述**:


**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|key|key|path|true|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«string»|
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|string||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": "",
	"success": true,
	"timestamp": 0
}
```


## 扫码登录二维码


**接口地址**:`/nnzk/sys/scanLoginQrcode`


**请求方式**:`POST`


**请求数据类型**:`application/json`


**响应数据类型**:`*/*`


**接口描述**:<p>扫码登录二维码</p>



**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|qrcodeId|qrcodeId|query|true|string||
|token|token|query|true|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«object»|
|201|Created||
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|object||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": {},
	"success": true,
	"timestamp": 0
}
```


# 知识库-文档管理


## 知识库-文档管理-添加


**接口地址**:`/nnzk/sys/files/add`


**请求方式**:`POST`


**请求数据类型**:`application/json`


**响应数据类型**:`*/*`


**接口描述**:<p>知识库-文档管理-添加</p>



**请求示例**:


```javascript
{
  "createBy": "",
  "createTime": "",
  "delFlag": "",
  "downCount": 0,
  "enableDown": "",
  "enableUpdat": "",
  "fileName": "",
  "fileSize": 0,
  "fileType": "",
  "id": "",
  "izFolder": "",
  "izRootFolder": "",
  "izStar": "",
  "parentId": "",
  "readCount": 0,
  "realname": "",
  "sharePerms": "",
  "shareUrl": "",
  "storeType": "",
  "tenantId": "",
  "updateBy": "",
  "updateTime": "",
  "url": "",
  "userData": "",
  "zipName": ""
}
```


**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|sysFiles|知识库-文档管理|body|true|sys_files对象|sys_files对象|
|&emsp;&emsp;createBy|创建人登录名称||false|string||
|&emsp;&emsp;createTime|创建日期||false|string(date-time)||
|&emsp;&emsp;delFlag|删除状态(0-正常,1-删除至回收站)||false|string||
|&emsp;&emsp;downCount|下载次数||false|integer(int32)||
|&emsp;&emsp;enableDown|是否允许下载(1：是  0：否)||false|string||
|&emsp;&emsp;enableUpdat|是否允许修改(1：是  0：否)||false|string||
|&emsp;&emsp;fileName|文件名称||false|string||
|&emsp;&emsp;fileSize|文件大小（kb）||false|number(double)||
|&emsp;&emsp;fileType|文档类型（folder:文件夹 excel:excel doc:word pp:ppt image:图片  archive:其他文档 video:视频）||false|string||
|&emsp;&emsp;id|主键id||false|string||
|&emsp;&emsp;izFolder|是否文件夹(1：是  0：否)||false|string||
|&emsp;&emsp;izRootFolder|是否为1级文件夹，允许为空 (1：是 )||false|string||
|&emsp;&emsp;izStar|是否标星(1：是  0：否)||false|string||
|&emsp;&emsp;parentId|父级id||false|string||
|&emsp;&emsp;readCount|阅读次数||false|integer(int32)||
|&emsp;&emsp;realname|||false|string||
|&emsp;&emsp;sharePerms|分享权限(1.关闭分享 2.允许所有联系人查看 3.允许任何人查看)||false|string||
|&emsp;&emsp;shareUrl|分享链接||false|string||
|&emsp;&emsp;storeType|文件上传类型(temp/本地上传(临时文件) manage/知识库)||false|string||
|&emsp;&emsp;tenantId|租户id||false|string||
|&emsp;&emsp;updateBy|更新人登录名称||false|string||
|&emsp;&emsp;updateTime|更新日期||false|string(date-time)||
|&emsp;&emsp;url|文件地址||false|string||
|&emsp;&emsp;userData|||false|string||
|&emsp;&emsp;zipName|||false|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«object»|
|201|Created||
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|object||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": {},
	"success": true,
	"timestamp": 0
}
```


## 知识库-文档管理-通过id删除


**接口地址**:`/nnzk/sys/files/delete`


**请求方式**:`DELETE`


**请求数据类型**:`application/x-www-form-urlencoded`


**响应数据类型**:`*/*`


**接口描述**:<p>知识库-文档管理-通过id删除</p>



**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|id|id|query|true|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«object»|
|204|No Content||
|401|Unauthorized||
|403|Forbidden||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|object||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": {},
	"success": true,
	"timestamp": 0
}
```


## 知识库-文档管理-批量删除


**接口地址**:`/nnzk/sys/files/deleteBatch`


**请求方式**:`DELETE`


**请求数据类型**:`application/x-www-form-urlencoded`


**响应数据类型**:`*/*`


**接口描述**:<p>知识库-文档管理-批量删除</p>



**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|ids|ids|query|true|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«object»|
|204|No Content||
|401|Unauthorized||
|403|Forbidden||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|object||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": {},
	"success": true,
	"timestamp": 0
}
```


## 知识库-文档管理-编辑


**接口地址**:`/nnzk/sys/files/edit`


**请求方式**:`POST`


**请求数据类型**:`application/json`


**响应数据类型**:`*/*`


**接口描述**:<p>知识库-文档管理-编辑</p>



**请求示例**:


```javascript
{
  "createBy": "",
  "createTime": "",
  "delFlag": "",
  "downCount": 0,
  "enableDown": "",
  "enableUpdat": "",
  "fileName": "",
  "fileSize": 0,
  "fileType": "",
  "id": "",
  "izFolder": "",
  "izRootFolder": "",
  "izStar": "",
  "parentId": "",
  "readCount": 0,
  "realname": "",
  "sharePerms": "",
  "shareUrl": "",
  "storeType": "",
  "tenantId": "",
  "updateBy": "",
  "updateTime": "",
  "url": "",
  "userData": "",
  "zipName": ""
}
```


**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|sysFiles|知识库-文档管理|body|true|sys_files对象|sys_files对象|
|&emsp;&emsp;createBy|创建人登录名称||false|string||
|&emsp;&emsp;createTime|创建日期||false|string(date-time)||
|&emsp;&emsp;delFlag|删除状态(0-正常,1-删除至回收站)||false|string||
|&emsp;&emsp;downCount|下载次数||false|integer(int32)||
|&emsp;&emsp;enableDown|是否允许下载(1：是  0：否)||false|string||
|&emsp;&emsp;enableUpdat|是否允许修改(1：是  0：否)||false|string||
|&emsp;&emsp;fileName|文件名称||false|string||
|&emsp;&emsp;fileSize|文件大小（kb）||false|number(double)||
|&emsp;&emsp;fileType|文档类型（folder:文件夹 excel:excel doc:word pp:ppt image:图片  archive:其他文档 video:视频）||false|string||
|&emsp;&emsp;id|主键id||false|string||
|&emsp;&emsp;izFolder|是否文件夹(1：是  0：否)||false|string||
|&emsp;&emsp;izRootFolder|是否为1级文件夹，允许为空 (1：是 )||false|string||
|&emsp;&emsp;izStar|是否标星(1：是  0：否)||false|string||
|&emsp;&emsp;parentId|父级id||false|string||
|&emsp;&emsp;readCount|阅读次数||false|integer(int32)||
|&emsp;&emsp;realname|||false|string||
|&emsp;&emsp;sharePerms|分享权限(1.关闭分享 2.允许所有联系人查看 3.允许任何人查看)||false|string||
|&emsp;&emsp;shareUrl|分享链接||false|string||
|&emsp;&emsp;storeType|文件上传类型(temp/本地上传(临时文件) manage/知识库)||false|string||
|&emsp;&emsp;tenantId|租户id||false|string||
|&emsp;&emsp;updateBy|更新人登录名称||false|string||
|&emsp;&emsp;updateTime|更新日期||false|string(date-time)||
|&emsp;&emsp;url|文件地址||false|string||
|&emsp;&emsp;userData|||false|string||
|&emsp;&emsp;zipName|||false|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«object»|
|201|Created||
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|object||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": {},
	"success": true,
	"timestamp": 0
}
```


## 知识库-文档管理-编辑


**接口地址**:`/nnzk/sys/files/edit`


**请求方式**:`PUT`


**请求数据类型**:`application/json`


**响应数据类型**:`*/*`


**接口描述**:<p>知识库-文档管理-编辑</p>



**请求示例**:


```javascript
{
  "createBy": "",
  "createTime": "",
  "delFlag": "",
  "downCount": 0,
  "enableDown": "",
  "enableUpdat": "",
  "fileName": "",
  "fileSize": 0,
  "fileType": "",
  "id": "",
  "izFolder": "",
  "izRootFolder": "",
  "izStar": "",
  "parentId": "",
  "readCount": 0,
  "realname": "",
  "sharePerms": "",
  "shareUrl": "",
  "storeType": "",
  "tenantId": "",
  "updateBy": "",
  "updateTime": "",
  "url": "",
  "userData": "",
  "zipName": ""
}
```


**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|sysFiles|知识库-文档管理|body|true|sys_files对象|sys_files对象|
|&emsp;&emsp;createBy|创建人登录名称||false|string||
|&emsp;&emsp;createTime|创建日期||false|string(date-time)||
|&emsp;&emsp;delFlag|删除状态(0-正常,1-删除至回收站)||false|string||
|&emsp;&emsp;downCount|下载次数||false|integer(int32)||
|&emsp;&emsp;enableDown|是否允许下载(1：是  0：否)||false|string||
|&emsp;&emsp;enableUpdat|是否允许修改(1：是  0：否)||false|string||
|&emsp;&emsp;fileName|文件名称||false|string||
|&emsp;&emsp;fileSize|文件大小（kb）||false|number(double)||
|&emsp;&emsp;fileType|文档类型（folder:文件夹 excel:excel doc:word pp:ppt image:图片  archive:其他文档 video:视频）||false|string||
|&emsp;&emsp;id|主键id||false|string||
|&emsp;&emsp;izFolder|是否文件夹(1：是  0：否)||false|string||
|&emsp;&emsp;izRootFolder|是否为1级文件夹，允许为空 (1：是 )||false|string||
|&emsp;&emsp;izStar|是否标星(1：是  0：否)||false|string||
|&emsp;&emsp;parentId|父级id||false|string||
|&emsp;&emsp;readCount|阅读次数||false|integer(int32)||
|&emsp;&emsp;realname|||false|string||
|&emsp;&emsp;sharePerms|分享权限(1.关闭分享 2.允许所有联系人查看 3.允许任何人查看)||false|string||
|&emsp;&emsp;shareUrl|分享链接||false|string||
|&emsp;&emsp;storeType|文件上传类型(temp/本地上传(临时文件) manage/知识库)||false|string||
|&emsp;&emsp;tenantId|租户id||false|string||
|&emsp;&emsp;updateBy|更新人登录名称||false|string||
|&emsp;&emsp;updateTime|更新日期||false|string(date-time)||
|&emsp;&emsp;url|文件地址||false|string||
|&emsp;&emsp;userData|||false|string||
|&emsp;&emsp;zipName|||false|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«object»|
|201|Created||
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|object||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": {},
	"success": true,
	"timestamp": 0
}
```


## 知识库-文档管理-分页列表查询


**接口地址**:`/nnzk/sys/files/list`


**请求方式**:`GET`


**请求数据类型**:`application/x-www-form-urlencoded`


**响应数据类型**:`*/*`


**接口描述**:<p>知识库-文档管理-分页列表查询</p>



**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|createBy|创建人登录名称|query|false|string||
|createTime|创建日期|query|false|string(date-time)||
|delFlag|删除状态(0-正常,1-删除至回收站)|query|false|string||
|downCount|下载次数|query|false|integer(int32)||
|enableDown|是否允许下载(1：是  0：否)|query|false|string||
|enableUpdat|是否允许修改(1：是  0：否)|query|false|string||
|fileName|文件名称|query|false|string||
|fileSize|文件大小（kb）|query|false|number(double)||
|fileType|文档类型（folder:文件夹 excel:excel doc:word pp:ppt image:图片  archive:其他文档 video:视频）|query|false|string||
|id|主键id|query|false|string||
|izFolder|是否文件夹(1：是  0：否)|query|false|string||
|izRootFolder|是否为1级文件夹，允许为空 (1：是 )|query|false|string||
|izStar|是否标星(1：是  0：否)|query|false|string||
|pageNo|pageNo|query|false|integer(int32)||
|pageSize|pageSize|query|false|integer(int32)||
|parentId|父级id|query|false|string||
|readCount|阅读次数|query|false|integer(int32)||
|realname||query|false|string||
|sharePerms|分享权限(1.关闭分享 2.允许所有联系人查看 3.允许任何人查看)|query|false|string||
|shareUrl|分享链接|query|false|string||
|storeType|文件上传类型(temp/本地上传(临时文件) manage/知识库)|query|false|string||
|tenantId|租户id|query|false|string||
|updateBy|更新人登录名称|query|false|string||
|updateTime|更新日期|query|false|string(date-time)||
|url|文件地址|query|false|string||
|userData||query|false|string||
|zipName||query|false|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«object»|
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|object||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": {},
	"success": true,
	"timestamp": 0
}
```


## 知识库-文档管理-通过id查询


**接口地址**:`/nnzk/sys/files/queryById`


**请求方式**:`GET`


**请求数据类型**:`application/x-www-form-urlencoded`


**响应数据类型**:`*/*`


**接口描述**:<p>知识库-文档管理-通过id查询</p>



**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|id|id|query|true|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«object»|
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|object||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": {},
	"success": true,
	"timestamp": 0
}
```


# 系统评论回复表


## 系统评论回复表-添加


**接口地址**:`/nnzk/sys/comment/add`


**请求方式**:`POST`


**请求数据类型**:`application/json`


**响应数据类型**:`*/*`


**接口描述**:<p>系统评论回复表-添加</p>



**请求示例**:


```javascript
{
  "commentContent": "",
  "commentId": "",
  "createBy": "",
  "createTime": "",
  "fromUserId": "",
  "id": "",
  "tableDataId": "",
  "tableName": "",
  "toUserId": "",
  "updateBy": "",
  "updateTime": ""
}
```


**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|sysComment|系统评论回复表|body|true|sys_comment对象|sys_comment对象|
|&emsp;&emsp;commentContent|回复内容||false|string||
|&emsp;&emsp;commentId|评论id(允许为空，不为空时，则为回复)||false|string||
|&emsp;&emsp;createBy|创建人||false|string||
|&emsp;&emsp;createTime|创建日期||false|string(date-time)||
|&emsp;&emsp;fromUserId|来源用户id||false|string||
|&emsp;&emsp;id|id||false|string||
|&emsp;&emsp;tableDataId|数据id||false|string||
|&emsp;&emsp;tableName|表名||false|string||
|&emsp;&emsp;toUserId|发送给用户id(允许为空)||false|string||
|&emsp;&emsp;updateBy|更新人||false|string||
|&emsp;&emsp;updateTime|更新日期||false|string(date-time)||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«string»|
|201|Created||
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|string||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": "",
	"success": true,
	"timestamp": 0
}
```


## 系统评论表-添加文件


**接口地址**:`/nnzk/sys/comment/addFile`


**请求方式**:`POST`


**请求数据类型**:`application/json`


**响应数据类型**:`*/*`


**接口描述**:<p>系统评论表-添加文件</p>



**请求参数**:


暂无


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«string»|
|201|Created||
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|string||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": "",
	"success": true,
	"timestamp": 0
}
```


## 系统评论表-添加文本


**接口地址**:`/nnzk/sys/comment/addText`


**请求方式**:`POST`


**请求数据类型**:`application/json`


**响应数据类型**:`*/*`


**接口描述**:<p>系统评论表-添加文本</p>



**请求示例**:


```javascript
{
  "commentContent": "",
  "commentId": "",
  "createBy": "",
  "createTime": "",
  "fromUserId": "",
  "id": "",
  "tableDataId": "",
  "tableName": "",
  "toUserId": "",
  "updateBy": "",
  "updateTime": ""
}
```


**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|sysComment|系统评论回复表|body|true|sys_comment对象|sys_comment对象|
|&emsp;&emsp;commentContent|回复内容||false|string||
|&emsp;&emsp;commentId|评论id(允许为空，不为空时，则为回复)||false|string||
|&emsp;&emsp;createBy|创建人||false|string||
|&emsp;&emsp;createTime|创建日期||false|string(date-time)||
|&emsp;&emsp;fromUserId|来源用户id||false|string||
|&emsp;&emsp;id|id||false|string||
|&emsp;&emsp;tableDataId|数据id||false|string||
|&emsp;&emsp;tableName|表名||false|string||
|&emsp;&emsp;toUserId|发送给用户id(允许为空)||false|string||
|&emsp;&emsp;updateBy|更新人||false|string||
|&emsp;&emsp;updateTime|更新日期||false|string(date-time)||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«string»|
|201|Created||
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|string||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": "",
	"success": true,
	"timestamp": 0
}
```


## 系统评论回复表-通过id删除


**接口地址**:`/nnzk/sys/comment/delete`


**请求方式**:`DELETE`


**请求数据类型**:`application/x-www-form-urlencoded`


**响应数据类型**:`*/*`


**接口描述**:<p>系统评论回复表-通过id删除</p>



**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|id|id|query|true|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«string»|
|204|No Content||
|401|Unauthorized||
|403|Forbidden||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|string||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": "",
	"success": true,
	"timestamp": 0
}
```


## 系统评论回复表-批量删除


**接口地址**:`/nnzk/sys/comment/deleteBatch`


**请求方式**:`DELETE`


**请求数据类型**:`application/x-www-form-urlencoded`


**响应数据类型**:`*/*`


**接口描述**:<p>系统评论回复表-批量删除</p>



**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|ids|ids|query|true|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«string»|
|204|No Content||
|401|Unauthorized||
|403|Forbidden||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|string||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": "",
	"success": true,
	"timestamp": 0
}
```


## 系统评论回复表-通过id删除


**接口地址**:`/nnzk/sys/comment/deleteOne`


**请求方式**:`DELETE`


**请求数据类型**:`application/x-www-form-urlencoded`


**响应数据类型**:`*/*`


**接口描述**:<p>系统评论回复表-通过id删除</p>



**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|id|id|query|true|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«string»|
|204|No Content||
|401|Unauthorized||
|403|Forbidden||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|string||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": "",
	"success": true,
	"timestamp": 0
}
```


## 系统评论回复表-编辑


**接口地址**:`/nnzk/sys/comment/edit`


**请求方式**:`POST`


**请求数据类型**:`application/json`


**响应数据类型**:`*/*`


**接口描述**:<p>系统评论回复表-编辑</p>



**请求示例**:


```javascript
{
  "commentContent": "",
  "commentId": "",
  "createBy": "",
  "createTime": "",
  "fromUserId": "",
  "id": "",
  "tableDataId": "",
  "tableName": "",
  "toUserId": "",
  "updateBy": "",
  "updateTime": ""
}
```


**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|sysComment|系统评论回复表|body|true|sys_comment对象|sys_comment对象|
|&emsp;&emsp;commentContent|回复内容||false|string||
|&emsp;&emsp;commentId|评论id(允许为空，不为空时，则为回复)||false|string||
|&emsp;&emsp;createBy|创建人||false|string||
|&emsp;&emsp;createTime|创建日期||false|string(date-time)||
|&emsp;&emsp;fromUserId|来源用户id||false|string||
|&emsp;&emsp;id|id||false|string||
|&emsp;&emsp;tableDataId|数据id||false|string||
|&emsp;&emsp;tableName|表名||false|string||
|&emsp;&emsp;toUserId|发送给用户id(允许为空)||false|string||
|&emsp;&emsp;updateBy|更新人||false|string||
|&emsp;&emsp;updateTime|更新日期||false|string(date-time)||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«string»|
|201|Created||
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|string||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": "",
	"success": true,
	"timestamp": 0
}
```


## 系统评论回复表-编辑


**接口地址**:`/nnzk/sys/comment/edit`


**请求方式**:`PUT`


**请求数据类型**:`application/json`


**响应数据类型**:`*/*`


**接口描述**:<p>系统评论回复表-编辑</p>



**请求示例**:


```javascript
{
  "commentContent": "",
  "commentId": "",
  "createBy": "",
  "createTime": "",
  "fromUserId": "",
  "id": "",
  "tableDataId": "",
  "tableName": "",
  "toUserId": "",
  "updateBy": "",
  "updateTime": ""
}
```


**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|sysComment|系统评论回复表|body|true|sys_comment对象|sys_comment对象|
|&emsp;&emsp;commentContent|回复内容||false|string||
|&emsp;&emsp;commentId|评论id(允许为空，不为空时，则为回复)||false|string||
|&emsp;&emsp;createBy|创建人||false|string||
|&emsp;&emsp;createTime|创建日期||false|string(date-time)||
|&emsp;&emsp;fromUserId|来源用户id||false|string||
|&emsp;&emsp;id|id||false|string||
|&emsp;&emsp;tableDataId|数据id||false|string||
|&emsp;&emsp;tableName|表名||false|string||
|&emsp;&emsp;toUserId|发送给用户id(允许为空)||false|string||
|&emsp;&emsp;updateBy|更新人||false|string||
|&emsp;&emsp;updateTime|更新日期||false|string(date-time)||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«string»|
|201|Created||
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|string||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": "",
	"success": true,
	"timestamp": 0
}
```


## 系统评论回复表-列表查询


**接口地址**:`/nnzk/sys/comment/fileList`


**请求方式**:`GET`


**请求数据类型**:`application/x-www-form-urlencoded`


**响应数据类型**:`*/*`


**接口描述**:<p>系统评论回复表-列表查询</p>



**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|commentContent|回复内容|query|false|string||
|commentId|评论id(允许为空，不为空时，则为回复)|query|false|string||
|createBy|创建人|query|false|string||
|createTime|创建日期|query|false|string(date-time)||
|fromUserId|来源用户id|query|false|string||
|id|id|query|false|string||
|tableDataId|数据id|query|false|string||
|tableName|表名|query|false|string||
|toUserId|发送给用户id(允许为空)|query|false|string||
|updateBy|更新人|query|false|string||
|updateTime|更新日期|query|false|string(date-time)||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«IPage«SysCommentFileVo»»|
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|IPage«SysCommentFileVo»|IPage«SysCommentFileVo»|
|&emsp;&emsp;current||integer(int64)||
|&emsp;&emsp;pages||integer(int64)||
|&emsp;&emsp;records||array|SysCommentFileVo|
|&emsp;&emsp;&emsp;&emsp;fileId||string||
|&emsp;&emsp;&emsp;&emsp;fileSize||number||
|&emsp;&emsp;&emsp;&emsp;name||string||
|&emsp;&emsp;&emsp;&emsp;storeType||string||
|&emsp;&emsp;&emsp;&emsp;sysFormFileId||string||
|&emsp;&emsp;&emsp;&emsp;type||string||
|&emsp;&emsp;&emsp;&emsp;url||string||
|&emsp;&emsp;size||integer(int64)||
|&emsp;&emsp;total||integer(int64)||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": {
		"current": 0,
		"pages": 0,
		"records": [
			{
				"fileId": "",
				"fileSize": 0,
				"name": "",
				"storeType": "",
				"sysFormFileId": "",
				"type": "",
				"url": ""
			}
		],
		"size": 0,
		"total": 0
	},
	"success": true,
	"timestamp": 0
}
```


## 系统评论回复表-分页列表查询


**接口地址**:`/nnzk/sys/comment/list`


**请求方式**:`GET`


**请求数据类型**:`application/x-www-form-urlencoded`


**响应数据类型**:`*/*`


**接口描述**:<p>系统评论回复表-分页列表查询</p>



**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|commentContent|回复内容|query|false|string||
|commentId|评论id(允许为空，不为空时，则为回复)|query|false|string||
|createBy|创建人|query|false|string||
|createTime|创建日期|query|false|string(date-time)||
|fromUserId|来源用户id|query|false|string||
|id|id|query|false|string||
|pageNo|pageNo|query|false|integer(int32)||
|pageSize|pageSize|query|false|integer(int32)||
|tableDataId|数据id|query|false|string||
|tableName|表名|query|false|string||
|toUserId|发送给用户id(允许为空)|query|false|string||
|updateBy|更新人|query|false|string||
|updateTime|更新日期|query|false|string(date-time)||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«IPage«sys_comment对象»»|
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|IPage«sys_comment对象»|IPage«sys_comment对象»|
|&emsp;&emsp;current||integer(int64)||
|&emsp;&emsp;pages||integer(int64)||
|&emsp;&emsp;records||array|sys_comment对象|
|&emsp;&emsp;&emsp;&emsp;commentContent|回复内容|string||
|&emsp;&emsp;&emsp;&emsp;commentId|评论id(允许为空，不为空时，则为回复)|string||
|&emsp;&emsp;&emsp;&emsp;createBy|创建人|string||
|&emsp;&emsp;&emsp;&emsp;createTime|创建日期|string||
|&emsp;&emsp;&emsp;&emsp;fromUserId|来源用户id|string||
|&emsp;&emsp;&emsp;&emsp;id|id|string||
|&emsp;&emsp;&emsp;&emsp;tableDataId|数据id|string||
|&emsp;&emsp;&emsp;&emsp;tableName|表名|string||
|&emsp;&emsp;&emsp;&emsp;toUserId|发送给用户id(允许为空)|string||
|&emsp;&emsp;&emsp;&emsp;updateBy|更新人|string||
|&emsp;&emsp;&emsp;&emsp;updateTime|更新日期|string||
|&emsp;&emsp;size||integer(int64)||
|&emsp;&emsp;total||integer(int64)||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": {
		"current": 0,
		"pages": 0,
		"records": [
			{
				"commentContent": "",
				"commentId": "",
				"createBy": "",
				"createTime": "",
				"fromUserId": "",
				"id": "",
				"tableDataId": "",
				"tableName": "",
				"toUserId": "",
				"updateBy": "",
				"updateTime": ""
			}
		],
		"size": 0,
		"total": 0
	},
	"success": true,
	"timestamp": 0
}
```


## 系统评论回复表-列表查询


**接口地址**:`/nnzk/sys/comment/listByForm`


**请求方式**:`GET`


**请求数据类型**:`application/x-www-form-urlencoded`


**响应数据类型**:`*/*`


**接口描述**:<p>系统评论回复表-列表查询</p>



**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|commentContent|回复内容|query|false|string||
|commentId|评论id(允许为空，不为空时，则为回复)|query|false|string||
|createBy|创建人|query|false|string||
|createTime|创建日期|query|false|string(date-time)||
|fromUserId|来源用户id|query|false|string||
|id|id|query|false|string||
|tableDataId|数据id|query|false|string||
|tableName|表名|query|false|string||
|toUserId|发送给用户id(允许为空)|query|false|string||
|updateBy|更新人|query|false|string||
|updateTime|更新日期|query|false|string(date-time)||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«IPage«SysCommentVO»»|
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|IPage«SysCommentVO»|IPage«SysCommentVO»|
|&emsp;&emsp;current||integer(int64)||
|&emsp;&emsp;pages||integer(int64)||
|&emsp;&emsp;records||array|SysCommentVO|
|&emsp;&emsp;&emsp;&emsp;commentContent||string||
|&emsp;&emsp;&emsp;&emsp;commentId||string||
|&emsp;&emsp;&emsp;&emsp;createTime|创建日期|string||
|&emsp;&emsp;&emsp;&emsp;fileList||array|SysCommentFileVo|
|&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;fileId||string||
|&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;fileSize||number||
|&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;name||string||
|&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;storeType||string||
|&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;sysFormFileId||string||
|&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;type||string||
|&emsp;&emsp;&emsp;&emsp;&emsp;&emsp;url||string||
|&emsp;&emsp;&emsp;&emsp;fromUserAvatar||string||
|&emsp;&emsp;&emsp;&emsp;fromUserId||string||
|&emsp;&emsp;&emsp;&emsp;fromUserId_dictText||string||
|&emsp;&emsp;&emsp;&emsp;id||string||
|&emsp;&emsp;&emsp;&emsp;tableDataId||string||
|&emsp;&emsp;&emsp;&emsp;tableName||string||
|&emsp;&emsp;&emsp;&emsp;toUserAvatar||string||
|&emsp;&emsp;&emsp;&emsp;toUserId||string||
|&emsp;&emsp;&emsp;&emsp;toUserId_dictText||string||
|&emsp;&emsp;size||integer(int64)||
|&emsp;&emsp;total||integer(int64)||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": {
		"current": 0,
		"pages": 0,
		"records": [
			{
				"commentContent": "",
				"commentId": "",
				"createTime": "",
				"fileList": [
					{
						"fileId": "",
						"fileSize": 0,
						"name": "",
						"storeType": "",
						"sysFormFileId": "",
						"type": "",
						"url": ""
					}
				],
				"fromUserAvatar": "",
				"fromUserId": "",
				"fromUserId_dictText": "",
				"id": "",
				"tableDataId": "",
				"tableName": "",
				"toUserAvatar": "",
				"toUserId": "",
				"toUserId_dictText": ""
			}
		],
		"size": 0,
		"total": 0
	},
	"success": true,
	"timestamp": 0
}
```


## 系统评论回复表-通过id查询


**接口地址**:`/nnzk/sys/comment/queryById`


**请求方式**:`GET`


**请求数据类型**:`application/x-www-form-urlencoded`


**响应数据类型**:`*/*`


**接口描述**:<p>系统评论回复表-通过id查询</p>



**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|id|id|query|true|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«sys_comment对象»|
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|sys_comment对象|sys_comment对象|
|&emsp;&emsp;commentContent|回复内容|string||
|&emsp;&emsp;commentId|评论id(允许为空，不为空时，则为回复)|string||
|&emsp;&emsp;createBy|创建人|string||
|&emsp;&emsp;createTime|创建日期|string(date-time)||
|&emsp;&emsp;fromUserId|来源用户id|string||
|&emsp;&emsp;id|id|string||
|&emsp;&emsp;tableDataId|数据id|string||
|&emsp;&emsp;tableName|表名|string||
|&emsp;&emsp;toUserId|发送给用户id(允许为空)|string||
|&emsp;&emsp;updateBy|更新人|string||
|&emsp;&emsp;updateTime|更新日期|string(date-time)||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": {
		"commentContent": "",
		"commentId": "",
		"createBy": "",
		"createTime": "",
		"fromUserId": "",
		"id": "",
		"tableDataId": "",
		"tableName": "",
		"toUserId": "",
		"updateBy": "",
		"updateTime": ""
	},
	"success": true,
	"timestamp": 0
}
```


# 编码校验规则


## 编码校验规则-添加


**接口地址**:`/nnzk/sys/checkRule/add`


**请求方式**:`POST`


**请求数据类型**:`application/json`


**响应数据类型**:`*/*`


**接口描述**:<p>编码校验规则-添加</p>



**请求示例**:


```javascript
{
  "createBy": "",
  "createTime": "",
  "id": "",
  "ruleCode": "",
  "ruleDescription": "",
  "ruleJson": "",
  "ruleName": "",
  "updateBy": "",
  "updateTime": ""
}
```


**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|sysCheckRule|编码校验规则|body|true|sys_check_rule对象|sys_check_rule对象|
|&emsp;&emsp;createBy|创建人||false|string||
|&emsp;&emsp;createTime|创建时间||false|string(date-time)||
|&emsp;&emsp;id|主键id||false|string||
|&emsp;&emsp;ruleCode|规则Code||false|string||
|&emsp;&emsp;ruleDescription|规则描述||false|string||
|&emsp;&emsp;ruleJson|规则JSON||false|string||
|&emsp;&emsp;ruleName|规则名称||false|string||
|&emsp;&emsp;updateBy|更新人||false|string||
|&emsp;&emsp;updateTime|更新时间||false|string(date-time)||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象|
|201|Created||
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|object||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": {},
	"success": true,
	"timestamp": 0
}
```


## 编码校验规则-通过Code校验传入的值


**接口地址**:`/nnzk/sys/checkRule/checkByCode`


**请求方式**:`GET`


**请求数据类型**:`application/x-www-form-urlencoded`


**响应数据类型**:`*/*`


**接口描述**:<p>编码校验规则-通过Code校验传入的值</p>



**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|ruleCode|ruleCode|query|true|string||
|value|value|query|true|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象|
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|object||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": {},
	"success": true,
	"timestamp": 0
}
```


## 编码校验规则-通过id删除


**接口地址**:`/nnzk/sys/checkRule/delete`


**请求方式**:`DELETE`


**请求数据类型**:`application/x-www-form-urlencoded`


**响应数据类型**:`*/*`


**接口描述**:<p>编码校验规则-通过id删除</p>



**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|id|id|query|true|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象|
|204|No Content||
|401|Unauthorized||
|403|Forbidden||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|object||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": {},
	"success": true,
	"timestamp": 0
}
```


## 编码校验规则-批量删除


**接口地址**:`/nnzk/sys/checkRule/deleteBatch`


**请求方式**:`DELETE`


**请求数据类型**:`application/x-www-form-urlencoded`


**响应数据类型**:`*/*`


**接口描述**:<p>编码校验规则-批量删除</p>



**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|ids|ids|query|true|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象|
|204|No Content||
|401|Unauthorized||
|403|Forbidden||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|object||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": {},
	"success": true,
	"timestamp": 0
}
```


## 编码校验规则-编辑


**接口地址**:`/nnzk/sys/checkRule/edit`


**请求方式**:`POST`


**请求数据类型**:`application/json`


**响应数据类型**:`*/*`


**接口描述**:<p>编码校验规则-编辑</p>



**请求示例**:


```javascript
{
  "createBy": "",
  "createTime": "",
  "id": "",
  "ruleCode": "",
  "ruleDescription": "",
  "ruleJson": "",
  "ruleName": "",
  "updateBy": "",
  "updateTime": ""
}
```


**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|sysCheckRule|编码校验规则|body|true|sys_check_rule对象|sys_check_rule对象|
|&emsp;&emsp;createBy|创建人||false|string||
|&emsp;&emsp;createTime|创建时间||false|string(date-time)||
|&emsp;&emsp;id|主键id||false|string||
|&emsp;&emsp;ruleCode|规则Code||false|string||
|&emsp;&emsp;ruleDescription|规则描述||false|string||
|&emsp;&emsp;ruleJson|规则JSON||false|string||
|&emsp;&emsp;ruleName|规则名称||false|string||
|&emsp;&emsp;updateBy|更新人||false|string||
|&emsp;&emsp;updateTime|更新时间||false|string(date-time)||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象|
|201|Created||
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|object||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": {},
	"success": true,
	"timestamp": 0
}
```


## 编码校验规则-编辑


**接口地址**:`/nnzk/sys/checkRule/edit`


**请求方式**:`PUT`


**请求数据类型**:`application/json`


**响应数据类型**:`*/*`


**接口描述**:<p>编码校验规则-编辑</p>



**请求示例**:


```javascript
{
  "createBy": "",
  "createTime": "",
  "id": "",
  "ruleCode": "",
  "ruleDescription": "",
  "ruleJson": "",
  "ruleName": "",
  "updateBy": "",
  "updateTime": ""
}
```


**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|sysCheckRule|编码校验规则|body|true|sys_check_rule对象|sys_check_rule对象|
|&emsp;&emsp;createBy|创建人||false|string||
|&emsp;&emsp;createTime|创建时间||false|string(date-time)||
|&emsp;&emsp;id|主键id||false|string||
|&emsp;&emsp;ruleCode|规则Code||false|string||
|&emsp;&emsp;ruleDescription|规则描述||false|string||
|&emsp;&emsp;ruleJson|规则JSON||false|string||
|&emsp;&emsp;ruleName|规则名称||false|string||
|&emsp;&emsp;updateBy|更新人||false|string||
|&emsp;&emsp;updateTime|更新时间||false|string(date-time)||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象|
|201|Created||
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|object||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": {},
	"success": true,
	"timestamp": 0
}
```


## 编码校验规则-分页列表查询


**接口地址**:`/nnzk/sys/checkRule/list`


**请求方式**:`GET`


**请求数据类型**:`application/x-www-form-urlencoded`


**响应数据类型**:`*/*`


**接口描述**:<p>编码校验规则-分页列表查询</p>



**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|createBy|创建人|query|false|string||
|createTime|创建时间|query|false|string(date-time)||
|id|主键id|query|false|string||
|pageNo|pageNo|query|false|integer(int32)||
|pageSize|pageSize|query|false|integer(int32)||
|ruleCode|规则Code|query|false|string||
|ruleDescription|规则描述|query|false|string||
|ruleJson|规则JSON|query|false|string||
|ruleName|规则名称|query|false|string||
|updateBy|更新人|query|false|string||
|updateTime|更新时间|query|false|string(date-time)||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象|
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|object||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": {},
	"success": true,
	"timestamp": 0
}
```


## 编码校验规则-通过id查询


**接口地址**:`/nnzk/sys/checkRule/queryById`


**请求方式**:`GET`


**请求数据类型**:`application/x-www-form-urlencoded`


**响应数据类型**:`*/*`


**接口描述**:<p>编码校验规则-通过id查询</p>



**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|id|id|query|true|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象|
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|object||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": {},
	"success": true,
	"timestamp": 0
}
```


# 网站公告表


## 网站公告表-添加


**接口地址**:`/nnzk/config/webNotice/add`


**请求方式**:`POST`


**请求数据类型**:`application/json`


**响应数据类型**:`*/*`


**接口描述**:<p>网站公告表-添加</p>



**请求示例**:


```javascript
{
  "content": "",
  "createBy": "",
  "createTime": "",
  "delFlag": 0,
  "enable": 0,
  "id": "",
  "name": "",
  "sortOrder": 0,
  "updateBy": "",
  "updateTime": ""
}
```


**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|webNotice|网站公告表|body|true|web_notice对象|web_notice对象|
|&emsp;&emsp;content|内容||false|string||
|&emsp;&emsp;createBy|创建人||false|string||
|&emsp;&emsp;createTime|创建日期||false|string(date-time)||
|&emsp;&emsp;delFlag|删除标识||false|integer(int32)||
|&emsp;&emsp;enable|是否启用||false|integer(int32)||
|&emsp;&emsp;id|主键||false|string||
|&emsp;&emsp;name|名称||false|string||
|&emsp;&emsp;sortOrder|顺序||false|integer(int32)||
|&emsp;&emsp;updateBy|更新人||false|string||
|&emsp;&emsp;updateTime|更新日期||false|string(date-time)||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«string»|
|201|Created||
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|string||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": "",
	"success": true,
	"timestamp": 0
}
```


## 网站公告表-通过id删除


**接口地址**:`/nnzk/config/webNotice/delete`


**请求方式**:`DELETE`


**请求数据类型**:`application/x-www-form-urlencoded`


**响应数据类型**:`*/*`


**接口描述**:<p>网站公告表-通过id删除</p>



**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|id|id|query|true|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«string»|
|204|No Content||
|401|Unauthorized||
|403|Forbidden||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|string||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": "",
	"success": true,
	"timestamp": 0
}
```


## 网站公告表-批量删除


**接口地址**:`/nnzk/config/webNotice/deleteBatch`


**请求方式**:`DELETE`


**请求数据类型**:`application/x-www-form-urlencoded`


**响应数据类型**:`*/*`


**接口描述**:<p>网站公告表-批量删除</p>



**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|ids|ids|query|true|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«string»|
|204|No Content||
|401|Unauthorized||
|403|Forbidden||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|string||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": "",
	"success": true,
	"timestamp": 0
}
```


## 网站公告表-编辑


**接口地址**:`/nnzk/config/webNotice/edit`


**请求方式**:`POST`


**请求数据类型**:`application/json`


**响应数据类型**:`*/*`


**接口描述**:<p>网站公告表-编辑</p>



**请求示例**:


```javascript
{
  "content": "",
  "createBy": "",
  "createTime": "",
  "delFlag": 0,
  "enable": 0,
  "id": "",
  "name": "",
  "sortOrder": 0,
  "updateBy": "",
  "updateTime": ""
}
```


**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|webNotice|网站公告表|body|true|web_notice对象|web_notice对象|
|&emsp;&emsp;content|内容||false|string||
|&emsp;&emsp;createBy|创建人||false|string||
|&emsp;&emsp;createTime|创建日期||false|string(date-time)||
|&emsp;&emsp;delFlag|删除标识||false|integer(int32)||
|&emsp;&emsp;enable|是否启用||false|integer(int32)||
|&emsp;&emsp;id|主键||false|string||
|&emsp;&emsp;name|名称||false|string||
|&emsp;&emsp;sortOrder|顺序||false|integer(int32)||
|&emsp;&emsp;updateBy|更新人||false|string||
|&emsp;&emsp;updateTime|更新日期||false|string(date-time)||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«string»|
|201|Created||
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|string||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": "",
	"success": true,
	"timestamp": 0
}
```


## 网站公告表-编辑


**接口地址**:`/nnzk/config/webNotice/edit`


**请求方式**:`PUT`


**请求数据类型**:`application/json`


**响应数据类型**:`*/*`


**接口描述**:<p>网站公告表-编辑</p>



**请求示例**:


```javascript
{
  "content": "",
  "createBy": "",
  "createTime": "",
  "delFlag": 0,
  "enable": 0,
  "id": "",
  "name": "",
  "sortOrder": 0,
  "updateBy": "",
  "updateTime": ""
}
```


**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|webNotice|网站公告表|body|true|web_notice对象|web_notice对象|
|&emsp;&emsp;content|内容||false|string||
|&emsp;&emsp;createBy|创建人||false|string||
|&emsp;&emsp;createTime|创建日期||false|string(date-time)||
|&emsp;&emsp;delFlag|删除标识||false|integer(int32)||
|&emsp;&emsp;enable|是否启用||false|integer(int32)||
|&emsp;&emsp;id|主键||false|string||
|&emsp;&emsp;name|名称||false|string||
|&emsp;&emsp;sortOrder|顺序||false|integer(int32)||
|&emsp;&emsp;updateBy|更新人||false|string||
|&emsp;&emsp;updateTime|更新日期||false|string(date-time)||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«string»|
|201|Created||
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|string||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": "",
	"success": true,
	"timestamp": 0
}
```


## 网站公告表-分页列表查询


**接口地址**:`/nnzk/config/webNotice/list`


**请求方式**:`GET`


**请求数据类型**:`application/x-www-form-urlencoded`


**响应数据类型**:`*/*`


**接口描述**:<p>网站公告表-分页列表查询</p>



**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|content|内容|query|true|string||
|enable|是否启用|query|true|integer(int32)||
|name|名称|query|true|string||
|sortOrder|顺序|query|true|integer(int32)||
|createBy|创建人|query|false|string||
|createTime|创建日期|query|false|string(date-time)||
|delFlag|删除标识|query|false|integer(int32)||
|id|主键|query|false|string||
|pageNo|pageNo|query|false|integer(int32)||
|pageSize|pageSize|query|false|integer(int32)||
|updateBy|更新人|query|false|string||
|updateTime|更新日期|query|false|string(date-time)||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«IPage«web_notice对象»»|
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|IPage«web_notice对象»|IPage«web_notice对象»|
|&emsp;&emsp;current||integer(int64)||
|&emsp;&emsp;pages||integer(int64)||
|&emsp;&emsp;records||array|web_notice对象|
|&emsp;&emsp;&emsp;&emsp;content|内容|string||
|&emsp;&emsp;&emsp;&emsp;createBy|创建人|string||
|&emsp;&emsp;&emsp;&emsp;createTime|创建日期|string||
|&emsp;&emsp;&emsp;&emsp;delFlag|删除标识|integer||
|&emsp;&emsp;&emsp;&emsp;enable|是否启用|integer||
|&emsp;&emsp;&emsp;&emsp;id|主键|string||
|&emsp;&emsp;&emsp;&emsp;name|名称|string||
|&emsp;&emsp;&emsp;&emsp;sortOrder|顺序|integer||
|&emsp;&emsp;&emsp;&emsp;updateBy|更新人|string||
|&emsp;&emsp;&emsp;&emsp;updateTime|更新日期|string||
|&emsp;&emsp;size||integer(int64)||
|&emsp;&emsp;total||integer(int64)||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": {
		"current": 0,
		"pages": 0,
		"records": [
			{
				"content": "",
				"createBy": "",
				"createTime": "",
				"delFlag": 0,
				"enable": 0,
				"id": "",
				"name": "",
				"sortOrder": 0,
				"updateBy": "",
				"updateTime": ""
			}
		],
		"size": 0,
		"total": 0
	},
	"success": true,
	"timestamp": 0
}
```


## 公告表-（启用状态）列表查询


**接口地址**:`/nnzk/config/webNotice/listValid`


**请求方式**:`GET`


**请求数据类型**:`application/x-www-form-urlencoded`


**响应数据类型**:`*/*`


**接口描述**:<p>公告表-（启用状态）列表查询</p>



**请求参数**:


暂无


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«List«web_notice对象»»|
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|array|web_notice对象|
|&emsp;&emsp;content|内容|string||
|&emsp;&emsp;createBy|创建人|string||
|&emsp;&emsp;createTime|创建日期|string(date-time)||
|&emsp;&emsp;delFlag|删除标识|integer(int32)||
|&emsp;&emsp;enable|是否启用|integer(int32)||
|&emsp;&emsp;id|主键|string||
|&emsp;&emsp;name|名称|string||
|&emsp;&emsp;sortOrder|顺序|integer(int32)||
|&emsp;&emsp;updateBy|更新人|string||
|&emsp;&emsp;updateTime|更新日期|string(date-time)||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": [
		{
			"content": "",
			"createBy": "",
			"createTime": "",
			"delFlag": 0,
			"enable": 0,
			"id": "",
			"name": "",
			"sortOrder": 0,
			"updateBy": "",
			"updateTime": ""
		}
	],
	"success": true,
	"timestamp": 0
}
```


## 网站公告表-通过id查询


**接口地址**:`/nnzk/config/webNotice/queryById`


**请求方式**:`GET`


**请求数据类型**:`application/x-www-form-urlencoded`


**响应数据类型**:`*/*`


**接口描述**:<p>网站公告表-通过id查询</p>



**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|id|id|query|true|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«web_notice对象»|
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|web_notice对象|web_notice对象|
|&emsp;&emsp;content|内容|string||
|&emsp;&emsp;createBy|创建人|string||
|&emsp;&emsp;createTime|创建日期|string(date-time)||
|&emsp;&emsp;delFlag|删除标识|integer(int32)||
|&emsp;&emsp;enable|是否启用|integer(int32)||
|&emsp;&emsp;id|主键|string||
|&emsp;&emsp;name|名称|string||
|&emsp;&emsp;sortOrder|顺序|integer(int32)||
|&emsp;&emsp;updateBy|更新人|string||
|&emsp;&emsp;updateTime|更新日期|string(date-time)||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": {
		"content": "",
		"createBy": "",
		"createTime": "",
		"delFlag": 0,
		"enable": 0,
		"id": "",
		"name": "",
		"sortOrder": 0,
		"updateBy": "",
		"updateTime": ""
	},
	"success": true,
	"timestamp": 0
}
```


# 网站配置表


## 网站配置表-添加


**接口地址**:`/nnzk/config/webConfig/add`


**请求方式**:`POST`


**请求数据类型**:`application/json`


**响应数据类型**:`*/*`


**接口描述**:<p>网站配置表-添加</p>



**请求示例**:


```javascript
{
  "createBy": "",
  "createTime": "",
  "delFlag": 0,
  "id": "",
  "name": "",
  "remark": "",
  "updateBy": "",
  "updateTime": "",
  "value": ""
}
```


**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|webConfig|网站配置表|body|true|web_config对象|web_config对象|
|&emsp;&emsp;createBy|创建人||false|string||
|&emsp;&emsp;createTime|创建日期||false|string(date-time)||
|&emsp;&emsp;delFlag|删除标识||false|integer(int32)||
|&emsp;&emsp;id|主键||false|string||
|&emsp;&emsp;name|配置名称||false|string||
|&emsp;&emsp;remark|配置值||false|string||
|&emsp;&emsp;updateBy|更新人||false|string||
|&emsp;&emsp;updateTime|更新日期||false|string(date-time)||
|&emsp;&emsp;value|配置值||false|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«string»|
|201|Created||
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|string||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": "",
	"success": true,
	"timestamp": 0
}
```


## 网站配置表-通过id删除


**接口地址**:`/nnzk/config/webConfig/delete`


**请求方式**:`DELETE`


**请求数据类型**:`application/x-www-form-urlencoded`


**响应数据类型**:`*/*`


**接口描述**:<p>网站配置表-通过id删除</p>



**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|id|id|query|true|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«string»|
|204|No Content||
|401|Unauthorized||
|403|Forbidden||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|string||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": "",
	"success": true,
	"timestamp": 0
}
```


## 网站配置表-批量删除


**接口地址**:`/nnzk/config/webConfig/deleteBatch`


**请求方式**:`DELETE`


**请求数据类型**:`application/x-www-form-urlencoded`


**响应数据类型**:`*/*`


**接口描述**:<p>网站配置表-批量删除</p>



**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|ids|ids|query|true|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«string»|
|204|No Content||
|401|Unauthorized||
|403|Forbidden||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|string||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": "",
	"success": true,
	"timestamp": 0
}
```


## 网站配置表-编辑


**接口地址**:`/nnzk/config/webConfig/edit`


**请求方式**:`POST`


**请求数据类型**:`application/json`


**响应数据类型**:`*/*`


**接口描述**:<p>网站配置表-编辑</p>



**请求示例**:


```javascript
{
  "createBy": "",
  "createTime": "",
  "delFlag": 0,
  "id": "",
  "name": "",
  "remark": "",
  "updateBy": "",
  "updateTime": "",
  "value": ""
}
```


**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|webConfig|网站配置表|body|true|web_config对象|web_config对象|
|&emsp;&emsp;createBy|创建人||false|string||
|&emsp;&emsp;createTime|创建日期||false|string(date-time)||
|&emsp;&emsp;delFlag|删除标识||false|integer(int32)||
|&emsp;&emsp;id|主键||false|string||
|&emsp;&emsp;name|配置名称||false|string||
|&emsp;&emsp;remark|配置值||false|string||
|&emsp;&emsp;updateBy|更新人||false|string||
|&emsp;&emsp;updateTime|更新日期||false|string(date-time)||
|&emsp;&emsp;value|配置值||false|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«string»|
|201|Created||
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|string||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": "",
	"success": true,
	"timestamp": 0
}
```


## 网站配置表-编辑


**接口地址**:`/nnzk/config/webConfig/edit`


**请求方式**:`PUT`


**请求数据类型**:`application/json`


**响应数据类型**:`*/*`


**接口描述**:<p>网站配置表-编辑</p>



**请求示例**:


```javascript
{
  "createBy": "",
  "createTime": "",
  "delFlag": 0,
  "id": "",
  "name": "",
  "remark": "",
  "updateBy": "",
  "updateTime": "",
  "value": ""
}
```


**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|webConfig|网站配置表|body|true|web_config对象|web_config对象|
|&emsp;&emsp;createBy|创建人||false|string||
|&emsp;&emsp;createTime|创建日期||false|string(date-time)||
|&emsp;&emsp;delFlag|删除标识||false|integer(int32)||
|&emsp;&emsp;id|主键||false|string||
|&emsp;&emsp;name|配置名称||false|string||
|&emsp;&emsp;remark|配置值||false|string||
|&emsp;&emsp;updateBy|更新人||false|string||
|&emsp;&emsp;updateTime|更新日期||false|string(date-time)||
|&emsp;&emsp;value|配置值||false|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«string»|
|201|Created||
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|string||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": "",
	"success": true,
	"timestamp": 0
}
```


## 网站配置表-查询全部


**接口地址**:`/nnzk/config/webConfig/getConfig`


**请求方式**:`GET`


**请求数据类型**:`application/x-www-form-urlencoded`


**响应数据类型**:`*/*`


**接口描述**:<p>网站配置表-查询全部</p>



**请求参数**:


暂无


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«List«WebConfigDTO»»|
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|array|WebConfigDTO|
|&emsp;&emsp;name|配置名称|string||
|&emsp;&emsp;value|配置值|string||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": [
		{
			"name": "",
			"value": ""
		}
	],
	"success": true,
	"timestamp": 0
}
```


## 网站配置表-是否开放八年级查询成绩


**接口地址**:`/nnzk/config/webConfig/isEighthGradeQueryScoreOpen`


**请求方式**:`GET`


**请求数据类型**:`application/x-www-form-urlencoded`


**响应数据类型**:`*/*`


**接口描述**:<p>网站配置表-是否开放八年级查询成绩</p>



**请求参数**:


暂无


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«boolean»|
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|boolean||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": true,
	"success": true,
	"timestamp": 0
}
```


## 网站配置表-分页列表查询


**接口地址**:`/nnzk/config/webConfig/list`


**请求方式**:`GET`


**请求数据类型**:`application/x-www-form-urlencoded`


**响应数据类型**:`*/*`


**接口描述**:<p>网站配置表-分页列表查询</p>



**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|name|配置名称|query|true|string||
|value|配置值|query|true|string||
|createBy|创建人|query|false|string||
|createTime|创建日期|query|false|string(date-time)||
|delFlag|删除标识|query|false|integer(int32)||
|id|主键|query|false|string||
|pageNo|pageNo|query|false|integer(int32)||
|pageSize|pageSize|query|false|integer(int32)||
|remark|配置值|query|false|string||
|updateBy|更新人|query|false|string||
|updateTime|更新日期|query|false|string(date-time)||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«IPage«web_config对象»»|
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|IPage«web_config对象»|IPage«web_config对象»|
|&emsp;&emsp;current||integer(int64)||
|&emsp;&emsp;pages||integer(int64)||
|&emsp;&emsp;records||array|web_config对象|
|&emsp;&emsp;&emsp;&emsp;createBy|创建人|string||
|&emsp;&emsp;&emsp;&emsp;createTime|创建日期|string||
|&emsp;&emsp;&emsp;&emsp;delFlag|删除标识|integer||
|&emsp;&emsp;&emsp;&emsp;id|主键|string||
|&emsp;&emsp;&emsp;&emsp;name|配置名称|string||
|&emsp;&emsp;&emsp;&emsp;remark|配置值|string||
|&emsp;&emsp;&emsp;&emsp;updateBy|更新人|string||
|&emsp;&emsp;&emsp;&emsp;updateTime|更新日期|string||
|&emsp;&emsp;&emsp;&emsp;value|配置值|string||
|&emsp;&emsp;size||integer(int64)||
|&emsp;&emsp;total||integer(int64)||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": {
		"current": 0,
		"pages": 0,
		"records": [
			{
				"createBy": "",
				"createTime": "",
				"delFlag": 0,
				"id": "",
				"name": "",
				"remark": "",
				"updateBy": "",
				"updateTime": "",
				"value": ""
			}
		],
		"size": 0,
		"total": 0
	},
	"success": true,
	"timestamp": 0
}
```


## 网站配置表-通过id查询


**接口地址**:`/nnzk/config/webConfig/queryById`


**请求方式**:`GET`


**请求数据类型**:`application/x-www-form-urlencoded`


**响应数据类型**:`*/*`


**接口描述**:<p>网站配置表-通过id查询</p>



**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|id|id|query|true|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«web_config对象»|
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|web_config对象|web_config对象|
|&emsp;&emsp;createBy|创建人|string||
|&emsp;&emsp;createTime|创建日期|string(date-time)||
|&emsp;&emsp;delFlag|删除标识|integer(int32)||
|&emsp;&emsp;id|主键|string||
|&emsp;&emsp;name|配置名称|string||
|&emsp;&emsp;remark|配置值|string||
|&emsp;&emsp;updateBy|更新人|string||
|&emsp;&emsp;updateTime|更新日期|string(date-time)||
|&emsp;&emsp;value|配置值|string||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": {
		"createBy": "",
		"createTime": "",
		"delFlag": 0,
		"id": "",
		"name": "",
		"remark": "",
		"updateBy": "",
		"updateTime": "",
		"value": ""
	},
	"success": true,
	"timestamp": 0
}
```


# 职务表


## 职务表-添加


**接口地址**:`/nnzk/sys/position/add`


**请求方式**:`POST`


**请求数据类型**:`application/json`


**响应数据类型**:`*/*`


**接口描述**:<p>职务表-添加</p>



**请求示例**:


```javascript
{
  "code": "",
  "companyId": "",
  "createBy": "",
  "createTime": "",
  "id": "",
  "name": "",
  "postRank": "",
  "sysOrgCode": "",
  "tenantId": 0,
  "updateBy": "",
  "updateTime": ""
}
```


**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|sysPosition|职务表|body|true|sys_position对象|sys_position对象|
|&emsp;&emsp;code|职务编码||false|string||
|&emsp;&emsp;companyId|公司id||false|string||
|&emsp;&emsp;createBy|创建人||false|string||
|&emsp;&emsp;createTime|创建时间||false|string(date-time)||
|&emsp;&emsp;id|id||false|string||
|&emsp;&emsp;name|职务名称||false|string||
|&emsp;&emsp;postRank|职级||false|string||
|&emsp;&emsp;sysOrgCode|组织机构编码||false|string||
|&emsp;&emsp;tenantId|租户ID||false|integer(int32)||
|&emsp;&emsp;updateBy|修改人||false|string||
|&emsp;&emsp;updateTime|修改时间||false|string(date-time)||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«sys_position对象»|
|201|Created||
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|sys_position对象|sys_position对象|
|&emsp;&emsp;code|职务编码|string||
|&emsp;&emsp;companyId|公司id|string||
|&emsp;&emsp;createBy|创建人|string||
|&emsp;&emsp;createTime|创建时间|string(date-time)||
|&emsp;&emsp;id|id|string||
|&emsp;&emsp;name|职务名称|string||
|&emsp;&emsp;postRank|职级|string||
|&emsp;&emsp;sysOrgCode|组织机构编码|string||
|&emsp;&emsp;tenantId|租户ID|integer(int32)||
|&emsp;&emsp;updateBy|修改人|string||
|&emsp;&emsp;updateTime|修改时间|string(date-time)||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": {
		"code": "",
		"companyId": "",
		"createBy": "",
		"createTime": "",
		"id": "",
		"name": "",
		"postRank": "",
		"sysOrgCode": "",
		"tenantId": 0,
		"updateBy": "",
		"updateTime": ""
	},
	"success": true,
	"timestamp": 0
}
```


## 职务表-通过id删除


**接口地址**:`/nnzk/sys/position/delete`


**请求方式**:`DELETE`


**请求数据类型**:`application/x-www-form-urlencoded`


**响应数据类型**:`*/*`


**接口描述**:<p>职务表-通过id删除</p>



**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|id|id|query|true|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«object»|
|204|No Content||
|401|Unauthorized||
|403|Forbidden||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|object||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": {},
	"success": true,
	"timestamp": 0
}
```


## 职务表-批量删除


**接口地址**:`/nnzk/sys/position/deleteBatch`


**请求方式**:`DELETE`


**请求数据类型**:`application/x-www-form-urlencoded`


**响应数据类型**:`*/*`


**接口描述**:<p>职务表-批量删除</p>



**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|ids|ids|query|true|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«sys_position对象»|
|204|No Content||
|401|Unauthorized||
|403|Forbidden||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|sys_position对象|sys_position对象|
|&emsp;&emsp;code|职务编码|string||
|&emsp;&emsp;companyId|公司id|string||
|&emsp;&emsp;createBy|创建人|string||
|&emsp;&emsp;createTime|创建时间|string(date-time)||
|&emsp;&emsp;id|id|string||
|&emsp;&emsp;name|职务名称|string||
|&emsp;&emsp;postRank|职级|string||
|&emsp;&emsp;sysOrgCode|组织机构编码|string||
|&emsp;&emsp;tenantId|租户ID|integer(int32)||
|&emsp;&emsp;updateBy|修改人|string||
|&emsp;&emsp;updateTime|修改时间|string(date-time)||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": {
		"code": "",
		"companyId": "",
		"createBy": "",
		"createTime": "",
		"id": "",
		"name": "",
		"postRank": "",
		"sysOrgCode": "",
		"tenantId": 0,
		"updateBy": "",
		"updateTime": ""
	},
	"success": true,
	"timestamp": 0
}
```


## 职务表-编辑


**接口地址**:`/nnzk/sys/position/edit`


**请求方式**:`POST`


**请求数据类型**:`application/json`


**响应数据类型**:`*/*`


**接口描述**:<p>职务表-编辑</p>



**请求示例**:


```javascript
{
  "code": "",
  "companyId": "",
  "createBy": "",
  "createTime": "",
  "id": "",
  "name": "",
  "postRank": "",
  "sysOrgCode": "",
  "tenantId": 0,
  "updateBy": "",
  "updateTime": ""
}
```


**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|sysPosition|职务表|body|true|sys_position对象|sys_position对象|
|&emsp;&emsp;code|职务编码||false|string||
|&emsp;&emsp;companyId|公司id||false|string||
|&emsp;&emsp;createBy|创建人||false|string||
|&emsp;&emsp;createTime|创建时间||false|string(date-time)||
|&emsp;&emsp;id|id||false|string||
|&emsp;&emsp;name|职务名称||false|string||
|&emsp;&emsp;postRank|职级||false|string||
|&emsp;&emsp;sysOrgCode|组织机构编码||false|string||
|&emsp;&emsp;tenantId|租户ID||false|integer(int32)||
|&emsp;&emsp;updateBy|修改人||false|string||
|&emsp;&emsp;updateTime|修改时间||false|string(date-time)||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«sys_position对象»|
|201|Created||
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|sys_position对象|sys_position对象|
|&emsp;&emsp;code|职务编码|string||
|&emsp;&emsp;companyId|公司id|string||
|&emsp;&emsp;createBy|创建人|string||
|&emsp;&emsp;createTime|创建时间|string(date-time)||
|&emsp;&emsp;id|id|string||
|&emsp;&emsp;name|职务名称|string||
|&emsp;&emsp;postRank|职级|string||
|&emsp;&emsp;sysOrgCode|组织机构编码|string||
|&emsp;&emsp;tenantId|租户ID|integer(int32)||
|&emsp;&emsp;updateBy|修改人|string||
|&emsp;&emsp;updateTime|修改时间|string(date-time)||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": {
		"code": "",
		"companyId": "",
		"createBy": "",
		"createTime": "",
		"id": "",
		"name": "",
		"postRank": "",
		"sysOrgCode": "",
		"tenantId": 0,
		"updateBy": "",
		"updateTime": ""
	},
	"success": true,
	"timestamp": 0
}
```


## 职务表-编辑


**接口地址**:`/nnzk/sys/position/edit`


**请求方式**:`PUT`


**请求数据类型**:`application/json`


**响应数据类型**:`*/*`


**接口描述**:<p>职务表-编辑</p>



**请求示例**:


```javascript
{
  "code": "",
  "companyId": "",
  "createBy": "",
  "createTime": "",
  "id": "",
  "name": "",
  "postRank": "",
  "sysOrgCode": "",
  "tenantId": 0,
  "updateBy": "",
  "updateTime": ""
}
```


**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|sysPosition|职务表|body|true|sys_position对象|sys_position对象|
|&emsp;&emsp;code|职务编码||false|string||
|&emsp;&emsp;companyId|公司id||false|string||
|&emsp;&emsp;createBy|创建人||false|string||
|&emsp;&emsp;createTime|创建时间||false|string(date-time)||
|&emsp;&emsp;id|id||false|string||
|&emsp;&emsp;name|职务名称||false|string||
|&emsp;&emsp;postRank|职级||false|string||
|&emsp;&emsp;sysOrgCode|组织机构编码||false|string||
|&emsp;&emsp;tenantId|租户ID||false|integer(int32)||
|&emsp;&emsp;updateBy|修改人||false|string||
|&emsp;&emsp;updateTime|修改时间||false|string(date-time)||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«sys_position对象»|
|201|Created||
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|sys_position对象|sys_position对象|
|&emsp;&emsp;code|职务编码|string||
|&emsp;&emsp;companyId|公司id|string||
|&emsp;&emsp;createBy|创建人|string||
|&emsp;&emsp;createTime|创建时间|string(date-time)||
|&emsp;&emsp;id|id|string||
|&emsp;&emsp;name|职务名称|string||
|&emsp;&emsp;postRank|职级|string||
|&emsp;&emsp;sysOrgCode|组织机构编码|string||
|&emsp;&emsp;tenantId|租户ID|integer(int32)||
|&emsp;&emsp;updateBy|修改人|string||
|&emsp;&emsp;updateTime|修改时间|string(date-time)||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": {
		"code": "",
		"companyId": "",
		"createBy": "",
		"createTime": "",
		"id": "",
		"name": "",
		"postRank": "",
		"sysOrgCode": "",
		"tenantId": 0,
		"updateBy": "",
		"updateTime": ""
	},
	"success": true,
	"timestamp": 0
}
```


## 职务表-分页列表查询


**接口地址**:`/nnzk/sys/position/list`


**请求方式**:`GET`


**请求数据类型**:`application/x-www-form-urlencoded`


**响应数据类型**:`*/*`


**接口描述**:<p>职务表-分页列表查询</p>



**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|code|职务编码|query|false|string||
|companyId|公司id|query|false|string||
|createBy|创建人|query|false|string||
|createTime|创建时间|query|false|string(date-time)||
|id|id|query|false|string||
|name|职务名称|query|false|string||
|pageNo|pageNo|query|false|integer(int32)||
|pageSize|pageSize|query|false|integer(int32)||
|postRank|职级|query|false|string||
|sysOrgCode|组织机构编码|query|false|string||
|tenantId|租户ID|query|false|integer(int32)||
|updateBy|修改人|query|false|string||
|updateTime|修改时间|query|false|string(date-time)||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«IPage«sys_position对象»»|
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|IPage«sys_position对象»|IPage«sys_position对象»|
|&emsp;&emsp;current||integer(int64)||
|&emsp;&emsp;pages||integer(int64)||
|&emsp;&emsp;records||array|sys_position对象|
|&emsp;&emsp;&emsp;&emsp;code|职务编码|string||
|&emsp;&emsp;&emsp;&emsp;companyId|公司id|string||
|&emsp;&emsp;&emsp;&emsp;createBy|创建人|string||
|&emsp;&emsp;&emsp;&emsp;createTime|创建时间|string||
|&emsp;&emsp;&emsp;&emsp;id|id|string||
|&emsp;&emsp;&emsp;&emsp;name|职务名称|string||
|&emsp;&emsp;&emsp;&emsp;postRank|职级|string||
|&emsp;&emsp;&emsp;&emsp;sysOrgCode|组织机构编码|string||
|&emsp;&emsp;&emsp;&emsp;tenantId|租户ID|integer||
|&emsp;&emsp;&emsp;&emsp;updateBy|修改人|string||
|&emsp;&emsp;&emsp;&emsp;updateTime|修改时间|string||
|&emsp;&emsp;size||integer(int64)||
|&emsp;&emsp;total||integer(int64)||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": {
		"current": 0,
		"pages": 0,
		"records": [
			{
				"code": "",
				"companyId": "",
				"createBy": "",
				"createTime": "",
				"id": "",
				"name": "",
				"postRank": "",
				"sysOrgCode": "",
				"tenantId": 0,
				"updateBy": "",
				"updateTime": ""
			}
		],
		"size": 0,
		"total": 0
	},
	"success": true,
	"timestamp": 0
}
```


## 职务表-通过code查询


**接口地址**:`/nnzk/sys/position/queryByCode`


**请求方式**:`GET`


**请求数据类型**:`application/x-www-form-urlencoded`


**响应数据类型**:`*/*`


**接口描述**:<p>职务表-通过code查询</p>



**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|code|code|query|true|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«sys_position对象»|
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|sys_position对象|sys_position对象|
|&emsp;&emsp;code|职务编码|string||
|&emsp;&emsp;companyId|公司id|string||
|&emsp;&emsp;createBy|创建人|string||
|&emsp;&emsp;createTime|创建时间|string(date-time)||
|&emsp;&emsp;id|id|string||
|&emsp;&emsp;name|职务名称|string||
|&emsp;&emsp;postRank|职级|string||
|&emsp;&emsp;sysOrgCode|组织机构编码|string||
|&emsp;&emsp;tenantId|租户ID|integer(int32)||
|&emsp;&emsp;updateBy|修改人|string||
|&emsp;&emsp;updateTime|修改时间|string(date-time)||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": {
		"code": "",
		"companyId": "",
		"createBy": "",
		"createTime": "",
		"id": "",
		"name": "",
		"postRank": "",
		"sysOrgCode": "",
		"tenantId": 0,
		"updateBy": "",
		"updateTime": ""
	},
	"success": true,
	"timestamp": 0
}
```


## 职务表-通过id查询


**接口地址**:`/nnzk/sys/position/queryById`


**请求方式**:`GET`


**请求数据类型**:`application/x-www-form-urlencoded`


**响应数据类型**:`*/*`


**接口描述**:<p>职务表-通过id查询</p>



**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|id|id|query|true|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«sys_position对象»|
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|sys_position对象|sys_position对象|
|&emsp;&emsp;code|职务编码|string||
|&emsp;&emsp;companyId|公司id|string||
|&emsp;&emsp;createBy|创建人|string||
|&emsp;&emsp;createTime|创建时间|string(date-time)||
|&emsp;&emsp;id|id|string||
|&emsp;&emsp;name|职务名称|string||
|&emsp;&emsp;postRank|职级|string||
|&emsp;&emsp;sysOrgCode|组织机构编码|string||
|&emsp;&emsp;tenantId|租户ID|integer(int32)||
|&emsp;&emsp;updateBy|修改人|string||
|&emsp;&emsp;updateTime|修改时间|string(date-time)||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": {
		"code": "",
		"companyId": "",
		"createBy": "",
		"createTime": "",
		"id": "",
		"name": "",
		"postRank": "",
		"sysOrgCode": "",
		"tenantId": 0,
		"updateBy": "",
		"updateTime": ""
	},
	"success": true,
	"timestamp": 0
}
```


# 表单评论文件


## 表单评论文件-添加


**接口地址**:`/nnzk/sys/formFile/add`


**请求方式**:`POST`


**请求数据类型**:`application/json`


**响应数据类型**:`*/*`


**接口描述**:<p>表单评论文件-添加</p>



**请求示例**:


```javascript
{
  "createBy": "",
  "createTime": "",
  "fileId": "",
  "fileType": "",
  "id": "",
  "tableDataId": "",
  "tableName": ""
}
```


**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|sysFormFile|表单评论文件|body|true|sys_form_file对象|sys_form_file对象|
|&emsp;&emsp;createBy|创建人登录名称||false|string||
|&emsp;&emsp;createTime|创建日期||false|string(date-time)||
|&emsp;&emsp;fileId|关联文件id||false|string||
|&emsp;&emsp;fileType|文档类型（folder:文件夹 excel:excel doc:word pp:ppt image:图片  archive:其他文档 video:视频）||false|string||
|&emsp;&emsp;id|id||false|string||
|&emsp;&emsp;tableDataId|数据id||false|string||
|&emsp;&emsp;tableName|表名||false|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«object»|
|201|Created||
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|object||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": {},
	"success": true,
	"timestamp": 0
}
```


## 表单评论文件-通过id删除


**接口地址**:`/nnzk/sys/formFile/delete`


**请求方式**:`DELETE`


**请求数据类型**:`application/x-www-form-urlencoded`


**响应数据类型**:`*/*`


**接口描述**:<p>表单评论文件-通过id删除</p>



**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|id|id|query|true|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«object»|
|204|No Content||
|401|Unauthorized||
|403|Forbidden||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|object||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": {},
	"success": true,
	"timestamp": 0
}
```


## 表单评论文件-批量删除


**接口地址**:`/nnzk/sys/formFile/deleteBatch`


**请求方式**:`DELETE`


**请求数据类型**:`application/x-www-form-urlencoded`


**响应数据类型**:`*/*`


**接口描述**:<p>表单评论文件-批量删除</p>



**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|ids|ids|query|true|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«object»|
|204|No Content||
|401|Unauthorized||
|403|Forbidden||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|object||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": {},
	"success": true,
	"timestamp": 0
}
```


## 表单评论文件-编辑


**接口地址**:`/nnzk/sys/formFile/edit`


**请求方式**:`POST`


**请求数据类型**:`application/json`


**响应数据类型**:`*/*`


**接口描述**:<p>表单评论文件-编辑</p>



**请求示例**:


```javascript
{
  "createBy": "",
  "createTime": "",
  "fileId": "",
  "fileType": "",
  "id": "",
  "tableDataId": "",
  "tableName": ""
}
```


**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|sysFormFile|表单评论文件|body|true|sys_form_file对象|sys_form_file对象|
|&emsp;&emsp;createBy|创建人登录名称||false|string||
|&emsp;&emsp;createTime|创建日期||false|string(date-time)||
|&emsp;&emsp;fileId|关联文件id||false|string||
|&emsp;&emsp;fileType|文档类型（folder:文件夹 excel:excel doc:word pp:ppt image:图片  archive:其他文档 video:视频）||false|string||
|&emsp;&emsp;id|id||false|string||
|&emsp;&emsp;tableDataId|数据id||false|string||
|&emsp;&emsp;tableName|表名||false|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«object»|
|201|Created||
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|object||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": {},
	"success": true,
	"timestamp": 0
}
```


## 表单评论文件-编辑


**接口地址**:`/nnzk/sys/formFile/edit`


**请求方式**:`PUT`


**请求数据类型**:`application/json`


**响应数据类型**:`*/*`


**接口描述**:<p>表单评论文件-编辑</p>



**请求示例**:


```javascript
{
  "createBy": "",
  "createTime": "",
  "fileId": "",
  "fileType": "",
  "id": "",
  "tableDataId": "",
  "tableName": ""
}
```


**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|sysFormFile|表单评论文件|body|true|sys_form_file对象|sys_form_file对象|
|&emsp;&emsp;createBy|创建人登录名称||false|string||
|&emsp;&emsp;createTime|创建日期||false|string(date-time)||
|&emsp;&emsp;fileId|关联文件id||false|string||
|&emsp;&emsp;fileType|文档类型（folder:文件夹 excel:excel doc:word pp:ppt image:图片  archive:其他文档 video:视频）||false|string||
|&emsp;&emsp;id|id||false|string||
|&emsp;&emsp;tableDataId|数据id||false|string||
|&emsp;&emsp;tableName|表名||false|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«object»|
|201|Created||
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|object||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": {},
	"success": true,
	"timestamp": 0
}
```


## 表单评论文件-分页列表查询


**接口地址**:`/nnzk/sys/formFile/list`


**请求方式**:`GET`


**请求数据类型**:`application/x-www-form-urlencoded`


**响应数据类型**:`*/*`


**接口描述**:<p>表单评论文件-分页列表查询</p>



**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|createBy|创建人登录名称|query|false|string||
|createTime|创建日期|query|false|string(date-time)||
|fileId|关联文件id|query|false|string||
|fileType|文档类型（folder:文件夹 excel:excel doc:word pp:ppt image:图片  archive:其他文档 video:视频）|query|false|string||
|id|id|query|false|string||
|pageNo|pageNo|query|false|integer(int32)||
|pageSize|pageSize|query|false|integer(int32)||
|tableDataId|数据id|query|false|string||
|tableName|表名|query|false|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«object»|
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|object||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": {},
	"success": true,
	"timestamp": 0
}
```


## 表单评论文件-通过id查询


**接口地址**:`/nnzk/sys/formFile/queryById`


**请求方式**:`GET`


**请求数据类型**:`application/x-www-form-urlencoded`


**响应数据类型**:`*/*`


**接口描述**:<p>表单评论文件-通过id查询</p>



**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|id|id|query|true|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«object»|
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|object||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": {},
	"success": true,
	"timestamp": 0
}
```


# 角色首页配置


## 角色首页配置-添加


**接口地址**:`/nnzk/sys/sysRoleIndex/add`


**请求方式**:`POST`


**请求数据类型**:`application/json`


**响应数据类型**:`*/*`


**接口描述**:<p>角色首页配置-添加</p>



**请求示例**:


```javascript
{
  "component": "",
  "createBy": "",
  "createTime": "",
  "id": "",
  "priority": 0,
  "roleCode": "",
  "route": true,
  "status": "",
  "sysOrgCode": "",
  "updateBy": "",
  "updateTime": "",
  "url": ""
}
```


**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|sysRoleIndex|角色首页配置|body|true|sys_role_index对象|sys_role_index对象|
|&emsp;&emsp;component|组件||false|string||
|&emsp;&emsp;createBy|创建人登录名称||false|string||
|&emsp;&emsp;createTime|创建日期||false|string(date-time)||
|&emsp;&emsp;id|id||false|string||
|&emsp;&emsp;priority|优先级||false|integer(int32)||
|&emsp;&emsp;roleCode|角色编码||false|string||
|&emsp;&emsp;route|是否路由菜单||false|boolean||
|&emsp;&emsp;status|状态||false|string||
|&emsp;&emsp;sysOrgCode|所属部门||false|string||
|&emsp;&emsp;updateBy|更新人登录名称||false|string||
|&emsp;&emsp;updateTime|更新日期||false|string(date-time)||
|&emsp;&emsp;url|路由地址||false|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«object»|
|201|Created||
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|object||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": {},
	"success": true,
	"timestamp": 0
}
```


## 角色首页配置-通过id删除


**接口地址**:`/nnzk/sys/sysRoleIndex/delete`


**请求方式**:`DELETE`


**请求数据类型**:`application/x-www-form-urlencoded`


**响应数据类型**:`*/*`


**接口描述**:<p>角色首页配置-通过id删除</p>



**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|id|id|query|true|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«object»|
|204|No Content||
|401|Unauthorized||
|403|Forbidden||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|object||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": {},
	"success": true,
	"timestamp": 0
}
```


## 角色首页配置-批量删除


**接口地址**:`/nnzk/sys/sysRoleIndex/deleteBatch`


**请求方式**:`DELETE`


**请求数据类型**:`application/x-www-form-urlencoded`


**响应数据类型**:`*/*`


**接口描述**:<p>角色首页配置-批量删除</p>



**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|ids|ids|query|true|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«object»|
|204|No Content||
|401|Unauthorized||
|403|Forbidden||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|object||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": {},
	"success": true,
	"timestamp": 0
}
```


## 角色首页配置-编辑


**接口地址**:`/nnzk/sys/sysRoleIndex/edit`


**请求方式**:`POST`


**请求数据类型**:`application/json`


**响应数据类型**:`*/*`


**接口描述**:<p>角色首页配置-编辑</p>



**请求示例**:


```javascript
{
  "component": "",
  "createBy": "",
  "createTime": "",
  "id": "",
  "priority": 0,
  "roleCode": "",
  "route": true,
  "status": "",
  "sysOrgCode": "",
  "updateBy": "",
  "updateTime": "",
  "url": ""
}
```


**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|sysRoleIndex|角色首页配置|body|true|sys_role_index对象|sys_role_index对象|
|&emsp;&emsp;component|组件||false|string||
|&emsp;&emsp;createBy|创建人登录名称||false|string||
|&emsp;&emsp;createTime|创建日期||false|string(date-time)||
|&emsp;&emsp;id|id||false|string||
|&emsp;&emsp;priority|优先级||false|integer(int32)||
|&emsp;&emsp;roleCode|角色编码||false|string||
|&emsp;&emsp;route|是否路由菜单||false|boolean||
|&emsp;&emsp;status|状态||false|string||
|&emsp;&emsp;sysOrgCode|所属部门||false|string||
|&emsp;&emsp;updateBy|更新人登录名称||false|string||
|&emsp;&emsp;updateTime|更新日期||false|string(date-time)||
|&emsp;&emsp;url|路由地址||false|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«object»|
|201|Created||
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|object||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": {},
	"success": true,
	"timestamp": 0
}
```


## 角色首页配置-编辑


**接口地址**:`/nnzk/sys/sysRoleIndex/edit`


**请求方式**:`PUT`


**请求数据类型**:`application/json`


**响应数据类型**:`*/*`


**接口描述**:<p>角色首页配置-编辑</p>



**请求示例**:


```javascript
{
  "component": "",
  "createBy": "",
  "createTime": "",
  "id": "",
  "priority": 0,
  "roleCode": "",
  "route": true,
  "status": "",
  "sysOrgCode": "",
  "updateBy": "",
  "updateTime": "",
  "url": ""
}
```


**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|sysRoleIndex|角色首页配置|body|true|sys_role_index对象|sys_role_index对象|
|&emsp;&emsp;component|组件||false|string||
|&emsp;&emsp;createBy|创建人登录名称||false|string||
|&emsp;&emsp;createTime|创建日期||false|string(date-time)||
|&emsp;&emsp;id|id||false|string||
|&emsp;&emsp;priority|优先级||false|integer(int32)||
|&emsp;&emsp;roleCode|角色编码||false|string||
|&emsp;&emsp;route|是否路由菜单||false|boolean||
|&emsp;&emsp;status|状态||false|string||
|&emsp;&emsp;sysOrgCode|所属部门||false|string||
|&emsp;&emsp;updateBy|更新人登录名称||false|string||
|&emsp;&emsp;updateTime|更新日期||false|string(date-time)||
|&emsp;&emsp;url|路由地址||false|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«object»|
|201|Created||
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|object||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": {},
	"success": true,
	"timestamp": 0
}
```


## 角色首页配置-分页列表查询


**接口地址**:`/nnzk/sys/sysRoleIndex/list`


**请求方式**:`GET`


**请求数据类型**:`application/x-www-form-urlencoded`


**响应数据类型**:`*/*`


**接口描述**:<p>角色首页配置-分页列表查询</p>



**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|component|组件|query|false|string||
|createBy|创建人登录名称|query|false|string||
|createTime|创建日期|query|false|string(date-time)||
|id|id|query|false|string||
|pageNo|pageNo|query|false|integer(int32)||
|pageSize|pageSize|query|false|integer(int32)||
|priority|优先级|query|false|integer(int32)||
|roleCode|角色编码|query|false|string||
|route|是否路由菜单|query|false|boolean||
|status|状态|query|false|string||
|sysOrgCode|所属部门|query|false|string||
|updateBy|更新人登录名称|query|false|string||
|updateTime|更新日期|query|false|string(date-time)||
|url|路由地址|query|false|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«object»|
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|object||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": {},
	"success": true,
	"timestamp": 0
}
```


## 角色首页配置-通过code查询


**接口地址**:`/nnzk/sys/sysRoleIndex/queryByCode`


**请求方式**:`GET`


**请求数据类型**:`application/x-www-form-urlencoded`


**响应数据类型**:`*/*`


**接口描述**:<p>角色首页配置-通过code查询</p>



**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|roleCode|roleCode|query|true|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«object»|
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|object||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": {},
	"success": true,
	"timestamp": 0
}
```


## 角色首页配置-通过id查询


**接口地址**:`/nnzk/sys/sysRoleIndex/queryById`


**请求方式**:`GET`


**请求数据类型**:`application/x-www-form-urlencoded`


**响应数据类型**:`*/*`


**接口描述**:<p>角色首页配置-通过id查询</p>



**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|id|id|query|true|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«object»|
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|object||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": {},
	"success": true,
	"timestamp": 0
}
```


# 部门权限表


## 部门权限表-添加


**接口地址**:`/nnzk/sys/sysDepartPermission/add`


**请求方式**:`POST`


**请求数据类型**:`application/json`


**响应数据类型**:`*/*`


**接口描述**:<p>部门权限表-添加</p>



**请求示例**:


```javascript
{
  "dataRuleIds": "",
  "departId": "",
  "id": "",
  "permissionId": ""
}
```


**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|sysDepartPermission|部门权限表|body|true|sys_depart_permission对象|sys_depart_permission对象|
|&emsp;&emsp;dataRuleIds|数据规则id||false|string||
|&emsp;&emsp;departId|部门id||false|string||
|&emsp;&emsp;id|id||false|string||
|&emsp;&emsp;permissionId|权限id||false|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«object»|
|201|Created||
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|object||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": {},
	"success": true,
	"timestamp": 0
}
```


## 部门权限表-通过id删除


**接口地址**:`/nnzk/sys/sysDepartPermission/delete`


**请求方式**:`DELETE`


**请求数据类型**:`application/x-www-form-urlencoded`


**响应数据类型**:`*/*`


**接口描述**:<p>部门权限表-通过id删除</p>



**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|id|id|query|true|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«object»|
|204|No Content||
|401|Unauthorized||
|403|Forbidden||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|object||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": {},
	"success": true,
	"timestamp": 0
}
```


## 部门权限表-批量删除


**接口地址**:`/nnzk/sys/sysDepartPermission/deleteBatch`


**请求方式**:`DELETE`


**请求数据类型**:`application/x-www-form-urlencoded`


**响应数据类型**:`*/*`


**接口描述**:<p>部门权限表-批量删除</p>



**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|ids|ids|query|true|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«object»|
|204|No Content||
|401|Unauthorized||
|403|Forbidden||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|object||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": {},
	"success": true,
	"timestamp": 0
}
```


## 部门权限表-编辑


**接口地址**:`/nnzk/sys/sysDepartPermission/edit`


**请求方式**:`POST`


**请求数据类型**:`application/json`


**响应数据类型**:`*/*`


**接口描述**:<p>部门权限表-编辑</p>



**请求示例**:


```javascript
{
  "dataRuleIds": "",
  "departId": "",
  "id": "",
  "permissionId": ""
}
```


**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|sysDepartPermission|部门权限表|body|true|sys_depart_permission对象|sys_depart_permission对象|
|&emsp;&emsp;dataRuleIds|数据规则id||false|string||
|&emsp;&emsp;departId|部门id||false|string||
|&emsp;&emsp;id|id||false|string||
|&emsp;&emsp;permissionId|权限id||false|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«object»|
|201|Created||
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|object||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": {},
	"success": true,
	"timestamp": 0
}
```


## 部门权限表-编辑


**接口地址**:`/nnzk/sys/sysDepartPermission/edit`


**请求方式**:`PUT`


**请求数据类型**:`application/json`


**响应数据类型**:`*/*`


**接口描述**:<p>部门权限表-编辑</p>



**请求示例**:


```javascript
{
  "dataRuleIds": "",
  "departId": "",
  "id": "",
  "permissionId": ""
}
```


**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|sysDepartPermission|部门权限表|body|true|sys_depart_permission对象|sys_depart_permission对象|
|&emsp;&emsp;dataRuleIds|数据规则id||false|string||
|&emsp;&emsp;departId|部门id||false|string||
|&emsp;&emsp;id|id||false|string||
|&emsp;&emsp;permissionId|权限id||false|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«object»|
|201|Created||
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|object||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": {},
	"success": true,
	"timestamp": 0
}
```


## 部门权限表-分页列表查询


**接口地址**:`/nnzk/sys/sysDepartPermission/list`


**请求方式**:`GET`


**请求数据类型**:`application/x-www-form-urlencoded`


**响应数据类型**:`*/*`


**接口描述**:<p>部门权限表-分页列表查询</p>



**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|dataRuleIds|数据规则id|query|false|string||
|departId|部门id|query|false|string||
|id|id|query|false|string||
|pageNo|pageNo|query|false|integer(int32)||
|pageSize|pageSize|query|false|integer(int32)||
|permissionId|权限id|query|false|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«object»|
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|object||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": {},
	"success": true,
	"timestamp": 0
}
```


## 部门权限表-通过id查询


**接口地址**:`/nnzk/sys/sysDepartPermission/queryById`


**请求方式**:`GET`


**请求数据类型**:`application/x-www-form-urlencoded`


**响应数据类型**:`*/*`


**接口描述**:<p>部门权限表-通过id查询</p>



**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|id|id|query|true|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«object»|
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|object||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": {},
	"success": true,
	"timestamp": 0
}
```


# 部门角色


## 部门角色-添加


**接口地址**:`/nnzk/sys/sysDepartRole/add`


**请求方式**:`POST`


**请求数据类型**:`application/json`


**响应数据类型**:`*/*`


**接口描述**:<p>部门角色-添加</p>



**请求示例**:


```javascript
{
  "createBy": "",
  "createTime": "",
  "departId": "",
  "description": "",
  "id": "",
  "roleCode": "",
  "roleName": "",
  "updateBy": "",
  "updateTime": ""
}
```


**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|sysDepartRole|部门角色|body|true|sys_depart_role对象|sys_depart_role对象|
|&emsp;&emsp;createBy|创建人||false|string||
|&emsp;&emsp;createTime|创建时间||false|string(date-time)||
|&emsp;&emsp;departId|部门id||false|string||
|&emsp;&emsp;description|描述||false|string||
|&emsp;&emsp;id|id||false|string||
|&emsp;&emsp;roleCode|部门角色编码||false|string||
|&emsp;&emsp;roleName|部门角色名称||false|string||
|&emsp;&emsp;updateBy|更新人||false|string||
|&emsp;&emsp;updateTime|更新时间||false|string(date-time)||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«object»|
|201|Created||
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|object||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": {},
	"success": true,
	"timestamp": 0
}
```


## 部门角色-通过id删除


**接口地址**:`/nnzk/sys/sysDepartRole/delete`


**请求方式**:`DELETE`


**请求数据类型**:`application/x-www-form-urlencoded`


**响应数据类型**:`*/*`


**接口描述**:<p>部门角色-通过id删除</p>



**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|id|id|query|true|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«object»|
|204|No Content||
|401|Unauthorized||
|403|Forbidden||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|object||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": {},
	"success": true,
	"timestamp": 0
}
```


## 部门角色-批量删除


**接口地址**:`/nnzk/sys/sysDepartRole/deleteBatch`


**请求方式**:`DELETE`


**请求数据类型**:`application/x-www-form-urlencoded`


**响应数据类型**:`*/*`


**接口描述**:<p>部门角色-批量删除</p>



**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|ids|ids|query|true|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«object»|
|204|No Content||
|401|Unauthorized||
|403|Forbidden||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|object||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": {},
	"success": true,
	"timestamp": 0
}
```


## 部门角色-编辑


**接口地址**:`/nnzk/sys/sysDepartRole/edit`


**请求方式**:`POST`


**请求数据类型**:`application/json`


**响应数据类型**:`*/*`


**接口描述**:<p>部门角色-编辑</p>



**请求示例**:


```javascript
{
  "createBy": "",
  "createTime": "",
  "departId": "",
  "description": "",
  "id": "",
  "roleCode": "",
  "roleName": "",
  "updateBy": "",
  "updateTime": ""
}
```


**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|sysDepartRole|部门角色|body|true|sys_depart_role对象|sys_depart_role对象|
|&emsp;&emsp;createBy|创建人||false|string||
|&emsp;&emsp;createTime|创建时间||false|string(date-time)||
|&emsp;&emsp;departId|部门id||false|string||
|&emsp;&emsp;description|描述||false|string||
|&emsp;&emsp;id|id||false|string||
|&emsp;&emsp;roleCode|部门角色编码||false|string||
|&emsp;&emsp;roleName|部门角色名称||false|string||
|&emsp;&emsp;updateBy|更新人||false|string||
|&emsp;&emsp;updateTime|更新时间||false|string(date-time)||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«object»|
|201|Created||
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|object||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": {},
	"success": true,
	"timestamp": 0
}
```


## 部门角色-编辑


**接口地址**:`/nnzk/sys/sysDepartRole/edit`


**请求方式**:`PUT`


**请求数据类型**:`application/json`


**响应数据类型**:`*/*`


**接口描述**:<p>部门角色-编辑</p>



**请求示例**:


```javascript
{
  "createBy": "",
  "createTime": "",
  "departId": "",
  "description": "",
  "id": "",
  "roleCode": "",
  "roleName": "",
  "updateBy": "",
  "updateTime": ""
}
```


**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|sysDepartRole|部门角色|body|true|sys_depart_role对象|sys_depart_role对象|
|&emsp;&emsp;createBy|创建人||false|string||
|&emsp;&emsp;createTime|创建时间||false|string(date-time)||
|&emsp;&emsp;departId|部门id||false|string||
|&emsp;&emsp;description|描述||false|string||
|&emsp;&emsp;id|id||false|string||
|&emsp;&emsp;roleCode|部门角色编码||false|string||
|&emsp;&emsp;roleName|部门角色名称||false|string||
|&emsp;&emsp;updateBy|更新人||false|string||
|&emsp;&emsp;updateTime|更新时间||false|string(date-time)||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«object»|
|201|Created||
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|object||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": {},
	"success": true,
	"timestamp": 0
}
```


## 部门角色-分页列表查询


**接口地址**:`/nnzk/sys/sysDepartRole/list`


**请求方式**:`GET`


**请求数据类型**:`application/x-www-form-urlencoded`


**响应数据类型**:`*/*`


**接口描述**:<p>部门角色-分页列表查询</p>



**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|createBy|创建人|query|false|string||
|createTime|创建时间|query|false|string(date-time)||
|departId|部门id|query|false|string||
|deptId|deptId|query|false|string||
|description|描述|query|false|string||
|id|id|query|false|string||
|pageNo|pageNo|query|false|integer(int32)||
|pageSize|pageSize|query|false|integer(int32)||
|roleCode|部门角色编码|query|false|string||
|roleName|部门角色名称|query|false|string||
|updateBy|更新人|query|false|string||
|updateTime|更新时间|query|false|string(date-time)||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«object»|
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|object||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": {},
	"success": true,
	"timestamp": 0
}
```


## 部门角色-通过id查询


**接口地址**:`/nnzk/sys/sysDepartRole/queryById`


**请求方式**:`GET`


**请求数据类型**:`application/x-www-form-urlencoded`


**响应数据类型**:`*/*`


**接口描述**:<p>部门角色-通过id查询</p>



**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|id|id|query|true|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«object»|
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|object||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": {},
	"success": true,
	"timestamp": 0
}
```


# 重复校验


## 重复校验接口


**接口地址**:`/nnzk/sys/duplicate/check`


**请求方式**:`GET`


**请求数据类型**:`application/x-www-form-urlencoded`


**响应数据类型**:`*/*`


**接口描述**:


**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|dataId|数据ID|query|false|string||
|fieldName|字段名|query|false|string||
|fieldVal|字段值|query|false|string||
|tableName|表名|query|false|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«string»|
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|string||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": "",
	"success": true,
	"timestamp": 0
}
```


# 高中学校表


## 高中学校表-添加


**接口地址**:`/nnzk/school/highSchool/add`


**请求方式**:`POST`


**请求数据类型**:`application/json`


**响应数据类型**:`*/*`


**接口描述**:<p>高中学校表-添加</p>



**请求示例**:


```javascript
{
  "adjustNum": 0,
  "adjustRate": 0,
  "areaCode": "",
  "baseNum": 0,
  "cityOthersQuery": 0,
  "cityOthersReg": 0,
  "classNum": 0,
  "createBy": "",
  "createTime": "",
  "delFlag": 0,
  "dispOrder": 0,
  "flag": 0,
  "foreignQuery": 0,
  "foreignReg": 0,
  "id": "",
  "innerSumScoreLimit": "",
  "introduceName": "",
  "isGiveUpAdmission": 0,
  "isNeedAudit": 0,
  "isOpenReview": 0,
  "lowestLevel": "",
  "printName": "",
  "privateOrder": 0,
  "schoolCode": "",
  "schoolName": "",
  "schoolType": 0,
  "shortName": "",
  "specQuery": 0,
  "specReg": 0,
  "specSumScoreLimit": "",
  "supplementFrequency": 0,
  "supplementNumber": 0,
  "updateBy": "",
  "updateTime": ""
}
```


**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|highSchool|高中学校表|body|true|high_school对象|high_school对象|
|&emsp;&emsp;adjustNum|调剂人数||false|integer(int32)||
|&emsp;&emsp;adjustRate|调剂比例||false|number(double)||
|&emsp;&emsp;areaCode|区域代码||false|string||
|&emsp;&emsp;baseNum|每班人数||false|integer(int32)||
|&emsp;&emsp;cityOthersQuery|是否开放查询本市其他权限||false|integer(int32)||
|&emsp;&emsp;cityOthersReg|是否开放登记本市其他权限||false|integer(int32)||
|&emsp;&emsp;classNum|计划班数||false|integer(int32)||
|&emsp;&emsp;createBy|创建人||false|string||
|&emsp;&emsp;createTime|创建日期||false|string(date-time)||
|&emsp;&emsp;delFlag|删除标识||false|integer(int32)||
|&emsp;&emsp;dispOrder|填报时的显示顺序||false|integer(int32)||
|&emsp;&emsp;flag|||false|integer(int32)||
|&emsp;&emsp;foreignQuery|是否开放查询外地生权限||false|integer(int32)||
|&emsp;&emsp;foreignReg|是否开放登记外地生权限||false|integer(int32)||
|&emsp;&emsp;id|主键||false|string||
|&emsp;&emsp;innerSumScoreLimit|本市其他||false|string||
|&emsp;&emsp;introduceName|介绍名称||false|string||
|&emsp;&emsp;isGiveUpAdmission|开放放弃补录||false|integer(int32)||
|&emsp;&emsp;isNeedAudit|是否需要审核||false|integer(int32)||
|&emsp;&emsp;isOpenReview|是否开放补录权限||false|integer(int32)||
|&emsp;&emsp;lowestLevel|正录总分线||false|string||
|&emsp;&emsp;printName|打印名称||false|string||
|&emsp;&emsp;privateOrder|privateOrder||false|integer(int32)||
|&emsp;&emsp;schoolCode|学校代码||false|string||
|&emsp;&emsp;schoolName|学校名称||false|string||
|&emsp;&emsp;schoolType|学校类型||false|integer(int32)||
|&emsp;&emsp;shortName|简称||false|string||
|&emsp;&emsp;specQuery|是否开放查询特长生权限||false|integer(int32)||
|&emsp;&emsp;specReg|是否开放登记特长生权限||false|integer(int32)||
|&emsp;&emsp;specSumScoreLimit|特长生/特招||false|string||
|&emsp;&emsp;supplementFrequency|补录次数||false|integer(int32)||
|&emsp;&emsp;supplementNumber|增补计划数||false|integer(int32)||
|&emsp;&emsp;updateBy|更新人||false|string||
|&emsp;&emsp;updateTime|更新日期||false|string(date-time)||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«string»|
|201|Created||
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|string||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": "",
	"success": true,
	"timestamp": 0
}
```


## 高中学校表-高中学校列表(不分页)


**接口地址**:`/nnzk/school/highSchool/allHighSchool`


**请求方式**:`GET`


**请求数据类型**:`application/x-www-form-urlencoded`


**响应数据类型**:`*/*`


**接口描述**:<p>高中学校表-高中学校列表(不分页)</p>



**请求参数**:


暂无


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«List«HighSchoolDTO»»|
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|array|HighSchoolDTO|
|&emsp;&emsp;adjustNum|调剂人数|integer(int32)||
|&emsp;&emsp;adjustRate|调剂比例|number(double)||
|&emsp;&emsp;areaCode|区域代码|string||
|&emsp;&emsp;baseNum|每班人数|integer(int32)||
|&emsp;&emsp;classNum|计划班数|integer(int32)||
|&emsp;&emsp;dispOrder|填报时的显示顺序|integer(int32)||
|&emsp;&emsp;id|主键|string||
|&emsp;&emsp;innerSumScoreLimit|本市其他|string||
|&emsp;&emsp;introduceName|介绍名称|string||
|&emsp;&emsp;isGiveUpAdmission|开放放弃补录|integer(int32)||
|&emsp;&emsp;isNeedAudit|是否需要审核|integer(int32)||
|&emsp;&emsp;isOpenReview|是否开放补录权限|integer(int32)||
|&emsp;&emsp;lowestLevel|正录总分线|string||
|&emsp;&emsp;printName|打印名称|string||
|&emsp;&emsp;privateOrder|privateOrder|integer(int32)||
|&emsp;&emsp;schoolCode|学校代码|string||
|&emsp;&emsp;schoolName|学校名称|string||
|&emsp;&emsp;schoolType|学校类型|string||
|&emsp;&emsp;shortName|简称|string||
|&emsp;&emsp;specSumScoreLimit|特长生/特招|string||
|&emsp;&emsp;supplementFrequency|补录次数|integer(int32)||
|&emsp;&emsp;supplementNumber|增补计划数|integer(int32)||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": [
		{
			"adjustNum": 0,
			"adjustRate": 0,
			"areaCode": "",
			"baseNum": 0,
			"classNum": 0,
			"dispOrder": 0,
			"id": "",
			"innerSumScoreLimit": "",
			"introduceName": "",
			"isGiveUpAdmission": 0,
			"isNeedAudit": 0,
			"isOpenReview": 0,
			"lowestLevel": "",
			"printName": "",
			"privateOrder": 0,
			"schoolCode": "",
			"schoolName": "",
			"schoolType": "",
			"shortName": "",
			"specSumScoreLimit": "",
			"supplementFrequency": 0,
			"supplementNumber": 0
		}
	],
	"success": true,
	"timestamp": 0
}
```


## 高中学校表-通过id删除


**接口地址**:`/nnzk/school/highSchool/delete`


**请求方式**:`DELETE`


**请求数据类型**:`application/x-www-form-urlencoded`


**响应数据类型**:`*/*`


**接口描述**:<p>高中学校表-通过id删除</p>



**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|id|id|query|true|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«string»|
|204|No Content||
|401|Unauthorized||
|403|Forbidden||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|string||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": "",
	"success": true,
	"timestamp": 0
}
```


## 高中学校表-批量删除


**接口地址**:`/nnzk/school/highSchool/deleteBatch`


**请求方式**:`DELETE`


**请求数据类型**:`application/x-www-form-urlencoded`


**响应数据类型**:`*/*`


**接口描述**:<p>高中学校表-批量删除</p>



**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|ids|ids|query|true|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«string»|
|204|No Content||
|401|Unauthorized||
|403|Forbidden||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|string||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": "",
	"success": true,
	"timestamp": 0
}
```


## 高中学校表-编辑


**接口地址**:`/nnzk/school/highSchool/edit`


**请求方式**:`POST`


**请求数据类型**:`application/json`


**响应数据类型**:`*/*`


**接口描述**:<p>高中学校表-编辑</p>



**请求示例**:


```javascript
{
  "adjustNum": 0,
  "adjustRate": 0,
  "areaCode": "",
  "baseNum": 0,
  "cityOthersQuery": 0,
  "cityOthersReg": 0,
  "classNum": 0,
  "createBy": "",
  "createTime": "",
  "delFlag": 0,
  "dispOrder": 0,
  "flag": 0,
  "foreignQuery": 0,
  "foreignReg": 0,
  "id": "",
  "innerSumScoreLimit": "",
  "introduceName": "",
  "isGiveUpAdmission": 0,
  "isNeedAudit": 0,
  "isOpenReview": 0,
  "lowestLevel": "",
  "printName": "",
  "privateOrder": 0,
  "schoolCode": "",
  "schoolName": "",
  "schoolType": 0,
  "shortName": "",
  "specQuery": 0,
  "specReg": 0,
  "specSumScoreLimit": "",
  "supplementFrequency": 0,
  "supplementNumber": 0,
  "updateBy": "",
  "updateTime": ""
}
```


**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|highSchool|高中学校表|body|true|high_school对象|high_school对象|
|&emsp;&emsp;adjustNum|调剂人数||false|integer(int32)||
|&emsp;&emsp;adjustRate|调剂比例||false|number(double)||
|&emsp;&emsp;areaCode|区域代码||false|string||
|&emsp;&emsp;baseNum|每班人数||false|integer(int32)||
|&emsp;&emsp;cityOthersQuery|是否开放查询本市其他权限||false|integer(int32)||
|&emsp;&emsp;cityOthersReg|是否开放登记本市其他权限||false|integer(int32)||
|&emsp;&emsp;classNum|计划班数||false|integer(int32)||
|&emsp;&emsp;createBy|创建人||false|string||
|&emsp;&emsp;createTime|创建日期||false|string(date-time)||
|&emsp;&emsp;delFlag|删除标识||false|integer(int32)||
|&emsp;&emsp;dispOrder|填报时的显示顺序||false|integer(int32)||
|&emsp;&emsp;flag|||false|integer(int32)||
|&emsp;&emsp;foreignQuery|是否开放查询外地生权限||false|integer(int32)||
|&emsp;&emsp;foreignReg|是否开放登记外地生权限||false|integer(int32)||
|&emsp;&emsp;id|主键||false|string||
|&emsp;&emsp;innerSumScoreLimit|本市其他||false|string||
|&emsp;&emsp;introduceName|介绍名称||false|string||
|&emsp;&emsp;isGiveUpAdmission|开放放弃补录||false|integer(int32)||
|&emsp;&emsp;isNeedAudit|是否需要审核||false|integer(int32)||
|&emsp;&emsp;isOpenReview|是否开放补录权限||false|integer(int32)||
|&emsp;&emsp;lowestLevel|正录总分线||false|string||
|&emsp;&emsp;printName|打印名称||false|string||
|&emsp;&emsp;privateOrder|privateOrder||false|integer(int32)||
|&emsp;&emsp;schoolCode|学校代码||false|string||
|&emsp;&emsp;schoolName|学校名称||false|string||
|&emsp;&emsp;schoolType|学校类型||false|integer(int32)||
|&emsp;&emsp;shortName|简称||false|string||
|&emsp;&emsp;specQuery|是否开放查询特长生权限||false|integer(int32)||
|&emsp;&emsp;specReg|是否开放登记特长生权限||false|integer(int32)||
|&emsp;&emsp;specSumScoreLimit|特长生/特招||false|string||
|&emsp;&emsp;supplementFrequency|补录次数||false|integer(int32)||
|&emsp;&emsp;supplementNumber|增补计划数||false|integer(int32)||
|&emsp;&emsp;updateBy|更新人||false|string||
|&emsp;&emsp;updateTime|更新日期||false|string(date-time)||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«string»|
|201|Created||
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|string||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": "",
	"success": true,
	"timestamp": 0
}
```


## 高中学校表-编辑


**接口地址**:`/nnzk/school/highSchool/edit`


**请求方式**:`PUT`


**请求数据类型**:`application/json`


**响应数据类型**:`*/*`


**接口描述**:<p>高中学校表-编辑</p>



**请求示例**:


```javascript
{
  "adjustNum": 0,
  "adjustRate": 0,
  "areaCode": "",
  "baseNum": 0,
  "cityOthersQuery": 0,
  "cityOthersReg": 0,
  "classNum": 0,
  "createBy": "",
  "createTime": "",
  "delFlag": 0,
  "dispOrder": 0,
  "flag": 0,
  "foreignQuery": 0,
  "foreignReg": 0,
  "id": "",
  "innerSumScoreLimit": "",
  "introduceName": "",
  "isGiveUpAdmission": 0,
  "isNeedAudit": 0,
  "isOpenReview": 0,
  "lowestLevel": "",
  "printName": "",
  "privateOrder": 0,
  "schoolCode": "",
  "schoolName": "",
  "schoolType": 0,
  "shortName": "",
  "specQuery": 0,
  "specReg": 0,
  "specSumScoreLimit": "",
  "supplementFrequency": 0,
  "supplementNumber": 0,
  "updateBy": "",
  "updateTime": ""
}
```


**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|highSchool|高中学校表|body|true|high_school对象|high_school对象|
|&emsp;&emsp;adjustNum|调剂人数||false|integer(int32)||
|&emsp;&emsp;adjustRate|调剂比例||false|number(double)||
|&emsp;&emsp;areaCode|区域代码||false|string||
|&emsp;&emsp;baseNum|每班人数||false|integer(int32)||
|&emsp;&emsp;cityOthersQuery|是否开放查询本市其他权限||false|integer(int32)||
|&emsp;&emsp;cityOthersReg|是否开放登记本市其他权限||false|integer(int32)||
|&emsp;&emsp;classNum|计划班数||false|integer(int32)||
|&emsp;&emsp;createBy|创建人||false|string||
|&emsp;&emsp;createTime|创建日期||false|string(date-time)||
|&emsp;&emsp;delFlag|删除标识||false|integer(int32)||
|&emsp;&emsp;dispOrder|填报时的显示顺序||false|integer(int32)||
|&emsp;&emsp;flag|||false|integer(int32)||
|&emsp;&emsp;foreignQuery|是否开放查询外地生权限||false|integer(int32)||
|&emsp;&emsp;foreignReg|是否开放登记外地生权限||false|integer(int32)||
|&emsp;&emsp;id|主键||false|string||
|&emsp;&emsp;innerSumScoreLimit|本市其他||false|string||
|&emsp;&emsp;introduceName|介绍名称||false|string||
|&emsp;&emsp;isGiveUpAdmission|开放放弃补录||false|integer(int32)||
|&emsp;&emsp;isNeedAudit|是否需要审核||false|integer(int32)||
|&emsp;&emsp;isOpenReview|是否开放补录权限||false|integer(int32)||
|&emsp;&emsp;lowestLevel|正录总分线||false|string||
|&emsp;&emsp;printName|打印名称||false|string||
|&emsp;&emsp;privateOrder|privateOrder||false|integer(int32)||
|&emsp;&emsp;schoolCode|学校代码||false|string||
|&emsp;&emsp;schoolName|学校名称||false|string||
|&emsp;&emsp;schoolType|学校类型||false|integer(int32)||
|&emsp;&emsp;shortName|简称||false|string||
|&emsp;&emsp;specQuery|是否开放查询特长生权限||false|integer(int32)||
|&emsp;&emsp;specReg|是否开放登记特长生权限||false|integer(int32)||
|&emsp;&emsp;specSumScoreLimit|特长生/特招||false|string||
|&emsp;&emsp;supplementFrequency|补录次数||false|integer(int32)||
|&emsp;&emsp;supplementNumber|增补计划数||false|integer(int32)||
|&emsp;&emsp;updateBy|更新人||false|string||
|&emsp;&emsp;updateTime|更新日期||false|string(date-time)||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«string»|
|201|Created||
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|string||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": "",
	"success": true,
	"timestamp": 0
}
```


## 高中学校表-由学校代码获取高中学校信息


**接口地址**:`/nnzk/school/highSchool/getHighschoolBySchCode`


**请求方式**:`GET`


**请求数据类型**:`application/x-www-form-urlencoded`


**响应数据类型**:`*/*`


**接口描述**:<p>高中学校表-由学校代码获取高中学校信息</p>



**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|schoolCode|schoolCode|query|false|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«high_school对象»|
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|high_school对象|high_school对象|
|&emsp;&emsp;adjustNum|调剂人数|integer(int32)||
|&emsp;&emsp;adjustRate|调剂比例|number(double)||
|&emsp;&emsp;areaCode|区域代码|string||
|&emsp;&emsp;baseNum|每班人数|integer(int32)||
|&emsp;&emsp;cityOthersQuery|是否开放查询本市其他权限|integer(int32)||
|&emsp;&emsp;cityOthersReg|是否开放登记本市其他权限|integer(int32)||
|&emsp;&emsp;classNum|计划班数|integer(int32)||
|&emsp;&emsp;createBy|创建人|string||
|&emsp;&emsp;createTime|创建日期|string(date-time)||
|&emsp;&emsp;delFlag|删除标识|integer(int32)||
|&emsp;&emsp;dispOrder|填报时的显示顺序|integer(int32)||
|&emsp;&emsp;flag||integer(int32)||
|&emsp;&emsp;foreignQuery|是否开放查询外地生权限|integer(int32)||
|&emsp;&emsp;foreignReg|是否开放登记外地生权限|integer(int32)||
|&emsp;&emsp;id|主键|string||
|&emsp;&emsp;innerSumScoreLimit|本市其他|string||
|&emsp;&emsp;introduceName|介绍名称|string||
|&emsp;&emsp;isGiveUpAdmission|开放放弃补录|integer(int32)||
|&emsp;&emsp;isNeedAudit|是否需要审核|integer(int32)||
|&emsp;&emsp;isOpenReview|是否开放补录权限|integer(int32)||
|&emsp;&emsp;lowestLevel|正录总分线|string||
|&emsp;&emsp;printName|打印名称|string||
|&emsp;&emsp;privateOrder|privateOrder|integer(int32)||
|&emsp;&emsp;schoolCode|学校代码|string||
|&emsp;&emsp;schoolName|学校名称|string||
|&emsp;&emsp;schoolType|学校类型|integer(int32)||
|&emsp;&emsp;shortName|简称|string||
|&emsp;&emsp;specQuery|是否开放查询特长生权限|integer(int32)||
|&emsp;&emsp;specReg|是否开放登记特长生权限|integer(int32)||
|&emsp;&emsp;specSumScoreLimit|特长生/特招|string||
|&emsp;&emsp;supplementFrequency|补录次数|integer(int32)||
|&emsp;&emsp;supplementNumber|增补计划数|integer(int32)||
|&emsp;&emsp;updateBy|更新人|string||
|&emsp;&emsp;updateTime|更新日期|string(date-time)||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": {
		"adjustNum": 0,
		"adjustRate": 0,
		"areaCode": "",
		"baseNum": 0,
		"cityOthersQuery": 0,
		"cityOthersReg": 0,
		"classNum": 0,
		"createBy": "",
		"createTime": "",
		"delFlag": 0,
		"dispOrder": 0,
		"flag": 0,
		"foreignQuery": 0,
		"foreignReg": 0,
		"id": "",
		"innerSumScoreLimit": "",
		"introduceName": "",
		"isGiveUpAdmission": 0,
		"isNeedAudit": 0,
		"isOpenReview": 0,
		"lowestLevel": "",
		"printName": "",
		"privateOrder": 0,
		"schoolCode": "",
		"schoolName": "",
		"schoolType": 0,
		"shortName": "",
		"specQuery": 0,
		"specReg": 0,
		"specSumScoreLimit": "",
		"supplementFrequency": 0,
		"supplementNumber": 0,
		"updateBy": "",
		"updateTime": ""
	},
	"success": true,
	"timestamp": 0
}
```


## 高中学校表-分页列表查询


**接口地址**:`/nnzk/school/highSchool/list`


**请求方式**:`GET`


**请求数据类型**:`application/x-www-form-urlencoded`


**响应数据类型**:`*/*`


**接口描述**:<p>高中学校表-分页列表查询</p>



**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|areaCode|区域代码|query|true|string||
|dispOrder|填报时的显示顺序|query|true|integer(int32)||
|introduceName|介绍名称|query|true|string||
|printName|打印名称|query|true|string||
|schoolCode|学校代码|query|true|string||
|schoolName|学校名称|query|true|string||
|schoolType|学校类型|query|true|integer(int32)||
|shortName|简称|query|true|string||
|adjustNum|调剂人数|query|false|integer(int32)||
|adjustRate|调剂比例|query|false|number(double)||
|baseNum|每班人数|query|false|integer(int32)||
|cityOthersQuery|是否开放查询本市其他权限|query|false|integer(int32)||
|cityOthersReg|是否开放登记本市其他权限|query|false|integer(int32)||
|classNum|计划班数|query|false|integer(int32)||
|createBy|创建人|query|false|string||
|createTime|创建日期|query|false|string(date-time)||
|delFlag|删除标识|query|false|integer(int32)||
|flag||query|false|integer(int32)||
|foreignQuery|是否开放查询外地生权限|query|false|integer(int32)||
|foreignReg|是否开放登记外地生权限|query|false|integer(int32)||
|id|主键|query|false|string||
|innerSumScoreLimit|本市其他|query|false|string||
|isGiveUpAdmission|开放放弃补录|query|false|integer(int32)||
|isNeedAudit|是否需要审核|query|false|integer(int32)||
|isOpenReview|是否开放补录权限|query|false|integer(int32)||
|lowestLevel|正录总分线|query|false|string||
|pageNo|pageNo|query|false|integer(int32)||
|pageSize|pageSize|query|false|integer(int32)||
|privateOrder|privateOrder|query|false|integer(int32)||
|specQuery|是否开放查询特长生权限|query|false|integer(int32)||
|specReg|是否开放登记特长生权限|query|false|integer(int32)||
|specSumScoreLimit|特长生/特招|query|false|string||
|supplementFrequency|补录次数|query|false|integer(int32)||
|supplementNumber|增补计划数|query|false|integer(int32)||
|updateBy|更新人|query|false|string||
|updateTime|更新日期|query|false|string(date-time)||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«IPage«high_school对象»»|
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|IPage«high_school对象»|IPage«high_school对象»|
|&emsp;&emsp;current||integer(int64)||
|&emsp;&emsp;pages||integer(int64)||
|&emsp;&emsp;records||array|high_school对象|
|&emsp;&emsp;&emsp;&emsp;adjustNum|调剂人数|integer||
|&emsp;&emsp;&emsp;&emsp;adjustRate|调剂比例|number||
|&emsp;&emsp;&emsp;&emsp;areaCode|区域代码|string||
|&emsp;&emsp;&emsp;&emsp;baseNum|每班人数|integer||
|&emsp;&emsp;&emsp;&emsp;cityOthersQuery|是否开放查询本市其他权限|integer||
|&emsp;&emsp;&emsp;&emsp;cityOthersReg|是否开放登记本市其他权限|integer||
|&emsp;&emsp;&emsp;&emsp;classNum|计划班数|integer||
|&emsp;&emsp;&emsp;&emsp;createBy|创建人|string||
|&emsp;&emsp;&emsp;&emsp;createTime|创建日期|string||
|&emsp;&emsp;&emsp;&emsp;delFlag|删除标识|integer||
|&emsp;&emsp;&emsp;&emsp;dispOrder|填报时的显示顺序|integer||
|&emsp;&emsp;&emsp;&emsp;flag||integer||
|&emsp;&emsp;&emsp;&emsp;foreignQuery|是否开放查询外地生权限|integer||
|&emsp;&emsp;&emsp;&emsp;foreignReg|是否开放登记外地生权限|integer||
|&emsp;&emsp;&emsp;&emsp;id|主键|string||
|&emsp;&emsp;&emsp;&emsp;innerSumScoreLimit|本市其他|string||
|&emsp;&emsp;&emsp;&emsp;introduceName|介绍名称|string||
|&emsp;&emsp;&emsp;&emsp;isGiveUpAdmission|开放放弃补录|integer||
|&emsp;&emsp;&emsp;&emsp;isNeedAudit|是否需要审核|integer||
|&emsp;&emsp;&emsp;&emsp;isOpenReview|是否开放补录权限|integer||
|&emsp;&emsp;&emsp;&emsp;lowestLevel|正录总分线|string||
|&emsp;&emsp;&emsp;&emsp;printName|打印名称|string||
|&emsp;&emsp;&emsp;&emsp;privateOrder|privateOrder|integer||
|&emsp;&emsp;&emsp;&emsp;schoolCode|学校代码|string||
|&emsp;&emsp;&emsp;&emsp;schoolName|学校名称|string||
|&emsp;&emsp;&emsp;&emsp;schoolType|学校类型|integer||
|&emsp;&emsp;&emsp;&emsp;shortName|简称|string||
|&emsp;&emsp;&emsp;&emsp;specQuery|是否开放查询特长生权限|integer||
|&emsp;&emsp;&emsp;&emsp;specReg|是否开放登记特长生权限|integer||
|&emsp;&emsp;&emsp;&emsp;specSumScoreLimit|特长生/特招|string||
|&emsp;&emsp;&emsp;&emsp;supplementFrequency|补录次数|integer||
|&emsp;&emsp;&emsp;&emsp;supplementNumber|增补计划数|integer||
|&emsp;&emsp;&emsp;&emsp;updateBy|更新人|string||
|&emsp;&emsp;&emsp;&emsp;updateTime|更新日期|string||
|&emsp;&emsp;size||integer(int64)||
|&emsp;&emsp;total||integer(int64)||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": {
		"current": 0,
		"pages": 0,
		"records": [
			{
				"adjustNum": 0,
				"adjustRate": 0,
				"areaCode": "",
				"baseNum": 0,
				"cityOthersQuery": 0,
				"cityOthersReg": 0,
				"classNum": 0,
				"createBy": "",
				"createTime": "",
				"delFlag": 0,
				"dispOrder": 0,
				"flag": 0,
				"foreignQuery": 0,
				"foreignReg": 0,
				"id": "",
				"innerSumScoreLimit": "",
				"introduceName": "",
				"isGiveUpAdmission": 0,
				"isNeedAudit": 0,
				"isOpenReview": 0,
				"lowestLevel": "",
				"printName": "",
				"privateOrder": 0,
				"schoolCode": "",
				"schoolName": "",
				"schoolType": 0,
				"shortName": "",
				"specQuery": 0,
				"specReg": 0,
				"specSumScoreLimit": "",
				"supplementFrequency": 0,
				"supplementNumber": 0,
				"updateBy": "",
				"updateTime": ""
			}
		],
		"size": 0,
		"total": 0
	},
	"success": true,
	"timestamp": 0
}
```


## 高中学校表-通过id查询


**接口地址**:`/nnzk/school/highSchool/queryById`


**请求方式**:`GET`


**请求数据类型**:`application/x-www-form-urlencoded`


**响应数据类型**:`*/*`


**接口描述**:<p>高中学校表-通过id查询</p>



**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|id|id|query|true|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«high_school对象»|
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|high_school对象|high_school对象|
|&emsp;&emsp;adjustNum|调剂人数|integer(int32)||
|&emsp;&emsp;adjustRate|调剂比例|number(double)||
|&emsp;&emsp;areaCode|区域代码|string||
|&emsp;&emsp;baseNum|每班人数|integer(int32)||
|&emsp;&emsp;cityOthersQuery|是否开放查询本市其他权限|integer(int32)||
|&emsp;&emsp;cityOthersReg|是否开放登记本市其他权限|integer(int32)||
|&emsp;&emsp;classNum|计划班数|integer(int32)||
|&emsp;&emsp;createBy|创建人|string||
|&emsp;&emsp;createTime|创建日期|string(date-time)||
|&emsp;&emsp;delFlag|删除标识|integer(int32)||
|&emsp;&emsp;dispOrder|填报时的显示顺序|integer(int32)||
|&emsp;&emsp;flag||integer(int32)||
|&emsp;&emsp;foreignQuery|是否开放查询外地生权限|integer(int32)||
|&emsp;&emsp;foreignReg|是否开放登记外地生权限|integer(int32)||
|&emsp;&emsp;id|主键|string||
|&emsp;&emsp;innerSumScoreLimit|本市其他|string||
|&emsp;&emsp;introduceName|介绍名称|string||
|&emsp;&emsp;isGiveUpAdmission|开放放弃补录|integer(int32)||
|&emsp;&emsp;isNeedAudit|是否需要审核|integer(int32)||
|&emsp;&emsp;isOpenReview|是否开放补录权限|integer(int32)||
|&emsp;&emsp;lowestLevel|正录总分线|string||
|&emsp;&emsp;printName|打印名称|string||
|&emsp;&emsp;privateOrder|privateOrder|integer(int32)||
|&emsp;&emsp;schoolCode|学校代码|string||
|&emsp;&emsp;schoolName|学校名称|string||
|&emsp;&emsp;schoolType|学校类型|integer(int32)||
|&emsp;&emsp;shortName|简称|string||
|&emsp;&emsp;specQuery|是否开放查询特长生权限|integer(int32)||
|&emsp;&emsp;specReg|是否开放登记特长生权限|integer(int32)||
|&emsp;&emsp;specSumScoreLimit|特长生/特招|string||
|&emsp;&emsp;supplementFrequency|补录次数|integer(int32)||
|&emsp;&emsp;supplementNumber|增补计划数|integer(int32)||
|&emsp;&emsp;updateBy|更新人|string||
|&emsp;&emsp;updateTime|更新日期|string(date-time)||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": {
		"adjustNum": 0,
		"adjustRate": 0,
		"areaCode": "",
		"baseNum": 0,
		"cityOthersQuery": 0,
		"cityOthersReg": 0,
		"classNum": 0,
		"createBy": "",
		"createTime": "",
		"delFlag": 0,
		"dispOrder": 0,
		"flag": 0,
		"foreignQuery": 0,
		"foreignReg": 0,
		"id": "",
		"innerSumScoreLimit": "",
		"introduceName": "",
		"isGiveUpAdmission": 0,
		"isNeedAudit": 0,
		"isOpenReview": 0,
		"lowestLevel": "",
		"printName": "",
		"privateOrder": 0,
		"schoolCode": "",
		"schoolName": "",
		"schoolType": 0,
		"shortName": "",
		"specQuery": 0,
		"specReg": 0,
		"specSumScoreLimit": "",
		"supplementFrequency": 0,
		"supplementNumber": 0,
		"updateBy": "",
		"updateTime": ""
	},
	"success": true,
	"timestamp": 0
}
```


# 高中权限


## 高中权限-添加


**接口地址**:`/nnzk/school/highSchoolPermission/add`


**请求方式**:`POST`


**请求数据类型**:`application/json`


**响应数据类型**:`*/*`


**接口描述**:<p>高中权限-添加</p>



**请求示例**:


```javascript
{
  "bmTcs": 0,
  "cxBmqk": 0,
  "cxBsqtdj": 0,
  "cxGjbdj": 0,
  "cxHzbdj": 0,
  "cxLqmd": 0,
  "cxMinzhubdj": 0,
  "cxMinzubdj": 0,
  "cxTcsbm": 0,
  "cxTcsdj": 0,
  "cxWdsbdj": 0,
  "cxWdsdj": 0,
  "djBsqt": 0,
  "djTcs": 0,
  "djWds": 0,
  "dyRxdjb": 0,
  "id": "",
  "privateOrder": 0,
  "schoolCode": "",
  "tzdjGjb": 0,
  "tzdjHzb": 0,
  "tzdjMinzhub": 0,
  "tzdjMinzub": 0,
  "tzdjWdsb": 0
}
```


**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|highSchoolPermission|高中权限|body|true|high_school_permission对象|high_school_permission对象|
|&emsp;&emsp;bmTcs|特长生报名||false|integer(int32)||
|&emsp;&emsp;cxBmqk|查询报名情况||false|integer(int32)||
|&emsp;&emsp;cxBsqtdj|查询本市其他登记||false|integer(int32)||
|&emsp;&emsp;cxGjbdj|查询国际班登记||false|integer(int32)||
|&emsp;&emsp;cxHzbdj|查询宏志班登记||false|integer(int32)||
|&emsp;&emsp;cxLqmd|查询录取名单||false|integer(int32)||
|&emsp;&emsp;cxMinzhubdj|查询民助班登记||false|integer(int32)||
|&emsp;&emsp;cxMinzubdj|查询民族班登记||false|integer(int32)||
|&emsp;&emsp;cxTcsbm|查询特长生报名||false|integer(int32)||
|&emsp;&emsp;cxTcsdj|查询特长生登记||false|integer(int32)||
|&emsp;&emsp;cxWdsbdj|查询外地生班登记||false|integer(int32)||
|&emsp;&emsp;cxWdsdj|查询外地生登记||false|integer(int32)||
|&emsp;&emsp;djBsqt|本市其他登记||false|integer(int32)||
|&emsp;&emsp;djTcs|特长生登记||false|integer(int32)||
|&emsp;&emsp;djWds|外地生登记||false|integer(int32)||
|&emsp;&emsp;dyRxdjb|打印入学登记表||false|integer(int32)||
|&emsp;&emsp;id|主键||false|string||
|&emsp;&emsp;privateOrder|排序码||false|integer(int32)||
|&emsp;&emsp;schoolCode|学校代码||false|string||
|&emsp;&emsp;tzdjGjb|国际班登记||false|integer(int32)||
|&emsp;&emsp;tzdjHzb|宏志班登记||false|integer(int32)||
|&emsp;&emsp;tzdjMinzhub|民助班登记||false|integer(int32)||
|&emsp;&emsp;tzdjMinzub|民族班登记||false|integer(int32)||
|&emsp;&emsp;tzdjWdsb|外地生班登记||false|integer(int32)||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«string»|
|201|Created||
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|string||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": "",
	"success": true,
	"timestamp": 0
}
```


## 高中权限-通过id删除


**接口地址**:`/nnzk/school/highSchoolPermission/delete`


**请求方式**:`DELETE`


**请求数据类型**:`application/x-www-form-urlencoded`


**响应数据类型**:`*/*`


**接口描述**:<p>高中权限-通过id删除</p>



**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|id|id|query|true|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«string»|
|204|No Content||
|401|Unauthorized||
|403|Forbidden||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|string||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": "",
	"success": true,
	"timestamp": 0
}
```


## 高中权限-批量删除


**接口地址**:`/nnzk/school/highSchoolPermission/deleteBatch`


**请求方式**:`DELETE`


**请求数据类型**:`application/x-www-form-urlencoded`


**响应数据类型**:`*/*`


**接口描述**:<p>高中权限-批量删除</p>



**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|ids|ids|query|true|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«string»|
|204|No Content||
|401|Unauthorized||
|403|Forbidden||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|string||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": "",
	"success": true,
	"timestamp": 0
}
```


## 高中权限-编辑


**接口地址**:`/nnzk/school/highSchoolPermission/edit`


**请求方式**:`POST`


**请求数据类型**:`application/json`


**响应数据类型**:`*/*`


**接口描述**:<p>高中权限-编辑</p>



**请求示例**:


```javascript
{
  "bmTcs": 0,
  "cxBmqk": 0,
  "cxBsqtdj": 0,
  "cxGjbdj": 0,
  "cxHzbdj": 0,
  "cxLqmd": 0,
  "cxMinzhubdj": 0,
  "cxMinzubdj": 0,
  "cxTcsbm": 0,
  "cxTcsdj": 0,
  "cxWdsbdj": 0,
  "cxWdsdj": 0,
  "djBsqt": 0,
  "djTcs": 0,
  "djWds": 0,
  "dyRxdjb": 0,
  "id": "",
  "privateOrder": 0,
  "schoolCode": "",
  "tzdjGjb": 0,
  "tzdjHzb": 0,
  "tzdjMinzhub": 0,
  "tzdjMinzub": 0,
  "tzdjWdsb": 0
}
```


**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|highSchoolPermission|高中权限|body|true|high_school_permission对象|high_school_permission对象|
|&emsp;&emsp;bmTcs|特长生报名||false|integer(int32)||
|&emsp;&emsp;cxBmqk|查询报名情况||false|integer(int32)||
|&emsp;&emsp;cxBsqtdj|查询本市其他登记||false|integer(int32)||
|&emsp;&emsp;cxGjbdj|查询国际班登记||false|integer(int32)||
|&emsp;&emsp;cxHzbdj|查询宏志班登记||false|integer(int32)||
|&emsp;&emsp;cxLqmd|查询录取名单||false|integer(int32)||
|&emsp;&emsp;cxMinzhubdj|查询民助班登记||false|integer(int32)||
|&emsp;&emsp;cxMinzubdj|查询民族班登记||false|integer(int32)||
|&emsp;&emsp;cxTcsbm|查询特长生报名||false|integer(int32)||
|&emsp;&emsp;cxTcsdj|查询特长生登记||false|integer(int32)||
|&emsp;&emsp;cxWdsbdj|查询外地生班登记||false|integer(int32)||
|&emsp;&emsp;cxWdsdj|查询外地生登记||false|integer(int32)||
|&emsp;&emsp;djBsqt|本市其他登记||false|integer(int32)||
|&emsp;&emsp;djTcs|特长生登记||false|integer(int32)||
|&emsp;&emsp;djWds|外地生登记||false|integer(int32)||
|&emsp;&emsp;dyRxdjb|打印入学登记表||false|integer(int32)||
|&emsp;&emsp;id|主键||false|string||
|&emsp;&emsp;privateOrder|排序码||false|integer(int32)||
|&emsp;&emsp;schoolCode|学校代码||false|string||
|&emsp;&emsp;tzdjGjb|国际班登记||false|integer(int32)||
|&emsp;&emsp;tzdjHzb|宏志班登记||false|integer(int32)||
|&emsp;&emsp;tzdjMinzhub|民助班登记||false|integer(int32)||
|&emsp;&emsp;tzdjMinzub|民族班登记||false|integer(int32)||
|&emsp;&emsp;tzdjWdsb|外地生班登记||false|integer(int32)||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«string»|
|201|Created||
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|string||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": "",
	"success": true,
	"timestamp": 0
}
```


## 高中权限-编辑


**接口地址**:`/nnzk/school/highSchoolPermission/edit`


**请求方式**:`PUT`


**请求数据类型**:`application/json`


**响应数据类型**:`*/*`


**接口描述**:<p>高中权限-编辑</p>



**请求示例**:


```javascript
{
  "bmTcs": 0,
  "cxBmqk": 0,
  "cxBsqtdj": 0,
  "cxGjbdj": 0,
  "cxHzbdj": 0,
  "cxLqmd": 0,
  "cxMinzhubdj": 0,
  "cxMinzubdj": 0,
  "cxTcsbm": 0,
  "cxTcsdj": 0,
  "cxWdsbdj": 0,
  "cxWdsdj": 0,
  "djBsqt": 0,
  "djTcs": 0,
  "djWds": 0,
  "dyRxdjb": 0,
  "id": "",
  "privateOrder": 0,
  "schoolCode": "",
  "tzdjGjb": 0,
  "tzdjHzb": 0,
  "tzdjMinzhub": 0,
  "tzdjMinzub": 0,
  "tzdjWdsb": 0
}
```


**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|highSchoolPermission|高中权限|body|true|high_school_permission对象|high_school_permission对象|
|&emsp;&emsp;bmTcs|特长生报名||false|integer(int32)||
|&emsp;&emsp;cxBmqk|查询报名情况||false|integer(int32)||
|&emsp;&emsp;cxBsqtdj|查询本市其他登记||false|integer(int32)||
|&emsp;&emsp;cxGjbdj|查询国际班登记||false|integer(int32)||
|&emsp;&emsp;cxHzbdj|查询宏志班登记||false|integer(int32)||
|&emsp;&emsp;cxLqmd|查询录取名单||false|integer(int32)||
|&emsp;&emsp;cxMinzhubdj|查询民助班登记||false|integer(int32)||
|&emsp;&emsp;cxMinzubdj|查询民族班登记||false|integer(int32)||
|&emsp;&emsp;cxTcsbm|查询特长生报名||false|integer(int32)||
|&emsp;&emsp;cxTcsdj|查询特长生登记||false|integer(int32)||
|&emsp;&emsp;cxWdsbdj|查询外地生班登记||false|integer(int32)||
|&emsp;&emsp;cxWdsdj|查询外地生登记||false|integer(int32)||
|&emsp;&emsp;djBsqt|本市其他登记||false|integer(int32)||
|&emsp;&emsp;djTcs|特长生登记||false|integer(int32)||
|&emsp;&emsp;djWds|外地生登记||false|integer(int32)||
|&emsp;&emsp;dyRxdjb|打印入学登记表||false|integer(int32)||
|&emsp;&emsp;id|主键||false|string||
|&emsp;&emsp;privateOrder|排序码||false|integer(int32)||
|&emsp;&emsp;schoolCode|学校代码||false|string||
|&emsp;&emsp;tzdjGjb|国际班登记||false|integer(int32)||
|&emsp;&emsp;tzdjHzb|宏志班登记||false|integer(int32)||
|&emsp;&emsp;tzdjMinzhub|民助班登记||false|integer(int32)||
|&emsp;&emsp;tzdjMinzub|民族班登记||false|integer(int32)||
|&emsp;&emsp;tzdjWdsb|外地生班登记||false|integer(int32)||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«string»|
|201|Created||
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|string||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": "",
	"success": true,
	"timestamp": 0
}
```


## 高中权限-分页列表查询


**接口地址**:`/nnzk/school/highSchoolPermission/list`


**请求方式**:`GET`


**请求数据类型**:`application/x-www-form-urlencoded`


**响应数据类型**:`*/*`


**接口描述**:<p>高中权限-分页列表查询</p>



**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|bmTcs|特长生报名|query|false|integer(int32)||
|cxBmqk|查询报名情况|query|false|integer(int32)||
|cxBsqtdj|查询本市其他登记|query|false|integer(int32)||
|cxGjbdj|查询国际班登记|query|false|integer(int32)||
|cxHzbdj|查询宏志班登记|query|false|integer(int32)||
|cxLqmd|查询录取名单|query|false|integer(int32)||
|cxMinzhubdj|查询民助班登记|query|false|integer(int32)||
|cxMinzubdj|查询民族班登记|query|false|integer(int32)||
|cxTcsbm|查询特长生报名|query|false|integer(int32)||
|cxTcsdj|查询特长生登记|query|false|integer(int32)||
|cxWdsbdj|查询外地生班登记|query|false|integer(int32)||
|cxWdsdj|查询外地生登记|query|false|integer(int32)||
|djBsqt|本市其他登记|query|false|integer(int32)||
|djTcs|特长生登记|query|false|integer(int32)||
|djWds|外地生登记|query|false|integer(int32)||
|dyRxdjb|打印入学登记表|query|false|integer(int32)||
|id|主键|query|false|string||
|pageNo|pageNo|query|false|integer(int32)||
|pageSize|pageSize|query|false|integer(int32)||
|privateOrder|排序码|query|false|integer(int32)||
|schoolCode|学校代码|query|false|string||
|tzdjGjb|国际班登记|query|false|integer(int32)||
|tzdjHzb|宏志班登记|query|false|integer(int32)||
|tzdjMinzhub|民助班登记|query|false|integer(int32)||
|tzdjMinzub|民族班登记|query|false|integer(int32)||
|tzdjWdsb|外地生班登记|query|false|integer(int32)||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«IPage«high_school_permission对象»»|
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|IPage«high_school_permission对象»|IPage«high_school_permission对象»|
|&emsp;&emsp;current||integer(int64)||
|&emsp;&emsp;pages||integer(int64)||
|&emsp;&emsp;records||array|high_school_permission对象|
|&emsp;&emsp;&emsp;&emsp;bmTcs|特长生报名|integer||
|&emsp;&emsp;&emsp;&emsp;cxBmqk|查询报名情况|integer||
|&emsp;&emsp;&emsp;&emsp;cxBsqtdj|查询本市其他登记|integer||
|&emsp;&emsp;&emsp;&emsp;cxGjbdj|查询国际班登记|integer||
|&emsp;&emsp;&emsp;&emsp;cxHzbdj|查询宏志班登记|integer||
|&emsp;&emsp;&emsp;&emsp;cxLqmd|查询录取名单|integer||
|&emsp;&emsp;&emsp;&emsp;cxMinzhubdj|查询民助班登记|integer||
|&emsp;&emsp;&emsp;&emsp;cxMinzubdj|查询民族班登记|integer||
|&emsp;&emsp;&emsp;&emsp;cxTcsbm|查询特长生报名|integer||
|&emsp;&emsp;&emsp;&emsp;cxTcsdj|查询特长生登记|integer||
|&emsp;&emsp;&emsp;&emsp;cxWdsbdj|查询外地生班登记|integer||
|&emsp;&emsp;&emsp;&emsp;cxWdsdj|查询外地生登记|integer||
|&emsp;&emsp;&emsp;&emsp;djBsqt|本市其他登记|integer||
|&emsp;&emsp;&emsp;&emsp;djTcs|特长生登记|integer||
|&emsp;&emsp;&emsp;&emsp;djWds|外地生登记|integer||
|&emsp;&emsp;&emsp;&emsp;dyRxdjb|打印入学登记表|integer||
|&emsp;&emsp;&emsp;&emsp;id|主键|string||
|&emsp;&emsp;&emsp;&emsp;privateOrder|排序码|integer||
|&emsp;&emsp;&emsp;&emsp;schoolCode|学校代码|string||
|&emsp;&emsp;&emsp;&emsp;tzdjGjb|国际班登记|integer||
|&emsp;&emsp;&emsp;&emsp;tzdjHzb|宏志班登记|integer||
|&emsp;&emsp;&emsp;&emsp;tzdjMinzhub|民助班登记|integer||
|&emsp;&emsp;&emsp;&emsp;tzdjMinzub|民族班登记|integer||
|&emsp;&emsp;&emsp;&emsp;tzdjWdsb|外地生班登记|integer||
|&emsp;&emsp;size||integer(int64)||
|&emsp;&emsp;total||integer(int64)||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": {
		"current": 0,
		"pages": 0,
		"records": [
			{
				"bmTcs": 0,
				"cxBmqk": 0,
				"cxBsqtdj": 0,
				"cxGjbdj": 0,
				"cxHzbdj": 0,
				"cxLqmd": 0,
				"cxMinzhubdj": 0,
				"cxMinzubdj": 0,
				"cxTcsbm": 0,
				"cxTcsdj": 0,
				"cxWdsbdj": 0,
				"cxWdsdj": 0,
				"djBsqt": 0,
				"djTcs": 0,
				"djWds": 0,
				"dyRxdjb": 0,
				"id": "",
				"privateOrder": 0,
				"schoolCode": "",
				"tzdjGjb": 0,
				"tzdjHzb": 0,
				"tzdjMinzhub": 0,
				"tzdjMinzub": 0,
				"tzdjWdsb": 0
			}
		],
		"size": 0,
		"total": 0
	},
	"success": true,
	"timestamp": 0
}
```


## 招办端-高中权限列表


**接口地址**:`/nnzk/school/highSchoolPermission/permissionList`


**请求方式**:`GET`


**请求数据类型**:`application/x-www-form-urlencoded`


**响应数据类型**:`*/*`


**接口描述**:<p>招办端-高中权限列表</p>



**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|groupCode|分组编码|query|false|string||
|schoolType|学校类型|query|false|integer(int32)||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«List«high_school_permission对象»»|
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|array|high_school_permission对象|
|&emsp;&emsp;bmTcs|特长生报名|integer(int32)||
|&emsp;&emsp;cxBmqk|查询报名情况|integer(int32)||
|&emsp;&emsp;cxBsqtdj|查询本市其他登记|integer(int32)||
|&emsp;&emsp;cxGjbdj|查询国际班登记|integer(int32)||
|&emsp;&emsp;cxHzbdj|查询宏志班登记|integer(int32)||
|&emsp;&emsp;cxLqmd|查询录取名单|integer(int32)||
|&emsp;&emsp;cxMinzhubdj|查询民助班登记|integer(int32)||
|&emsp;&emsp;cxMinzubdj|查询民族班登记|integer(int32)||
|&emsp;&emsp;cxTcsbm|查询特长生报名|integer(int32)||
|&emsp;&emsp;cxTcsdj|查询特长生登记|integer(int32)||
|&emsp;&emsp;cxWdsbdj|查询外地生班登记|integer(int32)||
|&emsp;&emsp;cxWdsdj|查询外地生登记|integer(int32)||
|&emsp;&emsp;djBsqt|本市其他登记|integer(int32)||
|&emsp;&emsp;djTcs|特长生登记|integer(int32)||
|&emsp;&emsp;djWds|外地生登记|integer(int32)||
|&emsp;&emsp;dyRxdjb|打印入学登记表|integer(int32)||
|&emsp;&emsp;id|主键|string||
|&emsp;&emsp;privateOrder|排序码|integer(int32)||
|&emsp;&emsp;schoolCode|学校代码|string||
|&emsp;&emsp;tzdjGjb|国际班登记|integer(int32)||
|&emsp;&emsp;tzdjHzb|宏志班登记|integer(int32)||
|&emsp;&emsp;tzdjMinzhub|民助班登记|integer(int32)||
|&emsp;&emsp;tzdjMinzub|民族班登记|integer(int32)||
|&emsp;&emsp;tzdjWdsb|外地生班登记|integer(int32)||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": [
		{
			"bmTcs": 0,
			"cxBmqk": 0,
			"cxBsqtdj": 0,
			"cxGjbdj": 0,
			"cxHzbdj": 0,
			"cxLqmd": 0,
			"cxMinzhubdj": 0,
			"cxMinzubdj": 0,
			"cxTcsbm": 0,
			"cxTcsdj": 0,
			"cxWdsbdj": 0,
			"cxWdsdj": 0,
			"djBsqt": 0,
			"djTcs": 0,
			"djWds": 0,
			"dyRxdjb": 0,
			"id": "",
			"privateOrder": 0,
			"schoolCode": "",
			"tzdjGjb": 0,
			"tzdjHzb": 0,
			"tzdjMinzhub": 0,
			"tzdjMinzub": 0,
			"tzdjWdsb": 0
		}
	],
	"success": true,
	"timestamp": 0
}
```


## 高中权限-打印


**接口地址**:`/nnzk/school/highSchoolPermission/print`


**请求方式**:`GET`


**请求数据类型**:`application/x-www-form-urlencoded`


**响应数据类型**:`*/*`


**接口描述**:<p>高中权限-打印</p>



**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|groupCode|分组编码|query|false|string||
|schoolType|学校类型|query|false|integer(int32)||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|HSchoolPermPrintOutputDTO|
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|count|总条数|integer(int32)|integer(int32)|
|data|数据列表|array|high_school_permission对象|
|&emsp;&emsp;bmTcs|特长生报名|integer(int32)||
|&emsp;&emsp;cxBmqk|查询报名情况|integer(int32)||
|&emsp;&emsp;cxBsqtdj|查询本市其他登记|integer(int32)||
|&emsp;&emsp;cxGjbdj|查询国际班登记|integer(int32)||
|&emsp;&emsp;cxHzbdj|查询宏志班登记|integer(int32)||
|&emsp;&emsp;cxLqmd|查询录取名单|integer(int32)||
|&emsp;&emsp;cxMinzhubdj|查询民助班登记|integer(int32)||
|&emsp;&emsp;cxMinzubdj|查询民族班登记|integer(int32)||
|&emsp;&emsp;cxTcsbm|查询特长生报名|integer(int32)||
|&emsp;&emsp;cxTcsdj|查询特长生登记|integer(int32)||
|&emsp;&emsp;cxWdsbdj|查询外地生班登记|integer(int32)||
|&emsp;&emsp;cxWdsdj|查询外地生登记|integer(int32)||
|&emsp;&emsp;djBsqt|本市其他登记|integer(int32)||
|&emsp;&emsp;djTcs|特长生登记|integer(int32)||
|&emsp;&emsp;djWds|外地生登记|integer(int32)||
|&emsp;&emsp;dyRxdjb|打印入学登记表|integer(int32)||
|&emsp;&emsp;id|主键|string||
|&emsp;&emsp;privateOrder|排序码|integer(int32)||
|&emsp;&emsp;schoolCode|学校代码|string||
|&emsp;&emsp;tzdjGjb|国际班登记|integer(int32)||
|&emsp;&emsp;tzdjHzb|宏志班登记|integer(int32)||
|&emsp;&emsp;tzdjMinzhub|民助班登记|integer(int32)||
|&emsp;&emsp;tzdjMinzub|民族班登记|integer(int32)||
|&emsp;&emsp;tzdjWdsb|外地生班登记|integer(int32)||
|total|总页数|integer(int32)|integer(int32)|


**响应示例**:
```javascript
{
	"count": 0,
	"data": [
		{
			"bmTcs": 0,
			"cxBmqk": 0,
			"cxBsqtdj": 0,
			"cxGjbdj": 0,
			"cxHzbdj": 0,
			"cxLqmd": 0,
			"cxMinzhubdj": 0,
			"cxMinzubdj": 0,
			"cxTcsbm": 0,
			"cxTcsdj": 0,
			"cxWdsbdj": 0,
			"cxWdsdj": 0,
			"djBsqt": 0,
			"djTcs": 0,
			"djWds": 0,
			"dyRxdjb": 0,
			"id": "",
			"privateOrder": 0,
			"schoolCode": "",
			"tzdjGjb": 0,
			"tzdjHzb": 0,
			"tzdjMinzhub": 0,
			"tzdjMinzub": 0,
			"tzdjWdsb": 0
		}
	],
	"total": 0
}
```


## 高中权限-通过id查询


**接口地址**:`/nnzk/school/highSchoolPermission/queryById`


**请求方式**:`GET`


**请求数据类型**:`application/x-www-form-urlencoded`


**响应数据类型**:`*/*`


**接口描述**:<p>高中权限-通过id查询</p>



**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|id|id|query|true|string||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«high_school_permission对象»|
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|high_school_permission对象|high_school_permission对象|
|&emsp;&emsp;bmTcs|特长生报名|integer(int32)||
|&emsp;&emsp;cxBmqk|查询报名情况|integer(int32)||
|&emsp;&emsp;cxBsqtdj|查询本市其他登记|integer(int32)||
|&emsp;&emsp;cxGjbdj|查询国际班登记|integer(int32)||
|&emsp;&emsp;cxHzbdj|查询宏志班登记|integer(int32)||
|&emsp;&emsp;cxLqmd|查询录取名单|integer(int32)||
|&emsp;&emsp;cxMinzhubdj|查询民助班登记|integer(int32)||
|&emsp;&emsp;cxMinzubdj|查询民族班登记|integer(int32)||
|&emsp;&emsp;cxTcsbm|查询特长生报名|integer(int32)||
|&emsp;&emsp;cxTcsdj|查询特长生登记|integer(int32)||
|&emsp;&emsp;cxWdsbdj|查询外地生班登记|integer(int32)||
|&emsp;&emsp;cxWdsdj|查询外地生登记|integer(int32)||
|&emsp;&emsp;djBsqt|本市其他登记|integer(int32)||
|&emsp;&emsp;djTcs|特长生登记|integer(int32)||
|&emsp;&emsp;djWds|外地生登记|integer(int32)||
|&emsp;&emsp;dyRxdjb|打印入学登记表|integer(int32)||
|&emsp;&emsp;id|主键|string||
|&emsp;&emsp;privateOrder|排序码|integer(int32)||
|&emsp;&emsp;schoolCode|学校代码|string||
|&emsp;&emsp;tzdjGjb|国际班登记|integer(int32)||
|&emsp;&emsp;tzdjHzb|宏志班登记|integer(int32)||
|&emsp;&emsp;tzdjMinzhub|民助班登记|integer(int32)||
|&emsp;&emsp;tzdjMinzub|民族班登记|integer(int32)||
|&emsp;&emsp;tzdjWdsb|外地生班登记|integer(int32)||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": {
		"bmTcs": 0,
		"cxBmqk": 0,
		"cxBsqtdj": 0,
		"cxGjbdj": 0,
		"cxHzbdj": 0,
		"cxLqmd": 0,
		"cxMinzhubdj": 0,
		"cxMinzubdj": 0,
		"cxTcsbm": 0,
		"cxTcsdj": 0,
		"cxWdsbdj": 0,
		"cxWdsdj": 0,
		"djBsqt": 0,
		"djTcs": 0,
		"djWds": 0,
		"dyRxdjb": 0,
		"id": "",
		"privateOrder": 0,
		"schoolCode": "",
		"tzdjGjb": 0,
		"tzdjHzb": 0,
		"tzdjMinzhub": 0,
		"tzdjMinzub": 0,
		"tzdjWdsb": 0
	},
	"success": true,
	"timestamp": 0
}
```


## 招办端-更新高中权限


**接口地址**:`/nnzk/school/highSchoolPermission/updatePermissionBatch`


**请求方式**:`POST`


**请求数据类型**:`application/json`


**响应数据类型**:`*/*`


**接口描述**:<p>招办端-更新高中权限</p>



**请求示例**:


```javascript
{
  "highSchoolPermissions": [
    {
      "bmTcs": 0,
      "cxBmqk": 0,
      "cxBsqtdj": 0,
      "cxGjbdj": 0,
      "cxHzbdj": 0,
      "cxLqmd": 0,
      "cxMinzhubdj": 0,
      "cxMinzubdj": 0,
      "cxTcsbm": 0,
      "cxTcsdj": 0,
      "cxWdsbdj": 0,
      "cxWdsdj": 0,
      "djBsqt": 0,
      "djTcs": 0,
      "djWds": 0,
      "dyRxdjb": 0,
      "id": "",
      "privateOrder": 0,
      "schoolCode": "",
      "tzdjGjb": 0,
      "tzdjHzb": 0,
      "tzdjMinzhub": 0,
      "tzdjMinzub": 0,
      "tzdjWdsb": 0
    }
  ]
}
```


**请求参数**:


| 参数名称 | 参数说明 | 请求类型    | 是否必须 | 数据类型 | schema |
| -------- | -------- | ----- | -------- | -------- | ------ |
|input|input|body|true|UpdateHighSchoolPermissionVO|UpdateHighSchoolPermissionVO|
|&emsp;&emsp;highSchoolPermissions|||false|array|high_school_permission对象|
|&emsp;&emsp;&emsp;&emsp;bmTcs|特长生报名||false|integer||
|&emsp;&emsp;&emsp;&emsp;cxBmqk|查询报名情况||false|integer||
|&emsp;&emsp;&emsp;&emsp;cxBsqtdj|查询本市其他登记||false|integer||
|&emsp;&emsp;&emsp;&emsp;cxGjbdj|查询国际班登记||false|integer||
|&emsp;&emsp;&emsp;&emsp;cxHzbdj|查询宏志班登记||false|integer||
|&emsp;&emsp;&emsp;&emsp;cxLqmd|查询录取名单||false|integer||
|&emsp;&emsp;&emsp;&emsp;cxMinzhubdj|查询民助班登记||false|integer||
|&emsp;&emsp;&emsp;&emsp;cxMinzubdj|查询民族班登记||false|integer||
|&emsp;&emsp;&emsp;&emsp;cxTcsbm|查询特长生报名||false|integer||
|&emsp;&emsp;&emsp;&emsp;cxTcsdj|查询特长生登记||false|integer||
|&emsp;&emsp;&emsp;&emsp;cxWdsbdj|查询外地生班登记||false|integer||
|&emsp;&emsp;&emsp;&emsp;cxWdsdj|查询外地生登记||false|integer||
|&emsp;&emsp;&emsp;&emsp;djBsqt|本市其他登记||false|integer||
|&emsp;&emsp;&emsp;&emsp;djTcs|特长生登记||false|integer||
|&emsp;&emsp;&emsp;&emsp;djWds|外地生登记||false|integer||
|&emsp;&emsp;&emsp;&emsp;dyRxdjb|打印入学登记表||false|integer||
|&emsp;&emsp;&emsp;&emsp;id|主键||false|string||
|&emsp;&emsp;&emsp;&emsp;privateOrder|排序码||false|integer||
|&emsp;&emsp;&emsp;&emsp;schoolCode|学校代码||false|string||
|&emsp;&emsp;&emsp;&emsp;tzdjGjb|国际班登记||false|integer||
|&emsp;&emsp;&emsp;&emsp;tzdjHzb|宏志班登记||false|integer||
|&emsp;&emsp;&emsp;&emsp;tzdjMinzhub|民助班登记||false|integer||
|&emsp;&emsp;&emsp;&emsp;tzdjMinzub|民族班登记||false|integer||
|&emsp;&emsp;&emsp;&emsp;tzdjWdsb|外地生班登记||false|integer||


**响应状态**:


| 状态码 | 说明 | schema |
| -------- | -------- | ----- | 
|200|OK|接口返回对象«string»|
|201|Created||
|401|Unauthorized||
|403|Forbidden||
|404|Not Found||


**响应参数**:


| 参数名称 | 参数说明 | 类型 | schema |
| -------- | -------- | ----- |----- | 
|code|返回代码|integer(int32)|integer(int32)|
|message|返回处理消息|string||
|result|返回数据对象|string||
|success|成功标志|boolean||
|timestamp|时间戳|integer(int64)|integer(int64)|


**响应示例**:
```javascript
{
	"code": 0,
	"message": "",
	"result": "",
	"success": true,
	"timestamp": 0
}
```