## Объект пользователя - user

### **Объект пользователя - тип user_short**
```c#
{
    "id": <string>,
    "name": <string>,
    "nickname": <string>,
    "photo_id": <string>,
    "online": <bool>,
    (optional) "bots": <bot> []
}
```

### **Объект пользователя - тип user_full**
```c#
{
    "id": <string>,
    "name": <string>,
    "nickname": <string>,
    "photo_id": <string>,
    "online": <bool>,
    "subs_count": <int>,
    "subers_count": <int>,
    (optional) "status": <string>,
    (optional) "education": <string>,
    (optional) "job": <string>,
    (optional) "location": <string>,
    (optional) "bots": <bot> []
}
```
