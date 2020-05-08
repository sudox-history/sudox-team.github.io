# auth.respondVerify

**Краткое описание**

Подтверждение или отклонение новой авторизации на другом неавторизированном устройстве пользователя

**Запрос клиента**
```c#
{
    "accept": <bool>,
    "public_key": <string>,
    "auth_id": <string>,
    "user_key_enc": <string>
}
```

**public_key** - [Смотрите документацию генерации ключей](https://libsodium.gitbook.io/doc/key_exchange)

1. При помощи сгенерированного public_key и public_key, который пришел от другого устройства в уведомлении update.newVerify получаем сессионный ключ [session_key](https://libsodium.gitbook.io/doc/key_exchange)

2. При помощи session_key шифруем user_key (был получен при регистрации) и получаем user_key_enc

**Ответ сервера**
```c#
{}
```

**Возможные коды результатов**
> 0000 - **OK**<br><br>
0001 - **SERVICE_UNAVAILABLE**<br><br>
0002 - **ACCESS_DENIED**<br><br>
0003 - **FORMAT_INVALID**<br><br>
0101 - **AUTH_NOT_FOUND**<br><br>
0104 - **AUTH_TYPE_INVALID**