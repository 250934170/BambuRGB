## 登录并获取 Token

## POST https://api.bambulab.cn/v1/user-service/user/login

**请求参数**

可以使用密码 或 验证码登录，不要同时提供。
```json
{
    "account": "<ACCOUNT>",
    "password":"<PASSWORD>",
    "code": "<VERIFICATION-CODE>",
}
```

**返回结果**

从响应体中获取 accessToken 和 refreshToken，通常有效期为大约 3 个月：
```json
{
	"accessToken": "[REMOVED]",
	"refreshToken": "[REMOVED]", // 通常与 accessToken 相同
	"loginType": "", // 如果是空字符串，说明可以直接使用 token；如果是 'verifyCode'，需要使用验证码登录
	"expiresIn": 7776000, // 有效期，单位为秒，约 3 个月
	... // 其他一些不重要的字段
}
```
