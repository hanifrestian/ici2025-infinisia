<!DOCTYPE html>
<html>
<head>
  <title>Customer Portal</title>
  <style>
    body { font-family: Arial, sans-serif; text-align: center; padding-top: 5vh; }
    h1 { font-size: 2rem; color: #333; margin: 20px; }
  </style>
</head>
<body>
  <div id="welcome">
    <h1 id="name-display">Welcome!</h1>
  </div>

  <script>
    // Parse URL parameter
    const urlParams = new URLSearchParams(window.location.search);
    const name = urlParams.get('name');

    // Update display with name
    document.getElementById('name-display').innerHTML = 
      name ? `Welcome, ${name}!` : 'Welcome!';
  </script>
</body>
</html>
