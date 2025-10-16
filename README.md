<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1" />
  <title>Simple Navigation</title>
  <style>
    body {
      font-family: Arial, sans-serif;
      max-width: 600px;
      margin: 40px auto;
      padding: 0 20px;
      color: #333;
    }
    nav {
      border-bottom: 2px solid #007BFF;
      padding-bottom: 10px;
      margin-bottom: 30px;
    }
    nav a {
      text-decoration: none;
      color: #007BFF;
      margin-right: 20px;
      font-weight: bold;
      padding: 6px 12px;
      border-radius: 5px;
      transition: background-color 0.3s;
    }
    nav a:hover {
      background-color: #007BFF;
      color: white;
    }
    h1 {
      color: #007BFF;
    }
    section {
      display: none;
    }
    section:target {
      display: block;
    }
    /* Show home by default */
    body:not(:target) section#home {
      display: block;
    }
  </style>
</head>
<body>

  <nav>
    <a href="#home">Home</a>
    <a href="#course">Course</a>
    <a href="#contact">Contact</a>
  </nav>

  <section id="home">
    <h1>Home Page</h1>
    <p>Welcome to the homepage of our simple static site.</p>
  </section>

  <section id="course">
    <h1>Course Page</h1>
    <p>Find all the course information here.</p>
  </section>

  <section id="contact">
    <h1>Contact Us</h1>
    <p>Get in touch with us via email or phone.</p>
  </section>

</body>
</html>

