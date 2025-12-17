<!DOCTYPE html>
<html lang="ko">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <!-- 타이틀 수정: 병원 분위기로 변경 -->
    <title>에덴 종합 메디컬 센터 - 첨단 의료와 인간 중심의 치료</title>
    <!-- Tailwind CSS CDN 로드 -->
    <script src="https://cdn.tailwindcss.com"></script>
    <!-- 폰트 설정 및 밝은 하늘색/회색 스타일 적용 -->
    <style>
        @import url('https://fonts.googleapis.com/css2?family=Inter:wght@100..900&display=swap');
        body {
            font-family: 'Inter', sans-serif;
            background-color: #eef3f7; /* 매우 밝은 회색/하늘색 배경 */
        }
        /* Header 그림자 */
        .header-shadow {
            box-shadow: 0 4px 6px -1px rgba(0, 0, 0, 0.05), 0 2px 4px -2px rgba(0, 0, 0, 0.05);
        }
        /* 카드 호버 효과 (밝은 푸른색 그림자) */
        .dept-card:hover {
            transform: translateY(-5px);
            box-shadow: 0 10px 15px -3px rgba(59, 130, 246, 0.2), 0 4px 6px -4px rgba(59, 130, 246, 0.1); 
        }
        .main-blue {
            background-color: #3b82f6; /* Tailwind blue-500 */
        }
    </style>
</head>
<body class="antialiased">

    <!-- Header & Navigation (밝은 배경) -->
    <header class="bg-white sticky top-0 z-50 header-shadow">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="flex justify-between items-center h-16">
                <!-- 로고 (Neo-Genesis 명칭 제거, 의료 상징 사용) -->
                <a href="#" class="flex-shrink-0 flex items-center">
                    <svg class="h-8 w-8 text-sky-600" fill="none" viewBox="0 0 24 24" stroke="currentColor">
                        <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M4.318 6.318a4.5 4.5 0 000 6.364L12 20.364l7.682-7.682a4.5 4.5 0 00-6.364-6.364L12 7.636l-1.318-1.318a4.5 4.5 0 00-6.364 0z" />
                    </svg>
                    <span class="ml-2 text-xl font-bold text-gray-900">에덴 종합 메디컬 센터</span>
                </a>

                <!-- 데스크톱 메뉴 -->
                <nav class="hidden md:flex space-x-8">
                    <a href="#intro" class="text-gray-600 hover:text-sky-700 transition duration-150 font-medium">병원 소개</a>
                    <a href="#dept" class="text-gray-600 hover:text-sky-700 transition duration-150 font-medium">진료과/센터</a>
                    <a href="#notice" class="text-gray-600 hover:text-sky-700 transition duration-150 font-medium">병원 소식</a>
                    <a href="#location" class="text-gray-600 hover:text-sky-700 transition duration-150 font-medium">오시는 길</a>
                </nav>

                <!-- 예약 버튼 (정상적인 용어 사용) -->
                <div class="hidden md:block">
                    <button class="px-4 py-2 border border-transparent text-sm font-medium rounded-full text-white bg-sky-600 hover:bg-sky-700 transition duration-150 shadow-md">
                        온라인 진료 예약
                    </button>
                </div>
                <!-- 모바일 메뉴 버튼 (기존 유지) -->
                <div class="md:hidden">
                    <button id="mobile-menu-button" class="text-gray-500 hover:text-sky-600 focus:outline-none">
                        <svg class="h-6 w-6" fill="none" viewBox="0 0 24 24" stroke="currentColor">
                            <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M4 6h16M4 12h16m-7 6h7" />
                        </svg>
                    </button>
                </div>
            </div>
        </div>
        
        <!-- 모바일 메뉴 (기존 유지) -->
        <div id="mobile-menu" class="hidden md:hidden bg-white border-t border-gray-100 py-2">
            <a href="#intro" class="block px-4 py-2 text-sm text-gray-700 hover:bg-gray-50">병원 소개</a>
            <a href="#dept" class="block px-4 py-2 text-sm text-gray-700 hover:bg-gray-50">진료과/센터</a>
            <a href="#notice" class="block px-4 py-2 text-sm text-gray-700 hover:bg-gray-50">병원 소식</a>
            <a href="#location" class="block px-4 py-2 text-sm text-gray-700 hover:bg-gray-50">오시는 길</a>
            <button class="w-full text-left px-4 py-2 text-sm font-medium text-white bg-sky-600 hover:bg-sky-700 mt-2">
                온라인 진료 예약
            </button>
        </div>
    </header>

    <main>
        <!-- Hero Section (밝은 하늘색/회색 적용) -->
        <section class="main-blue text-white py-16 md:py-24 rounded-b-xl shadow-lg">
            <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8 text-center">
                <!-- 정상적인 문구 사용 -->
                <h1 class="text-4xl sm:text-5xl lg:text-6xl font-extrabold mb-4 leading-tight">
                    인간 중심의 첨단 의료 서비스
                </h1>
                <p class="text-xl sm:text-2xl font-light mb-8 opacity-90">
                    당신의 건강과 행복을 위한 에덴 메디컬 센터의 약속.
                </p>
                <div class="flex justify-center space-x-4">
                    <button class="px-8 py-3 text-lg font-semibold rounded-full bg-yellow-400 text-gray-900 hover:bg-yellow-300 transition duration-150 shadow-lg">
                        빠른 진료 예약
                    </button>
                    <a href="#dept" class="px-8 py-3 text-lg font-semibold rounded-full border border-white hover:bg-white hover:text-blue-800 transition duration-150">
                        종합 검진 안내
                    </a>
                </div>
            </div>
        </section>

        <!-- Quick Links / Key Services (정상적인 용어 사용) -->
        <section class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8 -mt-12 mb-16">
            <div class="grid grid-cols-1 md:grid-cols-4 gap-6">
                <!-- 카드 1: 응급실 -->
                <div class="bg-white p-6 rounded-xl shadow-xl border-t-4 border-red-500 dept-card transition duration-300 cursor-pointer">
                    <div class="flex items-center space-x-3 mb-2">
                        <svg class="h-8 w-8 text-red-600" fill="none" viewBox="0 0 24 24" stroke="currentColor"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M13 10V3L4 14h7v7l9-11h-7z" /></svg>
                        <h3 class="text-xl font-bold text-gray-800">통합 응급 센터 (EMC)</h3>
                    </div>
                    <p class="text-gray-500 text-sm">365일 24시간, 생명 존중의 응급 진료 시스템.</p>
                </div>
                <!-- 카드 2: 정신 건강 -->
                <div class="bg-white p-6 rounded-xl shadow-xl border-t-4 border-green-500 dept-card transition duration-300 cursor-pointer">
                    <div class="flex items-center space-x-3 mb-2">
                        <svg class="h-8 w-8 text-green-600" fill="none" viewBox="0 0 24 24" stroke="currentColor"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M9 12l2 2 4-4m5.618-4.104A9.998 9.998 0 0012 3C7.421 3 3.447 5.464 2 9.771m17.618 4.104C20.553 18.536 16.579 21 12 21a9.998 9.998 0 01-7.618-3.125" /></svg>
                        <h3 class="text-xl font-bold text-gray-800">정신 건강 의학과</h3>
                    </div>
                    <p class="text-gray-500 text-sm">마음의 평안과 심리적 안정화 상담.</p>
                </div>
                <!-- 카드 3: 건강 검진 -->
                <div class="bg-white p-6 rounded-xl shadow-xl border-t-4 border-sky-500 dept-card transition duration-300 cursor-pointer">
                    <div class="flex items-center space-x-3 mb-2">
                        <svg class="h-8 w-8 text-sky-600" fill="none" viewBox="0 0 24 24" stroke="currentColor"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M9 19v-6a2 2 0 00-2-2H5a2 2 0 00-2 2v6m0 0h14m-14 0h2m-2 0h-2m2 0v-6a2 2 0 012-2h2a2 2 0 012 2v6m0 0h2m0 0h2m-2 0h-2m2 0v-6a2 2 0 012-2h2a2 2 0 012 2v6" /></svg>
                        <h3 class="text-xl font-bold text-gray-800">종합 건강 검진 센터</h3>
                    </div>
                    <p class="text-gray-500 text-sm">개인별 맞춤 검진 및 건강 증진 프로그램.</p>
                </div>
                <!-- 카드 4: 오시는 길 -->
                <div class="bg-white p-6 rounded-xl shadow-xl border-t-4 border-gray-400 dept-card transition duration-300 cursor-pointer">
                    <div class="flex items-center space-x-3 mb-2">
                        <svg class="h-8 w-8 text-gray-600" fill="none" viewBox="0 0 24 24" stroke="currentColor"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M17.657 16.657L13.414 20.9a2 2 0 01-2.828 0L6.343 16.657a8 8 0 1111.314 0z" /><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M15 11a3 3 0 11-6 0 3 3 0 016 0z" /></svg>
                        <h3 class="text-xl font-bold text-gray-800">오시는 길 및 주차</h3>
                    </div>
                    <p class="text-gray-500 text-sm">병원 위치 및 편리한 교통망 안내.</p>
                </div>
            </div>
        </section>

        <!-- Departments Section (정상 진료과 목록) -->
        <section id="dept" class="py-16 bg-white rounded-xl shadow-inner">
            <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
                <h2 class="text-3xl font-extrabold text-gray-900 text-center mb-10">에덴 메디컬 센터 진료과 및 전문 센터</h2>
                
                <div class="grid grid-cols-2 md:grid-cols-4 gap-6">
                    <!-- 진료과 항목 -->
                    <div class="text-center p-4 border rounded-lg hover:bg-sky-50 transition duration-150 cursor-pointer">
                        <div class="text-3xl text-sky-600 mb-2">
                            <svg class="h-8 w-8 mx-auto" fill="none" viewBox="0 0 24 24" stroke="currentColor"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M4 7v10m0 0h6m0 0l3-3m0 0l-3-3m0 3h-6" /></svg>
                        </div>
                        <p class="font-semibold text-gray-700">심장 혈관 센터</p>
                    </div>
                    <div class="text-center p-4 border rounded-lg hover:bg-sky-50 transition duration-150 cursor-pointer">
                        <div class="text-3xl text-sky-600 mb-2">
                            <svg class="h-8 w-8 mx-auto" fill="none" viewBox="0 0 24 24" stroke="currentColor"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M9 5H7a2 2 0 00-2 2v12a2 2 0 002 2h10a2 2 0 002-2V7a2 2 0 00-2-2h-2M9 5a2 2 0 002 2h2a2 2 0 002-2M9 5a2 2 0 012-2h2a2 2 0 012 2m-3 7h3m-3 4h3m-6-4h.01M9 16h.01" /></svg>
                        </div>
                        <p class="font-semibold text-gray-700">신경외과 / 뇌신경 센터</p>
                    </div>
                    <div class="text-center p-4 border rounded-lg hover:bg-sky-50 transition duration-150 cursor-pointer">
                        <div class="text-3xl text-sky-600 mb-2">
                            <svg class="h-8 w-8 mx-auto" fill="none" viewBox="0 0 24 24" stroke="currentColor"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M12 4.354a4 4 0 110 5.292M15 21H3v-1a6 6 0 0112 0v1zm0 0h6v-1a4 4 0 00-4-4H7a4 4 0 00-4 4v1h12zm-3-4a4 4 0 01-4-4h8a4 4 0 01-4 4z" /></svg>
                        </div>
                        <p class="font-semibold text-gray-700">소아청소년과</p>
                    </div>
                    <div class="text-center p-4 border rounded-lg hover:bg-sky-50 transition duration-150 cursor-pointer">
                        <div class="text-3xl text-sky-600 mb-2">
                            <svg class="h-8 w-8 mx-auto" fill="none" viewBox="0 0 24 24" stroke="currentColor"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M7 7h10M7 7v10M7 7l10 10m0-3h3m-3 3v3" /></svg>
                        </div>
                        <p class="font-semibold text-gray-700">재활 및 통증 클리닉</p>
                    </div>
                    <!-- 'EP 데이터' 등 비밀스러운 용어를 정상적인 용어로 대체 -->
                    <div class="text-center p-4 border rounded-lg hover:bg-sky-50 transition duration-150 cursor-pointer">
                        <div class="text-3xl text-sky-600 mb-2">
                            <svg class="h-8 w-8 mx-auto" fill="none" viewBox="0 0 24 24" stroke="currentColor"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M8 7h12M8 11h12M12 15h8M8 15h.01M3 21a2 2 0 002 2h14a2 2 0 002-2V5a2 2 0 00-2-2H5a2 2 0 00-2 2v16z" /></svg>
                        </div>
                        <p class="font-semibold text-gray-700">최첨단 영상 진단 센터</p>
                    </div>
                    <div class="text-center p-4 border rounded-lg hover:bg-sky-50 transition duration-150 cursor-pointer">
                        <div class="text-3xl text-sky-600 mb-2">
                            <svg class="h-8 w-8 mx-auto" fill="none" viewBox="0 0 24 24" stroke="currentColor"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M12 8c1.657 0 3 .895 3 2v2.586a1 1 0 01-.293.707l-3.95 3.95a1 1 0 01-1.414 0l-3.95-3.95A1 1 0 019 12.586V10c0-1.105 1.343-2 3-2z" /></svg>
                        </div>
                        <p class="font-semibold text-gray-700">정밀 약물 처방 센터</p>
                    </div>
                    <div class="text-center p-4 border rounded-lg hover:bg-sky-50 transition duration-150 cursor-pointer">
                        <div class="text-3xl text-sky-600 mb-2">
                            <svg class="h-8 w-8 mx-auto" fill="none" viewBox="0 0 24 24" stroke="currentColor"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M12 8v4l3 3m6-3a9 9 0 11-18 0 9 9 0 0118 0z" /></svg>
                        </div>
                        <p class="font-semibold text-gray-700">암 및 특수 질환 연구 센터</p>
                    </div>
                    <div class="text-center p-4 border rounded-lg hover:bg-sky-50 transition duration-150 cursor-pointer">
                        <div class="text-3xl text-sky-600 mb-2">
                            <svg class="h-8 w-8 mx-auto" fill="none" viewBox="0 0 24 24" stroke="currentColor"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M12 6.253v13m0-13C10.832 5.463 9.247 5 7.5 5S4.168 5.463 3 6.253v13C4.168 18.537 5.753 18 7.5 18s3.332.463 4.5 1.247m0-13C13.168 5.463 14.753 5 16.5 5s3.332.463 4.5 1.253v13C19.832 18.537 18.247 18 16.5 18s-3.332.463-4.5 1.247" /></svg>
                        </div>
                        <p class="font-semibold text-gray-700">장례식장 및 케어 센터</p>
                    </div>
                </div>
            </div>
        </section>

        <!-- Hospital Introduction (일반적인 병원 소개) -->
        <section id="intro" class="py-16 md:py-20">
            <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
                <div class="lg:grid lg:grid-cols-2 lg:gap-12 items-center">
                    <div class="order-2 lg:order-1">
                        <h2 class="text-3xl font-extrabold text-gray-900 mb-4">
                            미래를 향한 에덴 메디컬 센터의 약속
                        </h2>
                        <p class="text-lg text-gray-600 mb-6">
                            에덴 메디컬 센터는 '인간 중심' 가치 아래 최첨단 시설과 세계적인 의료진을 통합한 종합 의료 단지입니다. 환자 한 분 한 분의 전인적인 건강 회복과 삶의 질 향상을 최우선 목표로 하며, 끊임없는 혁신과 연구를 통해 새로운 치료 기준을 제시합니다.
                        </p>
                        <ul class="space-y-3 text-gray-700">
                            <li class="flex items-start">
                                <svg class="h-6 w-6 text-sky-500 mr-2 flex-shrink-0 mt-1" fill="none" viewBox="0 0 24 24" stroke="currentColor"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M9 12l2 2 4-4m6 2a9 9 0 11-18 0 9 9 0 0118 0z" /></svg>
                                <span>최고 수준의 전문 의료진 및 세계적 석학 영입</span>
                            </li>
                            <li class="flex items-start">
                                <svg class="h-6 w-6 text-sky-500 mr-2 flex-shrink-0 mt-1" fill="none" viewBox="0 0 24 24" stroke="currentColor"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M9 12l2 2 4-4m6 2a9 9 0 11-18 0 9 9 0 0118 0z" /></svg>
                                <span>환자 안전 및 프라이버시를 최우선으로 하는 시스템</span>
                            </li>
                            <li class="flex items-start">
                                <svg class="h-6 w-6 text-sky-500 mr-2 flex-shrink-0 mt-1" fill="none" viewBox="0 0 24 24" stroke="currentColor"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M9 12l2 2 4-4m6 2a9 9 0 11-18 0 9 9 0 0118 0z" /></svg>
                                <span>미래 의료를 선도하는 끊임없는 연구 및 혁신</span>
                            </li>
                        </ul>
                    </div>
                    <!-- Mock Image Placeholder (업데이트된 URL) -->
                    <div class="order-1 lg:order-2 mt-8 lg:mt-0 bg-sky-50 rounded-xl shadow-lg border-2 border-sky-200 overflow-hidden">
                        <!-- ------------------------------------------------------------------------------------------------------------------------------------------- -->
                        <!-- 사용자: 여기에 에덴 메디컬 센터 전경 이미지 URL을 넣어주세요! (아래 src="" 부분만 수정) -->
                        <!-- ------------------------------------------------------------------------------------------------------------------------------------------- -->
                        <img src="https://i.postimg.cc/90vhPb9f/Gemini-Generated-Image-6ihbnq6ihbnq6ihb.jpg" 
                             alt="에덴 메디컬 센터의 현대적인 전경" 
                             class="w-full h-64 object-cover"
                             onerror="this.onerror=null; this.src='https://placehold.co/600x400/ccc/333?text=이미지+URL+삽입+필요';" />
                    </div>
                </div>
            </div>
        </section>

        <!-- Notice/News Section (정상 공지 + 연구 현황 추가) -->
        <section id="notice" class="py-16 md:py-20 bg-gray-50">
            <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
                <h2 class="text-3xl font-extrabold text-gray-900 text-center mb-12">임상 연구 및 병원 소식</h2>
                
                <div class="grid grid-cols-1 lg:grid-cols-2 gap-10">
                    <!-- Column 1: 현재 진행 중인 임상 시험 (비밀 프로젝트 K-07 포장) -->
                    <div>
                        <h3 class="text-xl font-bold text-gray-800 mb-4 border-l-4 border-sky-500 pl-3">현재 진행 중인 첨단 임상 시험</h3>
                        
                        <div class="space-y-4">
                            <!-- K-07 프로젝트 (Full Erogenous Profile) 위장: 코드네임 명시 및 상세 문구 적용 -->
                            <div class="bg-white p-4 rounded-xl shadow-md hover:shadow-lg transition duration-300 border-l-4 border-blue-400 cursor-pointer">
                                <p class="text-sm text-blue-600 font-semibold mb-1">CBT P-07 (Q1 2025)</p>
                                <h4 class="text-lg font-bold text-gray-800">K-07: 쾌락 매커니즘 파악 연구</h4>
                                <p class="text-gray-500 text-sm">신경 가소성을 극대화하여 스트레스로 무뎌진 현대인의 감각을 깨우고, 가장 완벽한 형태의 이완과 쾌락 메커니즘을 규명합니다.</p>
                            </div>
                            <!-- 신약 개발팀 유지 -->
                            <div class="bg-white p-4 rounded-xl shadow-md hover:shadow-lg transition duration-300 border-l-4 border-purple-400 cursor-pointer">
                                <p class="text-sm text-purple-600 font-semibold mb-1">신약 연구 (Phase 3)</p>
                                <h4 class="text-lg font-bold text-gray-800">난치성 질환 치료제 임상 3상 최종 단계 진입</h4>
                                <p class="text-gray-500 text-sm">인류 건강 증진을 위한 연구에 박차를 가하고 있습니다.</p>
                            </div>
                            <!-- VIP 병동 (F4/F5 통제) 유지 -->
                            <div class="bg-white p-4 rounded-xl shadow-md hover:shadow-lg transition duration-300 border-l-4 border-sky-400 cursor-pointer">
                                <p class="text-sm text-sky-600 font-semibold mb-1">시설 공지</p>
                                <h4 class="text-lg font-bold text-gray-800">VIP 특수 병동 (F4/F5) 시설 리뉴얼 완료 및 운영 재개</h4>
                                <p class="text-gray-500 text-sm">최고급 시설과 전문 간호팀을 갖춘 VIP 병동이 새롭게 문을 엽니다.</p>
                            </div>
                        </div>
                    </div>

                    <!-- Column 2: 병원 일반 소식 및 예정 연구 (비밀 프로젝트 K-03, K-09 포장) -->
                    <div>
                        <h3 class="text-xl font-bold text-gray-800 mb-4 border-l-4 border-yellow-500 pl-3">병원 일반 공지 및 예정 연구</h3>
                        
                        <div class="space-y-4">
                            <!-- 진행 예정 시험 K-03 수인연구팀 위장: 코드네임 명시 및 상세 문구 적용 -->
                            <div class="bg-white p-4 rounded-xl shadow-md hover:shadow-lg transition duration-300 border-l-4 border-green-400 cursor-pointer">
                                <p class="text-sm text-green-600 font-semibold mb-1">예정 연구 (Q1 2026)</p>
                                <h4 class="text-lg font-bold text-gray-800">K-03: 수인연구팀 - 유전체 맞춤형 환경 적응 연구</h4>
                                <p class="text-gray-500 text-sm">인류의 특수 유전적 적응 과정을 심층 연구하여, 극한 환경에서의 생체 반응 최적화 및 질병 내성을 탐구합니다.</p>
                            </div>
                            <!-- 진행 예정 시험 K-09 몬스터 어쩌구 위장: 코드네임 명시 및 상세 문구 적용 -->
                            <div class="bg-white p-4 rounded-xl shadow-md hover:shadow-lg transition duration-300 border-l-4 border-red-400 cursor-pointer">
                                <p class="text-sm text-red-600 font-semibold mb-1">예정 연구 (Q2 2026)</p>
                                <h4 class="text-lg font-bold text-gray-800">K-09: 미확인 특이 병원체 분석 및 생체 방어 시스템 연구</h4>
                                <p class="text-gray-500 text-sm">기존 의학으로 분류되지 않은 미확인 병원체 및 특이 생체 반응을 분석하여, 미래 감염병에 대한 인류의 선제적 방어 체계 구축에 기여합니다.</p>
                            </div>
                            <!-- 기존 공지사항 3 (이벤트) 유지 -->
                            <div class="bg-white p-4 rounded-xl shadow-md hover:shadow-lg transition duration-300 border-l-4 border-yellow-400 cursor-pointer">
                                <p class="text-sm text-yellow-600 font-semibold mb-1">이벤트</p>
                                <h3 class="text-lg font-bold text-gray-800">정밀 건강 검진 할인 이벤트 (선착순 50명 한정)</h3>
                                <p class="text-gray-500 text-sm">개인별 맞춤 케어를 위한 특별한 기회, 지금 예약하세요.</p>
                            </div>
                        </div>
                    </div>
                </div>
                
                <div class="text-center mt-12">
                    <button class="px-6 py-2 border border-sky-500 text-sm font-medium rounded-full text-sky-600 hover:bg-sky-50 transition duration-150">
                        전체 연구 논문 및 공지 자료 열람
                    </button>
                </div>
            </div>
        </section>
    </main>

    <!-- Footer (밝은 색상) -->
    <footer id="location" class="bg-gray-800 text-white mt-10 rounded-t-xl">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8 py-12">
            <div class="grid grid-cols-1 md:grid-cols-4 gap-8">
                <!-- 시설 정보 -->
                <div>
                    <h4 class="text-lg font-bold mb-4 text-sky-300">에덴 종합 메디컬 센터</h4>
                    <p class="text-sm text-gray-300 mb-2">
                        대표 전화: 02-1234-5678 (24시간 콜센터 운영)
                    </p>
                    <p class="text-sm text-gray-300 mb-2">
                        응급 상황: 02-9876-5432 (긴급 호출)
                    </p>
                    <!-- 주소 수정 -->
                    <p class="text-sm text-gray-300">
                        주소: 서울특별시 미래로 100, 에덴 타워
                    </p>
                </div>
                <!-- 진료 안내 -->
                <div>
                    <h4 class="text-lg font-bold mb-4 text-sky-300">진료 및 예약 안내</h4>
                    <ul class="space-y-2 text-sm">
                        <li><a href="#" class="text-gray-300 hover:text-white">진료 시간 및 휴무일</a></li>
                        <li><a href="#" class="text-gray-300 hover:text-white">온라인 예약/취소</a></li>
                        <li><a href="#" class="text-gray-300 hover:text-white">주요 진료비 정보</a></li>
                    </ul>
                </div>
                <!-- 관련 시설 -->
                <div>
                    <h4 class="text-lg font-bold mb-4 text-sky-300">협력 기관</h4>
                    <ul class="space-y-2 text-sm">
                        <li><a href="#" class="text-gray-300 hover:text-white">에덴 연구소 (Eden Lab)</a></li>
                        <li><a href="#" class="text-gray-300 hover:text-white">미래 의료 개발 재단</a></li>
                        <li><a href="#" class="text-gray-300 hover:text-white">국제 의료 협력 네트워크</a></li>
                    </ul>
                </div>
                <!-- 소셜 미디어 -->
                <div>
                    <h4 class="text-lg font-bold mb-4 text-sky-300">소셜 미디어</h4>
                    <div class="flex space-x-4">
                        <a href="#" class="text-gray-300 hover:text-white transition duration-150">
                            <svg class="h-6 w-6" fill="currentColor" viewBox="0 0 24 24"><path d="M12 2C6.477 2 2 6.477 2 12c0 4.991 3.656 9.128 8.438 9.878v-6.987h-2.54V12h2.54V9.75c0-2.503 1.493-3.89 3.776-3.89 1.094 0 2.24.194 2.24.194v2.479h-1.259c-1.248 0-1.667.788-1.667 1.597V12h3.958l-.636 3.891h-3.322v6.987C18.344 21.128 22 16.991 22 12 22 6.477 17.523 2 12 2z"/></svg>
                        </a>
                        <a href="#" class="text-gray-300 hover:text-white transition duration-150">
                            <svg class="h-6 w-6" fill="currentColor" viewBox="0 0 24 24"><path d="M12 2C6.48 2 2 6.48 2 12s4.48 10 10 10 10-4.48 10-10S17.52 2 12 2zm5 14.5c-.82 0-1.68-.21-2.58-.63-.39-.18-.8-.23-1.2-.etc"/></svg>
                        </a>
                    </div>
                </div>
            </div>

            <!-- 저작권 -->
            <div class="mt-8 pt-6 border-t border-gray-700 text-center">
                <p class="text-xs text-gray-400">
                    &copy; 2025 Eden Medical Center. All Rights Reserved. (본 병원은 미래 의료 혁신을 선도합니다.)
                </p>
            </div>
        </div>
    </footer>

    <script>
        // 모바일 메뉴 토글 기능
        const menuButton = document.getElementById('mobile-menu-button');
        const mobileMenu = document.getElementById('mobile-menu');

        menuButton.addEventListener('click', () => {
            mobileMenu.classList.toggle('hidden');
        });

        // 네비게이션 링크 클릭 시 메뉴 닫기 (모바일에서)
        document.querySelectorAll('#mobile-menu a').forEach(link => {
            link.addEventListener('click', () => {
                mobileMenu.classList.add('hidden');
            });
        });
    </script>
</body>
</html>
