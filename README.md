<!DOCTYPE html>
<html lang="en">

<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <meta name="keywords" content="Digital Marketing, SEO, Social Media, Content Strategy, Marketing Specialist">
  <title>William Senn | Digital Marketing Portfolio</title>
  <link rel="stylesheet" href="style.css">
  <link href='https://unpkg.com/boxicons@2.1.4/css/boxicons.min.css' rel='stylesheet'>
  <style>
    * {
      margin: 0;
      paddingbx bxl-instagram-alt-sizing: border-box;
      text-decoration: none;
      border: none;
      outline: none;
      font-family: "Poppins", sans-serif;
    }

    :root {
      --bg-color: #080808;
      --second-bg-color: #131313;
      --text-color: white;
      --main-color: #ffb700f8;
    }

    html {
      font-size: 40%;
    }

    body {
      background: var(--bg-color);
      color: var(--text-color);
      padding-top: 5%;
    }

    .header {
      position: fixed;
      top: 0;
      left: 0;
      width: 100%;
      padding: 1%;
      background: rgba(0, 0, 0, 0.3);
      backdrop-filter: blur(5px);
      display: flex;
      justify-content: space-between;
      align-items: center;
      z-index: 5;
    }

    .header span {
      color: var(--main-color);
    }

    .header .logo {
      font-size: 1.5rem;
      color: white;
      font-weight: 400;
    }

    .logo:hover {
      transform: scale(1.3);
    }

    .logo span {
      text-shadow: 0 0 50px var(--main-color);
      padding-left: 10px;
    }

    .navbar a {
      font-size: 1.5rem;
      color: var(--text-color);
      margin-left: 5rem;
      font-weight: 500;
      transition: 0.3s ease;
      border-bottom: 3px solid transparent;
      margin-right: 15px;
      padding: 5px;
    }

    .navbar a:hover,
    .navbar a.active {
      color: var(--main-color);
      padding-bottom: 10px:
    }

    #menu-icon {
      font-size: .5rem;
      color: var(--main-color);
      display: none;
    }

    section.show {
      opacity: 1;
      transform: translateY(0);
    }

    .home {
      display: flex;
      align-items: center;
      justify-content: center;
      gap: 15rem;
    }

    .home-content {
      display: flex;
      flex-direction: column;
      align-items: baseline;
      text-align: left;
      justify-content: center;
      margin-top: 5rem;
    }

    .home-content .span {
      color: var(--main-color) box-shadow: 0 0 3px;
    }

    .home-content h3 {
      margin-bottom: 4rem;
      margin-top: 2rem;
      font-size: 1.7rem;
    }

    .home-content h1 {
      font-size: 4.5rem;
      font-weight: 700;
      margin-top: 1.5rem;
      line-height: 1;
    }

    .home-content span {
      color: var(--main-color);
    }

    .home-img img {
      position: center;
      top: 2rem;
      width: 52vw;
      max-height: 400px;
      box-shadow: 0 0 15px var(--main-color);
      cursor: pointer;
      transition: 0.4s ease-in-out;
      margin-top: 8.5rem;
      width: auto !important;
    }

    .home-img img:hover {
      box-shadow: 0 0 25px var(--main-color), 0 0 50px var(--main-color), 0 0 100px var(--main-color);
    }

    .home-content p {
      font-size: 1.8rem;
      font-weight: 500;
      line-height: 1.8;
      max-width: 1000px;
    }

    .social-icons a {
      display: inline-flex;
      justify-content: center;
      align-items: center;
      width: 2.5rem;
      height: 2.5rem;
      background: transparent;
      border: 2px solid var(--main-color);
      font-size: 1.5rem;
      border-radius: 50%;
      color: var(--main-color);
      margin: 3rem 1.5rem 3rem 0;
      transition: 0.3s ease-in-out;
    }

    .social-icons a:hover {
      color: var(--text-color);
      transform: scale(1.3) translateY(-5px);
      box-shadow: 0 0 25px var(--main-color);
      background-color: var(--main-color);
    }

    .btn {
      display: inline-block;
      padding: 1rem 2.2rem;
      background: var(--main-color);
      box-shadow: 0 0 25px var(--main-color);
      border-radius: 3rem;
      font-size: 1.6rem;
      color: black;
      border: 1px solid transparent;
      letter-spacing: 0.1rem;
      font-weight: 600;
      transition: 0.3s ease-in-out;
      cursor: pointer;
    }

    .btn:hover {
      transform: scale(1.05);
      box-shadow: 0 0 50px var(--main-color);
    }

    .btn-group {
      display: flex;
      align-items: center;
      gap: 1.5rem;
    }

    .btn-group a:nth-of-type(2) {
      background-color: black;
      color: var(--main-color);
      border: 2px solid var(--main-color);
      box-shadow: 0 0 25px transparent;
    }

    .btn-group a:nth-of-type(2):hover {
      box-shadow: 0 0 25px var(--main-color);
      background-color: var(--main-color);
      color: black;
    }

    .text-animation {
      font-size: 34px;
      font-weight: 600;
      min-width: 280px;
    }

    .text-animation span {
      position: relative;
    }

    .text-animation span::before {
      content: "American Made Products";
      color: var(--main-color);
      animation: words 20s infinite;
    }

    .text-animation span::after {
      content: "";
      background-color: var(--bg-color);
      position: absolute;
      width: calc(100% + 8px);
      height: 100%;
      border-left: 3px solid var(--bg-color);
      right: -8px;
      animation: cursor 0.6s infinite, typing 20s steps(14) infinite;
    }

    @keyframes cursor {
      to {
        border-left: 2px solid var(--main-color);
      }
    }

    @keyframes words {

      0%,
      20% {
        content: "SEO (Search Engine Optimization)";
      }

      21%,
      40% {
        content: "Content Creation";
      }

      41%,
      60% {
        content: "Data Analytics";
      }

      61%,
      80% {
        content: "Social Media Campaigns";
      }

      81%,
      100% {
        content: "Email Marketing Campaigns";
      }
    }

    @keyframes typing {

      5%,
      10%,
      15%,
      30%,
      35%,
      50%,
      55%,
      70%,
      75%,
      90%,
      95% {
        width: 0;
      }

      5%,
      20%,
      25%,
      40%,
      45%,
      60%,
      65%,
      80%,
      85% {
        width: calc(100% + 8px);
      }
    }

    .heading {
      font-size: 1.8rem;
      text-align: center;
      margin: 5rem 0;
    }

    .mystory {
      padding: 100px 15px;
      background: var(--second-bg-color);
    }

    .mystory .h2 {
      margin-bottom: 5rem;
    }

    .timeline-items {
      max-width: 500px;
      margin: auto;
      display: flex;
      flex-wrap: wrap;
      position: relative;
    }

    .timeline-items::before {
      content: "";
      position: absolute;
      width: 1px;
      height: 100%;
      background-color: var(--main-color);
      left: calc(50% - 1px);
    }

    .timeline-item {
      margin-bottom: 10px;
      width: 100%;
      position: relative;
    }

    .timeline-item:last-child {
      margin-bottom: 0;
    }

    .timeline-item:nth-child(odd) {
      padding-right: calc(50% + 10px);
      text-align: right;
    }

    .timeline-item:nth-child(even) {
      padding-left: calc(50% + 30px);
    }

    .timeline-dot {
      height: 15px;
      width: 15px;
      background-color: var(--main-color);
      box-shadow: 0 0 25px var(--main-color), 0 0 50px var(--main-color);
      position: absolute;
      left: calc(50% - 8px);
      border-radius: 50%;
      top: 2px;
    }

    .timeline-date {
      font-size: 30px;
      font-weight: 400;
      color: var(--text-color);
      margin: 15px 15px 15px;
    }

    .timeline-content {
      background-color: var(--bg-color);
      border: 1px solid var(--main-color);
      padding: 5px 5px;
      border-radius: 1rem;
      box-shadow: 0 0 10px var(--main-color);
      cursor: pointer;
      transition: 0.3s ease-in-out;
      font-size: 2.1rem;
    }

    .timeline-content:hover {
      transform: scale(1.05);
      box-shadow: 0 0 25px var(--main-color);
    }

    .timeline-content h3 {
      font-size: 2.6rem;
      color: var(--main-color);
    }

    #products {
      background: var(--second-bg-color);
      /* Darker background for the section */
      color: var(--text-color);
      /* Light text color for readability */
      padding: 30px;
      /* Padding around the content */
      margin: 20px 0;
      /* Vertical margin for separation */
      border-radius: 10px;
      /* Rounded corners */
      box-shadow: 0 3px 6px rgba(0, 0, 0, 0.16), 0 3px 6px rgba(0, 0, 0, 0.23);
      /* Subtle shadows for depth */
    }

    .products .heading {
      text-align: center;
      /* Central alignment for heading */
      color: var(--main-color);
      /* Highlight color for the heading */
      margin-bottom: 24px;
      /* Space below the heading */
      font-size: 1.3rem;
      /* Responsive font size */
    }

    .service-box {
      background: var(--bg-color);
      /* Slightly lighter background for the boxes */
      color: var(--text-color);
      /* Maintaining text readability */
      padding: 40px;
      /* Comfortable padding */
      margin-bottom: 60px;
      /* Space between boxes */
      border-left: 5px solid var(--main-color);
      /* Highlight with the main color */
      font-size: 2.3rem;
    }

    .service-title {
      font-size: 2.6rem;
      /* Larger font for titles */
      color: var(--main-color);
      /* Main accent color for titles */
    }

    #service1 {
      border-color: var(--main-color);
      /* Specific color accent */
    }

    #service2 {
      border-color: var(--main-color);
      /* Specific color accent */
    }

    #service3 {
      border-color: var(--main-color);
      /* Specific color accent */
    }

    @media (max-width: 768px) {
      #products {
        padding: 20px;
        margin: 20px 0;
        /* Smaller margins on smaller screens */
      }

      .service-box {
        padding: 5px;
      }

      .products,
      .heading,
      .h2 {
        font-size: 2.4rem;
        /* Smaller font size on small devices */
      }
    }

    .rating i.bxs-star {
      color: gold;
      font-size: 20px;
      /* Adjust this size based on preference */
    }

    .testimonials,
    .heading {
      color: var(--main-color);
    }

    .testimonial-ite {
      color: white;
      font-size: 2.3rem;
      padding: 20px;
    }

    .test3 {
      width: 200px;
      height: 275px;
      padding-left: 60px;
    }

    .aboutme {
      color: var(--main-color);
      text-align: center;
      margin-bottom: 5rem;
      font-size: 2.3rem;
      background: var(--second-bg-color);
      padding: 100px 15px;
    }

    .aboutme,
    .story {
      margin-bottom: 5%;
    }

    .story {
      color: white;
    }

    .contact {
      padding: 100px 15px;
      background: var(--second-bg-color);
      text-align: center;
    }

    .contact-container {
      max-width: 500px;
      margin: auto;
    }

    .contact-form {
      display: flex;
      flex-direction: column;
      gap: .8rem;
    }

    .input-box {
      position: relative;
      margin-bottom: 3rem;
    }

    .input-box input,
    .input-box textarea {
      width: 100%;
      padding: 1.5rem 2rem;
      background: var(--bg-color);
      border: 1px solid var(--main-color);
      border-radius: 2rem;
      color: var(--text-color);
      font-size: 2.6rem;
      outline: none;
      transition: 0.3s ease;
    }

    .input-box input:focus,
    .input-box textarea:focus {
      border-color: var(--main-color);
      box-shadow: 0 0 15px var(--main-color);
    }

    .input-box label {
      position: absolute;
      top: 1rem;
      left: 1rem;
      color: var(--text-color);
      pointer-events: none;
      transition: 0.3s ease;
    }

    .input-box input:focus~label,
    .input-box input:valid~label,
    .input-box textarea:focus~label,
    .input-box textarea:valid~label {
      top: 1rem;
      left: 1.8rem;
      background: var(--bg-color);
      padding: 0 1rem;
      color: var(--main-color);
    }

    textarea {
      min-height: 150px;
      resize: none;
    }

    .contact .btn {
      padding: 1rem 4rem;
      background: var(--main-color);
      border-radius: 2rem;
      color: black;
      font-size: 1.8rem;
      cursor: pointer;
      transition: 0.3s ease;
    }

    .contact .btn:hover {
      transform: scale(1.05);
      box-shadow: 0 0 30px var(--main-color);
    }

    footer {
      text-align: center;
      padding: 20px;
      background: #222;
      color: #fff;
    }
  </style>

</head>

<body>
  <header class="header">
    <div class="logo">
      <a href="#home"><span>William A. Senn</span></a>
    </div>
    <i class='bx bx-menu'></i>
    <nav class="navbar">
      <a href="#home" class="active">Projects</a>
      <a href="#mystory">My Story</a>
      <a href="#products">Skills</a>
      <a href="#testimonials">Testimonials</a>
      <a href="#aboutme">About Me</a>
      <a href="#contact">Contact</a>
    </nav>
  </header>

  <main>
    <section class="home" id="home">
      <div class="home-content">
        <h1> I'm a <span>Discrete Boss</span></h1>
        <h3 class="text-animation">Specializing in <span></span></h3>
        <p>I'm William Senn, an ambitious digital marketing specialist ready to drive brand growth through innovative strategies. Let's work together to elevate your brand and achieve your goals.</p>
        <div class="social-icons">
          <a href="https://www.linkedin.com/in/discreetboss/"><i class='bx bxl-linkedin'></i></a>
          <a href="https://github.com/DiscreetBoss"><i class='bx bxl-github'></i></a>

          <a href="https://x.com/WilliamSen9432"><i class='bx bxl-twitter'></i></a>
        </div>
        <div class="btn-group">
          <a href="#" class="btn">My Story</a>
          <a href="#contact" class="btn">Contact me</a>
        </div>
        <div class="home-img">
          <img src="https://t3.ftcdn.net/jpg/04/77/61/40/240_F_477614051_phXWPupiGjIYlUq5ZmYPsXT1pYISEia5.jpg" alt="Outdoor Dog Houses">
        </div>
      </div>
    </section>

    <section class="mystory" id="mystory">
      <h2 class="heading">Skills</h2>
      <div class="timeline-items">
        <article class="timeline-item">
          <div class="timeline-dot"></div>
          <time class="timeline-date">📊</time>
          <div class="timeline-content">
            <h3>Market Research Insights</h3>
            <p>Market research for digital marketing involves collecting and analyzing data to understand target audiences, their behaviors, preferences, and trends in the online space. It includes tools like surveys, social media analytics, and website metrics to gain insights into customer needs and competitive positioning. This research helps businesses tailor their digital marketing strategies, optimize campaigns, and improve overall engagement and conversion rates.</p>
          </div>
        </article>
        <article class="timeline-item">
          <div class="timeline-dot"></div>
          <time class="timeline-date">💼</time>
          <div class="timeline-content">
            <h3>Enhanced Brand Awareness</h3>
            <p>Enhanced brand awareness in brand strategy focuses on increasing recognition and visibility of a brand among target audiences. It involves creating a cohesive identity through consistent messaging, visual elements, and storytelling across various channels. Tactics may include content marketing, social media engagement, influencer partnerships, and public relations efforts. The goal is to build a strong presence in the market, fostering familiarity and trust, which can lead to customer loyalty and long-term success.</p>
          </div>
        </article>
        <article class="timeline-item">
          <div class="timeline-dot"></div>
          <time class="timeline-date">📈</time>
          <div class="timeline-content">
            <h3>Social Media Campaign</h3>
            <p>A social media campaign aimed at gaining +5k followers focuses on strategic engagement and content creation to attract and retain a larger audience. This involves developing eye-catching posts, utilizing targeted advertising, and leveraging popular trends or hashtags. Engaging with followers through interactive content, contests, and collaborations with influencers can also drive growth. The campaign’s success is measured through analytics, assessing not only follower count but also engagement rates and community growth, ultimately aiming to build a loyal online community.</p>
          </div>
        </article>
        <article class="timeline-item">
          <div class="timeline-dot"></div>
          <time class="timeline-date">🚀</time>
          <div class="timeline-content">
            <h3>SEO- Improve Rankings</h3>
            <p>An SEO project focused on improved rankings aims to enhance a website's visibility in search engine results through optimization techniques. This involves keyword research, on-page optimization (like meta tags and content quality), and off-page strategies such as backlink building. Technical SEO is also critical, addressing site speed, mobile-friendliness, and indexing issues. Regular performance monitoring and adjustments based on analytics help ensure that the site climbs in rankings over time, ultimately driving more organic traffic and increasing overall online presence.</p>

          </div>
        </article>
      </div>
    </section>

    <!-- Service Box 1 -->
    <article class="service-box">
      <h3 class="service-title" id="service1">Social Media Content Creation</h3>
      <p>
        As an intern at 15 Seconds of Fame, I developed engaging content tailored for various platforms, increasing audience interaction. My creativity helps campaigns that resonated with followers.
      </p>
    </article>
    <!-- Service Box 2 -->
    <article class="service-box">
      <h3 class="service-title" id="service2">Curation and Strategy</h3>
      <p>
        I curated relevant industry content and trends, ensuring our brand stayed ahead of the curve. This strategic approach not only bolstered our online presence but also reinforced our authority in the market.
      </p>
    </article>
    <!-- Service Box 3 -->
    <article class="service-box">
      <h3 class="service-title" id="service3">Analytics and Optimization </h3>
      <p>
        Utilizing Google Ads and Analytics, I tracked campaign performance and generated insights through Google Sheets. This data-driven approach allowed us to refine strategies, leading to a increase in conversion rates.
      </p>
    </article>
    </div>
    </section>

    <section class="aboutme" id="aboutme">
      <h2 class="heading">About Me</h2>
      <div class="aboutme-container">
        <div class="aboutme-item">
          <p class="story">Hello! My name is William Senn, My passion for digital marketing has been fueled by my experiences in the vibrant community of Columbia, SC, where I’ve seen how local businesses engage with their audiences and adapt to trends. This has deepened my desire to explore digital strategies that resonate on a local level.<br>

            I admire innovative marketing strategies and the real impact they can have on hard-working businesses. I understand the unique challenges that all companies face, and I’m dedicated to helping them reach their next step through effective digital marketing. I’ve earned certifications in digital marketing, e-commerce, and affiliate marketing, and I have developed skills in social media strategy, SEO, and content creation.<br>

            This is just the beginning for me—I don’t know where this journey will lead, but I’m committed to moving forward with positive steps. My goal is to strive to be the best leader I can be, continuously learning and growing. Collaboration is key for me; I believe the best ideas come from brainstorming together and leveraging diverse perspectives.<br>

            I’m excited about the possibility of contributing to a team that shares my commitment to helping businesses grow and succeed. I look forward to the opportunity to learn, grow, and make a positive impact in the digital marketing landscape.

            Thank you for considering my journey!</p>
        </div>
      </div>
    </section>

    <section class="testimonials" id="testimonials">
      <h2 class="heading">Testimonials</h2>
      <div class="wrapper">

        <!-- Testimonial 1 -->
        <div class="testimonial-ite">
          <img src="https://t4.ftcdn.net/jpg/05/06/51/51/240_F_506515178_z6nbk94MH6Pltj1lMUeDhh202LTGsBk5.jpg">
          <h2>Professor Rachel S. Kelly</h2>
          <div class="rating">
            <i class="bx bxs-star"></i>
            <i class="bx bxs-star"></i>
            <i class="bx bxs-star"></i>
            <i class="bx bxs-star"></i>
            <i class="bx bxs-star"></i>
          </div>
          <p>William brought a fresh perspective to our digital strategy that truly transformed our approach. His insights were invaluable, and he consistently delivered results.</p>
        </div>

        <!-- Testimonial 2 -->
        <div class="testimonial-ite">
          <img src="https://t3.ftcdn.net/jpg/02/92/15/52/240_F_292155261_bcEYIiVZeN1cKxXoo6xQFMqnATug7kzZ.jpg">
          <h2>Mentor John Smith</h2>
          <div class="rating">
            <i class="bx bxs-star"></i>
            <i class="bx bxs-star"></i>
            <i class="bx bxs-star"></i>
            <i class="bx bxs-star"></i>
            <i class="bx bxs-star"></i>
          </div>
          <p>Working with William was a game-changer. His dedication and creativity in digital marketing set him apart. He genuinely cares about helping brands succeed.</p>
        </div>

        <!-- Testimonial 3 -->
        <div class="testimonial-ite">
          <img src="https://t3.ftcdn.net/jpg/01/71/96/12/240_F_171961272_od3rgxnHhz3vzYcAOOAMqgd5ZT1G2i5h.jpg">
          <h2>Emily Rodriguez, Creative Lead</h2>
          <div class="rating">
            <i class="bx bxs-star"></i>
            <i class="bx bxs-star"></i>
            <i class="bx bxs-star"></i>
            <i class="bx bxs-star"></i>
            <i class="bx bxs-star"></i>
          </div>
          <p>William's enthusiasm for digital marketing is contagious. He brings innovative ideas to the table and knows how to execute them flawlessly.</p>
        </div>

      </div>
    </section>

    <section class="contact" id="contact">
      <h2 class="heading">Contact Me</h2>
      <p>I’m excited about new opportunities and collaborations. Feel free to reach out!</p><br>
      <div class="contact-container">
        <form action="#" class="contact-form">
          <div class="input-box">
            <input type="text" required>
            <label>Name</label>
          </div>
          <div class="input-box">
            <input type="email" required>
            <label>Email</label>
          </div>
          <div class="input-box">
            <textarea required></textarea>
            <label>Message</label>
          </div>
          <div class="btn-group">
            <button type="submit" class="btn">Send Message</button>
          </div>
        </form>
      </div>
    </section>

  </main>
  <footer>
    <div class="footer-content">
      <p>&copy; 2024 William A. Senn. All Rights Reserved.</p>
    </div>
  </footer>

</body>
<script>const sections = document.querySelectorAll("section");
window.addEventListener("scroll", () => {
  sections.forEach((section) => {
    {
      section.classList.add("show");
    }
  });
});
</script>
</html>
