# auth.verify

**Краткое описание**

Отправка подтверждения авторизации на другой авторизированный телефон пользователя 

**Запрос клиента**
```c#
{
    "auth_id": <string>,
    "public_key": <string>
}
```
**public_key** - [Смотрите документацию генерации ключей](https://libsodium.gitbook.io/doc/key_exchange)

**Ответ сервера**
```c#
{}
```

**Возможные коды результатов**
> 0000 - **OK**<br><br>
0001 - **SERVICE_UNAVAILABLE**<br><br>
0002 - **ACCESS_DENIED**<br><br>
0003 - **FORMAT_INVALID**<br><br>
0005 - **AUTH_NOT_FOUND**<br><br>
0104 - **AUTH_TYPE_INVALID**
