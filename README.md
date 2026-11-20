# Sunrise Projects

Каталог готовых проектов для Sunrise Launcher.

`projects.json` — индекс каталога. Каждый проект описывается отдельным JSON-документом в папке `projects/`.

## Схема проекта

```json
{
  "schemaVersion": 1,
  "id": "example",
  "name": "Название проекта",
  "description": "Описание",
  "minecraft": "26.2",
  "loader": { "type": "fabric", "version": "0.20.1" },
  "memoryMb": 6144,
  "revision": "1",
  "mods": [
    {
      "name": "Название мода",
      "url": "https://example.com/mod.jar",
      "fileName": "mod.jar",
      "sha1": "0123456789abcdef0123456789abcdef01234567",
      "size": 123456
    }
  ]
}
```

Поддерживаются загрузчики `vanilla` и `fabric`. Для каждого мода обязателен SHA-1, ссылки должны быть HTTPS.
