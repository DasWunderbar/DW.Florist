<!DOCTYPE html>
<html lang="zh-TW">
<head>
    <meta charset="UTF-8">
    <title>Das Wunderbar Florist - 管理後台</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <style>
        @import url('https://fonts.googleapis.com/css2?family=Noto+Serif+TC:wght@300;400&display=swap');
        body { font-family: 'Noto Serif TC', serif; background-color: #fdfaf6; }
    </style>
</head>
<body class="p-8">

    <h1 class="text-2xl text-[#8a7e72] mb-8">✿ Das Wunderbar Florist 後台</h1>

    <div class="bg-white p-6 rounded-2xl border border-[#ede5dd] mb-8">
        <h2 class="mb-4">新增作品</h2>
        <div class="grid grid-cols-3 gap-4">
            <input type="text" id="flowerName" placeholder="花禮名稱" class="border p-2 rounded">
            <input type="text" id="flowerPrice" placeholder="價格" class="border p-2 rounded">
            <button onclick="addFlower()" class="bg-[#c4a484] text-white rounded hover:bg-[#b09275]">確認上傳</button>
        </div>
    </div>

    <div id="flowerGrid" class="grid grid-cols-1 md:grid-cols-3 gap-6">
        </div>

    <script>
        function addFlower() {
            const name = document.getElementById('flowerName').value;
            const price = document.getElementById('flowerPrice').value;
            
            if(!name || !price) return alert('請填寫完整資訊');

            const grid = document.getElementById('flowerGrid');
            const card = document.createElement('div');
            card.className = "bg-white p-4 rounded-xl border border-[#ede5dd]";
            card.innerHTML = `
                <div class="h-40 bg-[#fdfaf6] mb-4 flex items-center justify-center text-[#d4c4b7]">圖片預覽區</div>
                <h4 class="font-medium">${name}</h4>
                <p class="text-sm text-gray-400">NT$ ${price}</p>
            `;
            grid.appendChild(card);
            
            // 清空輸入框
            document.getElementById('flowerName').value = '';
            document.getElementById('flowerPrice').value = '';
        }
    </script>
</body>
</html>
