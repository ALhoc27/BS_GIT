# IntelliJ IDEA и GitHub

## [Загрузить проект из IntelliJ IDEA в новый репозиторию GitHub](#user-content-fn-1)[^1]

**1.** [Создание нового репозитория на **GitHub**](#user-content-fn-2)[^2]

**2.** [Инициализация **Git** в **IntelliJ IDEA**](#user-content-fn-3)[^3]

**3.** С[вязывание локального проекта с удалённым репозиторием](#user-content-fn-4)[^4]

**4.** Добавление файлов в репозиторий

**5.** Создание первого коммита

**6.** Отправка кода в удалённый репозиторий

* Откройте терминал в **IntelliJ** (View → Tool Windows → Terminal).
*   Выполните следующую команду, чтобы добавить удалённый репозиторий:

    {% code overflow="wrap" %}
    ```bash
    Копировать кодgit remote add origin https://github.com/your-username/your-repo-name.git
    ```
    {% endcode %}
* Замените `your-username` на ваше имя пользователя GitHub, а `your-repo-name` на имя вашего репозитория.

{% tabs %}
{% tab title="1. Создание нового репозитория на GitHub:" %}
1. Войдите в свой аккаунт GitHub.
2. Перейдите на вкладку **Repositories** и нажмите кнопку **New**.
3. Нажмите **Create repository**
{% endtab %}

{% tab title="2. Инициализация Git в IntelliJ IDEA:" %}
**Инициализация Git в IntelliJ IDEA:**

2. Откройте свой проект в IntelliJ IDEA.
3. П[ерейдите в меню **VCS** (Version Control System) → **Enable Version Control Integration**.](#user-content-fn-5)[^5]
4. В выпадающем списке выберите **Git** и нажмите **OK**. Это инициализирует Git в вашем проекте.
{% endtab %}

{% tab title="3. Связывание локального проекта с удалённым репозиторием:" %}

{% endtab %}

{% tab title="4. Добавление файлов в репозиторий:" %}

{% endtab %}

{% tab title="5. Создание первого коммита:" %}

{% endtab %}

{% tab title="6. Отправка кода в удалённый репозиторий:" %}

{% endtab %}
{% endtabs %}

1. #### **Создание нового репозитория на GitHub:**

* Войдите в свой аккаунт GitHub.
* Перейдите на вкладку **Repositories** и нажмите кнопку **New**.
* Нажмите **Create repository**.

2. #### **Инициализация Git в IntelliJ IDEA:**

* Откройте свой проект в IntelliJ IDEA.
* П[ерейдите в меню **VCS** (Version Control System) → **Enable Version Control Integration**.](#user-content-fn-6)[^6]
* В выпадающем списке выберите **Git** и нажмите **OK**. Это инициализирует Git в вашем проекте.

## Привязать существующий проект в IntelliJ IDEA к новому репозиторию GitHub

1. **Создайте новый репозиторий на GitHub:**
   * Зайдите на [GitHub](https://github.com/).
   * В правом верхнем углу нажмите на "+" и выберите "New repository".
   * Нажмите "Create repository".
2. **Откройте IntelliJ IDEA**:
   * Откройте ваш проект в IntelliJ IDEA.
3. **Инициализируйте Git:**
   *   Если ваш проект ещё не инициализирован с использованием системы контроля версий Git, выполните следующие шаги:

       * Откройте терминал в IntelliJ IDEA (`View -> Tool Windows -> Terminal`).
       * Введите следующие команды:

       ```swift
       git init // Команда для инициализации Git
       git add . // Добавьте все файлы в индекс Git
       git commit -m "Initial commit" // Завершите первоначальный коммит
       ```
4. **Скопируйте URL вашего нового репозитория:**
   * Вернитесь на страницу вашего нового репозитория на GitHub.
   * Нажмите на кнопку "Code" и скопируйте URL репозитория.
5. **Привяжите IntelliJ IDEA к новому репозиторию:**
   * В IntelliJ IDEA выберите "VCS" в верхнем меню.
   * Выберите "Import into Version Control" -> "Share Project on GitHub".
   * Введите свои учетные данные GitHub, если требуется.
   * Вставьте скопированный URL репозитория.
   * Нажмите "Share".
6.  **Закоммитьте и запушьте изменения:**

    * После привязки к репозиторию выполните команды:

    ```bash
    git add .
    git commit -m "Initial commit"
    git push origin master
    ```

    * (Замените "master" на имя вашей ветки, если она отличается).

Теперь ваш проект связан с новым репозиторием GitHub. Вы можете делать коммиты, изменения и пушить их в ваш репозиторий на GitHub через IntelliJ IDEA.



## Импортировать проект с GitHub в вашу интегрированную среду разработки IntelliJ IDEA

1. Откройте IntelliJ IDEA.
2. Выберите "File" (Файл) -> "New" (Создать) -> "Project from Version Control" (Проект из системы контроля версий).
3. В выпадающем списке выберите "Git".
4. Вставьте URL вашего репозитория GitHub в поле "URL".
5. Укажите локальный путь, куда вы хотите сохранить проект.
6. Нажмите "Clone".

[^1]: **1.** Создание нового репозитория на **GitHub**

    **2.** Инициализация **Git** в **IntelliJ IDEA**

    **3.** Связывание локального проекта с удалённым репозиторием

    **4.** Добавление файлов в репозиторий

    **5.** Создание первого коммита

    **6.** Отправка кода в удалённый репозиторий

[^2]: **1.** Войдите в свой аккаунт **GitHub**.

    **2.** Перейдите на вкладку **Repositories** и нажмите кнопку **New**.

    **3.** Нажмите **Create repository**

    репозиторий

[^3]: **1.** Откройте свой проект в IntelliJ IDEA.

    **2.** П[ерейдите в меню **VCS** (Version Control System) → **Enable Version Control Integration**.](#user-content-fn-7)[^7]

    **3.** В выпадающем списке выберите **Git** и нажмите **OK**. Это инициализирует Git в вашем проекте.

[^4]: 

    * Откройте терминал в **IntelliJ** (View → Tool Windows → Terminal).

    <!---->

    *   Выполните следующую команду, чтобы добавить удалённый репозиторий:

        {% code overflow="wrap" %}
        ```bash
        Копировать кодgit remote add origin https://github.com/your-username/your-repo-name.git
        ```
        {% endcode %}

    <!---->

    * Замените `your-username` на ваше имя пользователя GitHub, а `your-repo-name` на имя вашего репозитория.

[^5]: ![](<.gitbook/assets/Снимок экрана 2024-09-18 в 11.11.21.png>)

[^6]: ![](<.gitbook/assets/Снимок экрана 2024-09-18 в 11.11.21.png>)
