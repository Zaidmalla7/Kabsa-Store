# 🛒 Kabsa Store - E-Commerce & Subscription Platform

![.NET Core](https://img.shields.io/badge/.NET%208-512BD4?style=for-the-badge&logo=dotnet&logoColor=white)
![C#](https://img.shields.io/badge/C%23-239120?style=for-the-badge&logo=c-sharp&logoColor=white)
![Razor](https://img.shields.io/badge/Razor-512BD4?style=for-the-badge&logo=dotnet&logoColor=white)
![SQL Server](https://img.shields.io/badge/SQL%20Server-CC2927?style=for-the-badge&logo=microsoft-sql-server&logoColor=white)
![Bootstrap](https://img.shields.io/badge/Bootstrap%205-7952B3?style=for-the-badge&logo=bootstrap&logoColor=white)

## 📝 About The Project
**Kabsa Store** is a live, production-grade digital subscription and e-commerce platform built with ASP.NET Core MVC. The system provides a seamless user experience for customers purchasing digital products and subscriptions, alongside a highly dynamic, secure, and fully-featured administrative dashboard for content, product, and order management.

🌐 **Live Demo:** [https://www.kabsa.store](https://www.kabsa.store)

---

## 📸 Screenshots

> **Note:** Here is a glimpse of the application's user interface and admin dashboard.

### 🏠 Home Page
<!-- حط رابط صورة الصفحة الرئيسية بين الأقواس تحت بدل كلمة LINK_HERE -->
<img width="1906" height="938" alt="Screenshot 2026-09-16 163846" src="https://github.com/user-attachments/assets/4f753d44-c60b-4492-9141-20cb2b736888" />


### 🛍️ All Products Page (Client Side)
<!-- حط رابط صورة صفحة جميع المنتجات للزبائن بين الأقواس تحت بدل كلمة LINK_HERE -->
<img width="1907" height="938" alt="Screenshot 2026-09-16 164001" src="https://github.com/user-attachments/assets/4d2c0416-2769-4782-abce-41dd94c5fa0f" />

### 📦 Packages Page (Client Side)
<!-- حط رابط صورة صفحة البكجات بين الأقواس تحت بدل كلمة LINK_HERE -->
<img width="1897" height="972" alt="Screenshot 2026-09-16 164056" src="https://github.com/user-attachments/assets/dbbab0b8-0b2e-4ba6-a81f-7156b535b2fd" />

### 🔐 Login Page
<!-- حط رابط صورة صفحة تسجيل الدخول بين الأقواس تحت بدل كلمة LINK_HERE -->
<img width="1919" height="864" alt="Screenshot 2026-09-16 164235" src="https://github.com/user-attachments/assets/2db3057c-f1a6-4002-b456-812589b84d41" />

### 📊 Admin Dashboard
<!-- حط رابط صورة الداشبورد بين الأقواس تحت بدل كلمة LINK_HERE -->
<img width="1903" height="970" alt="Screenshot 2026-09-16 164353" src="https://github.com/user-attachments/assets/4db1938d-4de3-4697-aba7-80f88ad51002" />

### ⚙️ Products Management (Admin Side)
<!-- حط رابط صورة إدارة المنتجات في لوحة التحكم بين الأقواس تحت بدل كلمة LINK_HERE -->
<img width="1900" height="947" alt="Screenshot 2026-09-16 164532" src="https://github.com/user-attachments/assets/98432bb5-1e5e-4888-a75d-a091c6edae1f" />

---

## 🛠️ Tech Stack & Technologies
* **Backend:** C#, .NET 8, ASP.NET Core MVC.
* **Database & ORM:** SQL Server, Entity Framework Core (LINQ, Code-First).
* **Frontend:** Razor, HTML5, CSS3, Bootstrap 5, AJAX, jQuery.
* **Libraries/Plugins:** SweetAlert2, DataTables (with PDF/Excel export), AOS Animations, Swiper.js.
* **SEO & Analytics:** Google Search Console, Google Analytics Integration, Meta Pixel.

---

## ✨ Key Features

### 👨‍💻 Admin Panel (Dashboard)
* **Smart Category & Product Management:** Full CRUD operations with logical constraints (e.g., preventing the deletion of a category if it contains active products).
* **Dynamic Pricing Engine:** Real-time auto-calculation of `FinalPrice` based on base `Price` and `DiscountPercentage`.
* **Asynchronous Operations:** Seamless status toggling (Active/Inactive) and deletion using AJAX without reloading the page.
* **Secure File Uploads:** Integrated `ImageService` for handling, validating, and saving product/category images.
* **Data Export:** Built-in DataTables functionality allowing admins to search, filter, and export data to Excel or PDF.

### 🛍️ Client-Side
* **WhatsApp Checkout Integration:** Smart integration generating fully formatted Unicode messages (with dynamic emojis, prices, and warranties) to finalize orders directly via WhatsApp.
* **Optimized UI/UX:** Responsive design with a dark-mode theme, toast notifications, and interactive modals.
* **Event Tracking:** Integrated Meta Pixel for tracking `InitiateCheckout` events to optimize ad campaigns.

---

## 🧠 Technical Challenges Overcome & What I Learned

During the development and deployment of Kabsa Store, I tackled several real-world engineering challenges:

1. **Image Handling & Production Performance:** Identified and resolved a severe performance issue related to heavy image loads in production. I implemented an image optimization and validation workflow within the `ImageService` to compress files and control formats, significantly reducing load times.
2. **Database Integrity with Transactions:** To prevent partial data saves or data corruption during complex operations (like saving a product with its packages and images), I utilized EF Core Database Transactions (`BeginTransactionAsync`, `CommitAsync`, `RollbackAsync`).
3. **Overcoming ModelState Silent Failures:** Dealt with hidden MVC `ModelState` validation conflicts during dynamic AJAX updates by intelligently clearing unnecessary validations (`ModelState.Clear()`) to ensure smooth database inserts.
4. **Smart Deletion Architecture:** Implemented `DbUpdateException` handling and backend validation checks to protect referential integrity, ensuring admins cannot accidentally delete records tied to existing foreign keys (e.g., Categories with linked Products).

---

## 📬 Contact & Links
* **Developer:** Zaid Yasser Mallah
* **LinkedIn:** [Zaid Mallah](https://www.linkedin.com/in/zaidyasser)
* **Email:** zaidalmallah444@gmail.com
