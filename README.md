
# 📚 Book Hub – Book Management App (Angular + Spring Boot + JWT)

Book Hub is a full-stack Book Management System built using Angular(frontend) and Spring Boot (backend) with JWT authentication. It allows users to login, register, and manage a list of books (CRUD operations).
Project PPT:https://docs.google.com/presentation/d/1R_9Wm3Bts3WAn1ZuXCjyZ4euz-G0PRtX/edit?usp=sharing&ouid=114043774088667102663&rtpof=true&sd=true
---

## 🌐 Live Demo
> Run locally with the steps below and explore:  
> Frontend: `http://localhost:4200`  
> Backend + Swagger: `http://localhost:8081/swagger-ui/index.html`

---

## 🧑‍💼 Features

### 🔐 Auth
- ✅ User **Login** & **Registration**
- ✅ JWT-based secure authentication
- ✅ AuthGuard-protected routes

### 📚 Book Management
- ➕ Add Book  
- ✏️ Edit Book  
- 🗑 Delete Book  
- 📖 View Book List  
- 📊 Dashboard with stats (total books, authors, recent books)

---

## 💻 Tech Stack

### Frontend – Angular
- Angular 16+
- Angular Routing
- Bootstrap 5
- HTTP Interceptor for JWT
- Forms & Form Validation

### Backend – Spring Boot
- Spring Boot 3
- Spring Security with JWT
- Spring Data JPA + Hibernate
- REST APIs with Swagger
- MySQL Database

---

## 🗂 Folder Structure

### 🚀 Backend (Spring Boot)
```

src/main/java/com/example/bookapi
├── controller         # Auth + Book API Controllers
├── entity             # User & Book entities
├── service            # Business logic
├── security           # JWT Auth + Config
├── config             # Swagger + CORS
├── repository         # JPA Repositories
├── exception          # Error handling
├── dto                # Request/Response DTOs

```

### 💻 Frontend (Angular)
```

src/app
├── add-book/          # AddBookComponent
├── edit-book/         # EditBookComponent
├── book-list/         # BookListComponent
├── dashboard/         # Dashboard stats
├── login/             # LoginComponent
├── register/          # RegisterComponent
├── navbar/            # NavbarComponent
├── auth-guard.ts      # Route protection
├── book.service.ts    # Service for Book APIs
├── app.routes.ts      # All app routes

````

---

## 🔧 Getting Started

### 🛠 Backend Setup
1. Clone the backend:
   ```bash
   git clone https://github.com/SanchitaDevkar/Backend-BookHub.git
   cd Backend-BookHub
````

2. Configure MySQL in `application.properties`:

   ```
   spring.datasource.url=jdbc:mysql://localhost:3306/bookhub
   spring.datasource.username=root
   spring.datasource.password=yourpassword
   ```

3. Run the backend server:

   ```bash
   mvn spring-boot:run
   ```

4. Open Swagger UI to test:

   ```
   http://localhost:8081/swagger-ui/index.html
   ```

---

### 💻 Frontend Setup

1. Clone the frontend:

   ```bash
   git clone https://github.com/SanchitaDevkar/Frontend-Coding-Challenge.git
   cd Frontend-Coding-Challenge
   ```

2. Install dependencies:

   ```bash
   npm install
   ```

3. Start the Angular app:

   ```bash
   ng serve
   ```

4. Open in browser:

   ```
   http://localhost:4200
   ```

---

## 🔐 JWT Auth Flow

1. User registers or logs in.
2. Backend returns JWT token.
3. Token is stored in browser `localStorage`.
4. All book-related requests are authenticated using the token.
5. Unauthorized users are redirected to `/login` via `AuthGuard`.

---

## 📊 Sample Dashboard Stats

* **Total Books**: 15
* **Recent Books**: "Clean Code", "Atomic Habits", "Angular for Beginners"
* **Top Authors**: Sanchita, Robert C. Martin

---

## 🧪 API Testing (via Swagger)

🔗 `http://localhost:8081/swagger-ui/index.html`

Available APIs:

* `/api/auth/register`
* `/api/auth/login`
* `/api/books` (GET, POST, PUT, DELETE)

---

## 👩‍💻 Author

Sanchita Devkar
💼 Full Stack Developer   

