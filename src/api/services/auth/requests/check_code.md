# auth.checkCode

**Краткое описание**

Проверка кода, введенного пользователем

**Запрос клиента**
```c#
{
    "auth_id": <string>,
    "auth_code": <int>
}
```

**Ответ сервера**
```c#
{}
```

**Возможные кода результатов**
> 0000 - **OK**<br><br>
0001 - **SERVICE_UNAVAILABLE**<br><br>
0002 - **ACCESS_DENIED**<br><br>
0003 - **FORMAT_INVALID**<br><br>
0101 - **AUTH_NOT_FOUND**<br><br>
0103 - **AUTH_DROPPED**<br><br>
0105 - **AUTH_CODE_INVALID**