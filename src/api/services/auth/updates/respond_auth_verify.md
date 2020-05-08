# updates.respondAuthVerify
accept, public_key, user_key_enc

**Краткое описание**

Уведомление результата запроса respondVerify на другом устройстве


**Уведомление от сервера**
```c#
{
    "accept": <bool>,
    (optional) "public_key": <string>,
    (optional) "user_key_enc": <string>
}
```