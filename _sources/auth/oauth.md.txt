# Oauth 外部验证

## 涉及的api:
```
oauth_xxx.request_oauth() -> (url:str,requestid:str)
oauth_xxx.login_oauth(requestid:str) -> dict
oauth_xxx.procress_oauth(requestid:str,quert:dict)
login.post_oauth(platform: str, metadata: str,nickname:Optional[str]=None) -> (userid:str,token:str)
```
## 调用流程
```python
伪代码,xxx为oauth提供者名称:
requestid,url=oauth_xxx.request_oauth()
# 用户使用url进行验证
result=oauth_xxx.login_oauth(requestid)
"""
result={"id":<平台侧用户标志符>,"nickname":<平台侧用户名/昵称(可能不包含)>}
"""
# 等待用户验证成功
uid,tokenlogin.post_oauth(xxx,result['id'],result.get(nickname))
# 使用返回的用户标志符注册/登录
```
## 实现流程
```python 
# TODO
```