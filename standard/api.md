# API

## JSON

数据交换格式: JSON(JavaScript Object Notation)

> JSON建构于两种结构: [object](#object) | [array](#array)

### value

- `object` = `{"key":value,...}`
- `array` = `[value,...]`
- `string` = `"jojo"`
- `number` = `0`
- `true`
- `false`
- `null`

### object

```json
{
    "name" : "jojo",
    "age" : 1,
    "married" : true,
    "key" : false,
    "score" : null,
    "dog" : {},
    "key" : [],
}
```

### array

> 数组中使用相同的数据类型

```json
["a", "b", "c", "d", "e"]
```

```json
[1, 2, 3, 4, 5]
```

## API

### Request

Method:

- GET
- POST
- HEAD
- PUT
- DELETE

### Response

#### Status Code

- 信息 100-199
- 成功 200
- 重定向 300
- 客户端错误 400
- 服务端错误 500

响应格式

- `code: int`
  - 0: 成功
  - 其他: 失败
- `data: object | array`
- `message: string`
  - 提示信息, 如失败原因
- `extra: object`
  - 扩展内容, 如翻页信息

```json
{
    "code": 0,
    "data": null,
    "message": "",
    "extra": null
}
```
