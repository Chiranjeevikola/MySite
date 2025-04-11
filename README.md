<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Kola Chiranjeevi Personal Site</title>
    <link href="https://fonts.googleapis.com/css2?family=Roboto:wght@300;400;700&display=swap" rel="stylesheet">
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/5.15.4/css/all.min.css">
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        body {
            font-family: 'Roboto', sans-serif;
            line-height: 1.6;
            color: #333;
            background-color: #f4f4f9;
        }

        .container {
            display: flex;
            max-width: 1200px;
            margin: 20px auto;
            background: #fff;
            box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
            border-radius: 8px;
            overflow: hidden;
        }

        .sidebar {
            width: 30%;
            background: #1a3c5e;
            color: #fff;
            padding: 30px;
            overflow-y: auto; /* Allow scrolling if content overflows */
            min-height: 100%; /* Ensure sidebar spans full height */
        }

        .sidebar h1 {
            font-size: 1.8em;
            margin-bottom: 10px;
        }

        .sidebar p {
            font-size: 0.95em;
            margin: 5px 0;
            opacity: 0.9;
        }

        .sidebar .contact-info {
            margin-top: 20px;
            margin-bottom: 20px;
        }

        .sidebar .contact-info p {
            display: flex;
            align-items: center;
        }

        .sidebar .contact-info i {
            margin-right: 10px;
            font-size: 1.2em;
        }

        .sidebar .section {
            margin-bottom: 20px;
        }

        .sidebar .section h2 {
            font-size: 1.3em;
            color: #fff;
            border-bottom: 1px solid rgba(255, 255, 255, 0.3);
            padding-bottom: 5px;
            margin-bottom: 10px;
        }

        .sidebar .section ul {
            list-style-type: disc;
            margin-left: 20px;
        }

        .main-content {
            width: 70%;
            padding: 30px;
        }

        .main-content .section {
            margin-bottom: 30px;
        }

        .main-content .section h2 {
            font-size: 1.5em;
            color: #1a3c5e;
            border-bottom: 2px solid #1a3c5e;
            padding-bottom: 5px;
            margin-bottom: 15px;
        }

        .main-content .section p, .main-content .section li {
            font-size: 1em;
            color: #555;
        }

        .main-content .section ul {
            list-style-type: disc;
            margin-left: 20px;
        }

        .education table {
            width: 100%;
            border-collapse: collapse;
            margin-top: 10px;
        }

        .education th, .education td {
            border: 1px solid #ddd;
            padding: 12px;
            text-align: left;
            font-size: 0.95em;
        }

        .education th {
            background: #1a3c5e;
            color: #fff;
            font-weight: 700;
        }

        .education td {
            background: #f9f9f9;
        }

        .skills-grid {
            display: grid;
            grid-template-columns: repeat(2, 1fr);
            gap: 10px;
        }

        .project-item, .cert-item {
            margin-bottom: 15px;
        }

        .project-item h4, .cert-item h4 {
            font-size: 1.1em;
            color: #1a3c5e;
        }

        .mobile-nav {
            display: none;
            background: #1a3c5e;
            color: #fff;
            padding: 15px;
            font-size: 1.2em;
            cursor: pointer;
            text-align: center;
        }

        @media (max-width: 768px) {
            .container {
                flex-direction: column;
                margin: 10px;
            }

            .sidebar, .main-content {
                width: 100%;
            }

            .sidebar {
                display: none;
                max-height: 100vh; /* Limit height on mobile */
                overflow-y: auto; /* Allow scrolling */
            }

            .sidebar.active {
                display: block;
            }

            .mobile-nav {
                display: block;
            }

            .skills-grid {
                grid-template-columns: 1fr;
            }

            .education table {
                display: block;
            }

            .education thead {
                display: none;
            }

            .education tr {
                display: block;
                margin-bottom: 15px;
                border: 1px solid #ddd;
                border-radius: 4px;
            }

            .education td {
                display: block;
                text-align: left;
                padding: 10px;
                border: none;
                border-bottom: 1px solid #eee;
                position: relative;
                font-size: 0.9em;
            }

            .education td:last-child {
                border-bottom: none;
            }

            .education td:before {
                content: attr(data-label);
                font-weight: bold;
                display: inline-block;
                width: 100px;
                color: #1a3c5e;
            }
        }
    </style>
</head>
<body>
    <div class="mobile-nav" onclick="toggleSidebar()">☰ Menu</div>
    <div class="container">
        <div class="sidebar">
            <h1>Kola Chiranjeevi</h1>
            <p>BTECH Graduate SRKREC(A)</p>
            <div class="contact-info">
                <p><i class="fas fa-envelope"></i> chirukola123@gmail.com</p>
                <p><i class="fas fa-phone"></i> +91 9703065484</p>
                <p><i class="fas fa-map-marker-alt"></i> 4-77, Kanagalavaripalem, Repalle, Bapatla, Andhra Pradesh-522265</p>
            </div>
            <div class="section">
                <h2>Languages Known</h2>
                <li>English</li>
		<li>Telugu</li>
            </div>
            <div class="section">
                <h2>Hobbies</h2>
                <ul>
                    <li>Playing Cricket</li>
                    <li>Chess</li>
                    <li>Stock Market Trading</li>
                </ul>
            </div>
        </div>
        <div class="main-content">
            <div class="section">
                <h2>Career Objective</h2>
                <p>Enthusiastic IT graduate with strong skills in Java, Python, SQL, and SAP ABAP. Passionate about problem-solving and software development. Seeking an entry-level role to apply my technical expertise and grow in a dynamic environment.</p>
                <p><strong>Area of Interest:</strong> Programming and Problem Solving</p>
            </div>
            <div class="section education">
                <h2>Academic Credentials</h2>
                <table>
                    <thead>
                        <tr>
                            <th>Course</th>
                            <th>Board</th>
                            <th>Institution</th>
                            <th>YOP</th>
                            <th>CGPA/%</th>
                        </tr>
                    </thead>
                    <tbody>
                        <tr>
                            <td data-label="Course">B.Tech (IT)</td>
                            <td data-label="Board">JNTU Kakinada</td>
                            <td data-label="Institution">Sagi Rama Krishnam Raju Engineering College, Bhimavaram</td>
                            <td data-label="Year">2023</td>
                            <td data-label="CGPA/%">7.04</td>
                        </tr>
                        <tr>
                            <td data-label="Course">Diploma (CME)</td>
                            <td data-label="Board">SBTET AP</td>
                            <td data-label="Institution">Diviseema Polytechnic College, Avanigadda</td>
                            <td data-label="Year">2020</td>
                            <td data-label="CGPA/%">85.23</td>
                        </tr>
                        <tr>
                            <td data-label="Course">SSC</td>
                            <td data-label="Board">Board of Secondary Education</td>
                            <td data-label="Institution">ZPHS Bobbarlanka</td>
                            <td data-label="Year">2017</td>
                            <td data-label="CGPA/%">9.00</td>
                        </tr>
                    </tbody>
                </table>
            </div>
            <div class="section">
                <h2>Technical Skills</h2>
                <div class="skills-grid">
                    <p><strong>Programming Languages:</strong> Java, Python</p>
                    <p><strong>Databases:</strong> MySQL</p>
<p><strong>SAP ABAP:</strong> DDIC, Views, Structures, Internal Tables, ALV Reports, Smartforms</p>
                    <p><strong>Web Technologies:</strong> HTML, CSS, JavaScript</p>
                    
                    <p><strong>Other:</strong> Networking, Security Protocols</p>
                    <p><strong>Cloud:</strong> Fundamentals of Cloud Computing</p>
                    <p><strong>Tools:</strong> MS Office, Software Development, Performance Optimization</p>
                    <p><strong>Soft Skills:</strong> Debugging, Analytical, Problem-Solving, Communication, Teamwork</p>
                </div>
            </div>
            <div class="section">
                <h2>Co-Curricular Activities</h2>
                <ul>
                    <li>Attended Java and MySQL workshops at SRKREC; improved coding efficiency and data retrieval speed by 20%.</li>
                    <li>Led a team of five members on a project for 6 months.</li>
                </ul>
            </div>
            <div class="section">
                <h2>Certifications</h2>
                <div class="cert-item">
                    <li>Data Analytics with Python</li>
                </div>
            </div>
            <div class="section">
                <h2>Internships & Projects</h2>
                <div class="project-item">
                    <h4>Diagnosis of Brain Tumor using Lightweight DL Model with Fine Tuning Approach</h4>
                    <p>Engineered a sophisticated algorithm leveraging CNN and YOLO, enabling accurate detection of malignant and benign brain tumors; increased diagnostic accuracy by 25% and reduced false positives by 15% with good model evaluation metrics.</p>
                </div>
                <div class="project-item">
                    <h4>Fake News Detection with Data Science & Artificial Intelligence</h4>
                    <p>Developed a simple fake news detection system using a combination of NLP and machine learning techniques, enhancing detection accuracy by 20%.</p>
                </div>
            </div>
        </div>
    </div>

    <script>
        function toggleSidebar() {
            document.querySelector('.sidebar').classList.toggle('active');
        }
    </script>
</body>
</html>
