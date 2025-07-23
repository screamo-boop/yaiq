# Yet Another Interview Questions

## Зачем?

Все делают свои репозитории для подготовки к интервью, а я чем хуже?

## Навигация

### [Kubernetes (junior)](/k8s/k8s_jun.md)

Дальше будет больше, если не заброшу

## Contributing

Закидываем пулл реквесты с соблюдением структуры репозитория. Создаем папку с темой, например `whatever`. В эту папку добавляем файл с именем по шаблону `{тема}_{уровень}.md`. В файле пишем вопросы и ответы, ответы прячем за спойлер.

Сделать вышеописанное можно следующим образом:

```bash
git clone https://github.com/screamo-boop/yaiq.git
cd yaiq
git checkout -b whatever
mkdir whatever
touch whatever/whatever_jun.md
```

В файл пишем по шаблону

```markdown
1. Продолжите фразу "Whatever is..."

<details>
  <summary>Ответ</summary>

  <pre>
  Whatever is worth doing is worth doing well.
  </pre>
</details>

```

После коммитим, пушим, открываем PR

```bash
git commit -am "Добавил вопросы про Whatever"
git push origin whatever
gh pr create --base main --head whatever --title "Добавил вопросы про whatever" --body "Добавил несколько вопросов про whatever уровня junior"
```
