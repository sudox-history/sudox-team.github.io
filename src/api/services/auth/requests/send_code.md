# НЕ ДЕЛАЕМ! auth.sendCode

**Краткое описание**

Повторная отправка кода на телефон пользователя

**Запрос клиента**
```c#
{}
```

**Ответ сервера**
```c#
{}
```

**Возможные коды результатов**
> 0000 - **OK**<br><br>
0001 - **SERVICE_UNAVAILABLE**<br><br> 
0003 - **FORMAT_INVALID**<br><br>
0005 - **AUTH_SESSION_NOT_FOUND**<br><br>
0103 - **AUTH_DROPPED**<br><br>
0106 - **AUTH_CODE_ALREADY_SENT**