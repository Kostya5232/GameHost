# Метод logout

| №       | Описание                                      | Входные параметры            | Ожидаемый результат |
| ------- | --------------------------------------------- | ---------------------------- | ------------------- |
| OUT-001 | Успешный выход пользователя                   | `'token' => 'valid_token'`   | "true"              |
| OUT-002 | Выход пользователя с недействительным токеном | `'token' => 'invalid_token'` | `[false, 400]`      |
| OUT-003 | Выход пользователя без передачи токена        | Пустой массив                | `[false, Error]`    |
| OUT-004 | Попытка выхода пользователя с пустым токеном  | `'token' => ''`              | `[false, Error]`    |