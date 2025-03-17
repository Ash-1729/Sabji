# Flask E-Commerce Grocery Store

## Overview
This is a web-based **E-Commerce Grocery Store** built using **Flask** and **MySQL**. Users can register, log in, and shop for groceries, while admins manage products, orders, and offers.

## Features
- **User Authentication**: Register and log in as Customer, Seller, or Admin.
- **Product Management**: Admins can add and manage products.
- **Shopping Cart**: Users can add items to their cart and place orders.
- **Order Processing**: Admins and users can track orders.
- **Discount System**: Admins can create promotional offers.
- **Delivery Assignment**: Orders are assigned to delivery personnel.

## Installation
### Prerequisites
- Python (3.x)
- MySQL Database

### Steps
1. **Clone the Repository**
   ```bash
   git clone https://github.com/your-repo/ecommerce-grocery-store.git
   cd ecommerce-grocery-store
   ```
2. **Create Virtual Environment & Install Dependencies**
   ```bash
   python -m venv venv
   source venv/bin/activate  # macOS/Linux
   venv\Scripts\activate   # Windows
   pip install -r requirements.txt
   ```
3. **Setup Database**
   - Configure `database_config.yaml` with MySQL credentials.
   - Create a MySQL database and import `Dump.sql`.
4. **Run the Application**
   ```bash
   python web_project_fix.py
   ```
   Access at: **http://127.0.0.1:5000/**

## Key Routes
- `/` - Homepage
- `/UserLogin` - User login
- `/customerRegister` - Register as a customer
- `/admin/<admin_id>` - Admin panel
- `/adminProduct/<admin_id>` - Manage products
- `/order/<user_id>` - Checkout
- `/placeOrder/<user_id>` - Confirm order

## File Structure
```
ECommerce-Grocery-Store/
│── templates/  # HTML files
│── static/  # CSS & JS
│── market/  # App logic
│── web_project_fix.py  # Main entry
│── database_config.yaml  # DB settings
│── requirements.txt  # Dependencies
│── Dump.sql  # Database schema
```

## License
This project is open-source under the **MIT License**. Feel free to contribute!

🚀 Happy Coding!

