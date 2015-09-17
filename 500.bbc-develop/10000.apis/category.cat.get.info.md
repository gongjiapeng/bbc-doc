# 获取指定类目信息(category.cat.get.info)

## 品牌类目相关API

### 

* 系统参数

| *字段* | *标题* | *数据类型* | *验证条件* | *示例值* | *默认值* | *详细说明* |
| ------------- | ------------- | ------------- | ------------- | ------------- | ------------- | ------------- |
| method | API的方法名 | string | required | trade.get | null | 标识请求的是哪个API |
| timestamp | 请求时间 | unix时间戳 | required , numeric , > time()-300 | 1440596821 | null | 标识API请求的发起时间，如果超时300秒则拒绝请求 |
| format | 返回数据格式 | string | required | json | json | 返回数据是json格式的，目前只支持json |
| v | 版本号 | string | required | v1 | null | 标识该接口的版本 |
| sign_type | 签名方式 | string | required | MD5 | null | 标识签名算法 |
| sign | 签名 | string | required | AAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAA | null | 数据签名，32位长度16进制数字 |


* 业务参数

| *字段* | *标题* | *数据类型* | *验证条件* | *示例值* | *默认值* | *详细说明* |
| ------------- | ------------- | ------------- | ------------- | ------------- | ------------- | ------------- |
| parent_id |  | int |  | 33 |  | 父类id |
| cat_id |  | string |  | 33 |  | 类目id,和cat_name二选一 |
| cat_path |  | string |  | 33 |  | 类目id |
| cat_name |  | string |  | 大家电 |  | 类目名称和cat_id二选一 |
| level |  | int |  | 1 |  | 类目等级1、2、3,当cat_name不为空时，此参数必填 |
| fields |  | field_list |  | cat_name,cat_id | cat_name,level,cat_id | 获取类目的指定字段 |


*返回内容示例

```



```
