# Основы работы с Git

1. #### Create a new repository&#x20;

Создадим новый репозиторий на [**https://github.com/new**](https://github.com/new)

Например: **`NewRepository`**

{% tabs %}
{% tab title="Create a new repository " %}
<figure><img src=".gitbook/assets/Снимок экрана 2024-09-17 в 17.31.45 (2).png" alt=""><figcaption></figcaption></figure>
{% endtab %}

{% tab title="Quick setup" %}
#### …or create a new repository on the command line

```
echo "# NewRepository" >> README.md
git init
git add README.md
git commit -m "first commit"
git branch -M main
git remote add origin git@github.com:ALhoc27/NewRepository.git
git push -u origin main
```

#### …or push an existing repository from the command line

```
git remote add origin git@github.com:ALhoc27/NewRepository.git
git branch -M main
git push -u origin main
```
{% endtab %}
{% endtabs %}
