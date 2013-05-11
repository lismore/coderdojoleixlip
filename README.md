coderdojoleixlip
================
<html>

<head>

<?php

//capture email address sent from html email form

$email = $_POST['email'];

//capture name sent from html email form

$name = $_POST['name'];

//Capture message sent from html email form

$message = $_POST['message'];

//setup mail and send

$to      = $email;

$subject = 'Email Demo';

$message = $message;

$headers = 'From: dojo@coderdojoleixlip.com' . "\r\n" .

    'Reply-To: dojo@coderdojoleixlip.com' . "\r\n" .

    'X-Mailer: PHP/' . phpversion();

mail($to, $subject, $message, $headers);



echo "Thanks for using our email form!";

?>

</head>

<body>

  <form>

		<input type='text' placeholder='Email' id='email' name='email'>

		<br/>

		<input type='text' placeholder='name' id='name' name='name'>

		<br/>

		<input type='text' placeholder='message' id='message' name='message'>

		<br/>

		<input type='button' id='submit'>

	</form>

</body>

</html>


coderdojoleixlip
