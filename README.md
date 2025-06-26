  ## BeautySalon — микросервисная система для управления салоном красоты
Проект представляет собой распределённую м## BeautySalon — микросервисная система для управления салоном красотыой Проект представляет собойраспределённую микросервисную backend-систему для управления салоном красоты. Реализованы сервисы аутентификации, сотрудники/услуги, бронирования. Каждый сервис изолирован, взаимодействие — через брокер RabbitMQ. Развёртывание — через Kubernetes и FluxCD (GitOps-подход).<!-- Подставь свой путь или ссылку -->

- ASP.NET Core 8, DDD + CQRS
- PostgreSQL, RabbitMQ
- Docker, Kubernetes
- Helm + FluxCD (GitOps)
- Микросервисы: Auth, Employees, Booking
---
## Сервисы проекта
| Сервис               | Назначение                                      | Репозиторий |
|----------------------|--------------------------------------------------|-------------|
| 👤 AuthAndClient     | Регистрация, авторизация, управление клиентами   | [🔗 GitHub](https://github.com/Woogie7/BeautySalon.AuthandClient) |
| 🧍 Employees         | Работа с сотрудниками, услугами и расписанием    | [🔗 GitHub](https://github.com/твой-ник/BeautySalon.Employees) |
| 📅 Booking           | Создание, подтверждение и управление бронированиями | [🔗 GitHub](/BeautySalon.Booking) |
| 🔗 Contracts         | Общие контракты между сервисами (DTO, Events)    | [🔗 GitHub](https://github.com/Woogie7/BeautySalon.Contracts) |
| 🚀 Deployments       | Манифесты Kubernetes и Helm-чарты для всех сервисов | [🔗 GitHub](https://github.com/Woogie7/BeautySalon.Deployments) |

---

## ⚙️ Технологии

- Язык: **C# (.NET 8)**
- БД: **PostgreSQL**
- Архитектура: **DDD**, **CQRS**, **Event-driven**
- Транспорт: **RabbitMQ**
- Контейнеризация: **Docker**, **Helm**, **Kubernetes**
- CI/CD: **GitHub Actions**, **FluxCD**

---

## 🚀 Как развернуть проект

1. Клонируйте репозиторий с манифестами:
```bash
git clone https://github.com/твой-ник/BeautySalon.Deployments
cd BeautySalon.Deployments
