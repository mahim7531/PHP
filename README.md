# 🐘 PHP Complete Guide (A–Z README)

## 🛠️ Requirements

* XAMPP / WAMP / LAMP
* PHP (latest version)
* Web Browser (Chrome)
* MySQL Database

---

## 📂 Project Structure

```
project/
│── index.php
│── config.php
│── insert.php
│── view.php
│── update.php
│── delete.php
│── style.css
```

---

## 🔤 PHP Basics (A–Z Topics)

### 🔹 A - Array

```php
<?php
$names = array("Rahim", "Karim", "Jamal");
print_r($names);
?>
```

---

### 🔹 B - Boolean

```php
<?php
$isActive = true;
?>
```

---

### 🔹 C - Conditional Statement

```php
<?php
$age = 18;
if($age >= 18){
    echo "Adult";
}else{
    echo "Minor";
}
?>
```

---

### 🔹 D - Database Connection

```php
<?php
$conn = mysqli_connect("localhost", "root", "", "student_db");
if(!$conn){
    die("Connection Failed");
}
?>
```

---

### 🔹 E - Echo

```php
<?php
echo "Hello PHP";
?>
```

---

### 🔹 F - Function

```php
<?php
function add($a, $b){
    return $a + $b;
}
echo add(2,3);
?>
```

---

### 🔹 G - GET Method

```php
<?php
$name = $_GET['name'];
echo $name;
?>
```

---

### 🔹 H - HTML with PHP

```php
<h1><?php echo "Welcome"; ?></h1>
```

---

### 🔹 I - Include File

```php
<?php include 'config.php'; ?>
```

---

### 🔹 J - JSON

```php
<?php
$data = array("name"=>"Rahim");
echo json_encode($data);
?>
```

---

### 🔹 K - Key-Value Array

```php
<?php
$student = ["name"=>"Rahim","age"=>20];
echo $student["name"];
?>
```

---

### 🔹 L - Loop

```php
<?php
for($i=1;$i<=5;$i++){
    echo $i;
}
?>
```

---

### 🔹 M - MySQL Insert

```php
<?php
mysqli_query($conn, "INSERT INTO students(name) VALUES('Rahim')");
?>
```

---

### 🔹 N - NULL

```php
<?php
$x = NULL;
?>
```

---

### 🔹 O - Object

```php
<?php
class Student{
    public $name;
}
?>
```

---

### 🔹 P - POST Method

```php
<?php
$name = $_POST['name'];
?>
```

---

### 🔹 Q - Query

```php
<?php
$result = mysqli_query($conn, "SELECT * FROM students");
?>
```

---

### 🔹 R - Return

```php
<?php
function test(){
    return "Hello";
}
?>
```

---

### 🔹 S - Session

```php
<?php
session_start();
$_SESSION['user'] = "admin";
?>
```

---

### 🔹 T - Trim

```php
<?php
$str = " Hello ";
echo trim($str);
?>
```

---

### 🔹 U - Update Query

```php
<?php
mysqli_query($conn, "UPDATE students SET name='Karim' WHERE id=1");
?>
```

---

### 🔹 V - Variable

```php
<?php
$name = "Mahim";
?>
```

---

### 🔹 W - While Loop

```php
<?php
$i=1;
while($i<=3){
    echo $i;
    $i++;
}
?>
```

---

### 🔹 X - XML (Simple)

```php
<?php
$xml = simplexml_load_string("<name>Rahim</name>");
echo $xml;
?>
```

---

### 🔹 Y - Year (Date)

```php
<?php
echo date("Y");
?>
```

---

### 🔹 Z - Zip File (Basic)

```php
<?php
$zip = new ZipArchive();
?>
```

---

## 🚀 Features

* CRUD Operation (Create, Read, Update, Delete)
* Form Handling
* Database Integration
* Session Management

---

# 💼 PHP & MySQL Interview Questions and Answers

## 📌 Introduction

This document contains important PHP and MySQL interview questions with simple and clear answers for beginners to intermediate learners.

---

## 🔹 Basic Questions

### ❓ What is PHP?

👉 PHP (Hypertext Preprocessor) is a server-side scripting language used to develop dynamic web applications.

---

### ❓ What is MySQL?

👉 MySQL is a relational database management system (RDBMS) used to store and manage data.

---

### ❓ What is the difference between GET and POST?

👉 GET sends data through the URL and is less secure.
👉 POST sends data in the request body and is more secure and suitable for large data.

---

### ❓ What is a variable in PHP?

👉 A variable is used to store data. Example: `$name = "John";`

---

### ❓ What is echo?

👉 `echo` is used to display output in PHP.

---

## 🔹 Intermediate Questions

### ❓ What is a session in PHP?

👉 A session is used to store user data on the server (commonly used in login systems).

---

### ❓ What is a cookie?

👉 A cookie stores small pieces of data on the user's browser.

---

### ❓ What is SQL?

👉 SQL (Structured Query Language) is used to manage and manipulate databases.

---

### ❓ What is a primary key?

👉 A primary key is a unique identifier for each record in a table.

---

### ❓ What is JOIN in MySQL?

👉 JOIN is used to combine data from multiple tables based on a related column.

---

## 🔹 Advanced Questions

### ❓ What is the difference between include and require in PHP?

👉 `include` shows a warning if the file is missing and continues execution.
👉 `require` shows a fatal error and stops execution.

---

### ❓ What is prepared statement?

👉 Prepared statements are used to execute SQL queries securely and prevent SQL injection.

---

### ❓ What is MVC?

👉 MVC (Model-View-Controller) is a design pattern used to separate application logic.

---

### ❓ What is normalization?

👉 Normalization is the process of organizing data in a database to reduce redundancy.

---

### ❓ What is indexing in MySQL?

👉 Indexing improves the speed of data retrieval in a database.

---
