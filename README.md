# -Prevent-blind-SQL-injection-LAB
Preventing blind SQL injection is similar to preventing error-based SQL injection

Go back to File Explorer and open blind-sql.

<img width="689" height="498" alt="image" src="https://github.com/user-attachments/assets/6e32a91e-e1fa-455f-91a9-8b6bd4d9dc67" />

Open process.php to view the code.

$userId = $_POST['userId'];

$sql = "SELECT user_id, user FROM users WHERE user_id = '$userId';";

<img width="696" height="475" alt="image" src="https://github.com/user-attachments/assets/a9782348-a152-4cb3-ba84-f2d073f3b269" />

Close the file. Browse to Updated Files and then open blind-sql.

<img width="693" height="471" alt="image" src="https://github.com/user-attachments/assets/b8837706-3d0d-49cd-a7c7-ed331ab13742" />

The updated process.php file uses a prepared statement to allow different inputs while preventing SQL injection.

<img width="693" height="480" alt="image" src="https://github.com/user-attachments/assets/e4478992-caf0-4ae6-8dff-facc35e1c865" />

Switch back to the blind-SQL page. In the Enter User ID box, enter:

'(apostrophe)

<img width="292" height="81" alt="image" src="https://github.com/user-attachments/assets/c5a5fded-c85d-4c04-ba5c-350ce37929f3" />
