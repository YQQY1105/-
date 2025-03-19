<!DOCTYPE html>
<html lang="zh-CN">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>政务服务 App 原型</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <style>
        body {
            font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, Helvetica, Arial, sans-serif;
        }
        .ios-status-bar {
            height: 44px;
        }
        .ios-home-indicator {
            height: 34px;
        }
        .ios-screen {
            width: 375px;
            height: 812px;
            overflow: hidden;
            position: relative;
        }
        .shadow-top {
            box-shadow: 0 -2px 10px rgba(0, 0, 0, 0.05);
        }
    </style>
</head>
<body class="bg-gray-100 p-6">
    <div class="max-w-6xl mx-auto">
        <h1 class="text-3xl font-bold text-center mb-10 text-blue-700">政务服务 App 原型设计</h1>
        
        <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-8">
            
            <!-- 欢迎页 -->
            <div class="ios-screen bg-white rounded-3xl shadow-lg overflow-hidden">
                <div class="ios-status-bar bg-white flex justify-between items-center px-6">
                    <span class="text-sm font-semibold">9:41</span>
                    <div class="flex space-x-2">
                        <svg xmlns="http://www.w3.org/2000/svg" class="h-4 w-4" fill="none" viewBox="0 0 24 24" stroke="currentColor">
                            <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M8 7H5a2 2 0 00-2 2v9a2 2 0 002 2h14a2 2 0 002-2V9a2 2 0 00-2-2h-3m-1 4l-3 3m0 0l-3-3m3 3V4" />
                        </svg>
                        <svg xmlns="http://www.w3.org/2000/svg" class="h-4 w-4" fill="none" viewBox="0 0 24 24" stroke="currentColor">
                            <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M12 18h.01M8 21h8a2 2 0 002-2V5a2 2 0 00-2-2H8a2 2 0 00-2 2v14a2 2 0 002 2z" />
                        </svg>
                    </div>
                </div>
                <div class="h-full flex flex-col justify-between">
                    <div class="flex-1 flex flex-col items-center justify-center px-8">
                        <img src="https://images.unsplash.com/photo-1584964422129-89b567b03239?ixlib=rb-1.2.1&auto=format&fit=crop&w=200&q=80" alt="Logo" class="w-32 h-32 object-cover mb-8 rounded-2xl shadow-md">
                        <h1 class="text-3xl font-bold text-blue-600 mb-4">政务服务</h1>
                        <p class="text-gray-500 text-center mb-8">便捷、高效、智能的政务服务平台</p>
                        <button class="w-full bg-blue-600 text-white py-3 rounded-lg font-medium mb-3">登录</button>
                        <button class="w-full border border-blue-600 text-blue-600 py-3 rounded-lg font-medium">注册</button>
                        <p class="mt-6 text-xs text-gray-400">可使用人脸识别、指纹或短信验证码快捷登录</p>
                    </div>
                    <div class="ios-home-indicator flex justify-center pb-2">
                        <div class="w-32 h-1 bg-gray-300 rounded-full"></div>
                    </div>
                </div>
            </div>
            
            <!-- 首页 -->
            <div class="ios-screen bg-gray-50 rounded-3xl shadow-lg overflow-hidden">
                <div class="ios-status-bar bg-white flex justify-between items-center px-6">
                    <span class="text-sm font-semibold">9:41</span>
                    <div class="flex space-x-2">
                        <svg xmlns="http://www.w3.org/2000/svg" class="h-4 w-4" fill="none" viewBox="0 0 24 24" stroke="currentColor">
                            <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M8 7H5a2 2 0 00-2 2v9a2 2 0 002 2h14a2 2 0 002-2V9a2 2 0 00-2-2h-3m-1 4l-3 3m0 0l-3-3m3 3V4" />
                        </svg>
                        <svg xmlns="http://www.w3.org/2000/svg" class="h-4 w-4" fill="none" viewBox="0 0 24 24" stroke="currentColor">
                            <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M12 18h.01M8 21h8a2 2 0 002-2V5a2 2 0 00-2-2H8a2 2 0 00-2 2v14a2 2 0 002 2z" />
                        </svg>
                    </div>
                </div>
                <div class="h-full flex flex-col">
                    <!-- 头部搜索区域 -->
                    <div class="bg-blue-600 px-4 pt-2 pb-6">
                        <div class="flex items-center justify-between mb-4">
                            <div class="flex items-center">
                                <h2 class="text-white text-xl font-bold">您好，张先生</h2>
                                <span class="ml-2 px-2 py-1 bg-blue-500 rounded-full text-xs text-white">已实名</span>
                            </div>
                            <div class="flex space-x-3">
                                <svg xmlns="http://www.w3.org/2000/svg" class="h-6 w-6 text-white" fill="none" viewBox="0 0 24 24" stroke="currentColor">
                                    <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M15 17h5l-1.405-1.405A2.032 2.032 0 0118 14.158V11a6.002 6.002 0 00-4-5.659V5a2 2 0 10-4 0v.341C7.67 6.165 6 8.388 6 11v3.159c0 .538-.214 1.055-.595 1.436L4 17h5m6 0v1a3 3 0 11-6 0v-1m6 0H9" />
                                </svg>
                                <svg xmlns="http://www.w3.org/2000/svg" class="h-6 w-6 text-white" fill="none" viewBox="0 0 24 24" stroke="currentColor">
                                    <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M7 8h10M7 12h4m1 8l-4-4H5a2 2 0 01-2-2V6a2 2 0 012-2h14a2 2 0 012 2v8a2 2 0 01-2 2h-3l-4 4z" />
                                </svg>
                            </div>
                        </div>
                        <div class="relative">
                            <input type="text" placeholder="搜索政务服务" class="w-full py-2 pl-10 pr-4 bg-white bg-opacity-20 text-white placeholder-white placeholder-opacity-70 rounded-lg focus:outline-none">
                            <svg xmlns="http://www.w3.org/2000/svg" class="h-5 w-5 absolute left-3 top-2.5 text-white opacity-70" fill="none" viewBox="0 0 24 24" stroke="currentColor">
                                <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M21 21l-6-6m2-5a7 7 0 11-14 0 7 7 0 0114 0z" />
                            </svg>
                        </div>
                    </div>
                    
                    <!-- 内容区域 -->
                    <div class="flex-1 overflow-auto px-4 pt-4">
                        <!-- 轮播图 -->
                        <div class="rounded-lg overflow-hidden mb-4 h-32 relative">
                            <img src="https://images.unsplash.com/photo-1517245386807-bb43f82c33c4?ixlib=rb-1.2.1&auto=format&fit=crop&w=375&q=80" class="w-full h-full object-cover" alt="Banner">
                            <div class="absolute bottom-2 right-2 bg-black bg-opacity-30 text-white text-xs px-2 py-1 rounded-full">
                                1/3
                            </div>
                        </div>
                        
                        <!-- 快捷服务 -->
                        <div class="bg-white rounded-lg p-4 mb-4">
                            <h3 class="text-base font-bold mb-3">快捷服务</h3>
                            <div class="grid grid-cols-4 gap-3">
                                <div class="flex flex-col items-center">
                                    <div class="w-12 h-12 bg-blue-50 rounded-full flex items-center justify-center mb-1">
                                        <svg xmlns="http://www.w3.org/2000/svg" class="h-6 w-6 text-blue-500" fill="none" viewBox="0 0 24 24" stroke="currentColor">
                                            <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M10 6H5a2 2 0 00-2 2v9a2 2 0 002 2h14a2 2 0 002-2V8a2 2 0 00-2-2h-5m-4 0V5a2 2 0 114 0v1m-4 0a2 2 0 104 0m-5 8a2 2 0 100-4 2 2 0 000 4zm0 0c1.306 0 2.417.835 2.83 2M9 14a3.001 3.001 0 00-2.83 2M15 11h3m-3 4h2" />
                                        </svg>
                                    </div>
                                    <span class="text-xs">身份证办理</span>
                                </div>
                                <div class="flex flex-col items-center">
                                    <div class="w-12 h-12 bg-green-50 rounded-full flex items-center justify-center mb-1">
                                        <svg xmlns="http://www.w3.org/2000/svg" class="h-6 w-6 text-green-500" fill="none" viewBox="0 0 24 24" stroke="currentColor">
                                            <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M3 12l2-2m0 0l7-7 7 7M5 10v10a1 1 0 001 1h3m10-11l2 2m-2-2v10a1 1 0 01-1 1h-3m-6 0a1 1 0 001-1v-4a1 1 0 011-1h2a1 1 0 011 1v4a1 1 0 001 1m-6 0h6" />
                                        </svg>
                                    </div>
                                    <span class="text-xs">不动产登记</span>
                                </div>
                                <div class="flex flex-col items-center">
                                    <div class="w-12 h-12 bg-red-50 rounded-full flex items-center justify-center mb-1">
                                        <svg xmlns="http://www.w3.org/2000/svg" class="h-6 w-6 text-red-500" fill="none" viewBox="0 0 24 24" stroke="currentColor">
                                            <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M9 5H7a2 2 0 00-2 2v12a2 2 0 002 2h10a2 2 0 002-2V7a2 2 0 00-2-2h-2M9 5a2 2 0 002 2h2a2 2 0 002-2M9 5a2 2 0 012-2h2a2 2 0 012 2" />
                                        </svg>
                                    </div>
                                    <span class="text-xs">证明开具</span>
                                </div>
                                <div class="flex flex-col items-center">
                                    <div class="w-12 h-12 bg-purple-50 rounded-full flex items-center justify-center mb-1">
                                        <svg xmlns="http://www.w3.org/2000/svg" class="h-6 w-6 text-purple-500" fill="none" viewBox="0 0 24 24" stroke="currentColor">
                                            <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M9 12l2 2 4-4m5.618-4.016A11.955 11.955 0 0112 2.944a11.955 11.955 0 01-8.618 3.04A12.02 12.02 0 003 9c0 5.591 3.824 10.29 9 11.622 5.176-1.332 9-6.03 9-11.622 0-1.042-.133-2.052-.382-3.016z" />
                                        </svg>
                                    </div>
                                    <span class="text-xs">社保查询</span>
                                </div>
                                <div class="flex flex-col items-center">
                                    <div class="w-12 h-12 bg-yellow-50 rounded-full flex items-center justify-center mb-1">
                                        <svg xmlns="http://www.w3.org/2000/svg" class="h-6 w-6 text-yellow-500" fill="none" viewBox="0 0 24 24" stroke="currentColor">
                                            <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M3 10h18M7 15h1m4 0h1m-7 4h12a3 3 0 003-3V8a3 3 0 00-3-3H6a3 3 0 00-3 3v8a3 3 0 003 3z" />
                                        </svg>
                                    </div>
                                    <span class="text-xs">税费缴纳</span>
                                </div>
                                <div class="flex flex-col items-center">
                                    <div class="w-12 h-12 bg-indigo-50 rounded-full flex items-center justify-center mb-1">
                                        <svg xmlns="http://www.w3.org/2000/svg" class="h-6 w-6 text-indigo-500" fill="none" viewBox="0 0 24 24" stroke="currentColor">
                                            <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M8 7V3m8 4V3m-9 8h10M5 21h14a2 2 0 002-2V7a2 2 0 00-2-2H5a2 2 0 00-2 2v12a2 2 0 002 2z" />
                                        </svg>
                                    </div>
                                    <span class="text-xs">预约办理</span>
                                </div>
                                <div class="flex flex-col items-center">
                                    <div class="w-12 h-12 bg-pink-50 rounded-full flex items-center justify-center mb-1">
                                        <svg xmlns="http://www.w3.org/2000/svg" class="h-6 w-6 text-pink-500" fill="none" viewBox="0 0 24 24" stroke="currentColor">
                                            <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M12 8v4l3 3m6-3a9 9 0 11-18 0 9 9 0 0118 0z" />
                                        </svg>
                                    </div>
                                    <span class="text-xs">进度查询</span>
                                </div>
                                <div class="flex flex-col items-center">
                                    <div class="w-12 h-12 bg-gray-50 rounded-full flex items-center justify-center mb-1">
                                        <svg xmlns="http://www.w3.org/2000/svg" class="h-6 w-6 text-gray-500" fill="none" viewBox="0 0 24 24" stroke="currentColor">
                                            <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M5 12h.01M12 12h.01M19 12h.01M6 12a1 1 0 11-2 0 1 1 0 012 0zm7 0a1 1 0 11-2 0 1 1 0 012 0zm7 0a1 1 0 11-2 0 1 1 0 012 0z" />
                                        </svg>
                                    </div>
                                    <span class="text-xs">更多服务</span>
                                </div>
                            </div>
                        </div>
                        
                        <!-- 便民服务 -->
                        <div class="bg-white rounded-lg p-4 mb-4">
                            <div class="flex justify-between items-center mb-3">
                                <h3 class="text-base font-bold">便民服务</h3>
                                <span class="text-xs text-gray-400">更多 ></span>
                            </div>
                            <div class="grid grid-cols-2 gap-3">
                                <div class="bg-blue-50 rounded-lg p-3 flex items-center">
                                    <div class="w-10 h-10 bg-blue-500 rounded-lg flex items-center justify-center mr-3">
                                        <svg xmlns="http://www.w3.org/2000/svg" class="h-5 w-5 text-white" fill="none" viewBox="0 0 24 24" stroke="currentColor">
                                            <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M13 16h-1v-4h-1m1-4h.01M21 12a9 9 0 11-18 0 9 9 0 0118 0z" />
                                        </svg>
                                    </div>
                                    <div>
                                        <h4 class="text-sm font-medium">政策咨询</h4>
                                        <p class="text-xs text-gray-500">最新政策解读</p>
                                    </div>
                                </div>
                                <div class="bg-green-50 rounded-lg p-3 flex items-center">
                                    <div class="w-10 h-10 bg-green-500 rounded-lg flex items-center justify-center mr-3">
                                        <svg xmlns="http://www.w3.org/2000/svg" class="h-5 w-5 text-white" fill="none" viewBox="0 0 24 24" stroke="currentColor">
                                            <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M9 5H7a2 2 0 00-2 2v12a2 2 0 002 2h10a2 2 0 002-2V7a2 2 0 00-2-2h-2M9 5a2 2 0 002 2h2a2 2 0 002-2M9 5a2 2 0 012-2h2a2 2 0 012 2m-3 7h3m-3 4h3m-6-4h.01M9 16h.01" />
                                        </svg>
                                    </div>
                                    <div>
                                        <h4 class="text-sm font-medium">办事指南</h4>
                                        <p class="text-xs text-gray-500">流程一目了然</p>
                                    </div>
                                </div>
                            </div>
                        </div>
                        
                        <!-- 热门服务 -->
                        <div class="bg-white rounded-lg p-4 mb-4">
                            <div class="flex justify-between items-center mb-3">
                                <h3 class="text-base font-bold">热门服务</h3>
                                <span class="text-xs text-gray-400">更多 ></span>
                            </div>
                            <div class="space-y-3">
                                <div class="flex items-center bg-gray-50 p-3 rounded-lg">
                                    <div class="w-12 h-12 bg-orange-500 rounded-lg flex items-center justify-center mr-3">
                                        <svg xmlns="http://www.w3.org/2000/svg" class="h-6 w-6 text-white" fill="none" viewBox="0 0 24 24" stroke="currentColor">
                                            <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M12 4.354a4 4 0 110 5.292M15 21H3v-1a6 6 0 0112 0v1zm0 0h6v-1a6 6 0 00-9-5.197M13 7a4 4 0 11-8 0 4 4 0 018 0z" />
                                        </svg>
                                    </div>
                                    <div>
                                        <h4 class="text-sm font-medium">户籍管理</h4>
                                        <p class="text-xs text-gray-500">随迁入户、户口迁移</p>
                                    </div>
                                    <div class="ml-auto">
                                        <span class="text-xs text-blue-500">立即办理 ></span>
                                    </div>
                                </div>
                                <div class="flex items-center bg-gray-50 p-3 rounded-lg">
                                    <div class="w-12 h-12 bg-blue-500 rounded-lg flex items-center justify-center mr-3">
                                        <svg xmlns="http://www.w3.org/2000/svg" class="h-6 w-6 text-white" fill="none" viewBox="0 0 24 24" stroke="currentColor">
                                            <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M3 12l2-2m0 0l7-7 7 7M5 10v10a1 1 0 001 1h3m10-11l2 2m-2-2v10a1 1 0 01-1 1h-3m-6 0a1 1 0 001-1v-4a1 1 0 011-1h2a1 1 0 011 1v4a1 1 0 001 1m-6 0h6" />
                                        </svg>
                                    </div>
                                    <div>
                                        <h4 class="text-sm font-medium">住房公积金</h4>
                                        <p class="text-xs text-gray-500">查询、提取、贷款</p>
                                    </div>
                                    <div class="ml-auto">
                                        <span class="text-xs text-blue-500">立即办理 ></span>
                                    </div>
                                </div>
                            </div>
                        </div>
                    </div>
                    
                    <!-- 底部导航 -->
                    <div class="bg-white shadow-top flex justify-around py-2">
                        <div class="flex flex-col items-center">
                            <svg xmlns="http://www.w3.org/2000/svg" class="h-6 w-6 text-blue-600" fill="none" viewBox="0 0 24 24" stroke="currentColor">
                                <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M3 12l2-2m0 0l7-7 7 7M5 10v10a1 1 0 001 1h3m10-11l2 2m-2-2v10a1 1 0 01-1 1h-3m-6 0a1 1 0 001-1v-4a1 1 0 011-1h2a1 1 0 011 1v4a1 1 0 001 1m-6 0h6" />
                            </svg>
                            <span class="text-xs text-blue-600 font-medium">首页</span>
                        </div>
                        <div class="flex flex-col items-center">
                            <svg xmlns="http://www.w3.org/2000/svg" class="h-6 w-6 text-gray-400" fill="none" viewBox="0 0 24 24" stroke="currentColor">
                                <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M9 5H7a2 2 0 00-2 2v12a2 2 0 002 2h10a2 2 0 002-2V7a2 2 0 00-2-2h-2M9 5a2 2 0 002 2h2a2 2 0 002-2M9 5a2 2 0 012-2h2a2 2 0 012 2" />
                            </svg>
                            <span class="text-xs text-gray-400">全部服务</span>
                        </div>
                        <div class="flex flex-col items-center">
                            <svg xmlns="http://www.w3.org/2000/svg" class="h-6 w-6 text-gray-400" fill="none" viewBox="0 0 24 24" stroke="currentColor">
                                <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M8 10h.01M12 10h.01M16 10h.01M9 16H5a2 2 0 01-2-2V6a2 2 0 012-2h14a2 2 0 012 2v8a2 2 0 01-2 2h-5l-5 5v-5z" />
                            </svg>
                            <span class="text-xs text-gray-400">消息</span>
                        </div>
                        <div class="flex flex-col items-center">
                            <svg xmlns="http://www.w3.org/2000/svg" class="h-6 w-6 text-gray-400" fill="none" viewBox="0 0 24 24" stroke="currentColor">
                                <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M16 7a4 4 0 11-8 0 4 4 0 018 0zM12 14a7 7 0 00-7 7h14a7 7 0 00-7-7z" />
                            </svg>
                            <span class="text-xs text-gray-400">我的</span>
                        </div>
                    </div>
                </div>
            </div>
            
            <!-- 服务详情页 -->
            <div class="ios-screen bg-gray-50 rounded-3xl shadow-lg overflow-hidden">
                <div class="ios-status-bar bg-white flex justify-between items-center px-6">
                    <span class="text-sm font-semibold">9:41</span>
                    <div class="flex space-x-2">
                        <svg xmlns="http://www.w3.org/2000/svg" class="h-4 w-4" fill="none" viewBox="0 0 24 24" stroke="currentColor">
                            <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M8 7H5a2 2 0 00-2 2v9a2 2 0 002 2h14a2 2 0 002-2V9a2 2 0 00-2-2h-3m-1 4l-3 3m0 0l-3-3m3 3V4" />
                        </svg>
                        <svg xmlns="http://www.w3.org/2000/svg" class="h-4 w-4" fill="none" viewBox="0 0 24 24" stroke="currentColor">
                            <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M12 18h.01M8 21h8a2 2 0 002-2V5a2 2 0 00-2-2H8a2 2 0 00-2 2v14a2 2 0 002 2z" />
                        </svg>
                    </div>
                </div>
                <div class="h-full flex flex-col">
                    <!-- 头部 -->
                    <div class="bg-white p-4 flex items-center">
                        <svg xmlns="http://www.w3.org/2000/svg" class="h-6 w-6 text-gray-400" fill="none" viewBox="0 0 24 24" stroke="currentColor">
                            <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M15 19l-7-7 7-7" />
                        </svg>
                        <h2 class="text-lg font-bold flex-1 text-center">身份证办理</h2>
                        <svg xmlns="http://www.w3.org/2000/svg" class="h-6 w-6 text-gray-400" fill="none" viewBox="0 0 24 24" stroke="currentColor">
                            <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M8.684 13.342C8.886 12.938 9 12.482 9 12c0-.482-.114-.938-.316-1.342m0 2.684a3 3 0 110-2.684m0 2.684l6.632 3.316m-6.632-6l6.632-3.316m0 0a3 3 0 105.367-2.684 3 3 0 00-5.367 2.684zm0 9.316a3 3 0 105.368 2.684 3 3 0 00-5.368-2.684z" />
                        </svg>
                    </div>
                    
                    <!-- 内容区域 -->
                    <div class="flex-1 overflow-auto px-4 pt-4">
                        <!-- 服务卡片 -->
                        <div class="bg-white rounded-lg overflow-hidden mb-4">
                            <div class="bg-blue-600 p-4 text-white">
                                <h3 class="text-lg font-bold">身份证办理</h3>
                                <p class="text-sm opacity-80">居民身份证申领、换领、补领</p>
                            </div>
                            <div class="p-4">
                                <div class="flex items-center mb-3">
                                    <svg xmlns="http://www.w3.org/2000/svg" class="h-5 w-5 text-blue-500 mr-2" fill="none" viewBox="0 0 24 24" stroke="currentColor">
                                        <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M12 8v4l3 3m6-3a9 9 0 11-18 0 9 9 0 0118 0z" />
                                    </svg>
                                    <span class="text-sm text-gray-600">办理时长：5-7个工作日</span>
                                </div>
                                <div class="flex items-center mb-3">
                                    <svg xmlns="http://www.w3.org/2000/svg" class="h-5 w-5 text-blue-500 mr-2" fill="none" viewBox="0 0 24 24" stroke="currentColor">
                                        <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M17.657 16.657L13.414 20.9a1.998 1.998 0 01-2.827 0l-4.244-4.243a8 8 0 1111.314 0z" />
                                        <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M15 11a3 3 0 11-6 0 3 3 0 016 0z" />
                                    </svg>
                                    <span class="text-sm text-gray-600">办理地点：户籍所在地派出所</span>
                                </div>
                                <div class="flex items-start mb-3">
                                    <svg xmlns="http://www.w3.org/2000/svg" class="h-5 w-5 text-blue-500 mr-2 mt-0.5" fill="none" viewBox="0 0 24 24" stroke="currentColor">
                                        <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M9 12h6m-6 4h6m2 5H7a2 2 0 01-2-2V5a2 2 0 012-2h5.586a1 1 0 01.707.293l5.414 5.414a1 1 0 01.293.707V19a2 2 0 01-2 2z" />
                                    </svg>
                                    <span class="text-sm text-gray-600">收费标准：首次办理免费，换领/补领
