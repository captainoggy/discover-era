# API Endpoints

## HTML API

### Root

- `GET /` - loads React web app

## JSON API

### Users

- `POST /api/users`
- `PATCH /api/users`

### Session

- `POST /api/session`
- `DELETE /api/session`
- `GET /api/session`

### Books

- `GET /api/books`
  - books index/search
  - accepts tags (if I get there)
- `GET /api/books/:book_id`

### Bookshelf

- `GET /api/bookshelf`
- `POST /api/bookshelf`
- `PATCH /api/bookshelf/:bookshelf_id`
- `DELETE /api/bookshelf/:bookshelf_id`
- `GET /api/bookshelf/:bookshelf_id/books`
  - index of all books for a shelf

### Author

- `GET /api/author/:author_id`

### Reviews

- `GET /api/books/:book_id/reviews`
  - index of all reviews for given book
- `POST /api/books/:book_id/reviews/new`
- `PATCH /api/books/:book_id/reviews/edit`
- `DELETE /api/books/:book_id/reviews/:review_id`

### Tags

- A book's tags will be included in the book show template
- `GET /api/tags`
  - includes query param for typeahead suggestions
- `POST /api/books/:book_id/tags`: add tag to book by name
- `DELETE /api/books/:book_id/tags/:tag_name`: remove tag from book by
  name
