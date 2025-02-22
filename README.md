# Software Architect // Архитектурная ката Room with a View

Этот проект содержит домашние задания, а так же проектную работу, выполненные в рамках курса Software Architect. В заданиях решается архитектурная ката Нила Форда "Room with a View".\
Автор проекта - **Кривопиша Сергей**

## Содержание

1. [Анализ требований и подготовка архитектурному решению](homework_01.md)
2. [Декомпозиция на функциональные компоненты](homework_02.md)
3. [Взаимодействие сервисов](homework_03.md)
4. [Системное проектирование](homework_04.md)

## Описание заданий

### 1. Анализ требований и подготовка архитектурному решению

В этом задании проводится анализ требований и описываются составляющие архитектурного решения для системы бронирования и управления номерами в отеле. Основные аспекты включают:

- Бизнес-контекст
- Бизнес-цели и бизнес-драйверы
- Стейкхолдеры и их потребности
- Пользовательские истории
- Атрибуты качества
- Критические сценарии и характеристики
- Архитектурные решения

[Подробнее](homework_01.md)

### 2. Декомпозиция на функциональные компоненты

В этом задании рассматриваются различные подходы к декомпозиции системы на функциональные компоненты:

- Декомпозиция на основе пользовательских потоков
- Декомпозиция на основе технических доменов
- Декомпозиция по функциональным областям

Каждый подход оценивается по критериям модифицируемости, локализации изменений, гибкости, легкости интеграции, сложности разработки и сопровождения, а также ориентации на бизнес.

[Подробнее](homework_02.md)

### 3. Взаимодействие сервисов

В этом задании рассматривается взаимодействие между основными сервисами системы бронирования и управления номерами отеля. Основные сервисы включают:

- Сервис бронирования
- Сервис управления статусами номеров
- Сервис управления доступом
- Сервис уведомлений
- Сервис аналитики

Оцениваются атрибуты качества (например, надежность, производительность, модифицируемость и т.д) с помощью конкретных сценариев и характеристик системы.

[Подробнее](homework_03.md)

### 4. Системное проектирование

В этом задании система рассматривается в контексте приложений и их контейнеров, декомпозируется слой данных, а так же описывается диаграмма деплоймента.

#### Основные компоненты развертывания:

1. **Kubernetes Cluster**  
    - **Frontend**: Поддержка CDN для доставки статики.  
    - **API Gateway**: Обеспечение единой точки входа для запросов.  
    - **Микросервисы**: Отдельные поды для каждого сервиса.  
    - **Event Bus**: Kafka для асинхронной обработки событий.

2. **Хранилище данных**
    - Внешние управляемые базы данных (например, AWS RDS, MongoDB Atlas).

4. **Мониторинг и логирование**  
    - **Prometheus + Grafana**: Сбор и визуализация метрик.  
    - **ELK-стек**: Централизованное логирование.

[Подробнее](homework_04.md)
