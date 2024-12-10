<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Mahir Khan Pathan - Legal Advisor</title>
    <style>
        body {
            font-family: 'Arial', sans-serif;
            margin: 0;
            padding: 0;
            background-color: #121212;
            color: #f4f4f4;
        }
        header {
            background-color: #1e1e1e;
            color: #fff;
            padding: 30px;
            text-align: center;
            border-bottom: 2px solid #444;
        }
        nav {
            background-color: #333;
            display: flex;
            justify-content: center;
            padding: 10px 0;
        }
        nav button {
            background: none;
            border: none;
            color: #f4f4f4;
            margin: 0 15px;
            font-size: 16px;
            cursor: pointer;
        }
        nav button:hover {
            color: #00bcd4;
        }
        nav button.active {
            color: #00bcd4;
            border-bottom: 2px solid #00bcd4;
        }
        main {
            max-width: 900px;
            margin: 20px auto;
            padding: 20px;
            background-color: #1e1e1e;
            border-radius: 8px;
            box-shadow: 0 0 10px rgba(0, 0, 0, 0.7);
        }
        section {
            display: none;
        }
        section.active {
            display: block;
        }
        h2 {
            color: #00bcd4;
            border-bottom: 2px solid #444;
            padding-bottom: 10px;
        }
        footer {
            background-color: #1e1e1e;
            color: #888;
            text-align: center;
            padding: 15px 0;
            margin-top: 30px;
        }
    </style>
</head>
<body>

<header>
    <h1>Mahir Khan Pathan</h1>
    <p>Legal Advisor</p>
</header>

<nav>
    <button class="tab-btn active" onclick="showTab('profile')">Profile</button>
    <button class="tab-btn" onclick="showTab('education')">Education</button>
    <button class="tab-btn" onclick="showTab('skills')">Skills</button>
    <button class="tab-btn" onclick="showTab('contact')">Contact</button>
</nav>

<main>
    <section id="profile" class="active">
        <h2>Profile</h2>
        <p>Legal advisor with expertise in banking and financial law, mediation, and corporate negotiations. Demonstrates a visionary approach in crafting strategic legal solutions, enhancing client positions, and mitigating risks. Known for exceptional communication skills and innovative methodologies, ensuring client satisfaction.</p>
    </section>

    <section id="education">
        <h2>Education</h2>
        <ul>
            <li><strong>City University of London</strong> - LLM in Banking & Finance Law (Sep 2023 - Sep 2024)</li>
            <li><strong>I.M. Nanavati Law College, Gujarat University</strong> - Bachelor of Law (Sep 2019 - Nov 2021)</li>
            <li><strong>LJ Commerce College, Gujarat University</strong> - Bachelor of Commerce (Dec 2016 - Nov 2018)</li>
        </ul>
    </section>

    <section id="skills">
        <h2>Skills</h2>
        <ul>
            <li>Mediation & Negotiation</li>
            <li>Corporate & Financial Law</li>
            <li>Investment Law</li>
            <li>Communication & Arbitration</li>
            <li>Property negotiations</li>
        </ul>
    </section>

    <section id="contact">
        <h2>Contact</h2>
        <p><strong>Email:</strong> <a href="mailto:Mahirkhan1799@gmail.com">Mahirkhan1799@gmail.com</a></p>
        
        <p><strong>LinkedIn:</strong> <a href="https://www.linkedin.com/in/mahirkhan1799" target="_blank">linkedin.com/in/mahirkhan1799</a></p>
    </section>
</main>

<footer>
    <p>&copy; 2024 Mahir Khan Pathan. All rights reserved.</p>
</footer>

<script>
    function showTab(tabId) {
        // Hide all sections
        document.querySelectorAll('section').forEach(section => {
            section.classList.remove('active');
        });

        // Remove active class from all buttons
        document.querySelectorAll('.tab-btn').forEach(button => {
            button.classList.remove('active');
        });

        // Show the selected tab
        document.getElementById(tabId).classList.add('active');

        // Add active class to the clicked button
        event.currentTarget.classList.add('active');
    }
</script>

</body>
</html>
