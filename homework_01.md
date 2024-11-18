# Анализ требований и подготовка архитектурному решению
Кривопиша Сергей\
Курс Software Architect

## Задача
В качестве кейса выбрана одна из архитектурных ката Нила Форда, а именно Room with a View: https://nealford.com/katas/kata?id=RoomWithAView

Необходимо провести анализ требований и описать составляющие архитектурного решения.

## Room with a View
A large hotel reservation company wants to build the next generation hotel reservation and management system specifically tailored to high-end resorts and spas where guests can view and reserve specific rooms.

- Users: Guests (hundreds), hotel staff (less than 20)
- Requirements:
  - Registration can be made via web, mobile, phone call, or walk-in.
  - Guests have the ability to either book a type of room (standard, deluxe, or suite) or choose a specific room to stay in by viewing pictures of each room and its location in the hotel.
  - The system must be able to maintain room status (booked, available, ready to clean, etc.) as well as when the room will be needed next.
  - It must also have state-of-the-art housekeeping management functionality so that cleaning and maintenance staff can be directed to various rooms based on priority and reservation need using proprietary devices supplied by the reservation company attached to the cleaning carts.
  - Standard reservation functionality (e.g., payments, registration info, etc.) will be done by leveraging the existing reservations system.
  - The system will be web-based and hosted by the reservation company.
- Additional Context:
  - 'Peak season is quickly approaching, so the system must be ready quickly or we have to wait until next year!'
  - Company is also investing heavily in cutting edge technology like smart room locks that open via a cell phone
  - Only interested in the high-end market
  - Sales people have tremendous clout in the organization; people often scramble to make their promises true

## Бизнес-контекст
Компания — крупный поставщик услуг по бронированию, стремящийся выйти на рынок премиум-класса, предлагая услуги для элитных курортов и спа-центров. Новый продукт, система бронирования и управления номерами, будет ориентирован на улучшение пользовательского опыта, предоставляя гостям удобный способ выбора номеров и усовершенствованные возможности для управления ресурсами отеля.

Конкурентные преимущества: вкладывает значительные средства в передовые технологии для создания уникального опыта и повышенного уровня безопасности и удобства для гостей. Кроме того, компания стремится оптимизировать внутренние процессы отелей, что важно для обеспечения качественного обслуживания.

Сроки: Система должна быть запущена до начала пикового сезона.

![image](https://github.com/user-attachments/assets/e18afad1-7bbe-4f43-bcea-b63650af4d39)

## Бизнес-цели и бизнес-драйверы
### Бизнес-драйверы
- Привлечение и удержание клиентов премиум-класса
- Инвестиции в передовые технологии как ключевой фактор дифференциации от конкурентов
- Снижение издержек и повышение эффективности благодаря улучшенной координации действий персонала, а так же интеграции с существующей системой бронирования
- Система должна быть готова к пиковому сезону

### Бизнес-цель
В короткие сроки разработать систему бронирования и управления номерами для самых требовательных элитных клиентов. Конкурентными преимуществами должны стать обеспечение высокого сервиса, интеграция с инновационными технологии для оптимизации обслуживания.

## Стейкхолдеры и их потребности
