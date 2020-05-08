# auth.create

**Краткое описание**

Создание сессии авторизации

**Запрос клиента**
```c#
{
    "user_phone": <string>
}
```

**user_phone** - российский (пока что) номер телефона, пример: 79991234556 

**Ответ сервера**
```c#
{
    "auth_id": <string>,
    "user_exists": <bool>
}
```

**Возможные коды результатов**
> 0000 - **OK**<br><br>
0001 - **SERVICE_UNAVAILABLE**<br><br>
0002 - **ACCESS_DENIED**<br><br>
0003 - **FORMAT_INVALID**<br><br>
0102 - **AUTH_EXISTS**<br><br>
0107 - **USER_PHONE_BANNED**