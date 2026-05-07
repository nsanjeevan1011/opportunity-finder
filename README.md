# opportunity-finder
AI powered opportunity finder website
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Opportunity Finder</title>
  <style>
    * { margin: 0; padding: 0; box-sizing: border-box; }

    body {
      font-family: Arial, sans-serif;
      background-color: #f0f4ff;
    }

    header {
      background-color: #2563eb;
      color: white;
      text-align: center;
      padding: 40px 20px;
    }

    header h1 { font-size: 36px; margin-bottom: 10px; }
    header p { font-size: 16px; opacity: 0.85; }

    .search-bar {
      display: flex;
      justify-content: center;
      margin: 30px auto;
      width: 90%;
      max-width: 600px;
      gap: 10px;
    }

    .search-bar input {
      flex: 1;
      padding: 12px 16px;
      border: 2px solid #2563eb;
      border-radius: 8px;
      font-size: 16px;
      outline: none;
    }

    .search-bar button {
      background-color: #2563eb;
      color: white;
      padding: 12px 24px;
      border: none;
      border-radius: 8px;
      font-size: 16px;
      cursor: pointer;
    }

    .cards {
      display: flex;
      flex-wrap: wrap;
      gap: 20px;
      justify-content: center;
      padding: 20px;
      max-width: 1100px;
      margin: 0 auto;
    }

    .card {
      background: white;
      border-radius: 12px;
      padding: 24px;
      width: 300px;
      box-shadow: 0 2px 10px rgba(0,0,0,0.08);
    }

    .card span {
      background-color: #dbeafe;
      color: #2563eb;
      font-size: 12px;
      padding: 4px 10px;
      border-radius: 20px;
    }

    .card h3 {
      font-size: 18px;
      margin: 12px 0 6px;
      color: #1e293b;
    }

    .card p {
      font-size: 14px;
      color: #64748b;
      margin-bottom: 16px;
    }

    .card button {
      background-color: #2563eb;
      color: white;
      border: none;
      padding: 10px 20px;
      border-radius: 8px;
      cursor: pointer;
      font-size: 14px;
      width: 100%;
    }
  </style>
</head>
<body>

  <header>
    <h1>🎯 Opportunity Finder</h1>
    <p>Discover internships, certifications, scholarships and more — powered by AI</p>
  </header>

  <div class="search-bar">
    <input type="text" id="searchInput" placeholder="Search opportunities..." />
    <button onclick="search()">Search</button>
  </div>

  <div class="cards" id="cardsContainer">

    <div class="card">
      <span>Internship</span>
      <h3>Google Summer Internship</h3>
      <p>Paid software engineering internship for CS students. Remote friendly.</p>
      <button>Apply Now</button>
    </div>

    <div class="card">
      <span>Certification</span>
      <h3>AWS Cloud Practitioner</h3>
      <p>Free foundational cloud certification. Beginner friendly. Globally recognized.</p>
      <button>Apply Now</button>
    </div>

    <div class="card">
      <span>Scholarship</span>
      <h3>Tata Scholarship 2025</h3>
      <p>Full scholarship for undergraduate students in engineering and technology fields.</p>
      <button>Apply Now</button>
    </div>

    <div class="card">
      <span>Certification</span>
      <h3>Meta Frontend Developer</h3>
      <p>Professional certificate in React and frontend development by Meta. Free to audit.</p>
      <button>Apply Now</button>
    </div>

    <div class="card">
      <span>Competition</span>
      <h3>Smart India Hackathon</h3>
      <p>National level hackathon with cash prizes. Open to all college students.</p>
      <button>Apply Now</button>
    </div>

    <div class="card">
      <span>Research</span>
      <h3>IITM Research Internship</h3>
      <p>Summer research program at IIT Madras for students interested in AI and ML.</p>
      <button>Apply Now</button>
    </div>

  </div>

  <script>
    function search() {
      const input = document.getElementById("searchInput").value.toLowerCase();
      const cards = document.querySelectorAll(".card");

      cards.forEach(card => {
        const text = card.innerText.toLowerCase();
        if (text.includes(input)) {
          card.style.display = "block";
        } else {
          card.style.display = "none";
        }
      });
    }
  </script>

</body>
</html>
git init
git add .
git commit -m "first commit"
git branch -M main
git remote add origin https://github.com/Sanjeevan N/opportunity-finder.git
git push -u origin main
Username for 'https://github.com':
Password for 'https://Sanjeevan N@github.com':
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
# 🎯 Opportunity Finder

**Built by: Sanjeevan N**
**Email: nsanjeevan1011@email.com**


## About This Project
An AI-powered platform that automatically collects and displays 
internships, scholarships, certifications and competitions 
for students — all in one place.

## Features
- 🤖 AI powered search and categorization
- 📊 Auto updated daily using web scraping
- 🎓 Covers internships, scholarships, certifications
- 📱 Mobile friendly design

## Tech Stack
- Frontend: HTML, CSS, JavaScript, React
- Backend: Python, FastAPI
- AI: Claude APIm
- Database: PostgreSQL
- Hosting: Vercel

## Why I Built This
I personally struggled to find opportunities as a student.
I built this to solve that problem for myself and others.

## Live Demo

