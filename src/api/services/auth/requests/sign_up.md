# auth.signUp

**Краткое описание**

Регистрация пользователя

**Запрос клиента**
```c#
{
    "auth_id": <string>,
    "user_name": <string>,
    "user_nickname": <string>,
    "user_key_hash": <string>
}
```

**user_key** - массив рандомных байтов длины 32 (crypto_aead_xchacha20poly1305_ietf_KEYBYTES) [используя](https://libsodium.gitbook.io/doc/generating_random_data). Требуется сохранить его в локальную базу данных.

**user_key_hash** - хэш user_key по [BLAKE2b](https://libsodium.gitbook.io/doc/hashing/generic_hashing)

**user_name** - ^([A-zА-я]{1,20}\\s?){2}$

**user_nickname** - ^[0-9A-z.:_\\-()]{1,30}$

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
0105 - **AUTH_CODE_INVALID**