
---

## 📝 3. `update.md`
**Goal:** Change the title to `"Nineteen Eighty-Four"`.

**Content for `update.md`:**
```markdown
# Update Operation

```python
from LibraryProject.bookshelf.models import Book
book = Book.objects.get(title="1984")
book.title = "Nineteen Eighty-Four"
book.save()
book.title
