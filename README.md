<html lang="ru">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Безопасная оплата заказа</title>
    <link rel="stylesheet" href="style.css">
    <style>
    * {
    box-sizing: border-box;
    margin: 0;
    padding: 0;
    font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;};
body {
    background-color: #f4f6f8;
    display: flex;
    justify-content: center;
    align-items: center;
    height: 100vh;
};
.payment-container {
    background: #ffffff;
    padding: 30px;
    border-radius: 8px;
    box-shadow: 0 4px 15px rgba(0, 0, 0, 0.05);
    width: 100%;
    max-width: 400px;
};
h2 {
    margin-bottom: 20px;
    color: #333;
    font-size: 24px;
    text-align: center;
}
.form-group {
    margin-bottom: 15px;
    display: flex;
    flex-direction: column;
}
.form-row {
    display: flex;
    gap: 15px;
}
.form-row .form-group {
    flex: 1;
}
label {
    font-size: 14px;
    color: #666;
    margin-bottom: 5px;
    font-weight: 500;
}
input {
    padding: 12px;
    border: 1px solid #ccc;
    border-radius: 4px;
    font-size: 16px;
    outline: none;
    transition: border-color 0.2s;
}
input:focus {
    border-color: #002f34; /* Фирменные цвета обычно меняются здесь */
}
.submit-btn {
    width: 100%;
    padding: 14px;
    background-color: #002f34;
    color: white;
    border: none;
    border-radius: 4px;
    font-size: 16px;
    font-weight: bold;
    cursor: pointer;
    transition: background-color 0.2s;
    margin-top: 10px;
}
.submit-btn:hover {
    background-color: #001f22;
}
</style>
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
