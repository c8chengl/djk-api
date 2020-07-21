# APP 接口文档



## 众惠金明细

```
/api/userFamily/currencyLog
```

```json
{
	"current": 1,
	"size": 20
}
```

```json

{
	"t": {
		"offset": 0,
		"limit": 2147483647,
		"total": 1,
		"size": 20,
		"pages": 1,
		"current": 1,
		"searchCount": true,
		"openSort": true,
		"optimizeCount": false,
		"records": [{
			"id": "1283698079204605952",
			"userId": "21",
			"digitalAsset": 0.0000,
			"stCurrency": 3.0000,
			"digitalAssetNew": 0.0000,
			"stCurrencyNew": 20003.0000,
			"remark": "系统赠送(永久)20000个众惠金",
			"createTime": "2020-07-16 09:40:47",
			"remarks": "test"
		}],
		"asc": true,
		"offsetCurrent": 0
	},
	"status": true,
	"msgCode": 200
}
```





## 众惠金互转

```
/api/userFamily/rotationSt
```

```json
{
	"familyId": "25", // 对方ID
	"stCurrency": "300", // 众惠金数量
	"pwd": "123456" // 支付密码
}
```



## 商家申请

- 添加 其他证件 字段 可上传多张图片
  - otherImgs
  - 逗号分隔字符串



## 附近商家

```
/api/NearbyC/getListByType
```

- 返回新增距离商家字段
  - distance
- 请求参数新增城市区域Code
  - areaCode





## 养老级别

```
/api/memberController/getMemberGrade
```

```json
{
	"t": {
		"gradeType": [{ // 所有级别
			"id": "1",
			"code": "vip_level_01",
			"name": "养老级别1星",
			"price": 11000,
			"privilege": "<span><span><span><div label-module=\"para\"><br></div></span></span></span>"
		}, {
			"id": "2",
			"code": "vip_level_02",
			"name": "养老级别2星",
			"price": 22000,
			"privilege": "<p><br></p>"
		}, {
			"id": "3",
			"code": "vip_level_03",
			"name": "养老级别3星",
			"price": 33000,
			"privilege": "<p><br></p>"
		}, {
			"id": "4",
			"code": "vip_level_04",
			"name": "养老级别4星",
			"price": 50000
		}, {
			"id": "5",
			"code": "vip_level_05",
			"name": "养老级别5星",
			"price": 100000
		}],
		"cusGrade": { // 我的级别
			"id": "1",
			"code": "vip_level_01",
			"name": "养老级别1星",
			"price": 11000,
			"privilege": "<span><span><span><div label-module=\"para\"><br></div></span></span></span>"
		}
	},
	"status": true,
	"msgCode": 200
}
```



## 文档

```
// 亲情号使用攻略
/api/userFamily/one/1

// 众惠金页面兑换规则
/api/userFamily/one/2

// 华兴众惠商家入驻服务协议
/api/userFamily/one/3

// 提现页面温馨提示
/api/userFamily/one/4

// 收益 右上角 帮助
/api/userFamily/one/5

// 华兴众惠用户注册服务协议
/api/userFamily/one/7

// 众惠金全面升级为亲情号 - 钱包页面头部
/api/userFamily/one/8

```

## 资金明细

```
/api/userController/getSystemCreditAssetsList
```
新增筛选参数
```
operateType
//    0收益,1支出,不传_全部
```



