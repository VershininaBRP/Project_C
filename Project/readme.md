# Распознавание конфликтных ситуаций с камер видеонаблюдения

## Введение:
Проект направлен на разработку системы машинного зрения, способной автоматически распознавать конфликтные ситуации (драки, агрессивное поведение) на видеозаписях с камер видеонаблюдения. 

**Основная цель** — повысить уровень общественной безопасности и оперативность реагирования в местах массового скопления людей и не только (метро, торговые центры, школы, улицы и т.д.).

**Ожидаемый результат**
Создание обученной модели, способной классифицировать видеоролики на два класса: "Насилие" и "Отсутствие насилия". Высокая точность распознавания: стремление достичь точности >85% на тестовом наборе.
Интеграция с Telegram-ботом: удобный интерфейс для демонстрации работы модели в реальном времени.
## Стек технологий:
Python, PyTorch, OpenCV, Torchvision, scikit-learn, tqdm, Telegram Bot.
## Датасет:
Базовый набор данных был получен с платформы Kaggle. Он содержал видеофрагменты, заранее размеченные как:
1. Violence (наличие агрессивного поведения);
2. NonViolence (обычные действия без конфликта);
   
Общий объём: 3900 видео: 1950 с насилием / 1950 без насилия.
Большинство видео короткие (до 3-6 секунд), что удобно для подачи в модель.

## Структура модели
![image](https://github.com/user-attachments/assets/58b8d111-e7e0-48c5-be89-081fa3f61d93)

**Метрики**

Модель сбалансирована, одинаково хорошо распознаёт оба класса.
![image](https://github.com/user-attachments/assets/ecb91ae3-d37f-427d-bb67-e343d099014e)

## Демонстрация работы модели (запись экрана телеграм-бота):
https://disk.yandex.ru/i/9KWp8GCyyyK8Mg
## Ссылки
1. Модель
   https://disk.yandex.ru/d/_WjSUfl5Lxyadg
2. Датасет
   https://disk.yandex.ru/d/Bp8vxqLuTBOwyA
3. Тетрадка-обучение
   https://github.com/VershininaBRP/Project_C/blob/main/Project/learn.ipynb
4. Тетрадка-телеграм бот
   https://github.com/VershininaBRP/Project_C/blob/main/Project/telegrambot.ipynb
5. Презентация
   https://disk.yandex.ru/d/QYhs45jN0Wopzg
6. Датасет 20 видео для просмотра работы модели
   https://disk.yandex.ru/d/Wue_c07STELB3Q
