# jeju
<!DOCTYPE html>
<html lang="ko">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>제주도 커플 여행 4박 5일 인포그래픽</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <script src="https://cdn.jsdelivr.net/npm/chart.js"></script>
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link href="https://fonts.googleapis.com/css2?family=Noto+Sans+KR:wght@400;700;900&display=swap" rel="stylesheet">
    <style>
        body {
            font-family: 'Noto Sans KR', sans-serif;
            background-color: #F0F9FF;
        }
        .chart-container {
            position: relative;
            width: 100%;
            max-width: 400px;
            margin-left: auto;
            margin-right: auto;
            height: 400px;
            max-height: 40vh;
        }
        .flow-line {
            width: 2px;
            background-color: #00A6ED;
            flex-grow: 1;
        }
        .flow-dot {
            width: 16px;
            height: 16px;
            border-radius: 9999px;
            background-color: #00A6ED;
            border: 2px solid white;
        }
        .icon-bg {
            background-color: #E0F2FE;
        }
    </style>
</head>
<body class="text-gray-800">

    <div class="container mx-auto p-4 md:p-8 max-w-5xl">

        <header class="text-center mb-12">
            <h1 class="text-4xl md:text-5xl font-black text-[#00A6ED] mb-2">제주도 커플 여행</h1>
            <p class="text-lg md:text-xl text-gray-600">4박 5일 힐링 & 미식 여정 (8/11 ~ 8/15)</p>
        </header>

        <main class="space-y-12">

            <section class="grid grid-cols-1 md:grid-cols-3 gap-6 text-center">
                <div class="bg-white p-6 rounded-xl shadow-lg border-l-4 border-[#F59E0B]">
                    <p class="text-5xl font-bold text-[#F59E0B]">5<span class="text-2xl ml-1">일</span></p>
                    <p class="mt-2 text-gray-600">여행 기간</p>
                </div>
                <div class="bg-white p-6 rounded-xl shadow-lg border-l-4 border-[#10B981]">
                    <p class="text-5xl font-bold text-[#10B981]">2<span class="text-2xl ml-1">가지</span></p>
                    <p class="mt-2 text-gray-600">날씨 테마 (비 ☔️ & 맑음 ☀️)</p>
                </div>
                <div class="bg-white p-6 rounded-xl shadow-lg border-l-4 border-[#6366F1]">
                    <p class="text-5xl font-bold text-[#6366F1]">3<span class="text-2xl ml-1">곳</span></p>
                    <p class="mt-2 text-gray-600">주요 숙소 지역</p>
                </div>
            </section>

            <section>
                <h2 class="text-3xl font-bold text-center mb-8">여행 타임라인</h2>
                <div class="relative">
                    <div class="hidden md:block absolute left-1/2 top-0 bottom-0 w-1 bg-sky-200 -translate-x-1/2"></div>
                    
                    <div class="space-y-12">
                        <div class="md:grid md:grid-cols-2 md:gap-8 items-start">
                            <div class="md:text-right md:pr-8 mb-4 md:mb-0">
                                <p class="text-2xl font-bold text-[#00A6ED]">1일차: 8/11 (일) ☔️</p>
                                <p class="text-gray-500">서쪽 해변, 비 오는 날의 감성</p>
                            </div>
                            <div class="bg-white p-6 rounded-xl shadow-lg relative border-t-4 border-[#00A6ED]">
                                <div class="hidden md:block absolute top-8 -left-10 w-4 h-4 bg-[#00A6ED] rounded-full"></div>
                                <p><span class="font-bold">점심:</span> 산방식당 (밀면)</p>
                                <p><span class="font-bold">활동:</span> 오설록 티 뮤지엄</p>
                                <p><span class="font-bold">저녁:</span> 독개물항 (딱새우회)</p>
                                <p><span class="font-bold">숙소:</span> 협재 제주 마루</p>
                            </div>
                        </div>

                        <div class="md:grid md:grid-cols-2 md:gap-8 items-start">
                            <div class="md:col-start-2 md:pl-8 mb-4 md:mb-0">
                                <p class="text-2xl font-bold text-[#00A6ED]">2일차: 8/12 (월) ☔️</p>
                                <p class="text-gray-500">실내에서 즐기는 서부권</p>
                            </div>
                            <div class="bg-white p-6 rounded-xl shadow-lg relative border-t-4 border-[#00A6ED] md:col-start-1 md:row-start-1">
                                <div class="hidden md:block absolute top-8 -right-10 w-4 h-4 bg-[#00A6ED] rounded-full"></div>
                                <p><span class="font-bold">점심:</span> 돌담밥상 (가정식)</p>
                                <p><span class="font-bold">활동:</span> 제주 유리 박물관, 커피템플</p>
                                <p><span class="font-bold">저녁:</span> 해안도로 흑돼지</p>
                                <p><span class="font-bold">숙소:</span> 협재 제주 마루</p>
                            </div>
                        </div>

                        <div class="md:grid md:grid-cols-2 md:gap-8 items-start">
                             <div class="md:text-right md:pr-8 mb-4 md:mb-0">
                                <p class="text-2xl font-bold text-[#F59E0B]">3일차: 8/13 (화) ☀️</p>
                                <p class="text-gray-500">맑은 날, 서귀포 힐링 시작</p>
                            </div>
                            <div class="bg-white p-6 rounded-xl shadow-lg relative border-t-4 border-[#F59E0B]">
                                <div class="hidden md:block absolute top-8 -left-10 w-4 h-4 bg-[#F59E0B] rounded-full"></div>
                                <p><span class="font-bold">활동:</span> 사려니숲길 산책</p>
                                <p><span class="font-bold">점심:</span> 오는정김밥 (포장)</p>
                                <p><span class="font-bold">저녁:</span> 서귀포 올레시장</p>
                                <p><span class="font-bold">숙소:</span> 서귀포 신라호텔</p>
                            </div>
                        </div>
                        
                        <div class="md:grid md:grid-cols-2 md:gap-8 items-start">
                            <div class="md:col-start-2 md:pl-8 mb-4 md:mb-0">
                                <p class="text-2xl font-bold text-[#F59E0B]">4일차: 8/14 (수) ☀️</p>
                                <p class="text-gray-500">서귀포 바다와 제주시의 밤</p>
                            </div>
                            <div class="bg-white p-6 rounded-xl shadow-lg relative border-t-4 border-[#F59E0B] md:col-start-1 md:row-start-1">
                                <div class="hidden md:block absolute top-8 -right-10 w-4 h-4 bg-[#F59E0B] rounded-full"></div>
                                <p><span class="font-bold">활동:</span> 외돌개 올레길</p>
                                <p><span class="font-bold">점심:</span> 자매국수 (고기국수)</p>
                                <p><span class="font-bold">저녁:</span> 제주항 갈치조림</p>
                                <p><span class="font-bold">숙소:</span> 제주 벤티모 호텔</p>
                            </div>
                        </div>

                        <div class="md:grid md:grid-cols-2 md:gap-8 items-start">
                             <div class="md:text-right md:pr-8 mb-4 md:mb-0">
                                <p class="text-2xl font-bold text-[#10B981]">5일차: 8/15 (목) ☀️</p>
                                <p class="text-gray-500">마지막 여정과 공항으로</p>
                            </div>
                            <div class="bg-white p-6 rounded-xl shadow-lg relative border-t-4 border-[#10B981]">
                                <div class="hidden md:block absolute top-8 -left-10 w-4 h-4 bg-[#10B981] rounded-full"></div>
                                <p><span class="font-bold">활동:</span> 기념품 쇼핑</p>
                                <p><span class="font-bold">오전 11시:</span> 렌트카 반납</p>
                                <p><span class="font-bold">오후 1:25:</span> 제주 공항 출발</p>
                            </div>
                        </div>
                    </div>
                </div>
            </section>

            <section class="grid grid-cols-1 md:grid-cols-2 gap-8 items-center">
                <div class="bg-white p-6 rounded-xl shadow-lg">
                    <h2 class="text-2xl font-bold text-center mb-4">여행 활동 분석</h2>
                    <p class="text-center text-gray-600 mb-4">이번 여행은 맛집 탐방과 자연/실내에서의 힐링이 균형을 이루는 코스입니다.</p>
                    <div class="chart-container h-64 md:h-80">
                        <canvas id="activityChart"></canvas>
                    </div>
                </div>
                 <div class="bg-white p-6 rounded-xl shadow-lg">
                    <h2 class="text-2xl font-bold text-center mb-6">제주 미식 로드</h2>
                    <div class="space-y-4">
                        <div class="flex items-center space-x-4">
                            <div class="w-12 h-12 rounded-full icon-bg flex items-center justify-center text-2xl">🍜</div>
                            <div>
                                <p class="font-bold">면 요리</p>
                                <p class="text-sm text-gray-600">산방식당 밀면, 자매국수 고기국수</p>
                            </div>
                        </div>
                        <div class="flex items-center space-x-4">
                            <div class="w-12 h-12 rounded-full icon-bg flex items-center justify-center text-2xl">🦐</div>
                            <div>
                                <p class="font-bold">해산물</p>
                                <p class="text-sm text-gray-600">독개물항 딱새우회, 제주항 갈치조림</p>
                            </div>
                        </div>
                        <div class="flex items-center space-x-4">
                            <div class="w-12 h-12 rounded-full icon-bg flex items-center justify-center text-2xl">🍖</div>
                            <div>
                                <p class="font-bold">육류</p>
                                <p class="text-sm text-gray-600">해안도로 흑돼지</p>
                            </div>
                        </div>
                        <div class="flex items-center space-x-4">
                            <div class="w-12 h-12 rounded-full icon-bg flex items-center justify-center text-2xl">🍚</div>
                            <div>
                                <p class="font-bold">현지 별미</p>
                                <p class="text-sm text-gray-600">돌담밥상, 오는정김밥, 올레시장 먹거리</p>
                            </div>
                        </div>
                    </div>
                </div>
            </section>

        </main>

        <footer class="text-center mt-12 text-gray-500 text-sm">
            <p>Canvas Infographics | 즐겁고 안전한 제주 여행 되세요!</p>
        </footer>

    </div>

    <script>
        const ctx = document.getElementById('activityChart').getContext('2d');
        const activityChart = new Chart(ctx, {
            type: 'doughnut',
            data: {
                labels: ['맛집 탐방', '자연/힐링', '감성/실내', '카페'],
                datasets: [{
                    label: '활동 비율',
                    data: [40, 25, 25, 10],
                    backgroundColor: [
                        '#F97316',
                        '#10B981',
                        '#00A6ED',
                        '#F59E0B'
                    ],
                    borderColor: '#FFFFFF',
                    borderWidth: 4,
                    hoverOffset: 8
                }]
            },
            options: {
                responsive: true,
                maintainAspectRatio: false,
                plugins: {
                    legend: {
                        position: 'bottom',
                        labels: {
                            padding: 20,
                            font: {
                                size: 14,
                                family: "'Noto Sans KR', sans-serif"
                            }
                        }
                    },
                    tooltip: {
                        callbacks: {
                            title: function(tooltipItems) {
                                const item = tooltipItems[0];
                                let label = item.chart.data.labels[item.dataIndex];
                                if (Array.isArray(label)) {
                                  return label.join(' ');
                                } else {
                                  return label;
                                }
                            }
                        }
                    }
                },
                cutout: '60%'
            }
        });
    </script>

</body>
</html>
