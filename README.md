# DevOps Project by Anton Artemov  
**Цель:** Изучение Docker, Kubernetes, Prometheus/Grafana и ELK-стека.  

## День 1: Docker  
- Запуск контейнера Nginx.  
- Создание Docker-образа для Python-приложения.  

### Скриншоты:  
- **Docker-образы:**  
  ![Docker Images](docs/screenshots/docker-images.jpg)  
- **Работа приложения:**  
  ![Python App](docs/screenshots/python-app.jpg)  
- **Сеть**
  ![Сетевые настройки](docs/screenshots/ip-addr.jpg)

# День 2: Docker Compose и PostgreSQL  
- Запуск связки **Nginx + PostgreSQL** через Docker Compose.  
- Автоматизация создания таблиц и данных через `init.sql`.  

### Скриншоты:
- **Запущенные контейнеры:**  
  ![Docker Compose PS](docs/screenshots/docker-compose-ps.jpg)  # Вывод `docker-compose ps`
- **Результат SQL-запроса:**  
  ![SQL Users](docs/screenshots/sql-users.png)  # Вывод `SELECT * FROM users;`
- **Структура проекта:**  
  ![Project Tree](docs/screenshots/tree.jpg)  # Вывод `tree`

### Команды:  
```bash
# Запуск Python-приложения
docker run -d -p 5000:5000 --name my-python-app my-python-app

