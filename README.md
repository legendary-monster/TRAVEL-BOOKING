# LOGIN PAGE
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Home</title>
  <link rel="stylesheet" href="styles.css">
  <link rel="stylesheet" href="https://maxcdn.bootstrapcdn.com/bootstrap/4.0.0/css/bootstrap.min.css">
</head>
<body>
  <div class="container">
    <h1>Welcome to the Website</h1>
    <button class="btn btn-primary" data-toggle="modal" data-target="#registerModal">Register</button>
    <button class="btn btn-secondary" data-toggle="modal" data-target="#loginModal">Login</button>
  </div>

  <!-- Register Modal -->
  <div class="modal fade" id="registerModal" tabindex="-1" role="dialog">
    <div class="modal-dialog" role="document">
      <div class="modal-content">
        <div class="modal-header">
          <h5 class="modal-title">Register</h5>
          <button type="button" class="close" data-dismiss="modal">&times;</button>
        </div>
        <div class="modal-body">
          <form id="registerForm" action="register.html">
            <input type="text" name="fullname" placeholder="Full Name" required>
            <input type="text" name="contact" placeholder="Contact" required>
            <input type="date" name="dob" placeholder="Date of Birth" required>
            <input type="email" name="email" placeholder="Email ID" required>
            <input type="password" name="password" placeholder="Password" required>
            <input type="text" name="gender" placeholder="Gender" required>
            <button type="submit" class="btn btn-primary">Register</button>
            <p><a href="#" data-toggle="modal" data-target="#loginModal" data-dismiss="modal">Already have an account? Login</a></p>
          </form>
        </div>
      </div>
    </div>
  </div>

  <!-- Login Modal -->
  <div class="modal fade" id="loginModal" tabindex="-1" role="dialog">
    <div class="modal-dialog" role="document">
      <div class="modal-content">
        <div class="modal-header">
          <h5 class="modal-title">Login</h5>
          <button type="button" class="close" data-dismiss="modal">&times;</button>
        </div>
        <div class="modal-body">
          <form id="loginForm" action="login.html">
            <input type="email" name="email" placeholder="Email ID" required>
            <input type="password" name="password" placeholder="Password" required>
            <button type="submit" class="btn btn-primary">Login</button>
            <p><a href="#" data-toggle="modal" data-target="#registerModal" data-dismiss="modal">Don't have an account? Register</a></p>
          </form>
        </div>
      </div>
    </div>
  </div>

  <script src="https://code.jquery.com/jquery-3.2.1.slim.min.js"></script>
  <script src="https://cdnjs.cloudflare.com/ajax/libs/popper.js/1.11.0/umd/popper.min.js"></script>
  <script src="https://maxcdn.bootstrapcdn.com/bootstrap/4.0.0/js/bootstrap.min.js"></script>
  <script src="scripts.js"></script>
</body>
</html>
