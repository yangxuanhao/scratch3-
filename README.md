<html lang="zh-CN"><head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Scratch 下载</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <link href="https://cdn.jsdelivr.net/npm/font-awesome@4.7.0/css/font-awesome.min.css" rel="stylesheet">
    <script>
        tailwind.config = {
            theme: {
                extend: {
                    colors: {
                        scratch: {
                            yellow: '#FFCC00',
                            blue: '#0096FF',
                            green: '#34D399',
                            purple: '#933EA',
                            orange: '#F97316',
                            dark: '#1E293B',
                            sky: '#87CEEB',
                            deepblue: '#1E40AF',
                            lightblue: '#2563EB'
                        }
                    },
                    fontFamily: {
                        scratch: ['Helvetica', 'Arial', 'sans-serif']
                    }
                }
            }
        }
    </script>
    <style type="text/tailwindcss">
        @layer utilities {
            .text-shadow {
                text-shadow: 0 2px 4px rgba(0,0,0,0.1);
            }
            .transition-bounce {
                transition-timing-function: cubic-bezier(0.34, 1.56, 0.64, 1);
            }
            .card-fade {
                animation: fadeIn 0.6s ease forwards;
            }
            @keyframes fadeIn {
                from { opacity: 0; transform: translateY(20px); }
                to { opacity: 1; transform: translateY(0); }
            }
        }
    </style>
</head>
<body class="bg-scratch-lightblue min-h-screen font-scratch">
    <!-- 导航栏 -->
    <header class="sticky top-0 z-50 bg-white/80 backdrop-blur-sm shadow-sm transition-all duration-300">
        <div class="container mx-auto px-4 py-3 flex justify-between items-center">
            <div class="flex items-center space-x-2">
                <img src="https://p3-flow-imagex-sign.byteimg.com/tos-cn-i-a9rns2rl98/rc/pc/code_assistant/3c39e3935d67413c853444501f76661e~tplv-a9rns2rl98-image.image?rcl=2025091222482042580A7F54F79D88052D&amp;rk3s=8e244e95&amp;rrcfp=e75484ac&amp;x-expires=1758293301&amp;x-signature=zYRXOab6bagactl0Wzo7qfm8hAg%3D" alt="Scratch Logo" class="w-10 h-10 rounded-full">
                <h1 class="text-xl font-bold text-scratch-dark hidden sm:block">Scratch</h1>
            </div>
            <nav class="hidden md:flex items-center">
                <a href="#download-card" class="text-scratch-blue font-medium download-link">下载</a>
            </nav>
            <button class="md:hidden text-gray-600 mobile-menu-button">
                <i class="fa fa-bars text-xl"></i>
            </button>
        </div>
        <!-- 移动端菜单 -->
        <div class="md:hidden hidden mobile-menu bg-white shadow-md">
            <div class="container mx-auto px-4 py-2">
                <a href="#download-card" class="block py-2 text-scratch-blue font-medium download-link">下载</a>
            </div>
        </div>
    </header>

    <!-- 主内容区 -->
    <main class="container mx-auto px-4 py-12 md:py-20">
        <!-- 标题区域 -->
        <div class="text-center mb-16">
            <h2 class="text-[clamp(2rem,5vw,3.5rem)] font-bold text-white mb-4 text-shadow">
                下载 Scratch
            </h2>
            <p class="text-blue-100 text-lg md:text-xl max-w-2xl mx-auto">
                离线创作、编程和分享你的Scratch项目，随时随地发挥创意
            </p>
        </div>

        <!-- 下载卡片 - 添加ID用于定位 -->
        <div id="download-card" class="max-w-4xl mx-auto bg-white rounded-2xl shadow-xl overflow-hidden transform transition-all duration-500 hover:shadow-2xl hover:-translate-y-1">
            <div class="md:flex">
                <!-- 左侧图片（放大且只保留一张） -->
                <div class="md:w-1/2 bg-gradient-to-br from-scratch-blue/10 to-scratch-purple/10 p-6 flex items-center justify-center">
                    <div class="w-full max-w-lg relative">
                        <div class="aspect-video bg-white rounded-xl shadow-xl overflow-hidden border-6 border-gray-800 relative z-10 transform transition-transform duration-500 hover:scale-[1.02]">
                            <img src="https://p3-flow-imagex-sign.byteimg.com/tos-cn-i-a9rns2rl98/rc/pc/code_assistant/21324259fcb24e5d83be75464531c842~tplv-a9rns2rl98-image.image?rcl=20250913135244A289DDCB1FE963F941B9&amp;rk3s=8e244e95&amp;rrcfp=e75484ac&amp;x-expires=1758347564&amp;x-signature=CzRTYW%2FLrnG%2F%2B1oZ%2BX1na48vjZs%3D" alt="Scratch项目编辑界面" class="w-full h-full object-cover">
                        </div>
                    </div>
                </div>
                
                <!-- 右侧下载信息 -->
                <div class="md:w-1/2 p-8 md:p-10 flex flex-col justify-center">
                    <div class="mb-6">
                        <div class="flex items-center space-x-3 mb-2">
                            <div class="w-3 h-3 rounded-full bg-scratch-green"></div>
                            <span class="text-scratch-dark font-medium">最新版本</span>
                        </div>
                        <h3 class="text-2xl font-bold text-scratch-dark">Scratch 3.29.1</h3>
                        <p class="text-gray-500 mt-1">发布于 2023年10月15日</p>
                    </div>
                    
                    <div class="space-y-4 mb-8">
                        <div class="flex items-start space-x-3">
                            <i class="fa fa-check-circle text-scratch-green mt-1"></i>
                            <p class="text-gray-600">离线创建和编辑Scratch项目</p>
                        </div>
                        <div class="flex items-start space-x-3">
                            <i class="fa fa-check-circle text-scratch-green mt-1"></i>
                            <p class="text-gray-600">支持所有Scratch功能和扩展</p>
                        </div>
                        <div class="flex items-start space-x-3">
                            <i class="fa fa-check-circle text-scratch-green mt-1"></i>
                            <p class="text-gray-600">创作不受网络连接限制</p>
                        </div>
                    </div>
                    
                    <div class="space-y-3">
                        <!-- Windows下载按钮 - 迅雷云盘链接 -->
                        <a href="https://pan.xunlei.com/s/VO_0yOT-JW13nOAW7XqPElI_A1?pwd=rm38#" target="_blank" class="w-full bg-scratch-blue hover:bg-scratch-blue/90 text-white font-medium py-3 px-6 rounded-lg flex items-center justify-center space-x-2 transition-all duration-300 hover:shadow-lg">
                            <i class="fa fa-download"></i>
                            <span>下载适用于 Windows</span>
                        </a>
                        
                        <!-- macOS下载按钮 - 迅雷云盘链接 -->
                        <a href="https://pan.xunlei.com/s/VO_0z8vGABlTtFE_xn3kj-3HA1?pwd=z64s" target="_blank" class="w-full bg-gray-200 hover:bg-gray-300 text-gray-800 font-medium py-3 px-6 rounded-lg flex items-center justify-center space-x-2 transition-all duration-300">
                            <i class="fa fa-apple"></i>
                            <span>下载适用于 macOS</span>
                        </a>
                        
                        <button class="w-full bg-scratch-orange hover:bg-scratch-orange/90 text-white font-medium py-3 px-6 rounded-lg flex items-center justify-center space-x-2 transition-all duration-300 hover:shadow-lg">
                            <i class="fa fa-heart"></i>
                            <span>支持我们 - 捐赠</span>
                        </button>
                    </div>
                </div>
            </div>
        </div>

        <!-- 系统要求 -->
        <div class="mt-16 max-w-4xl mx-auto bg-white rounded-2xl shadow-md p-8 transform transition-all duration-500 hover:shadow-xl hover:-translate-y-1">
            <h3 class="text-2xl font-bold text-scratch-dark mb-6">系统要求</h3>
            
            <div class="grid md:grid-cols-2 gap-8">
                <div class="p-4 rounded-xl transition-all duration-300 hover:bg-gray-50">
                    <h4 class="font-bold text-lg mb-4 flex items-center">
                        <i class="fa fa-windows text-gray-600 mr-2"></i>
                        Windows
                    </h4>
                    <ul class="space-y-2 text-gray-600">
                        <li class="flex items-start">
                            <i class="fa fa-circle text-xs text-gray-400 mt-1.5 mr-2"></i>
                            <span>Windows 7 或更高版本</span>
                        </li>
                        <li class="flex items-start">
                            <i class="fa fa-circle text-xs text-gray-400 mt-1.5 mr-2"></i>
                            <span>至少 1GB RAM</span>
                        </li>
                        <li class="flex items-start">
                            <i class="fa fa-circle text-xs text-gray-400 mt-1.5 mr-2"></i>
                            <span>至少 500MB 可用存储空间</span>
                        </li>
                    </ul>
                </div>
                
                <div class="p-4 rounded-xl transition-all duration-300 hover:bg-gray-50">
                    <h4 class="font-bold text-lg mb-4 flex items-center">
                        <i class="fa fa-apple text-gray-600 mr-2"></i>
                        macOS
                    </h4>
                    <ul class="space-y-2 text-gray-600">
                        <li class="flex items-start">
                            <i class="fa fa-circle text-xs text-gray-400 mt-1.5 mr-2"></i>
                            <span>macOS 10.13 或更高版本</span>
                        </li>
                        <li class="flex items-start">
                            <i class="fa fa-circle text-xs text-gray-400 mt-1.5 mr-2"></i>
                            <span>至少 1GB RAM</span>
                        </li>
                        <li class="flex items-start">
                            <i class="fa fa-circle text-xs text-gray-400 mt-1.5 mr-2"></i>
                            <span>至少 500MB 可用存储空间</span>
                        </li>
                    </ul>
                </div>
            </div>
        </div>
    </main>

    <!-- 页脚 -->
    <footer class="bg-scratch-dark text-white mt-20">
        <div class="container mx-auto px-4 py-12">
            <div class="grid grid-cols-1 md:grid-cols-2 gap-8">
                <div>
                    <div class="flex items-center space-x-2 mb-4">
                        <img src="https://p3-flow-imagex-sign.byteimg.com/tos-cn-i-a9rns2rl98/rc/pc/code_assistant/9101cb14124e4fbda6caf888b0b9e1c3~tplv-a9rns2rl98-image.image?rcl=20250913134941A2EFAE903A0D3BE51C2C&amp;rk3s=8e244e95&amp;rrcfp=e75484ac&amp;x-expires=1758347381&amp;x-signature=d480F%2FeOMCgZCDZp1%2FMrBYz%2FF6Y%3D" alt="Scratch Logo" class="w-8 h-8 rounded-full">
                        <h3 class="font-bold">Scratch</h3>
                    </div>
                    <p class="text-gray-400 text-sm">
                        Scratch是一个让你可以创建自己的互动故事、游戏和动画的编程语言和在线社区。
                    </p>
                </div>
                
                <div>
                    <h4 class="font-bold mb-4">联系我们</h4>
                    <ul class="space-y-2 text-gray-400 text-sm">
                        <li><a href="mailto:yxh120521@qq.com" class="hover:text-white transition-colors">yxh120521@qq.com</a></li>
                        <li><a href="#" class="hover:text-white transition-colors">反馈建议</a></li>
                    </ul>
                    <div class="flex space-x-4 mt-4">
                        <a href="#" class="text-gray-400 hover:text-white transition-colors">
                            <i class="fa fa-facebook"></i>
                        </a>
                        <a href="#" class="text-gray-400 hover:text-white transition-colors">
                            <i class="fa fa-twitter"></i>
                        </a>
                        <a href="#" class="text-gray-400 hover:text-white transition-colors">
                            <i class="fa fa-youtube-play"></i>
                        </a>
                        <a href="#" class="text-gray-400 hover:text-white transition-colors">
                            <i class="fa fa-instagram"></i>
                        </a>
                    </div>
                </div>
            </div>
            
            <div class="border-t border-gray-700 mt-8 pt-8 text-center text-gray-500 text-sm">
                <p>© 2025 Yang Xuanhao. 保留所有权利.</p>
            </div>
        </div>
    </footer>

    <!-- 捐赠模态框 -->
    <div id="donationModal" class="fixed inset-0 bg-black/70 z-50 hidden flex items-center justify-center p-4">
        <div class="bg-white rounded-2xl max-w-md w-full p-6 md:p-8 shadow-2xl transform transition-all">
            <div class="flex justify-between items-start mb-4">
                <h3 class="text-2xl font-bold text-scratch-dark">支持 Scratch</h3>
                <button id="closeDonationModal" class="text-gray-500 hover:text-gray-800 transition-colors">
                    <i class="fa fa-times text-xl"></i>
                </button>
            </div>
            
            <div class="mb-6 relative w-full" style="padding-top: 100%;">
                <img src="https://p3-flow-imagex-sign.byteimg.com/tos-cn-i-a9rns2rl98/rc/pc/code_assistant/846f4483e648419a91f0e07e39c7d01e~tplv-a9rns2rl98-image.image?rcl=20250913140828E6558427B4C2B2E50033&amp;rk3s=8e244e95&amp;rrcfp=e75484ac&amp;x-expires=1758348508&amp;x-signature=wF51BtgsnFGzEMjsFM10Vk9v7vk%3D" alt="孩子们使用Scratch编程的场景" class="absolute top-0 left-0 w-full h-full object-cover rounded-lg">
            </div>
            
            <p class="text-gray-600 mb-6">您的捐赠将帮助我们继续开发和维护Scratch平台，支持创意编程教育的发展。所有捐赠者都会被留下名字。</p>
            
            <button id="completeDonation" class="w-full bg-scratch-orange hover:bg-scratch-orange/90 text-white font-medium py-3 px-4 rounded-lg transition-colors">完成捐赠</button>
        </div>
    </div>

    <!-- JavaScript -->
    <script>
        // 导航栏滚动效果
        window.addEventListener('scroll', function() {
            const header = document.querySelector('header');
            if (window.scrollY > 50) {
                header.classList.add('py-2', 'shadow');
                header.classList.remove('py-3', 'shadow-sm');
            } else {
                header.classList.add('py-3', 'shadow-sm');
                header.classList.remove('py-2', 'shadow');
            }
        });

        // 移动端菜单切换
        const mobileMenuButton = document.querySelector('.mobile-menu-button');
        const mobileMenu = document.querySelector('.mobile-menu');
        
        mobileMenuButton.addEventListener('click', function() {
            mobileMenu.classList.toggle('hidden');
        });

        // 导航"下载"链接点击效果 - 滚动到下载卡片并高亮显示
        const downloadLinks = document.querySelectorAll('.download-link');
        const downloadCard = document.getElementById('download-card');
        
        downloadLinks.forEach(link => {
            link.addEventListener('click', function(e) {
                e.preventDefault();
                
                // 关闭移动端菜单（如果打开）
                if (!mobileMenu.classList.contains('hidden')) {
                    mobileMenu.classList.add('hidden');
                }
                
                // 滚动到下载卡片
                downloadCard.scrollIntoView({
                    behavior: 'smooth',
                    block: 'start'
                });
                
                // 添加高亮动画效果
                downloadCard.classList.add('card-fade', 'shadow-2xl');
                setTimeout(() => {
                    downloadCard.classList.remove('shadow-2xl');
                }, 1000);
            });
        });

        // 捐赠模态框功能
        const donationButton = document.querySelector('button:has(.fa-heart)');
        const donationModal = document.getElementById('donationModal');
        const closeDonationModal = document.getElementById('closeDonationModal');
        const completeDonationButton = document.getElementById('completeDonation');

        // 打开捐赠模态框
        donationButton.addEventListener('click', function() {
            donationModal.classList.remove('hidden');
            document.body.style.overflow = 'hidden';
        });

        // 关闭捐赠模态框的函数
        function closeModal() {
            donationModal.classList.add('hidden');
            document.body.style.overflow = 'auto';
        }

        // 关闭按钮事件
        closeDonationModal.addEventListener('click', closeModal);

        // 完成捐赠按钮事件 - 关闭模态框
        completeDonationButton.addEventListener('click', function() {
            alert('感谢您的支持！捐赠流程已完成。');
            closeModal();
        });

        // 点击模态框外部关闭
        donationModal.addEventListener('click', (e) => {
            if (e.target === donationModal) {
                closeModal();
            }
        });

        // 按钮点击效果
        const buttons = document.querySelectorAll('button, a[href]');
        buttons.forEach(button => {
            button.addEventListener('click', function() {
                this.classList.add('scale-95');
                setTimeout(() => {
                    this.classList.remove('scale-95');
                }, 200);
            });
        });
    </script>
    
    </body></html>
