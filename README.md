# qa_python

## Файлы проекта
- `main.py` - основной код приложения
- `tests.py` - тесты для приложения
- `README.md` - документация проекта

## Описание тестов

### Тесты добавления книг
1. **test_add_new_book_valid_names** — проверяет добавление книг с корректной длиной названия.  
   *Использует параметризацию для разных валидных имён.*
### Тесты жанров
2. **test_set_book_genre_valid_genre** — тестирует установку жанра для существующих книг.  
   *Параметризован для разных пар «книга жанр».*

3. **test_get_book_genre_returns_genre_for_valid_book_with_genre** — проверяет сценарий, когда книга существует и ей присвоен жанр.  

4. **test_get_book_genre_returns_empty_string_for_valid_book_without_genre** — проверяет случай, когда книга существует, но жанр не установлен

5. **test_get_book_genre_returns_none_for_nonexistent_book** — проверяет поведение метода для несуществующей книги

6. **test_get_books_with_specific_genre** — убеждается, что метод возвращает книги заданного жанра.  
   *Параметризован для разных жанров и наборов книг.*

7. **test_get_books_genre_returns_dictionary** — проверяет, что возвращается актуальный словарь books_genre с правильными парами.

8. **test_get_books_for_children_filters_correctly** — тестирует фильтрацию: книги с жанрами из genre_age_rating не попадают в список детских.
### Тесты избранного
9. **test_add_book_in_favorites** — проверяет добавление книги в избранное.  
   *Параметризован для разных книг.*

10. **test_delete_book_from_favorites_removes_book** — убеждается, что книга успешно удаляется из избранного.

11. **test_get_list_of_favorites_books_returns_correct_list** — подтверждает, что метод возвращает актуальный список избранных книг.
