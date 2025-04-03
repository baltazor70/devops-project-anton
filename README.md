# DevOps Project by Anton Artemov  
**Цель:** Изучение Docker, Kubernetes, Prometheus/Grafana и ELK-стека.  

## День 1: Docker  
- Запуск контейнера Nginx.  
- Создание Docker-образа для Python-приложения.  

### Скриншоты:  
- **Docker-образы:**  
  ![Docker Images](docs/screenshots/docker-images.png)  
- **Работа приложения:**  
  ![Python App](docs/screenshots/python-app.png)  
- **Сеть**
  ![Сетевые настройки](docs/screenshots/ip-addr.png)

# День 2: Docker Compose и PostgreSQL  
- Запуск связки **Nginx + PostgreSQL** через Docker Compose.  
- Автоматизация создания таблиц и данных через `init.sql`.  

### Скриншоты:
- **Запущенные контейнеры:**  
  ![Docker Compose PS](docs/screenshots/docker-compose-ps.png)  # Вывод `docker-compose ps`
- **Результат SQL-запроса:**  
  ![SQL Users](docs/screenshots/sql-users.png)  # Вывод `SELECT * FROM users;`
- **Структура проекта:**  
  ![Project Tree](docs/screenshots/tree.png)  # Вывод `tree`

## День 3: Kubernetes
- Запуск Python-приложения в Minikube.  
- Масштабирование до 2 реплик (как вы поддерживали 1500+ пользователей).  

### Скриншоты:
- **Kubernetes Pods:**  
  ![Kubernetes Pods](docs/screenshots/k8s-pods.png)  
- **Приложение в браузере:**  
  ![Python App in Kubernetes](docs/screenshots/k8s-python-app.png)

### Команды:  
```bash
# Запуск Python-приложения
docker run -d -p 5000:5000 --name my-python-app my-python-app
# Запуск сервисов
docker-compose up -d
# Подключение к PostgreSQL
docker-compose exec db psql -U postgres


