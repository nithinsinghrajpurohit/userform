[form.html](https://github.com/user-attachments/files/23395262/form.html)
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>User Details Form</title>
  <style>
    body {
      font-family: Arial, sans-serif;
      background: #f0f4f8;
      padding: 20px;
    }
    form {
      background: white;
      padding: 20px;
      border-radius: 8px;
      max-width: 500px;
      margin: auto;
      box-shadow: 0 0 10px rgba(0,0,0,0.1);
    }
    label {
      display: block;
      margin-top: 15px;
      font-weight: bold;
    }
    input, select {
      width: 100%;
      padding: 8px;
      margin-top: 5px;
      border-radius: 4px;
      border: 1px solid #ccc;
    }
    input[type="submit"] {
      background-color: #007bff;
      color: white;
      border: none;
      margin-top: 20px;
      cursor: pointer;
    }
    input[type="submit"]:hover {
      background-color: #0056b3;
    }
  </style>
</head>
<body>

  <form action="send_email.php" method="POST" enctype="multipart/form-data">
    <h2>Fill Your Details</h2>

    <label for="name">Name:</label>
    <input type="text" id="name" name="name" required>

    <label for="age">Age:</label>
    <input type="number" id="age" name="age" required>

    <label for="language">Language:</label>
<select id="language" name="language" required>
  <option value="">--Select Language--</option>
  <option value="Hindi">Hindi</option>
  <option value="Telugu">Telugu</option>
  <option value="English">English</option>
</select>

    <label for="college">College Name:</label>
    <input type="text" id="college" name="college" required>

    <label for="image">Select Image:</label>
    <input type="file" id="image" name="image" accept="image/*" required>

    <input type="submit" value="Submit">
  </form>

</body>
</html>
