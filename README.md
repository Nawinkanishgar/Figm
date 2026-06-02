# Ex09 Event Registration Web Application
## AIM:
To design, develop and deploy a web application for event registration.

## DESIGN STEPS:

### Step 1:
Create a new frame.

### Step 2:
Select any one preset size of your choice.

### Step 3:
Select the shapes you need.

### Step 4:
Import images as needed.

### Step 5:
Create pages based on your need and link them.

### Step 6:

Validate the HTML and CSS code.

### Step 6:

Publish the website in the given URL.

## DESIGN TOOL:
Figma

## CODE:

### figma.html
```html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Event Registration</title>

  <link href="https://fonts.googleapis.com/css2?family=Inter:wght@400;600&display=swap" rel="stylesheet">
  <link rel="stylesheet" href="style.css">
</head>

<body>

<!-- RADIO CONTROLS -->
<input type="radio" name="screen" id="home" checked>
<input type="radio" name="screen" id="events">
<input type="radio" name="screen" id="form">
<input type="radio" name="screen" id="success">

<div class="app">

  <!-- SCREEN 1 -->
  <div class="screen home">
    <h2>🎉 College Events</h2>
    <p>Register before seats fill up!</p>

    <label for="events" class="btn">Login</label>
    <label for="events" class="btn secondary">Register</label>
  </div>

  <!-- SCREEN 2 -->
  <div class="screen events">
    <h2>Events Available</h2>

    <label for="form" class="list-btn">Cricket</label>
    <label for="form" class="list-btn">Basketball</label>
    <label for="form" class="list-btn">Volleyball</label>
    <label for="form" class="list-btn">Badminton</label>
    <label for="form" class="list-btn">100M Race</label>
    <label for="form" class="list-btn">200M Race</label>
  </div>

  <!-- SCREEN 3 -->
  <div class="screen form">
    <h2>Register</h2>

    <input type="text" placeholder="Full Name">
    <input type="text" placeholder="Register Number">

    <div class="row">
      <input type="number" placeholder="Age">
      <input type="text" placeholder="Gender">
    </div>

    <input type="text" placeholder="Phone Number">
    <input type="email" placeholder="Email ID">

    <label for="success" class="btn">Submit</label>
  </div>

  <!-- SCREEN 4 -->
  <div class="screen success">
    <h2>✅ Success!</h2>
    <p>Registration Completed 🎉</p>

    <label for="home" class="btn">Go Home</label>
  </div>

</div>

</body>
</html>
```
### style.css 
```css
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
  font-family: 'Inter', sans-serif;
}

body {
  height: 100vh;
  display: flex;
  justify-content: center;
  align-items: center;
  background: url('https://images.unsplash.com/photo-1501281668745-f7f57925c3b4') no-repeat center/cover;
}

/* HIDE RADIO */
input[type="radio"] {
  display: none;
}

/* APP CONTAINER */
.app {
  width: 320px;
  height: 600px;
  background: rgba(0,0,0,0.65);
  backdrop-filter: blur(8px);
  border-radius: 20px;
  padding: 20px;
  color: white;
  position: relative;
}

/* SCREENS */
.screen {
  display: none;
  text-align: center;
}

/* SHOW BASED ON RADIO */
#home:checked ~ .app .home { display: block; }
#events:checked ~ .app .events { display: block; }
#form:checked ~ .app .form { display: block; }
#success:checked ~ .app .success { display: block; }

/* TEXT */
h2 {
  margin-bottom: 15px;
}

/* BUTTON */
.btn {
  display: block;
  margin: 10px 0;
  padding: 12px;
  background: #ff7a5c;
  border-radius: 8px;
  cursor: pointer;
}

.secondary {
  background: #555;
}

/* EVENT LIST */
.list-btn {
  display: block;
  margin: 8px 0;
  padding: 10px;
  background: white;
  color: black;
  border-radius: 6px;
  cursor: pointer;
}

/* FORM */
input {
  width: 100%;
  padding: 10px;
  margin: 6px 0;
  border-radius: 6px;
  border: none;
}

.row {
  display: flex;
  gap: 10px;
}

.row input {
  width: 50%;
}
```

## OUTPUT:
<img width="1919" height="951" alt="image" src="https://github.com/user-attachments/assets/ce92f7e9-4b94-4160-ba19-7f186cff8d19" />
<img width="1919" height="956" alt="image" src="https://github.com/user-attachments/assets/c7386881-7d61-4281-bfd0-252635f8f909" />
<img width="1919" height="956" alt="image" src="https://github.com/user-attachments/assets/ea120695-cc80-4cb7-aa0f-735c35dfffdb" />
<img width="1919" height="940" alt="image" src="https://github.com/user-attachments/assets/e1f5c863-8abc-42c3-a595-b0c19b169ec6" />


## RESULT:
The program to design, develop and deploy a web application for event registration is completed successfully.
