## Метод - users:get

### **Запрос клиента**
```c#
{
    "users_ids": <string> [],
    "user_type": <int>,
    "expand_bots": <bool>
}
```

>**user_type** - это параметр, принимающий в себя либо **1** (full), либо **2** (short)

>**expand_bots** - возвращать ботов или нет

### **Ответ сервера**
```c#
{
    "result": <int>,
    "users": <user_short, user_full> [],
    (optional) "bots": <bot> []
}
```

[Объект пользователя - user](../../../objects/user.md)

[Объект бота - bot](../../../objects/bot.md)
