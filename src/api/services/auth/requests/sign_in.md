# auth.signIn

**Краткое описание**

Авторизация пользователя


**Запрос клиента**
```c#
{
    "auth_id": <string>,
    "user_key_hash": <string>
}
```

**user_key_hash** - хэш user_key по [BLAKE2b](https://libsodium.gitbook.io/doc/hashing/generic_hashing)

**Ответ сервера**
```c#
{
    "user_id": <string>,
    "user_secret": <string>
}
```

**Возможные коды результатов**
> 0000 - **OK**<br><br>
0001 - **SERVICE_UNAVAILABLE**<br><br>
0002 - **ACCESS_DENIED**<br><br>
0003 - **FORMAT_INVALID**<br><br>
0101 - **AUTH_NOT_FOUND**<br><br>
0104 - **AUTH_TYPE_INVALID**<br><br>
0105 - **AUTH_CODE_INVALID**<br><br>
0108 - **USER_KEY_HASH_INVALID**