
---

## 📝 2. `retrieve.md`
**Goal:** Retrieve and display the book's attributes.

**Content for `retrieve.md`:**
```markdown
# Retrieve Operation

```python
from LibraryProject.bookshelf.models import Book
book = Book.objects.get(title="1984")
book.title
book.author
book.publication_year
