
---

## 📝 4. `delete.md`
**Goal:** Delete the book and confirm.

**Content for `delete.md`:**
```markdown
# Delete Operation

```python
from bookshelf.models import Book
book = Book.objects.get(title="Nineteen Eighty-Four")
book.delete()

Book.objects.all()
