
- **retrieve.md**
```markdown
# Retrieve Operation
```python
book = Book.objects.get(title="1984")
book.title, book.author, book.publication_year
# ('1984', 'George Orwell', 1949)
