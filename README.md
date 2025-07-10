  ## BeautySalon — микросервисная система для управления салоном красоты
Проект представляет собой распределённую м## BeautySalon — микросервисная система для управления салоном красотыой Проект представляет собойраспределённую микросервисную backend-систему для управления салоном красоты. Реализованы сервисы аутентификации, сотрудники/услуги, бронирования. Каждый сервис изолирован, взаимодействие — через брокер RabbitMQ. Развёртывание — через Kubernetes и FluxCD (GitOps-подход).
---
## Сервисы проекта
| Сервис               | Назначение                                      | Репозиторий |
|----------------------|--------------------------------------------------|-------------|
| AuthAndClient     | Регистрация, авторизация, управление клиентами   | [🔗 GitHub](https://github.com/Woogie7/BeautySalon.AuthandClient) |
| Employees         | Работа с сотрудниками, услугами и расписанием    | [🔗 GitHub](https://github.com/Woogie7/BeautySalon.Employees) |
| Booking           | Создание, подтверждение и управление бронированиями | [🔗 GitHub](https://github.com/Woogie7/BeautySalon.Booking) |
| Contracts         | Общие контракты между сервисами (DTO, Events)    | [🔗 GitHub](https://github.com/Woogie7/BeautySalon.Contracts) |
| Deployments       | Манифесты Kubernetes и Helm-чарты для всех сервисов | [🔗 GitHub](https://github.com/Woogie7/BeautySalon.Deployments) |
