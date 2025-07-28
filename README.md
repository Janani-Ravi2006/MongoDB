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

## 🗃️ Creating Collection & Document

To insert a single document into a collection. If the collection does not exist, MongoDB will create it automatically.

### 🔹 Syntax
```js
db.collectionName.insertOne({ document })

#Example
db.products.insertOne({name:'Iphone 15',price:80000})

### 💡 Scrollable Insert Command

```js
db.products.insertOne({name: 'Lenovo Legion', price: 120000, brand: 'Lenovo', productType: 'Laptop', specification: {ram: '16 GB', processor: 'i7 13th Gen', storageType: 'SSD', storageSize: '1 TB'}})



