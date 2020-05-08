# Структура *API*-запроса

### Сообщение от клиента

Формат: 
```c#
{
    "method_name": <string>,
    "data": <JSONObject>
}
```

**Пример:**
```c#
{
    "method_name": "auth.create",
    "data": {
        "user_phone": <string>
    }
} 
```

**Сообщение от сервера**
```c#
{
    "method_name": <string>,
    "method_result": <int>,
    "data": <JSONObject>
}
```

**Пример:**
```c#
{
    "method_name": "auth.create",
    "method_result": 0,
    "data": {
        "auth_token": "h39fg292gd209ygf",
        "user_exist": false
    }
} 
```

**result** - результат выполнения запроса
(см. [Коды результатов](./results_code.md)).