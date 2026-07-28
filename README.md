# html-27
<!DOCTYPE html>
<html lang="uz">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Portfolio To'ri</title>
  <link rel="stylesheet" href="style.css">
</head>
<body>

  <div class="portfolio-grid">
    <!-- Header (Sarlavha) - To'liq kenglikda -->
    <header class="header">
      <h1>Mening Portfoliom</h1>
    </header>

    <!-- Birinchi loyiha (Featured) - 2 ustunni egallaydi -->
    <div class="card featured">
      <h2>Loyiha 1 (Asosiy)</h2>
      <p>Bu loyiha 2 ustun kengligida joylashgan.</p>
    </div>

    <!-- Boshqa loyiha kartalari -->
    <div class="card">
      <h2>Loyiha 2</h2>
      <p>Kichik tavsif.</p>
    </div>

    <div class="card">
      <h2>Loyiha 3</h2>
      <p>Kichik tavsif.</p>
    </div>

    <div class="card">
      <h2>Loyiha 4</h2>
      <p>Kichik tavsif.</p>
    </div>

    <div class="card">
      <h2>Loyiha 5</h2>
      <p>Kichik tavsif.</p>
    </div>

    <!-- Footer - To'liq kenglikda -->
    <footer class="footer">
      <p>&copy; 2026 Mening Portfoliom. Barcha huquqlar himoyalangan.</p>
    </footer>
  </div>

</body>
</html>

css
* {
  box-sizing: border-box;
  margin: 0;
  padding: 0;
  font-family: Arial, sans-serif;
}

body {
  background-color: #f4f6f9;
  padding: 20px;
}

/* Main Grid Container - 3 ustunli to'r */
.portfolio-grid {
  display: grid;
  grid-template-columns: repeat(3, 1fr); /* 3 ustunli grid */
  gap: 20px;
  max-width: 1000px;
  margin: 0 auto;
}

/* Sarlavha (Header) - To'liq kenglik (1 / -1) */
.header {
  grid-column: 1 / -1;
  background-color: #2c3e50;
  color: #fff;
  padding: 20px;
  text-align: center;
  border-radius: 8px;
}

/* Footer - To'liq kenglik (1 / -1) */
.footer {
  grid-column: 1 / -1;
  background-color: #2c3e50;
  color: #fff;
  padding: 15px;
  text-align: center;
  border-radius: 8px;
}

/* Barcha loyiha kartalari ko'rinishi */
.card {
  background-color: #ffffff;
  padding: 20px;
  border-radius: 8px;
  box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1);
}

/* Birinchi loyiha - 2 ustunni egallaydi (span 2) */
.card.featured {
  grid-column: span 2;
  background-color: #e8f4fd;
  border: 1px solid #3498db;
}
