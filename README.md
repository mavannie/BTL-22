<!DOCTYPE html>
<html>
<head>
  <title>Greenroot Investment</title>
  <style>
    body { font-family: Arial; background: #f5f5f5; text-align: center; padding: 40px; }
    .card { background: white; padding: 20px; margin: auto; border-radius: 12px; box-shadow: 0 4px 10px rgba(0,0,0,0.1); max-width: 400px; }
    .btn { background: green; color: white; padding: 10px 20px; border: none; border-radius: 8px; font-size: 16px; }
    input { padding: 10px; width: 80%; margin-bottom: 10px; border-radius: 6px; border: 1px solid #ccc; }
  </style>
</head>
<body>
  <div class="card">
    <h2>Greenroot Investment</h2>
    <p>Daily Return: <strong>14%</strong></p>
    <input type="number" id="amount" placeholder="Enter amount (Min: 500 KES)">
    <button class="btn" onclick="calculate()">Invest Now</button>
    <p id="result"></p>
  </div>

  <script>
    function calculate() {
      const amount = document.getElementById('amount').value;
      if (amount >= 500) {
        const profit = (amount * 0.14).toFixed(2);
        document.getElementById('result').innerText = `Daily Profit: KES ${profit}`;
      } else {
        document.getElementById('result').innerText = "Minimum investment is 500 KES.";
      }
    }
  </script>
</body>
</html># BTL-22
