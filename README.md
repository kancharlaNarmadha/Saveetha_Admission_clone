# Saveetha_Admission_clone
## Date:

## Objective:
To design a landing page clone of Saveetha Engineering College’s Admission Enquiry form using HTML and CSS. This activity reinforces skills in layout design, form creation, user input handling, responsive structure, and visual styling based on a real-world example.

## Tasks:
#### 1. Analyze the Landing Page Layout:
Observe the split-screen layout with a promotional section on the left and a form on the right.

Note the use of background images, text styling, and branding elements.

#### 2. Create the HTML Structure:
Use semantic tags like ```<section>, <header>, <form>, and <footer>``` to organize content.

Structure the form with input fields such as name, email, phone, password, city, state, course, specialization, captcha, and checkbox.

#### 3. Add Form Functionality:
Include appropriate input types (text, email, tel, password, select, etc.) with placeholders and labels.

Use the <button> element for the "APPLY NOW" action.

#### 4. Apply CSS Styling:
Implement a split layout using flexbox or grid.

Style the form elements with padding, shadows, background colors, and rounded borders.

Include hover effects and button transitions to match the original look.

#### 5. Incorporate Images and Branding:
Add the institution logo and use matching fonts and colors.

Place a background image or blurred overlay behind the form content if needed.

#### 6. Ensure Responsiveness:
Make sure the page adapts to different screen sizes using media queries.

Maintain readability and layout integrity on both desktop and mobile.

## HTML Code:
```
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Saveetha Admission Enquiry</title>
  <link rel="stylesheet" href="style.css" />
</head>
<body>
  <div class="main-container">
    <div class="left-content">
      <img src="flexy.png" alt="Logo" class="logo" />
      <p class="tnea">TNEA CODE    <strong>1216</strong></p>
      <h2>INDUSTRY 5.0</h2>
      <p>Ready Curriculum Imparting<br><strong>21st Century Skills</strong></p>
      <button class="yellow-btn">Apply Now <span>▼</span></button>
    </div>

    <div class="right-form">
      <form class="form-box">
        <h3>Admissions Open 2025</h3>

        <input type="text" placeholder=" Enter Name *" required />
        <input type="email" placeholder=" Enter Email Address *" required />
        <input type="tel" placeholder=" Enter Mobile Number *" required />
        <input type="password" placeholder=" Any Password of Your Choice *" required />

        <div class="double-input">
          <input type="text" placeholder=" State *" required />
          <input type="text" placeholder="City *" required />
        </div>

        <div class="double-input">
          <input type="text" placeholder=" Course *" required />
          <input type="text" placeholder=" Specialization *" required />
        </div>

        <div class="captcha">
          <img src="cap.jpg" alt="captcha" />
          <input type="text" placeholder="Enter text as shown" required />
        </div>

        <div class="checkbox-area">
          <input type="checkbox" required />
          <span>I authorise Saveetha Engineering College to contact me via Email/SMS/Call.</span>
        </div>

        <button class="apply-btn">APPLY NOW ▶</button>

        <p class="login-text">Already have an Account? <a href="#">Login</a><br><a href="#">Resend Verification Email</a></p>
      </form>
    </div>
  </div>
</body>
</html>

```

## CSS Code:
```
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
  font-family: 'Segoe UI', sans-serif;
}

body {
  background-image: url('zoo.png');
  background-size: cover;
  background-position: center;
  background-repeat: no-repeat;
  min-height: 10vh;
  color: white;
}

.main-container {
  display: flex;
  width: 100%;
  min-height: 100vh;
  backdrop-filter: (2px);
  background-color: rgba(0, 0, 0, 0.3);
}

.left-content {
  flex: 1;
  padding: 60px 40px;
  display: flex;
  flex-direction: column;
  justify-content: center;
}

.logo {
  width: 100px;
  margin-bottom: 20px;
}

.tnea {
  font-size: 18px;
  background: #fff;
  color: #000;
  padding: 6px 10px;
  border-radius: 4px;
  display: inline-block;
  margin-bottom: 20px;
}

.left-content h2 {
  font-size: 36px;
  color: #ffea00;
  margin-bottom: 10px;
}

.left-content p {
  font-size: 18px;
  line-height: 1.5;
}

.left-content .yellow-btn {
  margin-top: 40px;
  background: #ffea00;
  color: black;
  border: none;
  padding: 12px 24px;
  font-size: 16px;
  border-radius: 6px;
  cursor: pointer;
}

.right-form {
  flex: 1;
  display: flex;
  justify-content: center;
  align-items: center;
}

.form-box {
  background: rgba(0,0,0,0.3);
  padding: 30px;
  width: 90%;
  max-width: 400px;
  border-radius: 10px;
}

.form-box h3 {
  text-align: center;
  margin-bottom: 20px;
  font-size: 22px;
}

.form-box input[type="text"],
.form-box input[type="email"],
.form-box input[type="tel"],
.form-box input[type="password"] {
  width: 100%;
  padding: 10px;
  margin-top: 10px;
  border-radius: 6px;
  border: none;
  font-size: 14px;
}

.double-input {
  display: flex;
  gap: 10px;
  margin-top: 10px;
}

.double-input input {
  flex: 1;
}

.captcha {
  display: flex;
  gap: 10px;
  margin-top: 10px;
  align-items: center;
}

.captcha img {
  height: 40px;
  border-radius: 4px;
}

.checkbox-area {
  display: flex;
  align-items: flex-start;
  gap: 10px;
  margin-top: 10px;
  font-size: 12px;
}

.apply-btn {
  width: 100%;
  margin-top: 20px;
  padding: 12px;
  background-color: #f5c518;
  color: black;
  font-size: 16px;
  font-weight: bold;
  border: none;
  border-radius: 6px;
  cursor: pointer;
}

.login-text {
  text-align: center;
  font-size: 13px;
  margin-top: 20px;
  color: #ccc;
}

.login-text a {
  color: #ffd700;
  text-decoration: none;
}

```


## Output:
![image](https://github.com/user-attachments/assets/d55ffe62-ae40-475c-a94b-4bbee182233a)


## Result:
A landing page clone of Saveetha Engineering College’s Admission Enquiry form using HTML and CSS is designed successfully.
