# testdomain
<?php
if ($_SERVER["REQUEST_METHOD"] == "POST") {
    // Retrieve the values submitted in the login form
    $username = $_POST["username"];
    $password = $_POST["password"];

    // Replace this with your actual authentication logic
    $validUsername = "Amir";
    $validPassword = "Capo";

    // Check if the submitted credentials are valid
    if ($username == $validUsername && $password == $validPassword) {
        // Authentication successful
        echo "Login Successful!";
    } else {
        // Authentication failed
        echo "Wrong Username or Password";
    }
} else {
    // Redirect to the login page if accessed directly without a POST request
    header("Location: Fakedomain.html");
    exit();
}
?>
