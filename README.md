<!doctype html>
<html>
<head>
<meta name="viewport" content="width=device-width, initial-scale=1" />
<style>
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

body {
  font-family: -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, sans-serif;
  background: linear-gradient(135deg, #f5f3ef 0%, #e8e4dc 100%);
  color: #3d3d3d;
  min-height: 100vh;
}

.header {
  text-align: center;
  padding: 40px 20px 30px;
  background: linear-gradient(135deg, #d4af37 0%, #b8933d 100%);
  box-shadow: 0 4px 20px rgba(212, 175, 55, 0.3);
}

.header h1 {
  font-size: 32px;
  font-weight: 700;
  color: #ffffff;
  margin-bottom: 8px;
  letter-spacing: 2px;
  text-shadow: 0 2px 4px rgba(0, 0, 0, 0.1);
}

.header p {
  font-size: 14px;
  color: #f5f5f5;
  font-weight: 400;
  letter-spacing: 1px;
}

.category {
  padding: 24px;
  background: #ffffff;
  margin: 20px 15px;
  border-radius: 20px;
  box-shadow: 0 8px 24px rgba(0, 0, 0, 0.08);
  transition: transform 0.3s ease, box-shadow 0.3s ease;
}

.category:hover {
  transform: translateY(-4px);
  box-shadow: 0 12px 32px rgba(0, 0, 0, 0.12);
}

.category-title {
  font-size: 24px;
  font-weight: 700;
  color: #b8933d;
  margin-bottom: 20px;
  padding-bottom: 12px;
  border-bottom: 3px solid #d4af37;
  letter-spacing: 1px;
  text-transform: uppercase;
}

.item {
  display: flex;
  justify-content: space-between;
  align-items: flex-start;
  padding: 18px;
  margin: 10px 0;
  border-radius: 12px;
  background: #fafaf8;
  transition: all 0.3s cubic-bezier(0.4, 0, 0.2, 1);
  cursor: pointer;
  position: relative;
  overflow: hidden;
}

.item::before {
  content: '';
  position: absolute;
  top: 0;
  left: -100%;
  width: 100%;
  height: 100%;
  background: linear-gradient(90deg, transparent, rgba(212, 175, 55, 0.1), transparent);
  transition: left 0.5s ease;
}

.item:hover::before {
  left: 100%;
}

.item:hover {
  background: linear-gradient(135deg, #f9f7f3 0%, #f0ede6 100%);
  box-shadow: 0 4px 16px rgba(212, 175, 55, 0.2);
  transform: translateX(4px);
}

.item:active {
  transform: scale(0.98);
  background: linear-gradient(135deg, #d4af37 0%, #b8933d 100%);
  box-shadow: 0 2px 8px rgba(212, 175, 55, 0.4);
}

.item:active .item-name,
.item:active .item-desc,
.item:active .item-price {
  color: #ffffff;
}

.item-info {
  flex: 1;
  z-index: 1;
}

.item-name {
  font-size: 17px;
  font-weight: 600;
  color: #3d3d3d;
  margin-bottom: 6px;
  transition: color 0.3s ease;
}

.item:hover .item-name {
  color: #b8933d;
}

.item-desc {
  font-size: 13px;
  color: #7a7a7a;
  line-height: 1.5;
  transition: color 0.3s ease;
}

.item-price {
  font-size: 20px;
  font-weight: 700;
  color: #b8933d;
  white-space: nowrap;
  margin-left: 15px;
  z-index: 1;
  transition: all 0.3s ease;
}

.item:hover .item-price {
  transform: scale(1.1);
  color: #d4af37;
}

.nav-buttons {
  display: flex;
  gap: 12px;
  padding: 20px 15px;
  overflow-x: auto;
  -webkit-overflow-scrolling: touch;
  scroll-snap-type: x mandatory;
}

.nav-buttons::-webkit-scrollbar {
  display: none;
}

.nav-btn {
  white-space: nowrap;
  padding: 12px 24px;
  border-radius: 25px;
  border: none;
  background: linear-gradient(135deg, #d4af37 0%, #b8933d 100%);
  color: #ffffff;
  text-decoration: none;
  font-size: 15px;
  font-weight: 600;
  letter-spacing: 0.5px;
  scroll-snap-align: start;
  box-shadow: 0 4px 12px rgba(212, 175, 55, 0.3);
  transition: all 0.3s cubic-bezier(0.4, 0, 0.2, 1);
  cursor: pointer;
  position: relative;
  overflow: hidden;
}

.nav-btn::before {
  content: '';
  position: absolute;
  top: 50%;
  left: 50%;
  width: 0;
  height: 0;
  border-radius: 50%;
  background: rgba(255, 255, 255, 0.3);
  transform: translate(-50%, -50%);
  transition: width 0.6s, height 0.6s;
}

.nav-btn:active::before {
  width: 300px;
  height: 300px;
}

.nav-btn:hover {
  transform: translateY(-2px);
  box-shadow: 0 6px 20px rgba(212, 175, 55, 0.4);
  background: linear-gradient(135deg, #e0bd4a 0%, #c49f47 100%);
}

.nav-btn:active {
  transform: scale(0.95);
  box-shadow: 0 2px 8px rgba(212, 175, 55, 0.3);
}

.footer {
  text-align: center;
  padding: 40px 20px;
  background: #f5f3ef;
  color: #7a7a7a;
  font-size: 13px;
  margin-top: 30px;
}

.footer a {
  color: #b8933d;
  text-decoration: none;
  font-weight: 600;
  transition: color 0.3s ease;
}

.footer a:hover {
  color: #d4af37;
}
</style>
</head>

<body>
<div class="header">
  <h1>SHISHA POINT BAR</h1>
  <p>МЕНЮ</p>
</div>

<div class="nav-buttons">
  <a class="nav-btn" href="#nargile">Наргиле</a>
  <a class="nav-btn" href="#lemonades">Лимонади</a>
  <a class="nav-btn" href="#tea">Чай</a>
  <a class="nav-btn" href="#coffee">Кафе</a>
  <a class="nav-btn" href="#food">Хапване</a>
  <a class="nav-btn" href="#beer">Бира</a>
  <a class="nav-btn" href="#cocktails">Коктейли</a>
</div>

<div class="category" id="nargile">
  <div class="category-title">Наргиле</div>
  <div class="item">
    <div class="item-info">
      <div class="item-name">Класическо наргиле</div>
      <div class="item-desc">Традиционни вкусове</div>
    </div>
    <div class="item-price">25 лв</div>
  </div>
  <div class="item">
    <div class="item-info">
      <div class="item-name">Премиум наргиле</div>
      <div class="item-desc">Ексклузивна селекция</div>
    </div>
    <div class="item-price">35 лв</div>
  </div>
</div>

<div class="category" id="lemonades">
  <div class="category-title">Лимонади</div>
  <div class="item">
    <div class="item-info">
      <div class="item-name">Класическа лимонада</div>
      <div class="item-desc">Свежа и освежаваща</div>
    </div>
    <div class="item-price">8 лв</div>
  </div>
  <div class="item">
    <div class="item-info">
      <div class="item-name">Ягодова лимонада</div>
      <div class="item-desc">С пресни ягоди</div>
    </div>
    <div class="item-price">10 лв</div>
  </div>
</div>

<div class="category" id="cocktails">
  <div class="category-title">Коктейли</div>
  <div class="item">
    <div class="item-info">
      <div class="item-name">Мохито</div>
      <div class="item-desc">Ром, мента, лайм</div>
    </div>
    <div class="item-price">12 лв</div>
  </div>
  <div class="item">
    <div class="item-info">
      <div class="item-name">Маргарита</div>
      <div class="item-desc">Текила, лайм, сол</div>
    </div>
    <div class="item-price">14 лв</div>
  </div>
</div>

<div class="footer">
  <p>© 2024 Shisha Point Bar</p>
  <p><a href="https://www.shishapointbar.store">www.shishapointbar.store</a></p>
</div>

</body>
</html>
