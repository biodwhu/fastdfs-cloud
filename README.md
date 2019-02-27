# fastdfs-cloud

biod lab, distributed file storage



## 用户注册

请求地址：http://file.biodwhu.cn/register

请求类型：GET

返回参数：

- `appid`：唯一数字
- `appsecret`：xxfdsafdsafsqweqwesdfasdfasdxcmasfasd（查询秘钥，文件上传下载均需要秘钥）



## 文件上传表单页

请求地址：http://file.biodwhu.cn/fastdfs/upload

请求类型：GET





## 文件上传

请求地址：http://file.biodwhu.cn/fastdfs/upload

请求类型：POST

请求参数：

- `file`，name = "file"，form表单形式上传（最大限制2000kb）
- `appsecret`：注册至本平台的 key

返回参数：

```json
{
"fileid":5,
"filename":"ab_01_1_qrs.csv",
"fileurl":"http://172.16.2.23:8888/group1/M00/00/00/xxxxxxxxxxxxxxxxxxxx.csv",
"appid":40
}
```



## 用户文件

请求地址：http://file.biodwhu.cn/fastdfs/own/list

请求类型：POST

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
            "file_time":"2019-01-24 09:59:59"
        },
        {
            "file_id":"xfasdfasdfsadfasdf",
            "file_url":"http://xxxx/group1/xxdasfasdfasdf",
            "file_time":"2019-01-24 09:59:59"
        },
        {
            "file_id":"xfasdfasdfsadfasdf",
            "file_url":"http://xxxx/group1/xxdasfasdfasdf",
            "file_time":"2019-01-24 09:59:59"
        }
    ]
}
```

