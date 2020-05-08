# НЕ ДЕЛАЕМ! auth.signInForce

**Краткое описание**

Авторизация без передачи пользовательского ключа (бех чатов)


**Запрос клиента**
```c#
{
    "auth_code": <int>
}
```

**auth_code** - 5-значное число

**Ответ сервера**
```c#
{
    "user_secret": <string>,
    "user_id": <string>
}
```

**Возможные коды результатов**
> 0000 - **OK**<br><br>
0001 - **SERVICE_UNAVAILABLE**<br><br>
0003 - **FORMAT_INVALID**<br><br>
0101 - **SESSION_NOT_FOUND**<br><br>
0103 - **AUTH_DROPPED**<br><br>
0104 - **AUTH_TYPE_INVALID**<br><br>
0105 - **AUTH_CODE_INVALID**