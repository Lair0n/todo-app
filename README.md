## Описание проекта
Простое консольное приложение для управления задачами (Todo List) на Java с автоматизированной сборкой, тестированием и развертыванием через GitHub Actions CI/CD.

## 📋 Функциональность
- ✅ Добавление задач (`add <task>`)
- ✅ Удаление задач по индексу (`remove <index>`)  
- ✅ Просмотр списка задач (`list`)
- ✅ Выход из приложения (`exit`)
- ✅ Автоматическая нормализация пробелов
- ✅ Игнорирование пустых строк

## 🛠 Технологический стек
- **Язык:** Java 17
- **Сборка:** Gradle 8.5
- **Тестирование:** JUnit 5
- **CI/CD:** GitHub Actions
- **Версионность:** Git + GitHub Flow

## 📁 Структура проекта
todo-app/
├── src/
│ ├── main/java/org/example/
│ │ ├── TodoApp.java # Главный класс приложения
│ │ └── TodoList.java # Логика работы со списком задач
│ └── test/java/org/example/
│ └── TodoListTest.java # Юнит-тесты
├── .github/workflows/
│ └── ci.yml # CI/CD конфигурация
├── build.gradle # Конфигурация сборки
├── gradle.properties # Настройки версий
└── README.md # Документация
### Сборка проекта
./gradlew clean build

Запуск тестов
./gradlew test

Запуск приложения
./gradlew run



Локальная проверка (ВСЕ РАБОТАЕТ)
Результаты локального тестирования:
✅ Сборка проекта - .\gradlew.bat clean build - BUILD SUCCESSFUL

✅ JAR-файлы созданы - todo-app-0.1.0.jar (3.44 KB) и todo-app-all.jar (3.47 KB)

✅ Тесты проходят - все 4 теста PASSED:

AppTest > appHasAGreeting() PASSED

TodoListTest > remove() PASSED

TodoListTest > addEmptyIgnored() PASSED

TodoListTest > addAndList() PASSED

✅ Приложение запускается через Gradle - .\gradlew.bat run работает корректно

✅ Структура проекта - все ключевые файлы присутствуют

⚠️ Проблемы с GitHub Actions
Текущий статус CI/CD:
❌ GitHub Actions workflow - завершается с ошибками

❌ Автоматические релизы - не создаются

✅ Локальная сборка - полностью работоспособна

История запусков workflow:
Зафиксировано 15 workflow runs с различными ошибками

Workflow "Java CI with Gradle" запускается при каждом push

Большинство запусков завершаются неудачно


