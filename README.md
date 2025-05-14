# Advanced HTML5 Elements and Forms

<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Registration Page</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            line-height: 1.6;
            margin: 20px;
        }
        table {
            width: 100%;
            border-collapse: collapse;
            margin: 20px 0;
        }
        th, td {
            border: 1px solid #ddd;
            padding: 8px;
            text-align: left;
        }
        th {
            background-color: #f2f2f2;
        }
        form {
            max-width: 500px;
            margin: 20px 0;
        }
        .form-group {
            margin-bottom: 15px;
        }
        label {
            display: block;
            margin-bottom: 5px;
            font-weight: bold;
        }
    </style>
</head>
<body>
    <header>
        <h1>Registration Page</h1>
    </header>

    <main>
        <!-- Ordered list with Roman numerals -->
        <section>
            <h2>Steps to Register</h2>
            <ol type="I">
                <li>Fill out the registration form</li>
                <li>Verify your email address</li>
                <li>Complete your profile</li>
                <li>Start using our services</li>
            </ol>
        </section>

        <!-- External image from Pexels -->
        <section>
            <h2>Sample Image</h2>
            <img src="https://images.pexels.com/photos/674010/pexels-photo-674010.jpeg" 
                 alt="Colorful abstract art" 
                 width="500"
                 loading="lazy">
        </section>

        <!-- Contacts table -->
        <section>
            <h2>Contact List</h2>
            <table>
                <thead>
                    <tr>
                        <th>Name</th>
                        <th>Address</th>
                        <th>Mobile</th>
                        <th>Email</th>
                    </tr>
                </thead>
                <tbody>
                    <tr>
                        <td>John Doe</td>
                        <td>123 Main St, Anytown</td>
                        <td>555-0101</td>
                        <td>john@example.com</td>
                    </tr>
                    <tr>
                        <td>Jane Smith</td>
                        <td>456 Oak Ave, Somewhere</td>
                        <td>555-0202</td>
                        <td>jane@example.com</td>
                    </tr>
                    <tr>
                        <td>Bob Johnson</td>
                        <td>789 Pine Rd, Nowhere</td>
                        <td>555-0303</td>
                        <td>bob@example.com</td>
                    </tr>
                    <tr>
                        <td>Alice Brown</td>
                        <td>321 Elm Blvd, Anywhere</td>
                        <td>555-0404</td>
                        <td>alice@example.com</td>
                    </tr>
                    <tr>
                        <td>Charlie Davis</td>
                        <td>654 Maple Ln, Everywhere</td>
                        <td>555-0505</td>
                        <td>charlie@example.com</td>
                    </tr>
                </tbody>
            </table>
        </section>

        <!-- Registration form -->
        <section>
            <h2>Registration Form</h2>
            <form id="registration-form" action="/submit" method="POST">
                <!-- Text inputs -->
                <div class="form-group">
                    <label for="name">Full Name*</label>
                    <input type="text" id="name" name="name" 
                           placeholder="Enter your full name" 
                           required 
                           minlength="3">
                </div>

                <div class="form-group">
                    <label for="email">Email*</label>
                    <input type="email" id="email" name="email" 
                           placeholder="example@domain.com" 
                           required>
                </div>

                <div class="form-group">
                    <label for="password">Password*</label>
                    <input type="password" id="password" name="password" 
                           placeholder="Create a password (min 8 characters)" 
                           required 
                           minlength="8">
                </div>

                <div class="form-group">
                    <label for="dob">Date of Birth*</label>
                    <input type="date" id="dob" name="dob" required>
                </div>

                <!-- Dropdown -->
                <div class="form-group">
                    <label for="country">Country*</label>
                    <select id="country" name="country" required>
                        <option value="" disabled selected>Select your country</option>
                        <option value="us">United States</option>
                        <option value="uk">United Kingdom</option>
                        <option value="ca">Canada</option>
                        <option value="au">Australia</option>
                        <option value="other">Other</option>
                    </select>
                </div>

                <!-- Radio buttons -->
                <div class="form-group">
                    <label>Gender</label>
                    <div>
                        <input type="radio" id="male" name="gender" value="male">
                        <label for="male" style="display: inline; font-weight: normal;">Male</label>
                    </div>
                    <div>
                        <input type="radio" id="female" name="gender" value="female">
                        <label for="female" style="display: inline; font-weight: normal;">Female</label>
                    </div>
                    <div>
                        <input type="radio" id="other" name="gender" value="other">
                        <label for="other" style="display: inline; font-weight: normal;">Other</label>
                    </div>
                </div>

                <!-- Checkboxes -->
                <div class="form-group">
                    <label>Interests (Select all that apply)</label>
                    <div>
                        <input type="checkbox" id="news" name="interests" value="news">
                        <label for="news" style="display: inline; font-weight: normal;">Newsletters</label>
                    </div>
                    <div>
                        <input type="checkbox" id="promo" name="interests" value="promo">
                        <label for="promo" style="display: inline; font-weight: normal;">Promotions</label>
                    </div>
                    <div>
                        <input type="checkbox" id="updates" name="interests" value="updates">
                        <label for="updates" style="display: inline; font-weight: normal;">Product Updates</label>
                    </div>
                </div>

                <!-- Submit button -->
                <div class="form-group">
                    <button type="submit">Register</button>
                </div>
            </form>
        </section>
    </main>

    <footer>
        <p>&copy; 2023 Registration Page. All rights reserved.</p>
    </footer>
</body>
</html>
