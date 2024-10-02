
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Ahmed Dahloop's Profile</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            background-color: #f0f0f0;
            margin: 0;
            padding: 0;
            display: flex;
            justify-content: center;
            align-items: center;
            height: 100vh;
            flex-direction: column;
            animation: fadeIn 2s ease-in-out;
        }

        @keyframes fadeIn {
            from { opacity: 0; }
            to { opacity: 1; }
        }

        h3 {
            color: #3498db;
            text-align: center;
            font-size: 2.5em;
            animation: colorChange 3s infinite;
        }

        @keyframes colorChange {
            0% { color: #3498db; }
            50% { color: #e74c3c; }
            100% { color: #3498db; }
        }

        p {
            color: #2c3e50;
            font-size: 1.2em;
            margin: 20px 0;
            text-align: center;
        }

        .icons {
            display: flex;
            justify-content: center;
            align-items: center;
            gap: 10px;
        }

        .icons a {
            text-decoration: none;
            font-size: 1.5em;
            color: #3498db;
        }

        .icons img {
            width: 40px;
            height: 40px;
            vertical-align: middle;
        }

        .visitor-count {
            font-size: 1.2em;
            color: #16a085;
            margin-top: 20px;
            animation: bounce 2s infinite;
        }

        @keyframes bounce {
            0%, 100% { transform: translateY(0); }
            50% { transform: translateY(-10px); }
        }

        .highlight {
            color: #e74c3c;
            font-weight: bold;
        }
    </style>
</head>
<body>

<h3>Welcome to Ahmed Dahloop's Profile!</h3>

<p>👨‍💻 As a CS student, I'm constantly learning and exploring new technologies to improve my skills.</p>

<!-- Visitor count -->
<p class="visitor-count">👀 Visitors: <span id="visitorCount" class="highlight">0</span></p>

<!-- Icons and links -->
<div class="icons">
    <!-- WhatsApp Link -->
    <a href="https://wa.me/1234567890" target="_blank" title="Contact me on WhatsApp">
        <img src="https://upload.wikimedia.org/wikipedia/commons/6/6b/WhatsApp.svg" alt="WhatsApp">
    </a>
    <!-- Assiut University Icon -->
    <a href="https://www.aun.edu.eg/" target="_blank" title="Assiut University">
        <img src="https://upload.wikimedia.org/wikipedia/commons/4/46/Assiut_university_logo.png" alt="Assiut University">
    </a>
</div>

<!-- JavaScript to increment visitor count -->
<script>
    let visitorCount = localStorage.getItem('visitCount');
    if (!visitorCount) {
        visitorCount = 0;
    }
    visitorCount++;
    localStorage.setItem('visitCount', visitorCount);
    document.getElementById('visitorCount').textContent = visitorCount;
</script>

</body>
</html>





