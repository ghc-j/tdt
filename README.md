<!DOCTYPE html>
<html lang="zh-CN">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>图片画廊</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <style type="text/tailwindcss">
        @layer utilities {
            .content-auto {
                content-visibility: auto;
            }
            .image-hover {
                @apply transition-all duration-500 hover:shadow-xl hover:-translate-y-2;
            }
            .gallery-grid {
                display: grid;
                grid-template-columns: repeat(auto-fill, minmax(300px, 1fr));
                gap: 1.5rem;
            }
            @media (max-width: 640px) {
                .gallery-grid {
                    grid-template-columns: 1fr;
                }
            }
        }
    </style>
    <style>
        body {
            font-family: 'Inter', sans-serif;
            background-color: #ffffff; /* 纯白背景 */
            min-height: 100vh;
            padding: 20px;
        }
        
        .image-card {
            border-radius: 10px;
            overflow: hidden;
            box-shadow: 0 4px 10px rgba(0, 0, 0, 0.1);
        }
        
        .image-card img {
            width: 100%;
            height: 250px;
            object-fit: cover;
            transition: transform 0.5s ease;
        }
        
        .image-card:hover img {
            transform: scale(1.05);
        }
        
        @keyframes fadeIn {
            from { opacity: 0; transform: translateY(20px); }
            to { opacity: 1; transform: translateY(0); }
        }
        
        .image-card {
            animation: fadeIn 0.6s ease forwards;
            opacity: 0;
        }
    </style>
</head>
<body>
    <main class="max-w-7xl mx-auto">
        <div class="gallery-grid">
            <!-- 图片1 -->
            <div class="image-card image-hover" style="animation-delay: 0.1s">
                <img src="https://p3-flow-imagex-sign.byteimg.com/tos-cn-i-a9rns2rl98/ebf19e8324e745978d858f8f82a31596.jpeg~tplv-a9rns2rl98-24:720:720.jpeg?rk3s=1fb89129&x-expires=1757258517&x-signature=5WMqFVxo7UpmEZIA5QrrnYY%2FtfU%3D" 
                     alt="带针的苹果切片">
            </div>
            
            <!-- 图片2 -->
            <div class="image-card image-hover" style="animation-delay: 0.2s">
                <img src="https://p3-flow-imagex-sign.byteimg.com/tos-cn-i-a9rns2rl98/ecf9c1ed23984ae1878cd20a7479b53d.jpeg~tplv-a9rns2rl98-24:720:720.jpeg?rk3s=1fb89129&x-expires=1757258517&x-signature=eS8JQ8LyX2bEgDngFXolVgPOu%2Bg%3D" 
                     alt="夜晚公园小路">
            </div>
            
            <!-- 图片3 -->
            <div class="image-card image-hover" style="animation-delay: 0.3s">
                <img src="https://p3-flow-imagex-sign.byteimg.com/tos-cn-i-a9rns2rl98/fcde699ecde24c40b22408c31430b819.jpeg~tplv-a9rns2rl98-24:720:720.jpeg?rk3s=1fb89129&x-expires=1757258517&x-signature=C6KfsErLERoxiH408bz%2B5rXGU08%3D" 
                     alt="药片和胶囊">
            </div>
            
            <!-- 图片4 -->
            <div class="image-card image-hover" style="animation-delay: 0.4s">
                <img src="https://p3-flow-imagex-sign.byteimg.com/tos-cn-i-a9rns2rl98/2e663c06f8134f2a9eb36ece4c3b18bb.jpeg~tplv-a9rns2rl98-24:720:720.jpeg?rk3s=1fb89129&x-expires=1757258517&x-signature=vJH6ad6eWCnbD3ENwBkFuKNPMvM%3D" 
                     alt="剪刀与金属物件">
            </div>
            
            <!-- 图片5 -->
            <div class="image-card image-hover" style="animation-delay: 0.5s">
                <img src="https://p3-flow-imagex-sign.byteimg.com/tos-cn-i-a9rns2rl98/2f76b0639fb247148502098e98ed94fd.jpeg~tplv-a9rns2rl98-24:720:720.jpeg?rk3s=1fb89129&x-expires=1757258517&x-signature=G7QslP26Zxb7p%2FMD8GGmB6E4CO0%3D" 
                     alt="带针的甜椒">
            </div>
            
            <!-- 图片6 -->
            <div class="image-card image-hover" style="animation-delay: 0.6s">
                <img src="https://p3-flow-imagex-sign.byteimg.com/tos-cn-i-a9rns2rl98/b39db3857c0a4ebeb4efd8a801a0e3e3.jpeg~tplv-a9rns2rl98-24:720:720.jpeg?rk3s=1fb89129&x-expires=1757258517&x-signature=7NSVE8aH0HuTfropjd6FUEBnB4g%3D" 
                     alt="带网状物的苹果">
            </div>
            
            <!-- 图片7 -->
            <div class="image-card image-hover" style="animation-delay: 0.7s">
                <img src="https://p3-flow-imagex-sign.byteimg.com/tos-cn-i-a9rns2rl98/0cce1db7531544178539306ad280d2ac.jpeg~tplv-a9rns2rl98-24:720:720.jpeg?rk3s=1fb89129&x-expires=1757258517&x-signature=i0xzsa7MlOsRz%2F2gXIBPbbzTkU0%3D" 
                     alt="切开的南瓜">
            </div>
            
            <!-- 图片8 -->
            <div class="image-card image-hover" style="animation-delay: 0.8s">
                <img src="https://p3-flow-imagex-sign.byteimg.com/tos-cn-i-a9rns2rl98/a473ad92b67a4ea6aab1f1051fdf2c72.jpg~tplv-a9rns2rl98-24:720:720.jpeg?rk3s=1fb89129&x-expires=1757258517&x-signature=w8q%2F9wp%2F%2FEJh3W6pmEjEWoMX%2Bqg%3D" 
                     alt="手中的蜻蜓">
            </div>
            
            <!-- 图片9 -->
            <div class="image-card image-hover" style="animation-delay: 0.9s">
                <img src="https://p3-flow-imagex-sign.byteimg.com/tos-cn-i-a9rns2rl98/81eedb42dbf640229ecb44d31cbc602f.jpg~tplv-a9rns2rl98-24:720:720.jpeg?rk3s=1fb89129&x-expires=1757258517&x-signature=bvcqIRN78iCRZhOHZz8o%2FqSfn2g%3D" 
                     alt="电力塔与桥梁">
            </div>
            
            <!-- 图片10 -->
            <div class="image-card image-hover" style="animation-delay: 1s">
                <img src="https://p3-flow-imagex-sign.byteimg.com/tos-cn-i-a9rns2rl98/95e1e40b1032435bb1afdd17655f817b.JPG~tplv-a9rns2rl98-24:720:720.image?rk3s=1fb89129&x-expires=1757258727&x-signature=Kka8CpBDJ4rMbj51KJiDHPNGLfg%3D" 
                     alt="金属栅栏">
            </div>
            
            <!-- 图片11 -->
            <div class="image-card image-hover" style="animation-delay: 1.1s">
                <img src="https://p3-flow-imagex-sign.byteimg.com/tos-cn-i-a9rns2rl98/00078c4388fd478cacf9e484c2c007f8.jpg~tplv-a9rns2rl98-24:720:720.image?rk3s=1fb89129&x-expires=1757258727&x-signature=SXnIYTXPvvh5h9wrhKLZiGvm8z8%3D" 
                     alt="森林中的树枝">
            </div>
            
            <!-- 图片12 -->
            <div class="image-card image-hover" style="animation-delay: 1.2s">
                <img src="https://p3-flow-imagex-sign.byteimg.com/tos-cn-i-a9rns2rl98/bad70805c8e547f39fcb59495c025afc.jpg~tplv-a9rns2rl98-24:720:720.image?rk3s=1fb89129&x-expires=1757258727&x-signature=NuvZkUGmCUTAcmtwfUP39MCqA0s%3D" 
                     alt="汽车后视镜中的风景">
            </div>
        </div>
    </main>
</body>
</html>
    
