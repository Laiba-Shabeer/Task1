# 📚 Bookstore API (Laravel)

## Project Overview
This project is a RESTful API built with Laravel that allows CRUD operations on books.  
You can create, read, update, and delete books with properties like title, author, price, ISBN, and published date.

---

## Technologies Used
- PHP 8.x  
- Laravel Framework 10+  
- MySQL Database  
- Composer  
- Postman (for API testing)

---

## How to Run Locally

1. **Clone the repository:**
   ```bash
   git clone https://github.com/Laiba-Shabeer/Task1.git
   cd bookstore-api
2. **Install Dependencies:**
   composer install

3. **Edit .env and update DB settings:**
   DB_DATABASE=bookstore
   DB_USERNAME=root
   DB_PASSWORD=your_password

4. **Generate app key:**
   php artisan key:generate

5. **Run migrations:**
    php artisan migrate

6. **Start the development server:**
    php artisan serve

7. **Open your browser and visit:**
    http://127.0.0.1:8000



## API Endpoints


    | Method | Endpoint          | Description       | Sample JSON Input (POST/PUT)                                                                                               |
| ------ | ----------------- | ----------------- | -------------------------------------------------------------------------------------------------------------------------- |
| POST   | `/api/books`      | Create a new book | `{ "title": "Atomic Habits", "author": "James Clear", "price": 20, "isbn": "1234567890", "published_date": "2018-10-16" }` |
| GET    | `/api/books`      | Get all books     | N/A                                                                                                                        |
| GET    | `/api/books/{id}` | Get a book by ID  | N/A                                                                                                                        |
| PUT    | `/api/books/{id}` | Update a book     | `{ "title": "Updated Title", "price": 25 }`                                                                                |
| DELETE | `/api/books/{id}` | Delete a book     | N/A                                                                                                                        |


## Testing the API with Postman
1.Open Postman.

2.Use the appropriate HTTP method and URL, e.g., POST http://127.0.0.1:8000/api/books.

3.For POST and PUT requests:

4.Select Body > raw > JSON.

5.Paste the JSON sample shown above.

6.Click Send to test the request.

7.Review the JSON response.


