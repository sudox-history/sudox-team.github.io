# Cтруктура API-уведомления

### Сообщение от сервера

Формат: 
```c#
{
    "update_name": <string>,
    "data": <JSONObject>
}
```

**Пример:**
```c#
{
    "update_name": "updates.newAuthVerify",
    "data": {
        "public_key": <string>
    }
} 