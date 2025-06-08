<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1" />
  <title>Online Income Explosion: Make ₦0 to ₦1M</title>
  <link href="https://fonts.googleapis.com/css2?family=Outfit:wght@400;700;900&display=swap" rel="stylesheet" />
  <style>
    * {
      margin: 0;
      padding: 0;
      box-sizing: border-box;
      font-family: 'Outfit', sans-serif;
    }
    body {
      background: linear-gradient(135deg, #0f0c29, #302b63, #24243e);
      color: #fff;
      padding: 30px 20px;
      line-height: 1.7;
      min-height: 100vh;
    }
    header {
      text-align: center;
      margin-bottom: 30px;
      animation: fadeInDown 1s ease-in-out;
    }
    header h1 {
      font-size: 2.2rem;
      font-weight: 900;
      color: #ffbf00;
      margin-bottom: 10px;
    }
    .timer {
      background: #000;
      padding: 12px 18px;
      display: inline-block;
      font-weight: 700;
      font-size: 1.3rem;
      border: 2px dashed #ffbf00;
      margin-top: 10px;
      border-radius: 12px;
      animation: pulse 1.5s infinite;
    }
    .btn-buy {
      display: inline-block;
      margin: 14px auto;
      padding: 10px 20px;
      border-radius: 8px;
      font-weight: bold;
      background: #00ffcc;
      color: #000;
      text-decoration: none;
      box-shadow: 0 0 10px #00ffcc80;
      transition: all 0.3s ease;
      cursor: pointer;
    }
    .btn-buy.small {
      font-size: 0.9rem;
      padding: 8px 14px;
      box-shadow: none;
    }
    .btn-buy:hover {
      background: #00ccaa;
    }
    .section {
      background: rgba(255, 255, 255, 0.05);
      border: 1px solid #444;
      border-radius: 16px;
      padding: 25px;
      margin-bottom: 30px;
      backdrop-filter: blur(6px);
      animation: fadeIn 1.2s ease-in-out;
      max-width: 800px;
      margin-left: auto;
      margin-right: auto;
    }
    .strip {
      background: #ffbf00;
      color: #000;
      padding: 20px;
      border-radius: 12px;
      font-weight: bold;
      margin: 30px auto;
      text-align: center;
      max-width: 800px;
    }
    h2 {
      color: #ffbf00;
      font-size: 1.6rem;
      margin-bottom: 12px;
      text-align: center;
    }
    ul {
      list-style-type: none;
      padding-left: 0;
      margin-bottom: 15px;
    }
    ul li {
      margin-bottom: 10px;
      padding-left: 1.4em;
      position: relative;
    }
    ul li::before {
      content: "✅";
      position: absolute;
      left: 0;
      top: 0;
      font-size: 1.2rem;
    }
    /* Testimonials */
    .testimonials {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
      gap: 20px;
      max-width: 800px;
      margin: 20px auto 40px auto;
    }
    .testimonial {
      background: #111;
      border-left: 4px solid #ffbf00;
      padding: 15px 20px;
      border-radius: 12px;
      font-size: 0.95rem;
      color: #ddd;
      display: flex;
      flex-direction: column;
      justify-content: flex-start;
    }
    .testimonial strong {
      color: #00ffcc;
      margin-bottom: 8px;
      font-weight: 700;
    }
    .testimonial img {
      margin-top: 12px;
      border-radius: 10px;
      width: 100%;
      height: auto;
      object-fit: contain;
      box-shadow: 0 0 10px #00ffcc44;
      max-height: 180px;
    }
    /* Book cover image */
    .book-cover {
      width: 100%;
      max-width: 400px;
      display: block;
      margin: 20px auto 25px auto;
      border-radius: 10px;
      box-shadow: 0 0 12px rgba(255, 255, 255, 0.2);
    }
    /* FAQ */
    .faq {
      font-size: 0.85rem;
      max-width: 800px;
      margin: 40px auto 20px auto;
      line-height: 1.5;
      color: #ccc;
    }
    .faq h2 {
      color: #ffbf00;
      font-size: 1.2rem;
      margin-bottom: 20px;
      text-align: center;
    }
    .faq h3 {
      color: #00ffcc;
      margin-bottom: 6px;
      font-weight: 700;
    }
    .faq p {
      margin-bottom: 14px;
    }
    /* WhatsApp Contact */
    .contact {
      .faq-contact {
  max-width: 800px;
  margin: 10px auto 40px auto;
  font-size: 0.85rem;
  text-align: center;
}
.faq-contact a {
  color: #25d366; /* bright WhatsApp green */
  font-weight: 700;
  text-decoration: none;
  transition: color 0.3s ease;
}
.faq-contact a:hover {
  color: #1ebe57; /* slightly darker green on hover */
};
    }
    .contact a {
      color: #25d366;
      font-weight: 700;
      font-size: 1.1rem;
      text-decoration: none;
      border: 2px solid #25d366;
      padding: 10px 18px;
      border-radius: 30px;
      display: inline-block;
      transition: all 0.3s ease;
    }
    .contact a:hover {
      background-color: #25d366;
      color: #fff;
    }
    /* Animations */
    @keyframes fadeInDown {
      from {
        opacity: 0;
        transform: translateY(-20px);
      }
      to {
        opacity: 1;
        transform: translateY(0);
      }
    }
    @keyframes fadeIn {
      from {
        opacity: 0;
      }
      to {
        opacity: 1;
      }
    }
    @keyframes pulse {
      0% {
        transform: scale(1);
      }
      50% {
        transform: scale(1.05);
      }
      100% {
        transform: scale(1);
      }
    }
    @media (max-width: 768px) {
      .testimonials {
        grid-template-columns: 1fr;
      }
      .section, .strip, .faq {
        margin-left: 10px;
        margin-right: 10px;
      }
    }
  </style>
</head>
<body>
  <header>
    <h1>
      Online Income Explosion: Learn Affiliate Marketing, Dropshipping & Trading — Get From ₦0 to ₦1 Million FAST!
    </h1>
    <div class="timer" id="countdown">🔥 Hurry! Offer ends soon 🔥</div>
    <div>
      <a href="https://selar.com/p/661746?affiliate=jtb5" class="btn-buy">Buy Now — ₦25,000 Only</a>
    </div>
  </header>

  <div class="section">
    <h2>From Broke to Bank — This Changed Everything</h2>
    <p>
      I was stuck. Broke. Tired. Searching for answers online. Until I discovered these 3 digital money systems that don’t require tech skills or capital.
    </p>
    <p>
      Now I earn weekly, from anywhere — just with my phone. And inside this guide, I’ve broken it down <em>step-by-step</em> so you can do the same.
    </p>
    <div>
      <a href="https://selar.com/p/661646?affiliate=jtb5" class="btn-buy small">Start Now — ₦25k</a>
    </div>
  </div>

  <div class="section">
    <h2>What’s Inside the Guide?</h2>
    <ul>
      <li>Exact strategies used by top earners in Nigeria and beyond</li>
      <li>No experience needed — just your phone and data</li>
      <li>Learn how to build traffic and convert it into income</li>
      <li>Full mobile-optimized blueprint with daily plans</li>
      <li>From scratch to consistent ₦100k+ weeks</li>
    </ul>
    <img class="book-cover" src="https://i.ibb.co/tMD8LBCN/IMG-20250601-WA0011.jpg" alt="Book Cover" />
    <div>
      <a href="https://selar.com/p/661646?affiliate=jtb5" class="btn-buy small">Buy Now — ₦25,000</a>
    </div>
  </div>

  <div class="strip">No Skills? No Laptop? No Problem. This is for YOU.</div>

  <div class="section">
    <h2>Who Is This For?</h2>
    <ul>
      <li>Students or NYSC looking to make money online fast</li>
      <li>9–5 workers tired of earning peanuts</li>
      <li>Hustlers selling online but not making real profit</li>
      <li>Ambitious people who want to build something real online</li>
      <li>Anyone ready to finally change their life with digital skills</li>
    </ul>
    <div>
      <a href="https://selar.com/p/661646?affiliate=jtb5" class="btn-buy small">Let’s Get Started</a>
    </div>
  </div>

  <div class="section">
    <h2>🔥 Special Limited Time Offer</h2>
    <p><strong>Old Price: ₦80,000 — New Price: ₦25,000 Only</strong></p>
    <p>100% Refund Guarantee — If It Doesn’t Work for You, Get Your Money Back!</p>
    <div>
      <a href="https://selar.com/p/661646?affiliate=jtb5" class="btn-buy">Get It Now — Only ₦25k</a>
    </div>
  </div>

  <div class="section">
    <h2>🔥 Bonuses If You Order Before Countdown Ends</h2>
    <ul>
      <li>Bonus 1: A private video on how I flipped ₦7k to ₦250k in 2 weeks</li>
      <li>Bonus 2: Access to a Telegram support group</li>
      <li>Bonus 3: A ready-made template to start affiliate sales today</li>
    </ul>
    <p style="color: #ffbf00; font-weight: bold; text-align: center;">
      These bonuses disappear after the countdown ends!
    </p>
    <div style="text-align: center;">
      <a href="https://selar.com/p/661646?affiliate=jtb5" class="btn-buy small">Claim It Now — ₦25k</a>
    </div>
  </div>

  <!-- Testimonials Section -->
  <h2>💬 Real Nigerians. Real Results.</h2>
  <div class="section">
  <h2>🎥 Watch This Before You Buy</h2>
  <p>When I shot this video, I was deep in my hustle — no fancy setup, just raw truth from someone who figured out how to go from ₦0 to consistent cash flow online.</p>
  <p>It's less than 60 seconds, but it might shift how you think about online income forever. Watch it.</p>

  <iframe width="100%" height="400" src="https://www.youtube.com/embed/R3zfWLYWi2c" 
    title="Online Income Guide" frameborder="0" 
    allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" 
    allowfullscreen style="margin-top: 15px; border-radius: 12px;"></iframe>

  <div style="text-align:center; margin-top:20px;">
    <a href="https://selar.com/p/661646?affiliate=jtb5" class="btn-buy small">Buy Now After Watching</a>
  </div>
</div>
  <div class="testimonials">
    <div class="testimonial">
      <strong>Balogun from Ibadan:</strong>
      I never thought ₦400k in one week was possible — till I applied these exact steps.
      <img src="https://i.ibb.co/8gxnX0gH/Screenshot-20250531-131959-Whats-App.jpg" alt="Balogun Testimonial" />
    </div>
    <div class="testimonial">
      <strong>Semilore from Lagos:</strong>
      I made over ₦1M in my first month. From struggling with debts to funding my own apartment.
      <img src="https://i.ibb.co/sv3BWjZs/Screenshot-20250531-132925-Whats-App-Business.jpg" alt="Semilore Testimonial" />
    </div>
    <div class="testimonial">
      <strong>Mary from Port Harcourt:</strong>
      I had no job for 7 months. This changed my entire life. I now sell digital products and trade on the side.
    </div>
    <div class="testimonial">
      <strong>Kelvin from Abuja:</strong>
      I used to work 9–5 and barely saved ₦20k monthly. Now I earn 5x that from my phone.
    </div>
    <div class="testimonial">
      <strong>Tina from Osogbo:</strong>
      I was scared to try. But the way it was explained inside made it too easy. Now I help others too.
    </div>
  </div>

  <!-- FAQ Section -->
  <div class="faq">
    <h2>Frequently Asked Questions</h2>

    <h3>1. Do I need a laptop or special skills?</h3>
    <p>No. All you need is a smartphone and an internet connection. This guide is made for beginners with zero experience.</p>

    <h3>2. How soon can I start earning?</h3>
    <p>If you follow the steps daily, you can start seeing results within the first week.</p>

    <h3>3. Is the price really ₦25,000?</h3>
    <p>Yes, this is a special discount from the usual ₦80,000. The price will go back up once the timer ends.</p>

    <h3>4. What if I don’t get results?</h3>
    <p>We offer a 100% money-back guarantee if you apply the methods and don’t get results.</p>

    <h3>5. Can I do this alongside my job or school?</h3>
    <p>Absolutely! These strategies are designed to fit into any schedule.</p>

    <h3>6. Is there support if I get stuck?</h3>
    <p>Yes, you get access to a private Telegram group where you can ask questions and get help.</p>

    <h3>7. Are the bonuses really limited?</h3>
    <p>Yes, the bonuses are only available while the countdown timer is active.</p>

    <h3>8. How do I contact you for questions?</h3>
    <p>You can reach me directly via WhatsApp below.</p>
  </div>

  <!-- WhatsApp Contact -->
  <div class="contact">
    <a href="https://wa.link/4gmsqi" target="_blank" rel="noopener noreferrer">
      📲 Contact Me on WhatsApp
    </a>
  </div>

  <script>
    // Example countdown timer script — replace with your own logic or remove if not needed
    // For demonstration, counts down from 24 hours from page load
    const countdownEl = document.getElementById('countdown');
const TIMER_KEY = 'countdownStartTime';

function getCountdownStart() {
  let start = localStorage.getItem(TIMER_KEY);
  if (!start) {
    start = Date.now();
    localStorage.setItem(TIMER_KEY, start);
  }
  return parseInt(start, 10);
}

function updateTimer() {
  const startTime = getCountdownStart();
  const now = Date.now();
  const elapsed = now - startTime;
  const totalDuration = 24 * 60 * 60 * 1000; // 24 hours in ms
  const remaining = totalDuration - elapsed;

  if (remaining <= 0) {
    countdownEl.innerHTML = "⏰ Offer expired!";
    localStorage.removeItem(TIMER_KEY); // reset timer for next visit if you want
    return;
  }

  let hours = Math.floor((remaining % (1000 * 60 * 60 * 24)) / (1000 * 60 * 60));
  let minutes = Math.floor((remaining % (1000 * 60 * 60)) / (1000 * 60));
  let seconds = Math.floor((remaining % (1000 * 60)) / 1000);

  countdownEl.innerHTML = `🔥 Hurry! Offer ends in ${hours}h ${minutes}m ${seconds}s 🔥`;
}

setInterval(updateTimer, 1000);
updateTimer();
  </script>
<a href="https://selar.com/p/661646?affiliate=jtb5" class="floating-buy-btn">Buy Now</a>

<style>
  .floating-buy-btn {
    position: fixed;
    bottom: 20px;
    right: 20px;
    background: #00ffcc;
    color: #000;
    padding: 14px 20px;
    border-radius: 50px;
    font-weight: bold;
    text-decoration: none;
    box-shadow: 0 0 12px #00ffcc80;
    z-index: 999;
    transition: background 0.3s ease;
  }
  .floating-buy-btn:hover {
    background: #00ccaa;
  }
</style>
</body>
</html>
