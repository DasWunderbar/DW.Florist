<!DOCTYPE html>
<html lang="zh-TW">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Das Wunderbar Florist </title>
    <script src="https://cdn.tailwindcss.com"></script>
    <link href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0/css/all.min.css" rel="stylesheet">
    <style>
        @import url('https://fonts.googleapis.com/css2?family=Noto+Serif+TC:wght@300;400&display=swap');
        body { font-family: 'Noto Serif TC', serif; background-color: #fdfaf6; color: #5c544d; }
        .bg-earth { background-color: #eaddcf; }
        .text-earth { color: #8a7e72; }
        .flower-border { border-top: 2px dashed #d4c4b7; margin: 20px 0; position: relative; }
        .flower-border::after { content: '✿'; position: absolute; right: 0; top: -15px; color: #c4a484; }
    </style>
</head>
<body class="p-8">

    <!-- 導航欄 -->
    <nav class="flex justify-between items-center mb-12 border-b border-[#d4c4b7] pb-6">
        <h1 class="text-2xl tracking-widest text-[#8a7e72]">✿ Das Wunderbar Florist</h1>
        <div class="space-x-6 text-sm underline-offset-4 underline">
            <a href="#">作品瀏覽</a>
            <a href="#">顧客管理</a>
            <a href="#">後台分析</a>
            <a href="#">折扣設定</a>
        </div>
    </nav>

    <!-- 儀表板區域 -->
    <main class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-4 gap-6">
        
        <!-- 作品編輯模組 -->
        <section class="bg-white p-6 rounded-2xl shadow-sm border border-[#ede5dd]">
            <h2 class="text-lg mb-4 flex items-center"><i class="fa-solid fa-pen-nib mr-2"></i> 作品編輯</h2>
            <div class="space-y-3">
                <button class="w-full py-2 bg-[#f4ece4] hover:bg-[#eaddcf] transition rounded-lg">上傳新花禮</button>
                <button class="w-full py-2 bg-[#f4ece4] hover:bg-[#eaddcf] transition rounded-lg">管理現有庫存</button>
            </div>
        </section>

        <!-- 顧客管理系統 -->
        <section class="bg-white p-6 rounded-2xl shadow-sm border border-[#ede5dd]">
            <h2 class="text-lg mb-4 flex items-center"><i class="fa-solid fa-users mr-2"></i> 顧客管理</h2>
            <p class="text-sm text-gray-500 mb-2">本月新增會員: 24 位</p>
            <div class="h-1 bg-[#ede5dd] rounded-full overflow-hidden">
                <div class="h-full bg-[#c4a484] w-3/4"></div>
            </div>
        </section>

        <!-- 後台分析 -->
        <section class="bg-white p-6 rounded-2xl shadow-sm border border-[#ede5dd]">
            <h2 class="text-lg mb-4 flex items-center"><i class="fa-solid fa-chart-line mr-2"></i> 銷售分析</h2>
            <div class="text-2xl font-light text-[#8a7e72]">NT$ 128,400</div>
            <p class="text-xs text-gray-400">本月營收概況</p>
        </section>

        <!-- 折扣設定 -->
        <section class="bg-white p-6 rounded-2xl shadow-sm border border-[#ede5dd]">
            <h2 class="text-lg mb-4 flex items-center"><i class="fa-solid fa-tag mr-2"></i> 折扣設定</h2>
            <div class="flex items-center justify-between">
                <span class="text-sm">春日祭 9折</span>
                <input type="checkbox" checked class="accent-[#c4a484]">
            </div>
        </section>

    </main>

    <!-- 裝飾線 -->
    <div class="flower-border"></div>

    <!-- 商品展示預覽 -->
    <section class="mt-12">
        <h3 class="text-xl mb-8">精選花禮預覽</h3>
        <div class="grid grid-cols-1 sm:grid-cols-2 lg:grid-cols-3 gap-8">
            <!-- 卡片 1 -->
            <div class="bg-white p-2 rounded-xl border border-[#ede5dd]">
                <div class="h-48 bg-[#fdfaf6] mb-4 flex items-center justify-center text-[#d4c4b7]">圖片區</div>
                <h4 class="px-2 font-medium">晨曦之禮 - 永生花盒</h4>
                <p class="px-2 text-sm text-gray-400">NT$ 1,880</p>
            </div>
            <!-- 卡片 2 -->
            <div class="bg-white p-2 rounded-xl border border-[#ede5dd]">
                <div class="h-48 bg-[#fdfaf6] mb-4 flex items-center justify-center text-[#d4c4b7]">圖片區</div>
                <h4 class="px-2 font-medium">午後森林 - 鮮花束</h4>
                <p class="px-2 text-sm text-gray-400">NT$ 2,200</p>
            </div>
            <!-- 卡片 3 -->
            <div class="bg-white p-2 rounded-xl border border-[#ede5dd]">
                <div class="h-48 bg-[#fdfaf6] mb-4 flex items-center justify-center text-[#d4c4b7]">圖片區</div>
                <h4 class="px-2 font-medium">靜謐時光 - 乾燥花環</h4>
                <p class="px-2 text-sm text-gray-400">NT$ 1,550</p>
            </div>
        </div>
    </section>

    <footer class="mt-20 text-center text-xs text-[#c4a484]">
        © 2026 Das Wunderbar Florist. Design with elegance.
    </footer>

</body>
</html>
