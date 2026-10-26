# JPMart - Store Management Android Application

A native Android application built with Java and SQLite to streamline retail store operations, product inventory management, and order processing.

---

## Key Features

- **Authentication & Security:** 
  - Role-based login system separating Administrator and Staff privileges.
  - User password security protected with **BCrypt** hashing.
- **Inventory & Category Management:** 
  - Full CRUD operations for categories and products.
  - Track product quantities, unit prices, and restocking dates.
- **Customer Directory:** 
  - Manage customer profiles, contact information, and purchase references.
- **Order Processing & POS:**
  - Cart management system calculating dynamic order totals.
  - Structured billing history with order headers and line-item details (`HoaDon` & `HoaDonChiTiet`).

---

## Database Architecture (SQLite)

- `NhanVien`: User credentials, roles, and administrative data.
- `KhachHang`: Customer profile and contact directory.
- `DanhMuc`: Product classifications.
- `SanPham`: Product inventory items and pricing references.
- `HoaDon`: Transaction records linked to employees and customers.
- `HoaDonChiTiet`: Line items recording quantity and sold prices at checkout time.

---

## Tech Stack & Architecture

- **Language:** Java
- **Platform:** Android SDK
- **Database:** SQLite (`SQLiteOpenHelper`)
- **Security:** BCrypt Password Hashing
- **Architecture:** MVC / DAO Pattern
