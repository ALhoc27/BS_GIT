# IntelliJ IDEA и GitHub

## [Загрузить проект из IntelliJ IDEA в новый репозиторию GitHub](#user-content-fn-1)[^1]

## Загрузить проект из IntelliJ IDEA в новый репозиторию GitHub

{% tabs %}
{% tab title="1. Создание нового репозитория на GitHub:" %}
1. Войдите в свой аккаунт GitHub.
2. Перейдите на вкладку **Repositories** и нажмите кнопку **New**.
3. Нажмите **Create repository**
{% endtab %}

{% tab title="2. Инициализация Git в IntelliJ IDEA:" %}
**Инициализация Git в IntelliJ IDEA:**

2. Откройте свой проект в IntelliJ IDEA.
3. П[ерейдите в меню **VCS** (Version Control System) → **Enable Version Control Integration**.](#user-content-fn-2)[^2]
4. В выпадающем списке выберите **Git** и нажмите **OK**. Это инициализирует Git в вашем проекте.
{% endtab %}

{% tab title="Untitled" %}

{% endtab %}

{% tab title="Untitled" %}

{% endtab %}

{% tab title="Untitled" %}

{% endtab %}
{% endtabs %}

1. #### **Создание нового репозитория на GitHub:**

* Войдите в свой аккаунт GitHub.
* Перейдите на вкладку **Repositories** и нажмите кнопку **New**.
* Нажмите **Create repository**.

2. #### **Инициализация Git в IntelliJ IDEA:**

* Откройте свой проект в IntelliJ IDEA.
* П[ерейдите в меню **VCS** (Version Control System) → **Enable Version Control Integration**.](#user-content-fn-3)[^3]
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

[^2]: ![](<.gitbook/assets/Снимок экрана 2024-09-18 в 11.11.21.png>)

[^3]: ![](<.gitbook/assets/Снимок экрана 2024-09-18 в 11.11.21.png>)
