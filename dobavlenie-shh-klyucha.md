# Добавление SHH-ключа

### Пошаговая инструкция (в терминале):

**Шаг 1:** Создайте SSH-ключ

{% code overflow="wrap" fullWidth="true" %}
```swift
ssh-keygen -t ed25519 -C "your_email@example.com"
// Note: If you are using a legacy system that doesn't support the Ed25519 algorithm, use:
ssh-keygen -t rsa -b 4096 -C "your_email@example.com"
// -t rsa указывает использовать алгритм RSA.
// -b 4096 указывает на битовую длину ключа (4096 бит - это хорошо для безопасности).
// -C "your_email@example.com" позволяет добавить комментарий к ключу (обычно это ваш адрес электронной почты).
```
{% endcode %}

**Шаг 2:** Получите ваш публичный SSH-ключ&#x20;

Выведите содержимое вашего публичного SSH-ключа с помощью следующей команды:

```bash
cat ~/.ssh/id_rsa.pub
```

<details>

<summary><em><mark style="color:purple;">Как посмотреть свой открытый ключ SSH на macOS</mark></em> </summary>

Просмотр ключей на macOS:\
Откройте окно терминала и введите команду:

```bash
cat ~/.ssh/id_rsa.pub
```

или:

```bash
cat /Users/USERNAME/.ssh/id_rsa.pub
```

Где USERNAME – ваше имя пользователя macOS.\
Приведенные выше команды выведут ваш открытый ключ SSH.

![](<.gitbook/assets/Снимок экрана 2024-09-17 в 20.01.48.png>)

Для отображения скрытых папок:\
`command + shift + .`

⁠ ![](<.gitbook/assets/Снимок экрана 2024-09-17 в 20.03.08.png>)

</details>



> В finder, `command+shift+G`
>
> /Users/alexander/.ssh
