## login(name: str, token: str) -> int | None

登录，如果成功则返回bot的id，否则返回None。

参数：

- name：bot的名字
- token：bot的token

返回值：int | None

## register(name: str, token: str) -> int | None

注册，如果成功则返回bot的id，否则返回None。

参数：

- name：bot的名字
- token：bot的token

返回值：int | None

## join(bot_id: int, chat_id: int) -> bool

加入聊天室，如果成功则返回True，否则返回False。

参数：

- bot_id：bot的id 
- chat_id：聊天室的id 

返回值：bool 

## quit(bot_id: int, chat_id: int) -> bool 

 退出聊天室，如果成功则返回True，否则返回False。

 参数：

 - bot_id：bot的id 
 - chat_id：聊天室的id 

 返回值：bool 

## kick(bot_id: int, kicked_user_id: int, chat_id: int) -> bool 

 踢出用户，如果成功则返回True，否则返回False。

 参数：

 - bot_id：bot的id 
 - kicked_user_id：被踢出用户的id 
 - chat_id：聊天室的id 

 返回值：bool 

## rename(bot_id: int, new_name: str, chat_id: int) -> bool 

 重命名聊天室，如果成功则返回True，否则返回False。

 参数：

 - bot_id：bot的id 
 - new_name：新的聊天室名称 
 - chat_id：聊天室的id 

 返回值：bool 

## check_send(self, bot_id: int, chat_id: int) -> bool 

 检查是否可以发送消息。如果可以发送消息则返回True，否则返回False。

 参数：

 - bot_id：bot的id 
 - chat_id：聊天室的id 

 返回值：bool 

## check_create_session(self, bot_id: int, chat_id: int) -> bool 

 检查是否可以创建会话。如果可以创建会话则返回True，否则返回False。

 参数：

 - bot_id：bot的id 
 - chat_id：聊天室的id 

 返回值：bool 

## modify_user_permission(self, chat_id: int, bot_id: int, modified_user_id: int, name: str, value: bool) -> bool 

 修改用户权限。如果修改成功则返回True，否则返回False。

 参数：

 - chat_id ：聊天室的 id 
 - bot _ id ：bot 的 id 
 - modified _ user _ id ：要修改权限的用户 id 
 - name ：要修改权限的名称 
 - value ：要修改权限的值 

 返回值 ：bool 

## modify _ permission (self , chat _ id : int , bot _ id : int , name : str , value : bool ) -> bool  

 修改聊天室权限。如果修改成功则返回True ， 否则返回 False。  

 参数 ：  

 - chat _ id ：聊天室的 id  
 - bot _ id ：bot 的 id  
 - name ：要修改权限的名称  
 - value ：要修改权限
