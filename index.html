<!DOCTYPE html>
<html lang="vi">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Canh Pin Xe Điện</title>
    <style>
        * { box-sizing: border-box; }
        body { font-family: Arial, sans-serif; text-align: center; background: #f4f4f9; padding: 20px; margin: 0; }
        .card { background: white; padding: 25px 20px; border-radius: 15px; box-shadow: 0 4px 8px rgba(0,0,0,0.1); max-width: 350px; margin: auto; }
        h2 { color: #333; margin-top: 0; }
        .distance-text { font-size: 18px; font-weight: bold; margin: 15px 0; color: #444; }
        .progress-bar { background: #e0e0e0; border-radius: 10px; height: 25px; width: 100%; margin-bottom: 20px; overflow: hidden; }
        .progress { background: #4CAF50; height: 100%; width: 0%; transition: width 0.3s; }
        
        /* Khu vực nhập số km tùy chỉnh */
        .custom-input-box { border: 2px dashed #008CBA; border-radius: 10px; padding: 12px; margin-bottom: 15px; background: #fdfdfd; }
        .input-label { font-size: 14px; font-weight: bold; color: #008CBA; margin-bottom: 8px; text-align: left; display: block; }
        .input-group { display: table; width: 100%; }
        .input-cell-left { display: table-cell; width: 65%; padding-right: 8px; }
        .input-cell-right { display: table-cell; width: 35%; vertical-align: top; }
        .input-km { width: 100%; padding: 10px; font-size: 15px; border: 1px solid #ccc; border-radius: 6px; text-align: center; }
        .btn-add { background: #00A2D1; color: white; border: none; padding: 10px; font-size: 15px; border-radius: 6px; cursor: pointer; width: 100%; font-weight: bold; }
        
        /* Các nút bấm nhanh */
        .btn { background: #20b2aa; color: white; border: none; padding: 12px 20px; font-size: 15px; border-radius: 8px; cursor: pointer; margin-bottom: 10px; width: 100%; font-weight: bold; }
        .btn-danger { background: #f44336; margin-top: 5px; }
        .alert { color: #f44336; font-weight: bold; margin-top: 15px; display: none; font-size: 15px; background: #ffebee; padding: 8px; border-radius: 5px; }
    </style>
</head>
<body>

<div class="card">
    <h2>🔋 Giám Sát Bình Xe</h2>
    <div class="distance-text">Đã đi: <span id="distance">0</span> / 35 km</div>
    
    <div class="progress-bar">
        <div id="progress" class="progress"></div>
    </div>

    <div class="custom-input-box">
        <label class="input-label" for="customKm">✍️ Hôm nay đi được:</label>
        <div class="input-group">
            <div class="input-cell-left">
                <input type="number" id="customKm" class="input-km" step="0.1" min="0" placeholder="Nhập số km...">
            </div>
            <div class="input-cell-right">
                <button class="btn-add" onclick="addCustomKm()">Thêm</button>
            </div>
        </div>
    </div>

    <button class="btn" onclick="addKm(3)">➕ Bấm khi đi được 3km</button>
    <button class="btn" onclick="addKm(5)">➕ Bấm khi đi được 5km</button>
    <button class="btn btn-danger" onclick="resetKm()">🔄 Sạc đầy (Reset)</button>

    <div id="alert-msg" class="alert">⚠️ BÌNH SẮP HẾT! CẦN SẠC NGAY!</div>
</div>

<script>
    let maxKm = 35;
    // Tự động tải số km đã lưu từ bộ nhớ điện thoại
    let currentKm = parseFloat(localStorage.getItem('currentKm')) || 0;
    updateUI();

    // Hàm thêm số km nhập tay
    function addCustomKm() {
        let inputEl = document.getElementById('customKm');
        let val = parseFloat(inputEl.value);
        
        if (isNaN(val) || val <= 0) {
            alert("Bro vui lòng nhập một số km hợp lệ nhé!");
            return;
        }
        
        addKm(val);
        inputEl.value = ''; // Nhập xong tự xóa chữ trong ô để lần sau nhập tiếp
    }

    // Hàm xử lý cộng dồn kmchung
    function addKm(km) {
        currentKm = currentKm + km;
        if (currentKm > maxKm) currentKm = maxKm;
        
        // Làm tròn lấy 1 chữ số thập phân cho đẹp (ví dụ 3.5km)
        currentKm = Math.round(currentKm * 10) / 10;
        
        localStorage.setItem('currentKm', currentKm);
        updateUI();
    }

    // Hàm Reset khi sạc đầy bình
    function resetKm() {
        if(confirm("Bro đã sạc đầy bình và muốn reset đúng không?")) {
            currentKm = 0;
            localStorage.setItem('currentKm', 0);
            updateUI();
        }
    }

    // Hàm cập nhật giao diện
    function updateUI()
