# AI-анализ
AI-анализ лабораторных показателей — инструмент на Go для помощи врачам в интерпретации анализов. Интегрирует симптомы и прогнозы. 
Возможности
- Помощь в интерпретации: Автоматический разбор показателей с объяснениями.
- Прогнозы: Прогнозирование исходов на основе ML-моделей.
- Сопоставление с симптомами: Корреляция анализов с симптомами для диагноза.
 Архитектура
- Модульная: Модули интерпретации, прогнозов, сопоставления.
- Backend: Go с Chi роутером, SQLBoiler для ORM (PostgreSQL).
- AI-компоненты: Gonum/ML для моделей, интеграция с Scikit-learn via gRPC.
- Хранение: PostgreSQL для баз знаний.
- Обработка: Асинхронная с channels.
- Развертывание: Docker, cloud-ready.

 Инструменты и технологии
- Язык: Go 1.21+
- Фреймворки: Chi (HTTP), SQLBoiler (ORM), Gonum/ML.
- Базы данных: PostgreSQL.
- AI/ML: Gonum, внешние ML сервисы.
- CI/CD: Travis CI.
- Тестирование: Go test, benchmarks.
- Другие: Docker, Prometheus.

 Установка
1. Клонируйте: `git clone https://github.com/yourusername/ai-lab-analysis.git`
2. `go mod tidy`
3. .env setup.
4. `go run main.go`
5. Docker: `docker build .`

 Использование
- Ввод: POST `/api/analyze/lab` с JSON.
- Результат: GET `/api/report/{id}`
- Демо: Тестовые данные в repo.

## Автор
Квачёв Александр — Go-разработчик  
GitHub: [AleksKAG](https://github.com/AleksKAG)  
Telegram: [@Kurtalex27](https://t.me/Kurtalex27)
