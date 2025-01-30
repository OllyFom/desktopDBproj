# desktopDBproj
# Проект: Социальная сеть на C++ с использованием Qt и PostgreSQL

## Описание проекта

Проект представляет собой десктопное приложение, реализованное на C++ с использованием фреймворка Qt и базы данных PostgreSQL. Приложение предоставляет пользователям возможность авторизации, создания аккаунта, публикации постов, подписки на других пользователей, просмотра ленты новостей, а также взаимодействия с контентом (лайки).

## Основные функции

1. **Авторизация и регистрация:**
   - Пользователь может войти в систему, используя свои учетные данные.
   - Новые пользователи могут зарегистрироваться, создав новый аккаунт.

2. **Публикация постов:**
   - Авторизованные пользователи могут создавать и публиковать посты.
   - Посты могут содержать текст, изображения и другие медиафайлы.

3. **Подписки:**
   - Пользователи могут подписываться на других пользователей.
   - Подписчики могут видеть посты тех, на кого они подписаны, в своей ленте новостей.

4. **Лента новостей:**
   - Лента новостей формируется из постов пользователей, на которых подписан текущий пользователь.
   - Посты отображаются в хронологическом порядке.

5. **Просмотр страницы пользователя:**
   - Пользователи могут просматривать страницы других пользователей, чтобы увидеть их посты и информацию.

6. **Лайки:**
   - Пользователи могут ставить лайки на понравившиеся посты.
   - Количество лайков отображается под каждым постом.

## Структура проекта

Проект разработан с использованием принципов объектно-ориентированного программирования (ООП). Основные классы и компоненты:

- **User:** Класс, представляющий пользователя. Содержит информацию о пользователе, такие как логин, пароль, список подписок и постов.
- **Post:** Класс, представляющий пост. Содержит текст поста, автора, дату публикации и количество лайков.
- **view_profile** Класс, представляющий окно просмотра информации другого пользователя
- **view_posts** Класс, представляющий окно просмотра постов пользователей подписок
- **signin** Класс, представляющий окно просмотра страницы авторизации
- **Profile** Класс, представляющий окно просмотра информации своего профиля. Показывает имя пользователя, количество подписок и подписчиков, предоставляет доступ к переходу в другие окна
- **my_subscriptions**Класс, представляющий окно просмотра подписчиков
- **my_posts_view** Класс, представляющий окно просмотра всех постов текущего пользователя
- **moderator_profile** Класс, представляющий окно просмотра текущего профиля модератора.
- **editProfile** Класс, представляющий окно редактуры информации профиля
- **create_Mypost**Класс, представляющий окно просмотра создания поста и информации о нем.
- **check_posts**Класс, представляющий окно просмотра полльзовательских постов и их редактуры, удаления.

## Используемые технологии

- **C++:** Основной язык программирования.
- **Qt:** Фреймворк для создания графического интерфейса и работы с базой данных.
- **PostgreSQL:** Реляционная база данных для хранения пользователей, постов, подписок и лайков.
