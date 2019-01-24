# fastdfs-cloud

biod lab, distributed file storage



## 用户注册

请求地址：http://file.biodwhu.cn/fastdfs/user/register

请求类型：POST

请求参数：

- `app_id`：biodwhu-ecg
- `app_secret`：xxfdsafdsafsqweqwesdfasdfasdxcmasfasd



## 文件上传

请求地址：http://file.biodwhu.cn/fastdfs/upload

请求类型：POST

请求参数：

- `formdata`，name = "file"，form表单形式上传（最大限制2000kb）
- [可选] `base64`：文件字符串 图片转换
  - [图片转 Base64](http://imgbase64.duoshitong.com/)
- `appsecret`：注册至本平台的 key

返回参数：

```json
{
	"file_id":"XXAFSDFSDFQWWDSF",
	"file_url":"http://xxxx/group1/xxdasfasdfasdf"
}
```



## 用户文件

请求地址：http://file.biodwhu.cn/fastdfs/own/list

请求类型：GET

请求参数：

- `app_id`：biodwhu-ecg
- `app_secret`：xxfdsafdsafsqweqwesdfasdfasdxcmasfasd

返回参数：

```json
{
	"code":200,
	"msg":"查询成功",
    "data":[
        {
            "file_id":"xfasdfasdfsadfasdf",
            "file_url":"http://xxxx/group1/xxdasfasdfasdf",
            "file_time":"2019-01-24 09:59:59",
        },
        {
            "file_id":"xfasdfasdfsadfasdf",
            "file_url":"http://xxxx/group1/xxdasfasdfasdf",
            "file_time":"2019-01-24 09:59:59",
        },
        {
            "file_id":"xfasdfasdfsadfasdf",
            "file_url":"http://xxxx/group1/xxdasfasdfasdf",
            "file_time":"2019-01-24 09:59:59",
        }
    ]
}
```

