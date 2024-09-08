<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Password Protected Video Links</title>
    <script>
        function checkPassword() {
            const correctPassword = "132141319"; // ใส่รหัสผ่านที่ถูกต้องที่นี่
            const passwordInput = document.getElementById("password").value;
            const messageElement = document.getElementById("message");

            if (passwordInput === correctPassword) {
                messageElement.innerHTML = '<a href="https://youtu.be/0wevMKSS9Tk?si=cHV7J2tQaXAkgHME" target="_blank">ดูวิดีโอ</a'; // แทนที่ correctVideoLink ด้วยลิ้งค์วิดีโอที่ถูกต้อง
            } else {
                messageElement.innerHTML = 'มาเสือกใช่มั้ย ลองกดสิ <a href="https://youtu.be/dQw4w9WgXcQ?si=F9nklQzBFiS-tY-o
                " target="_blank">ดูวิดีโอ</a>'; // แทนที่ wrongVideoLink ด้วยลิ้งค์วิดีโอที่ผิด
            }

            // ทำให้ข้อความปรากฏขึ้น
            messageElement.style.display = "block";
        }
    </script>
</head>
<body>
    <h2>ใส่รหัสผ่านเพื่อดูวิดีโอ</h2>
    <input type="password" id="password" placeholder="ใส่รหัสผ่าน">
    <button onclick="checkPassword()">ยืนยัน</button>
    <p id="message" style="display: none;"></p>
</body>
</html>

<!---
Helloworld09557/Helloworld09557 is a ✨ special ✨ repository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take a look at you
