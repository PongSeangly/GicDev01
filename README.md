<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Employee Registration Form</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            background-color: #f4f4f4;
            margin: 0;
            padding: 0;
        }

        .container {
            max-width: 600px;
            margin: 20px auto;
            background: #fff;
            padding: 20px;
            border-radius: 8px;
            box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
        }

        h2 {
            text-align: center;
        }

        form {
            margin-top: 20px;
        }

        label {
            display: block;
            font-weight: bold;
            margin-bottom: 5px;
        }

        input[type="text"],
        input[type="email"],
        input[type="tel"],
        select,
        textarea {
            width: 100%;
            padding: 10px;
            margin-bottom: 10px;
            border: 1px solid #ccc;
            border-radius: 4px;
            box-sizing: border-box;
        }

        input[type="file"] {
            margin-bottom: 10px;
        }

        input[type="submit"],
        input[type="reset"] {
            background-color: #4caf50;
            color: #fff;
            padding: 10px 20px;
            border: none;
            border-radius: 4px;
            cursor: pointer;
        }

        input[type="submit"]:hover,
        input[type="reset"]:hover {
            background-color: #45a049;
        }
    </style>
</head>
<body>
    <div class="container">
        <h2>Employee Registration Form</h2>
        <form action="#" method="post" enctype="multipart/form-data">
          <input type="radio" id="mr" name="title" value="Mr." style="margin-right: 5px;">
          <label for="mr">Mr.</label>
          
          <input type="radio" id="mrs" name="title" value="Mrs." style="margin-right: 5px;">
          <label for="mrs">Mrs.</label>
          
          <input type="radio" id="ms" name="title" value="Ms." style="margin-right: 5px;">
          <label for="ms">Ms.</label>
          

            <label for="fname">First Name:</label>
            <input type="text" id="fname" name="firstname" required>

            <label for="lname">Last Name:</label>
            <input type="text" id="lname" name="lastname" required>

            <label for="address1">Mail Address 1:</label>
            <input type="text" id="address1" name="address1" required>

            <label for="address2">Mail Address 2:</label>
            <input type="text" id="address2" name="address2">

            <label for="city">City:</label>
            <input type="text" id="city" name="city" required>

            <label for="state">State:</label>
            <input type="text" id="state" name="state" required>

            <label for="zip">Zip:</label>
            <input type="text" id="zip" name="zip" required>

            <label for="photo">Upload Photo:</label>
            <input type="file" id="photo" name="photo" accept="image/*">

            <label for="email">E-Mail:</label>
            <input type="email" id="email" name="email" required>

            <label for="mobile">Mobile:</label>
            <input type="tel" id="mobile" name="mobile" pattern="[0-9]{10}" required>

            <label for="language">Language:</label>
            <select id="language" name="language" required>
                <option value="Gujarati">Gujarati</option>
                <option value="Hindi">Hindi</option>
                <option value="English">English</option>
                <option value="Marathi">Marathi</option>
            </select>

            <label for="additional">Additional Information:</label>
            <textarea id="additional" name="additional" rows="4" cols="50"></textarea>

            <!-- Submit and Reset buttons -->
            <input type="submit" value="Submit">
            <input type="reset" value="Reset">
        </form>
    </div>
</body>
</html>
