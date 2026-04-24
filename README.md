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

