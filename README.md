# 📦 MongoDB Setup Guide

This guide will help you install and configure MongoDB, and walk you through basic NoSQL commands.

---

## ⚙️ How to Configure MongoDB

### Step 1: Install MongoDB Database
Download MongoDB Community Server:  
👉 [MongoDB Community Download](https://www.mongodb.com/try/download/community)

### Step 2: Install MongoDB Shell (mongosh)
Download MongoDB Shell:  
👉 [MongoDB Shell Download](https://www.mongodb.com/try/download/shell)

---

## 🧩 NoSQL Commands

### ✅ Connecting to MongoDB Server

1. Open **Command Prompt (cmd)**.
2. Type `mongosh` and press `Enter`.

---

Show database
#The following command is used to show avaliable database list.

show dbs

Command to connect database
The following command is used to connect with database even if database is not exists it will create new database.
#Syntax
use [database name]
#Example
use maxishop


<details> <summary>📦 Insert an Embedded Document</summary>
js
Copy
Edit
db.products.insertOne({
  name: 'Lenovo Legion',
  price: 120000,
  brand: 'Lenovo',
  productType: 'Laptop',
  specification: {
    ram: '16 GB',
    processor: 'i7 13th Gen',
    storageType: 'SSD',
    storageSize: '1 TB'
  }
});
</details>


db.products.insertOne({name: 'Lenovo Legion', price: 120000, brand: 'Lenovo', productType: 'Laptop', specification: {ram: '16 GB', processor: 'i7 13th Gen', storageType: 'SSD', storageSize: '1 TB'}})



### 💡 Scrollable Insert Command

```js
db.products.insertOne({name: 'Lenovo Legion', price: 120000, brand: 'Lenovo', productType: 'Laptop', specification: {ram: '16 GB', processor: 'i7 13th Gen', storageType: 'SSD', storageSize: '1 TB'}})

