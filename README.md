# api-calendar-facade

Корневой фасадный проект для приложения internal layer api-calendar

## Подключение

Для подключения сервисов api-calendar, необходимо добавить `rb-api-calendar-facade` в раздел `dependencies` своего чарта.

```yaml
# your-helm-facade.yml
dependencies:
  - name: rb-api-calendar-facade
    condition: rb-api-calendar-facade.enabled
    version: ^1.0.0
    repository: '@dbp'
```

Фасад включает 
- выделенный postgresql, kafka

Конфигурация приложения для агент используется умолчательная, поставляемая с агентом