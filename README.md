<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Order Form</title>
  <link rel="stylesheet" href="style.css">
</head>
<body>
  <div class="container">
    <h1>🛒 Order Form</h1>
    <form id="orderForm">
      <label for="name">Full Name</label>
      <input type="text" id="name" name="name" required>

      <label for="phone">Phone Number</label>
      <input type="tel" id="phone" name="phone" required>

      <label for="size">Size</label>
      <select id="size" name="size" required>
        <option value="">-- Select Size --</option>
        <option value="XS">XS</option>
        <option value="S">S</option>
        <option value="M">M</option>
        <option value="L">L</option>
        <option value="XL">XL</option>
        <option value="XXL">XXL</option>
      </select>

      <label for="address">Address</label>
      <textarea id="address" name="address" required></textarea>

      <button type="submit">Submit & Pay</button>
    </form>
  </div>

  <script>
    document.getElementById("orderForm").addEventListener("submit", function(event){
      event.preventDefault();
      // 👉 Tukar link bawah ni dengan link payment kau (contoh ToyyibPay)
      window.location.href = "https://toyyibpay.com/your-payment-link";
    });
  </script>
</body>
</html>
