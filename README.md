<html lang="ru">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Безопасная оплата заказа</title>
    <link rel="stylesheet" href="style.css">
</head>
<body>
    <div class="payment-container">
        <h2>Оплата картой</h2>
        <form id="payment-form">
            <!-- Номер карты -->
            <div class="form-group">
                <label for="card-number">Номер карты</label>
                <input type="text" id="card-number" placeholder="0000 0000 0000 0000" maxlength="19" required>
            </div>
          <div class="form-row">
                <!-- Срок действия -->
                <div class="form-group">
                    <label for="card-expiry">Срок действия</label>
                    <input type="text" id="card-expiry" placeholder="ММ/ГГ" maxlength="5" required>
                </div>
                <!-- CVV/CVC -->
                <div class="form-group">
                    <label for="card-cvv">CVC / CVV</label>
                    <input type="password" id="card-cvv" placeholder="123" maxlength="3" required>
                </div>
            </div>
<!-- Имя владельца -->
            <div class="form-group">
                <label for="card-holder">Имя владельца</label>
                <input type="text" id="card-holder" placeholder="IVAN IVANOV" required>
            </div>
<button type="submit" class="submit-btn">Оплатить заказ</button>
        </form>
    </div>
<script src="script.js"></script>
</body>
</html>
