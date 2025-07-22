# Create Operation

```python
from LibraryProject.bookshelf.models import Book
book = Book.objects.create(title="1984", author="George Orwell", publication_year=1949)
book 
```


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


---

## 📝 4. `delete.md`
**Goal:** Delete the book and confirm.

**Content for `delete.md`:**
```markdown
# Delete Operation

```python
from LibraryProject.bookshelf.models import Book
book = Book.objects.get(title="Nineteen Eighty-Four")
book.delete()

Book.objects.all()
