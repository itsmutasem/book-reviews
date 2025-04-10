# 📚 Book Review App

A Laravel-based web application that allows users to browse books, leave star-rated reviews, and filter listings by popularity and average rating. This project demonstrates advanced Eloquent querying, caching strategies, and clean Laravel architecture.

Tech Stack:
- Framework: Laravel
- Frontend: Blade + Tailwind CSS
- Caching: Laravel Cache
- Database: SQLite
- Components: Custom Blade components (Star Rating UI)

Core Features:
✅ Book Listing & Search
- Search books by title
- Filter by:
1- Popular Last Month
2- Popular Last 6 Months
3- Highest Rated Last Month
4- Highest Rated Last 6 Months

✅ Book Details Page
- Shows average rating + number of reviews
- List of latest reviews
- Add your own review (with a star rating)

✅ Review System
- Add a review with form validation
- Star rating from 1 to 5
- Real-time cache invalidation on create/update/delete

✅ Performance Optimizations
- Caching queries by filter + search
- Cache invalidation for books and reviews using model events
- Reusable scopes to avoid code duplication

- What I Gained From This Project:
🔹 Mastered One-to-Many Relationships in Eloquent
 🔹 Built reusable Local Query Scopes for filtering and sorting
 🔹 Used withCount, withAvg, and advanced query techniques
 🔹 Created and used Model Factories & Seeders for data
 🔹 Implemented Query Caching and fine-grained invalidation
 🔹 Leveraged Scoped Resource Controllers for clean routing
 🔹 Built and reused Blade Components for UI consistency

## 📁 Installation

```bash
git clone https://github.com/itsmutasem/book-review-app.git
cd book-review-app
composer install
cp .env.example .env
php artisan key:generate
touch database/database.sqlite
php artisan migrate --seed
php artisan serve
```
Make sure to update your .env file to SQLite
```
DB_CONNECTION=sqlite
DB_DATABASE=book-review
```
