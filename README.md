# Shelfbound
"A gentle, aesthetically pleasing platform for book lovers to share and discover soft, heartwarming book recommendations. Featuring user submissions, a monthly featured book, and a welcoming reading community."
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Shelfbound</title>
  <link href="https://fonts.googleapis.com/css2?family=Quicksand:wght@400;600&display=swap" rel="stylesheet" />
  <style>
    * {
      margin: 0;
      padding: 0;
      box-sizing: border-box;
    }
    body {
      font-family: 'Quicksand', sans-serif;
      background-color: #fdf6f0;
      color: #333;
      line-height: 1.6;
      padding: 20px;
    }
    header {
      text-align: center;
      padding: 2rem 0;
    }
    header h1 {
      font-size: 2.5rem;
      color: #b07b6d;
    }
    nav {
      text-align: center;
      margin-bottom: 2rem;
    }
    nav a {
      text-decoration: none;
      color: #b07b6d;
      margin: 0 1rem;
      font-weight: 600;
    }
    .bookshelf {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
      gap: 1.5rem;
      max-width: 1000px;
      margin: auto;
    }
    .book {
      background: #fff7f0;
      padding: 1rem;
      border-radius: 12px;
      box-shadow: 0 2px 5px rgba(0, 0, 0, 0.05);
      text-align: center;
    }
    .book img {
      width: 100%;
      height: auto;
      border-radius: 10px;
      margin-bottom: 1rem;
    }
    .book h3 {
      color: #a45c40;
    }
    .book p {
      font-size: 0.9rem;
      margin-top: 0.5rem;
    }
    .form-section {
      max-width: 800px;
      margin: 3rem auto;
      padding: 2rem;
      background: #fffaf6;
      border-radius: 12px;
      box-shadow: 0 2px 8px rgba(0,0,0,0.05);
    }
    .form-section h2 {
      color: #b07b6d;
      text-align: center;
      margin-bottom: 1rem;
    }
    .form-button {
      display: block;
      text-align: center;
      margin-top: 1rem;
    }
    .form-button a {
      background: #b07b6d;
      color: white;
      padding: 12px 24px;
      border-radius: 8px;
      text-decoration: none;
      font-weight: 600;
    }
    .testimonials {
      max-width: 800px;
      margin: 4rem auto;
      text-align: center;
    }
    .testimonials h2 {
      color: #b07b6d;
      margin-bottom: 2rem;
    }
    .testimonial {
      background: #fffaf6;
      margin: 1rem auto;
      padding: 1.5rem;
      border-radius: 12px;
      box-shadow: 0 2px 5px rgba(0, 0, 0, 0.05);
      font-style: italic;
    }

    /* Book of the Month styling */
    .book-of-the-month {
      background-color: #ffecd1;
      padding: 2rem;
      border-radius: 12px;
      box-shadow: 0 2px 8px rgba(0, 0, 0, 0.1);
      margin-bottom: 3rem;
      text-align: center;
    }
    .book-of-the-month h2 {
      color: #b07b6d;
      margin-bottom: 1rem;
    }
    .book.highlight {
      background: #fff;
      border: 2px solid #b07b6d;
      padding: 1.5rem;
      border-radius: 12px;
      box-shadow: 0 2px 5px rgba(0, 0, 0, 0.05);
    }
    .book.highlight img {
      width: 80%;
      height: auto;
      margin-bottom: 1rem;
      border-radius: 8px;
    }
    .explore-link {
      text-decoration: none;
      color: #fff;
      background-color: #b07b6d;
      padding: 12px 24px;
      border-radius: 8px;
      font-weight: 600;
    }

    footer {
      text-align: center;
      margin-top: 3rem;
      font-size: 0.8rem;
      color: #aaa;
    }
  </style>
</head>
<body>
  <header>
    <h1>Shelfbound</h1>
    <p>Gentle book recommendations for soft hearts 📚✨</p>
  </header>
  <nav>
    <a href="#">Home</a>
    <a href="#form">Submit a Book</a>
  </nav>
  <main>
    <!-- Book of the Month Section -->
    <section class="book-of-the-month">
      <h2>Book of the Month</h2>
      <div class="book highlight">
        <img src="https://m.media-amazon.com/images/I/71A8XM3f-EL._AC_UL1500_.jpg" alt="Fearless by Lauren Roberts" />
        <h3>Fearless</h3>
        <p>Paedyn and Kai return to Ilya in this heart-stopping romantasy.</p>
        <a href="#" class="explore-link">Explore More</a>
      </div>
    </section>
    <section class="bookshelf">
      <div class="book">
        <img src="https://upload.wikimedia.org/wikipedia/en/0/0a/Fourth_Wing_%28Rebecca_Yarros%29.png" alt="Fourth Wing cover" />
        <h3>Fourth Wing</h3>
        <p>by Rebecca Yarros</p>
        <p>Epic fantasy romance with dragons and danger.</p>
      </div>
      <div class="book">
        <img src="https://m.media-amazon.com/images/I/81s0B6NYXML._AC_UF1000,1000_QL80_.jpg" alt="It Ends With Us cover" />
        <h3>It Ends With Us</h3>
        <p>by Colleen Hoover</p>
        <p>An emotional journey of love and strength.</p>
      </div>
      <div class="book">
        <img src="https://upload.wikimedia.org/wikipedia/en/e/e1/Lessons_in_Chemistry_%28Bonnie_Garmus%29.png" alt="Lessons in Chemistry cover" />
        <h3>Lessons in Chemistry</h3>
        <p>by Bonnie Garmus</p>
        <p>Sharp, witty, and brilliantly empowering.</p>
      </div>
    </section>
    <section id="form" class="form-section">
      <h2>Submit a Book Recommendation</h2>
      <p style="text-align:center; margin-bottom:1rem;">Have a favorite book? Let us know so we can share it with others!</p>
      <div class="form-button">
        <a href="https://docs.google.com/forms/d/e/1FAIpQLSchuPUkzvWdrBuHdgG1touabhES2kVRe9BKfXUKqSCUFtJ2Mg/viewform" target="_blank">Open Submission Form</a>
      </div>
    </section>
    <section class="testimonials">
      <h2>What our fellow bookworms say—</h2>
      <div class="testimonial">“Shelfbound helped me fall in love with reading again.”</div>
      <div class="testimonial">“I always find something gentle and magical here.”</div>
      <div class="testimonial">“Submitting my favorite book felt like sharing a secret with friends.”</div>
    </section>
  </main>
  <footer>
    <p>&copy; 2025 Shelfbound. Made with love for book lovers.</p>
  </footer>
</body>
</html>
