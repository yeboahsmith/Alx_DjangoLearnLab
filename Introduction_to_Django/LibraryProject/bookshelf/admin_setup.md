# Django Admin Configuration for Book Model

## Admin Registration
In `bookshelf/admin.py`, the `Book` model was registered with a custom `BookAdmin` class:

```python
from django.contrib import admin
from .models import Book

@admin.register(Book)
class BookAdmin(admin.ModelAdmin):
    list_display = ("title", "author", "publication_year")
    list_filter = ("publication_year", "author")
    search_fields = ("title", "author")
