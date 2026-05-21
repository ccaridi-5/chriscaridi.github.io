---
@import "{{ site.theme }}";

/* 1. IMPORT SPACE & SCI-FI FONTS */
@import url('https://fonts.googleapis.com/css2?family=Orbitron:wght@600;800&family=Space+Grotesk:wght@400;500;700&display=swap');

/* 2. APPLY PURPLE GALAXY BACKGROUND & TEXT COLORS */
body {
  background-image: url('../../Purple%20Galaxy.jpg') !important;
  background-size: cover;
  background-attachment: fixed;
  background-position: center;
  background-color: #0b0612; /* Deep space dark fallback color */
  font-family: 'Space Grotesk', sans-serif;
  color: #f0ebf8; /* Soft starlight white/pale silver for maximum readability */
}

/* 3. PROTECT TEXT READABILITY */
/* This adds a semi-transparent dark nebula shroud behind your text so it doesn't get lost in the galaxy image */
.wrapper, .container, main, article, .page-content {
  background: rgba(15, 10, 28, 0.85) !important; 
  border: 1px solid rgba(168, 85, 247, 0.2); /* Faint cosmic purple border */
  border-radius: 12px;
  padding: 40px;
  box-shadow: 0 0 30px rgba(168, 85, 247, 0.15); /* Soft outer nebula glow */
}

/* 4. GLOWING NEBULA HEADINGS */
h1 {
  font-family: 'Orbitron', sans-serif;
  color: #38bdf8; /* Brilliant star cyan */
  text-shadow: 0 0 10px rgba(56, 189, 248, 0.5);
  font-weight: 800;
}

h2, h3 {
  font-family: 'Orbitron', sans-serif;
  color: #c084fc; /* Vibrant nebula purple */
  text-shadow: 0 0 8px rgba(192, 132, 252, 0.4);
  font-weight: 600;
  border-bottom: 1px solid rgba(192, 132, 252, 0.2);
  padding-bottom: 8px;
}

/* 5. COSMIC LINK ACCENTS */
a {
  color: #f472b6; /* Radiant cosmic pink */
  text-decoration: none;
  transition: all 0.3s ease;
}

a:hover {
  color: #38bdf8; /* Swaps to star cyan on hover */
  text-shadow: 0 0 12px rgba(56, 189, 248, 0.8);
}
