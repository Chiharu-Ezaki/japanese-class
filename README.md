<!DOCTYPE html>
<html lang="ja" class="scroll-smooth">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title><ruby>技能実習生<rt class="text-xs font-normal">ぎのうじっしゅうせい</rt></ruby>向け オンライン<ruby>日本語<rt class="text-xs font-normal">にほんご</rt></ruby><ruby>会話力強化<rt class="text-xs font-normal">かいわりょくきょうか</rt></ruby>プログラム</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <script src="https://cdn.jsdelivr.net/npm/chart.js@3.7.1/dist/chart.min.js"></script>
    <!-- Font: Inter (Tailwind Default) -->
    <!-- Palette: Calm Harmony (Neutral Blue & Yellow Accent) -->
    <style>
        .chart-container {
            position: relative;
            width: 100%;
            max-width: 400px;
            margin-left: auto;
            margin-right: auto;
            height: 300px;
            max-height: 400px;
        }
        @media (min-width: 768px) {
            .chart-container {
                height: 350px;
            }
        }
        /* Tab Styles for Active State */
        .tab-btn.active {
            border-color: #2563eb; /* blue-600 */
            background-color: #dbeafe; /* blue-100 */
            color: #1e40af; /* blue-800 */
            font-weight: 600;
        }
        .tab-btn {
            border-color: transparent;
            transition: all 0.2s ease-in-out;
        }
        .tab-panel {
            display: none;
            /* Simple fade-in effect for smooth transition */
            animation: fadeIn 0.5s;
        }
        .tab-panel.active {
            display: block;
        }
        @keyframes fadeIn {
            from { opacity: 0; transform: translateY(10px); }
            to { opacity: 1; transform: translateY(0); }
        }
    </style>
</head>
<body class="bg-gray-50 text-gray-800 font-sans">

    <!-- Header & Navigation (Fixed at Top) -->
    <header class="bg-white shadow-lg sticky top-0 z-50">
        <nav class="container mx-auto px-4 sm:px-6 lg:px-8 flex justify-between items-center h-16">
            <h1 class="text-lg md:text-xl font-extrabold text-blue-700">オンライン<ruby>日本語<rt class="text-xs font-normal">にほんご</rt></ruby><ruby>会話<rt class="text-xs font-normal">かいわ</rt></ruby>プログラム</h1>
            <div class="space-x-2 sm:space-x-4">
                <a href="#problem" class="text-sm sm:text-base text-gray-600 hover:text-blue-600 transition duration-150"><ruby>課題<rt class="text-xs font-normal">かだい</rt></ruby>と<ruby>目的<rt class="text-xs font-normal">もくてき</rt></ruby></a>
                <a href="#program" class="text-sm sm:text-base text-gray-600 hover:text-blue-600 transition duration-150">プログラム<ruby>詳細<rt class="text-xs font-normal">しょうさい</rt></ruby></a>
                <a href="#price" class="text-sm sm:text-base text-gray-600 hover:text-blue-600 transition duration-150"><ruby>料金<rt class="text-xs font-normal">りょうきん</rt></ruby></a>
                <a href="#flow" class="text-sm sm:text-base text-gray-600 hover:text-blue-600 transition duration-150"><ruby>導入<rt class="text-xs font-normal">どうにゅう</rt></ruby>の<ruby>流<rt class="text-xs font-normal">なが</rt></ruby>れ</a>
            </div>
        </nav>
    </header>

    <!-- Main Content -->
    <main class="container mx-auto p-4 sm:p-6 lg:p-8">

        <!-- 1. Hero Section (Title) -->
        <section class="text-center pt-12 pb-16">
            <h2 class="text-3xl md:text-5xl font-extrabold text-gray-900 leading-tight">
                <ruby>技能実習生<rt class="text-xs font-normal">ぎのうじっしゅうせい</rt></ruby>向け<br class="sm:hidden">「<span class="text-blue-600"><ruby>来日後<rt class="text-xs font-normal">らいにちご</rt></ruby>すぐに<ruby>役立<rt class="text-xs font-normal">やくだ</rt></ruby>つ！</span>」<br>
                オンライン<ruby>日本語<rt class="text-xs font-normal">にほんご</rt></ruby><ruby>会話力強化<rt class="text-xs font-normal">かいわりょくきょうか</rt></ruby>プログラム
            </h2>
            <p class="mt-6 text-lg md:text-2xl text-gray-700 font-semibold">
                <ruby>日本人<rt class="text-xs font-normal">にほんじん</rt></ruby>との<ruby>会話<rt class="text-xs font-normal">かいわ</rt></ruby>に<ruby>自信<rt class="text-xs font-normal">じしん</rt></ruby>を！<br class="sm:hidden">「<ruby>話<rt class="text-xs font-normal">はな</rt></ruby>す<ruby>度胸<rt class="text-xs font-normal">どきょう</rt></ruby>」を<ruby>育成<rt class="text-xs font-normal">いくせい</rt></ruby>する4<ruby>週間<rt class="text-xs font-normal">しゅうかん</rt></ruby><ruby>集中<rt class="text-xs font-normal">しゅうちゅう</rt></ruby>トライアル
            </p>
        </section>

        <!-- 2. Problem & Goal (Sec 2 & 3) -->
        <section id="problem" class="pt-16 -mt-12 pb-16">
            <h3 class="text-3xl font-bold text-center mb-12 text-gray-900">なぜ<ruby>今<rt class="text-xs font-normal">いま</rt></ruby>、<ruby>会話力強化<rt class="text-xs font-normal">かいわりょくきょうか</rt></ruby>が<ruby>必要<rt class="text-xs font-normal">ひつよう</rt></ruby>なのか？</h3>
            <div class="max-w-6xl mx-auto grid md:grid-cols-2 gap-8 px-4">
                
                <div class="bg-white p-6 rounded-xl shadow-xl border-t-4 border-red-400 transform transition duration-300 hover:scale-[1.02]">
                    <h4 class="text-2xl font-semibold text-red-700 mb-4">🇯🇵 <ruby>現状<rt class="text-xs font-normal">げんじょう</rt></ruby>の<ruby>課題<rt class="text-xs font-normal">かだい</rt></ruby>：<br><ruby>知識<rt class="text-xs font-normal">ちしき</rt></ruby>があっても、<ruby>会話<rt class="text-xs font-normal">かいわ</rt></ruby>に<ruby>自信<rt class="text-xs font-normal">じしん</rt></ruby>が<ruby>持<rt class="text-xs font-normal">も</rt></ruby>てない</h4>
                    <p class="text-gray-700 mb-4 max-w-lg mx-auto">
                        このセクションでは、<ruby>多<rt class="text-xs font-normal">おお</rt></ruby>くの<ruby>技能実習生<rt class="text-xs font-normal">ぎのうじっしゅうせい</rt></ruby>が<ruby>直面<rt class="text-xs font-normal">ちょくめん</rt></ruby>する<ruby>共通<rt class="text-xs font-normal">きょうつう</rt></ruby>の<ruby>悩<rt class="text-xs font-normal">なや</rt></ruby>みを<ruby>探<rt class="text-xs font-normal">さが</rt></ruby>ります。N5レベルの<ruby>知識<rt class="text-xs font-normal">ちしき</rt></ruby>はあっても、<ruby>実際<rt class="text-xs font-normal">じっさい</rt></ruby>の<ruby>現場<rt class="text-xs font-normal">げんば</rt></ruby>でのコミュニケーションには<ruby>大<rt class="text-xs font-normal">おお</rt></ruby>きな<ruby>壁<rt class="text-xs font-normal">かべ</rt></ruby>が<ruby>存在<rt class="text-xs font-normal">そんざい</rt></ruby>します。
                    </p>
                    <ul class="space-y-3">
                        <li class="flex items-start">
                            <span class="text-red-500 font-bold text-xl mr-3">✕</span>
                            <div>
                                <h5 class="font-semibold text-gray-800"><ruby>知識<rt class="text-xs font-normal">ちしき</rt></ruby>と<ruby>実践<rt class="text-xs font-normal">じっせん</rt></ruby>のギャップ</h5>
                                <p class="text-gray-600">N5の<ruby>文法<rt class="text-xs font-normal">ぶんぽう</rt></ruby>は<ruby>知<rt class="text-xs font-normal">し</rt></ruby>っていても、**「<ruby>実践的<rt class="text-xs font-normal">じっせんてき</rt></ruby>な<ruby>会話<rt class="text-xs font-normal">かいわ</rt></ruby>」**に<ruby>自信<rt class="text-xs font-normal">じしん</rt></ruby>がない<ruby>方<rt class="text-xs font-normal">かた</rt></ruby>が<ruby>多<rt class="text-xs font-normal">おお</rt></ruby>いのが<ruby>現状<rt class="text-xs font-normal">げんじょう</rt></ruby>です。</p>
                            </div>
                        </li>
                        <li class="flex items-start">
                            <span class="text-red-500 font-bold text-xl mr-3">✕</span>
                            <div>
                                <h5 class="font-semibold text-gray-800"><ruby>来日後<rt class="text-xs font-normal">らいにちご</rt></ruby>の「<ruby>心理的<rt class="text-xs font-normal">しんりてき</rt></ruby>な<ruby>壁<rt class="text-xs font-normal">かべ</rt></ruby>」</h5>
                                <p class="text-gray-600">「<ruby>話<rt class="text-xs font-normal">はな</rt></ruby>すことにビビって」しまい、<ruby>定着<rt class="text-xs font-normal">ていちゃく</rt></ruby>や<ruby>業務理解<rt class="text-xs font-normal">ぎょうむりかい</rt></ruby>の<ruby>大<rt class="text-xs font-normal">おお</rt></ruby>きな<ruby>障壁<rt class="text-xs font-normal">しょうへき</rt></ruby>になりかねません。</p>
                            </div>
                        </li>
                    </ul>
                </div>
                
                <div class="bg-white p-6 rounded-xl shadow-xl border-t-4 border-blue-400 transform transition duration-300 hover:scale-[1.02]">
                    <h4 class="text-2xl font-semibold text-blue-700 mb-4">🎯 <ruby>本講座<rt class="text-xs font-normal">ほんこうざ</rt></ruby>の<ruby>目的<rt class="text-xs font-normal">もくてき</rt></ruby>とゴール：<br>「<ruby>話<rt class="text-xs font-normal">はな</rt></ruby>す<ruby>度胸<rt class="text-xs font-normal">どきょう</rt></ruby>」をつけ、<ruby>即戦力<rt class="text-xs font-normal">そくせんりょく</rt></ruby>に！</h4>
                    <p class="text-gray-700 mb-4 max-w-lg mx-auto">
                        <ruby>本<rt class="text-xs font-normal">ほん</rt></ruby>プログラムは、<ruby>単<rt class="text-xs font-normal">たん</rt></ruby>なる<ruby>知識<rt class="text-xs font-normal">ちしき</rt></ruby>の<ruby>詰<rt class="text-xs font-normal">つ</rt></ruby>め<ruby>込<rt class="text-xs font-normal">こ</rt></ruby>みではありません。<ruby>現場<rt class="text-xs font-normal">げんば</rt></ruby>で<ruby>即座<rt class="text-xs font-normal">そくざ</rt></ruby>に<ruby>役立<rt class="text-xs font-normal">やくだ</rt></ruby>つ「<ruby>使<rt class="text-xs font-normal">つか</rt></ruby>えるスキル」と「<ruby>自信<rt class="text-xs font-normal">じしん</rt></ruby>」を<ruby>育成<rt class="text-xs font-normal">いくせい</rt></ruby>することに<ruby>特化<rt class="text-xs font-normal">とっか</rt></ruby>しています。
                    </p>
                    <ul class="space-y-3">
                        <li class="flex items-start">
                            <span class="text-blue-500 font-bold text-xl mr-3">✅</span>
                            <div>
                                <h5 class="font-semibold text-gray-800"><ruby>核心的<rt class="text-xs font-normal">かくしんてき</rt></ruby>な<ruby>目標<rt class="text-xs font-normal">もくひょう</rt></ruby>：ビビらない<ruby>度胸<rt class="text-xs font-normal">どきょう</rt></ruby></h5>
                                <p class="text-gray-600">「<ruby>日本<rt class="text-xs font-normal">にほん</rt></ruby><ruby>入国後<rt class="text-xs font-normal">にゅうこくご</rt></ruby>、<ruby>日本人<rt class="text-xs font-normal">にほんじん</rt></ruby>と<ruby>会話<rt class="text-xs font-normal">かいわ</rt></ruby>するのに**ビビらない<ruby>度胸<rt class="text-xs font-normal">どきょう</rt></ruby>**をつける」ことを<ruby>最重要視<rt class="text-xs font-normal">さいじゅうようし</rt></ruby>します。</p>
                            </div>
                        </li>
                        <li class="flex items-start">
                            <span class="text-blue-500 font-bold text-xl mr-3">✅</span>
                            <div>
                                <h5 class="font-semibold text-gray-800"><ruby>緊急<rt class="text-xs font-normal">きんきゅう</rt></ruby><ruby>対応力<rt class="text-xs font-normal">たいおうりょく</rt></ruby>の<ruby>獲得<rt class="text-xs font-normal">かくとく</rt></ruby></h5>
                                <p class="text-gray-600"><ruby>体調不良<rt class="text-xs font-normal">たいちょうふりょう</rt></ruby>や<ruby>製品<rt class="text-xs font-normal">せいひん</rt></ruby><ruby>不良<rt class="text-xs font-normal">ふりょう</rt></ruby>など、**「トラブル<ruby>時<rt class="text-xs font-normal">じ</rt></ruby>」**に<ruby>必要<rt class="text-xs font-normal">ひつよう</rt></ruby>な<ruby>報告<rt class="text-xs font-normal">ほうこく</rt></ruby>・<ruby>相談<rt class="text-xs font-normal">そうだん</rt></ruby>ができるスキルを<ruby>身<rt class="text-xs font-normal">み</rt></ruby>につけます。</p>
                            </div>
                        </li>
                        <li class="flex items-start">
                            <span class="text-blue-500 font-bold text-xl mr-3">✅</span>
                            <div>
                                <h5 class="font-semibold text-gray-800"><ruby>心理的<rt class="text-xs font-normal">しんりてき</rt></ruby>ハードルの<ruby>打破<rt class="text-xs font-normal">だは</rt></ruby></h5>
                                <p class="text-gray-600"><ruby>日本人<rt class="text-xs font-normal">にほんじん</rt></ruby>とのコミュニケーションに<ruby>対<rt class="text-xs font-normal">たい</rt></ruby>する<ruby>心理的<rt class="text-xs font-normal">しんりてき</rt></ruby>ハードルを<ruby>下<rt class="text-xs font-normal">さ</rt></ruby>げ、<ruby>積極性<rt class="text-xs font-normal">せっきょくせい</rt></ruby>を<ruby>引<rt class="text-xs font-normal">ひ</rt></ruby>き<ruby>出<rt class="text-xs font-normal">だ</rt></ruby>します。</p>
                            </div>
                        </li>
                    </ul>
                </div>
            </div>
        </section>

        <!-- 3. Program Details (Sec 4, 5, 6) -->
        <section id="program" class="pt-16 -mt-12 pb-16 bg-white rounded-xl shadow-2xl">
            <h3 class="text-3xl font-bold text-center mb-12 text-gray-900">🌟 プログラム<ruby>詳細<rt class="text-xs font-normal">しょうさい</rt></ruby>：<br>「アウトプット」に<ruby>特化<rt class="text-xs font-normal">とっか</rt></ruby>した<ruby>実践的<rt class="text-xs font-normal">じっせんてき</rt></ruby>トレーニング</h3>
            
            <p class="max-w-3xl mx-auto text-center text-gray-700 mb-10 px-4">
                <ruby>本<rt class="text-xs font-normal">ほん</rt></ruby>プログラムがどのようにして「<ruby>話<rt class="text-xs font-normal">はな</rt></ruby>す<ruby>自信<rt class="text-xs font-normal">じしん</rt></ruby>」を<ruby>育<rt class="text-xs font-normal">そだ</rt></ruby>てるのか、その<ruby>秘密<rt class="text-xs font-normal">ひみつ</rt></ruby>をご<ruby>紹介<rt class="text-xs font-normal">しょうかい</rt></ruby>します。<ruby>下<rt class="text-xs font-normal">した</rt></ruby>のタブをクリックして、「<ruby>概要<rt class="text-xs font-normal">がいよう</rt></ruby>」「4<ruby>週間<rt class="text-xs font-normal">しゅうかん</rt></ruby>カリキュラム」「60<ruby>分<rt class="text-xs font-normal">ふん</rt></ruby>の<ruby>授業構成<rt class="text-xs font-normal">じゅぎょうこうせい</rt></ruby>」をそれぞれご<ruby>確認<rt class="text-xs font-normal">かくにん</rt></ruby>ください。
            </p>

            <!-- Tabs Navigation -->
            <div class="flex justify-center border-b border-gray-300 mb-8 space-x-1 sm:space-x-4">
                <button class="tab-btn active py-3 px-3 sm:px-6 text-base sm:text-lg font-medium text-gray-600 border-b-4 focus:outline-none rounded-t-lg" data-tab="overview"><ruby>概要<rt class="text-xs font-normal">がいよう</rt></ruby></button>
                <button class="tab-btn py-3 px-3 sm:px-6 text-base sm:text-lg font-medium text-gray-600 border-b-4 focus:outline-none rounded-t-lg" data-tab="curriculum">4<ruby>週間<rt class="text-xs font-normal">しゅうかん</rt></ruby>カリキュラム</button>
                <button class="tab-btn py-3 px-3 sm:px-6 text-base sm:text-lg font-medium text-gray-600 border-b-4 focus:outline-none rounded-t-lg" data-tab="lesson">60<ruby>分<rt class="text-xs font-normal">ふん</rt></ruby>の<ruby>授業<rt class="text-xs font-normal">じゅぎょう</rt></ruby></button>
            </div>

            <!-- Tabs Content -->
            <div id="tab-content" class="max-w-5xl mx-auto px-4">

                <!-- Tab 1: Overview (Sec 4) -->
                <div id="tab-overview" class="tab-panel active">
                    <h4 class="text-2xl font-semibold text-center mb-8 text-gray-800"><ruby>講座<rt class="text-xs font-normal">こうざ</rt></ruby>の<ruby>特徴<rt class="text-xs font-normal">とくちょう</rt></ruby></h4>
                    <div class="grid sm:grid-cols-2 lg:grid-cols-3 gap-6">
                        <div class="bg-gray-50 p-5 rounded-lg shadow-md border border-gray-200">
                            <h5 class="font-bold text-lg text-blue-700 mb-2">👤 <ruby>対象者<rt class="text-xs font-normal">たいしょうしゃ</rt></ruby></h5>
                            <p><ruby>日本<rt class="text-xs font-normal">にほん</rt></ruby><ruby>入国<rt class="text-xs font-normal">にゅうこく</rt></ruby>が<ruby>決<rt class="text-xs font-normal">き</rt></ruby>まっている<ruby>方<rt class="text-xs font-normal">かた</rt></ruby> (N5<ruby>程度<rt class="text-xs font-normal">ていど</rt></ruby>)<br>特に「<ruby>会話<rt class="text-xs font-normal">かいわ</rt></ruby>への<ruby>自信<rt class="text-xs font-normal">じしん</rt></ruby>」を<ruby>強化<rt class="text-xs font-normal">きょうか</rt></ruby>したい<ruby>方<rt class="text-xs font-normal">かた</rt></ruby></p>
                        </div>
                        <div class="bg-gray-50 p-5 rounded-lg shadow-md border border-gray-200">
                            <h5 class="font-bold text-lg text-blue-700 mb-2">🗓️ <ruby>期間<rt class="text-xs font-normal">きかん</rt></ruby>と<ruby>頻度<rt class="text-xs font-normal">ひんど</rt></ruby></h5>
                            <p class="font-semibold"><ruby>月<rt class="text-xs font-normal">げつ</rt></ruby>〜<ruby>金<rt class="text-xs font-normal">きん</rt></ruby>の<ruby>毎日<rt class="text-xs font-normal">まいにち</rt></ruby>1<ruby>時間<rt class="text-xs font-normal">じかん</rt></ruby> $\times$ 4<ruby>週間<rt class="text-xs font-normal">しゅうかん</rt></ruby></p>
                            <p class="text-sm text-gray-600">（<ruby>計<rt class="text-xs font-normal">けい</rt></ruby>20<ruby>回<rt class="text-xs font-normal">かい</rt></ruby><ruby>集中<rt class="text-xs font-normal">しゅうちゅう</rt></ruby>コース）</p>
                        </div>
                        <div class="bg-gray-50 p-5 rounded-lg shadow-md border border-gray-200">
                            <h5 class="font-bold text-lg text-blue-700 mb-2">💻 <ruby>形式<rt class="text-xs font-normal">けいしき</rt></ruby>と<ruby>規模<rt class="text-xs font-normal">きぼ</rt></ruby></h5>
                            <p>オンライン（Zoom<ruby>等利用<rt class="text-xs font-normal">とうりよう</rt></ruby>）<br><ruby>少人数制<rt class="text-xs font-normal">しょうにんずうせい</rt></ruby>（〜10<ruby>名<rt class="text-xs font-normal">めい</rt></ruby><ruby>推奨<rt class="text-xs font-normal">すいしょう</rt></ruby>）</p>
                        </div>
                        <div class="bg-gray-50 p-5 rounded-lg shadow-md border border-gray-200">
                            <h5 class="font-bold text-lg text-blue-700 mb-2">👨‍🏫 <ruby>講師<rt class="text-xs font-normal">こうし</rt></ruby></h5>
                            <p><ruby>経験豊富<rt class="text-xs font-normal">けいけんほうふ</rt></ruby>な<ruby>日本語<rt class="text-xs font-normal">にほんご</rt></ruby><ruby>会話指導<rt class="text-xs font-normal">かいわしどう</rt></ruby><ruby>専門<rt class="text-xs font-normal">せんもん</rt></ruby>の<ruby>講師<rt class="text-xs font-normal">こうし</rt></ruby>が<ruby>担当<rt class="text-xs font-normal">たんとう</rt></ruby>します。</p>
                        </div>
                        <div class="bg-gray-50 p-5 rounded-lg shadow-md border border-gray-200 col-span-1 sm:col-span-2 lg:col-span-1">
                            <h5 class="font-bold text-lg text-blue-700 mb-2">💥 <ruby>最大<rt class="text-xs font-normal">さいだい</rt></ruby>の<ruby>特徴<rt class="text-xs font-normal">とくちょう</rt></ruby></h5>
                            <p class="font-semibold text-red-600"><ruby>会話<rt class="text-xs font-normal">かいわ</rt></ruby>の「ロープレ」と「<ruby>発表<rt class="text-xs font-normal">はっぴょう</rt></ruby>」を<ruby>重視<rt class="text-xs font-normal">じゅうし</rt></ruby>した、<ruby>実践主義<rt class="text-xs font-normal">じっせんしゅぎ</rt></ruby>のトレーニング</p>
                        </div>
                    </div>
                </div>

                <!-- Tab 2: Curriculum (Sec 5) -->
                <div id="tab-curriculum" class="tab-panel">
                    <h4 class="text-2xl font-semibold text-center mb-8 text-gray-800">🗓️ <ruby>現場直結型<rt class="text-xs font-normal">げんばちょっけつがた</rt></ruby>：4<ruby>週間<rt class="text-xs font-normal">しゅうかん</rt></ruby>カリキュリキュラム</h4>
                    <p class="text-center text-gray-700 mb-8"><ruby>導入前<rt class="text-xs font-normal">どうにゅうまえ</rt></ruby>と<ruby>最終<rt class="text-xs font-normal">さいしゅう</rt></ruby>ヒアリングテストで、<ruby>会話力<rt class="text-xs font-normal">かいわりょく</rt></ruby>の<ruby>成長<rt class="text-xs font-normal">せいちょう</rt></ruby>を<ruby>具体的<rt class="text-xs font-normal">ぐたいてき</rt></ruby>に<ruby>可視化<rt class="text-xs font-normal">かしか</rt></ruby>します。</p>
                    <div class="relative pl-8">
                        <!-- Vertical line -->
                        <div class="absolute left-12 top-0 bottom-0 w-1 bg-blue-200 rounded"></div>
                        
                        <div class="relative mb-8">
                            <div class="absolute left-0 top-1.5 w-10 h-10 bg-blue-600 rounded-full text-white flex items-center justify-center font-bold z-10 text-sm">1<ruby>週<rt class="text-xs font-normal">しゅう</rt></ruby></div>
                            <div class="ml-16 p-6 bg-blue-50 rounded-lg shadow-md border border-blue-200 transform hover:shadow-lg transition duration-300">
                                <h5 class="font-bold text-lg text-blue-800 mb-2"><ruby>第<rt class="text-xs font-normal">だい</rt></ruby>1<ruby>週<rt class="text-xs font-normal">しゅう</rt></ruby>：<ruby>日常会話<rt class="text-xs font-normal">にちじょうかいわ</rt></ruby>の<ruby>基礎固<rt class="text-xs font-normal">きそがため</rt></ruby>め</h5>
                                <p class="text-gray-700"><ruby>自己紹介<rt class="text-xs font-normal">じこしょうかい</rt></ruby>、<ruby>挨拶<rt class="text-xs font-normal">あいさつ</rt></ruby>、<ruby>家族<rt class="text-xs font-normal">かぞく</rt></ruby>のこと、インドネシアのことなど、「<ruby>話<rt class="text-xs font-normal">はな</rt></ruby>すこと」そのものに<ruby>慣<rt class="text-xs font-normal">な</rt></ruby>れることを<ruby>目指<rt class="text-xs font-normal">めざ</rt></ruby>します。</p>
                                <p class="font-semibold text-blue-600 mt-2"><ruby>学習<rt class="text-xs font-normal">がくしゅう</rt></ruby><ruby>効果<rt class="text-xs font-normal">こうか</rt></ruby>：「<ruby>話<rt class="text-xs font-normal">はな</rt></ruby>すことに<ruby>慣<rt class="text-xs font-normal">な</rt></ruby>れる」</p>
                            </div>
                        </div>
                        <div class="relative mb-8">
                            <div class="absolute left-0 top-1.5 w-10 h-10 bg-blue-600 rounded-full text-white flex items-center justify-center font-bold z-10 text-sm">2<ruby>週<rt class="text-xs font-normal">しゅう</rt></ruby></div>
                            <div class="ml-16 p-6 bg-blue-50 rounded-lg shadow-md border border-blue-200 transform hover:shadow-lg transition duration-300">
                                <h5 class="font-bold text-lg text-blue-800 mb-2"><ruby>第<rt class="text-xs font-normal">だい</rt></ruby>2<ruby>週<rt class="text-xs font-normal">しゅう</rt></ruby>：<ruby>職場<rt class="text-xs font-normal">しょくば</rt></ruby>での<ruby>基礎会話<rt class="text-xs font-normal">きそかいわ</rt></ruby></h5>
                                <p class="text-gray-700"><ruby>業務指示<rt class="text-xs font-normal">ぎょうむしじ</rt></ruby>の<ruby>受領<rt class="text-xs font-normal">じゅりょう</rt></ruby>、<ruby>質問<rt class="text-xs font-normal">しつもん</rt></ruby>、<ruby>依頼<rt class="text-xs font-normal">いらい</rt></ruby>、<ruby>感謝<rt class="text-xs font-normal">かんしゃ</rt></ruby>など、<ruby>職場<rt class="text-xs font-normal">しょくば</rt></ruby>での<ruby>円滑<rt class="text-xs font-normal">えんかつ</rt></ruby>なコミュニケーションの<ruby>土台<rt class="text-xs font-normal">どだい</rt></ruby>を<ruby>築<rt class="text-xs font-normal">きず</rt></ruby>きます。</p>
                                <p class="font-semibold text-blue-600 mt-2"><ruby>学習<rt class="text-xs font-normal">がくしゅう</rt></ruby><ruby>効果<rt class="text-xs font-normal">こうか</rt></ruby>：「<ruby>基礎的<rt class="text-xs font-normal">きそてき</rt></ruby>な<ruby>報連相<rt class="text-xs font-normal">ほうれんそう</rt></ruby>」</p>
                            </div>
                        </div>
                        <div class="relative mb-8">
                            <div class="absolute left-0 top-1.5 w-10 h-10 bg-blue-600 rounded-full text-white flex items-center justify-center font-bold z-10 text-sm">3<ruby>週<rt class="text-xs font-normal">しゅう</rt></ruby></div>
                            <div class="ml-16 p-6 bg-red-50 rounded-lg shadow-md border border-red-300 transform hover:shadow-lg transition duration-300">
                                <h5 class="font-bold text-lg text-red-700 mb-2"><ruby>第<rt class="text-xs font-normal">だい</rt></ruby>3<ruby>週<rt class="text-xs font-normal">しゅう</rt></ruby>：<ruby>職場<rt class="text-xs font-normal">しょくば</rt></ruby>でのトラブル<ruby>会話<rt class="text-xs font-normal">かいわ</rt></ruby>【<ruby>最重要<rt class="text-xs font-normal">さいじゅうよう</rt></ruby>】</h5>
                                <p class="text-gray-700"><ruby>体調不良<rt class="text-xs font-normal">たいちょうふりょう</rt></ruby>の<ruby>報告<rt class="text-xs font-normal">ほうこく</rt></ruby>、<ruby>製品<rt class="text-xs font-normal">せいひん</rt></ruby><ruby>不良<rt class="text-xs font-normal">ふりょう</rt></ruby>や<ruby>機械故障<rt class="text-xs font-normal">きかいこしょう</rt></ruby>の<ruby>報告<rt class="text-xs font-normal">ほうこく</rt></ruby>、<ruby>遅刻<rt class="text-xs font-normal">ちこく</rt></ruby><ruby>連絡<rt class="text-xs font-normal">れんらく</rt></ruby>など、<ruby>緊急時<rt class="text-xs font-normal">きんきゅうじ</rt></ruby>に<ruby>必要<rt class="text-xs font-normal">ひつよう</rt></ruby>な<ruby>会話<rt class="text-xs font-normal">かいわ</rt></ruby>を<ruby>集中<rt class="text-xs font-normal">しゅうちゅう</rt></ruby><ruby>練習<rt class="text-xs font-normal">れんしゅう</rt></ruby>します。</p>
                                <p class="font-semibold text-red-600 mt-2"><ruby>学習<rt class="text-xs font-normal">がくしゅう</rt></ruby><ruby>効果<rt class="text-xs font-normal">こうか</rt></ruby>：「<ruby>緊急時<rt class="text-xs font-normal">きんきゅうじ</rt></ruby>の<ruby>対応力<rt class="text-xs font-normal">たいおうりょく</rt></ruby>」</p>
                            </div>
                        </div>
                        <div class="relative mb-8">
                            <div class="absolute left-0 top-1.5 w-10 h-10 bg-blue-600 rounded-full text-white flex items-center justify-center font-bold z-10 text-sm">4<ruby>週<rt class="text-xs font-normal">しゅう</rt></ruby></div>
                            <div class="ml-16 p-6 bg-blue-50 rounded-lg shadow-md border border-blue-200 transform hover:shadow-lg transition duration-300">
                                <h5 class="font-bold text-lg text-blue-800 mb-2"><ruby>第<rt class="text-xs font-normal">だい</rt></ruby>4<ruby>週<rt class="text-xs font-normal">しゅう</rt></ruby>：1ヶ<ruby>月<rt class="text-xs font-normal">げつ</rt></ruby>の<ruby>総復習<rt class="text-xs font-normal">そうふくしゅう</rt></ruby>と<ruby>応用練習<rt class="text-xs font-normal">おうようれんしゅう</rt></ruby></h5>
                                <p class="text-gray-700"><ruby>総合的<rt class="text-xs font-normal">そうごうてき</rt></ruby>なロールプレイングや、<ruby>日本人<rt class="text-xs font-normal">にほんじん</rt></ruby>との<ruby>文化<rt class="text-xs font-normal">ぶんか</rt></ruby>の<ruby>違<rt class="text-xs font-normal">ちが</rt></ruby>いに<ruby>関<rt class="text-xs font-normal">かん</rt></ruby>するQ&Aを<ruby>通<rt class="text-xs font-normal">とお</rt></ruby>じて、<ruby>学<rt class="text-xs font-normal">まな</rt></ruby>んだことを<ruby>定着<rt class="text-xs font-normal">ていちゃく</rt></ruby>させます。</p>
                                <p class="font-semibold text-blue-600 mt-2"><ruby>学習<rt class="text-xs font-normal">がくしゅう</rt></ruby><ruby>効果<rt class="text-xs font-normal">こうか</rt></ruby>：「<ruby>自信<rt class="text-xs font-normal">じしん</rt></ruby>の<ruby>定着<rt class="text-xs font-normal">ていちゃく</rt></ruby>」</p>
                            </div>
                        </div>
                    </div>
                </div>

                <!-- Tab 3: Lesson Structure (Sec 6) -->
                <div id="tab-lesson" class="tab-panel">
                    <h4 class="text-2xl font-semibold text-center mb-8 text-gray-800">🎤 アウトプット<ruby>中心<rt class="text-xs font-normal">ちゅうしん</rt></ruby>：60<ruby>分間<rt class="text-xs font-normal">ふんかん</rt></ruby>の<ruby>授業構成<rt class="text-xs font-normal">じゅぎょうこうせい</rt></ruby></h4>
                    <p class="text-center text-gray-700 mb-8 px-4"><ruby>授業時間<rt class="text-xs font-normal">じゅぎょうじかん</rt></ruby>の3<ruby>分<rt class="text-xs font-normal">ぶん</rt></ruby>の2<ruby>以上<rt class="text-xs font-normal">いじょう</rt></ruby>が「ロープレ」と「<ruby>発表<rt class="text-xs font-normal">はっぴょう</rt></ruby>」という、<ruby>実践的<rt class="text-xs font-normal">じっせんてき</rt></ruby>な<ruby>構成<rt class="text-xs font-normal">こうせい</rt></ruby>です。<ruby>間違<rt class="text-xs font-normal">まちが</rt></ruby>いを<ruby>恐<rt class="text-xs font-normal">おそ</rt></ruby>れず、<ruby>積極的<rt class="text-xs font-normal">せっきょくてき</rt></ruby>に<ruby>発言<rt class="text-xs font-normal">はつげん</rt></ruby>できる<ruby>環境<rt class="text-xs font-normal">かんきょう</rt></ruby>づくりを<ruby>徹底<rt class="text-xs font-normal">てってい</rt></ruby>します。</p>
                    
                    <div class="chart-container">
                        <canvas id="lessonChart"></canvas>
                    </div>

                    <div class="mt-8 grid md:grid-cols-3 gap-4 text-center">
                        <div class="p-4 bg-gray-100 rounded-lg shadow-inner">
                            <h5 class="font-semibold text-lg text-gray-800">0-20<ruby>分<rt class="text-xs font-normal">ふん</rt></ruby>: トピックス<ruby>練習<rt class="text-xs font-normal">れんしゅう</rt></ruby></h5>
                            <p class="text-sm text-gray-600">その<ruby>日<rt class="text-xs font-normal">ひ</rt></ruby>の<ruby>表現<rt class="text-xs font-normal">ひょうげん</rt></ruby>のインプットと<ruby>反復練習<rt class="text-xs font-normal">はんぷくれんしゅう</rt></ruby></p>
                        </div>
                        <div class="p-4 bg-blue-100 rounded-lg shadow-inner">
                            <h5 class="font-semibold text-lg text-blue-800">20-40<ruby>分<rt class="text-xs font-normal">ふん</rt></ruby>: <ruby>会話<rt class="text-xs font-normal">かいわ</rt></ruby>ロープレ</h5>
                            <p class="text-sm text-gray-600"><ruby>場面<rt class="text-xs font-normal">ばめん</rt></ruby>を<ruby>想定<rt class="text-xs font-normal">そうてい</rt></ruby>した<ruby>実践的<rt class="text-xs font-normal">じっせんてき</rt></ruby>な<ruby>対話練習<rt class="text-xs font-normal">たいわれんしゅう</rt></ruby></p>
                        </div>
                        <div class="p-4 bg-green-100 rounded-lg shadow-inner">
                            <h5 class="font-semibold text-lg text-green-800">40-60<ruby>分<rt class="text-xs font-normal">ふん</rt></ruby>: <ruby>発表<rt class="text-xs font-normal">はっぴょう</rt></ruby>＆フィードバック</h5>
                            <p class="text-sm text-gray-600">「<ruby>人前<rt class="text-xs font-normal">ひとまえ</rt></ruby>で<ruby>話<rt class="text-xs font-normal">はな</rt></ruby>す<ruby>度胸<rt class="text-xs font-normal">どきょう</rt></ruby>」の<ruby>育成<rt class="text-xs font-normal">いくせい</rt></ruby>を<ruby>行<rt class="text-xs font-normal">おこな</rt></ruby>います。</p>
                        </div>
                    </div>
                </div>
            </div>
        </section>

        <!-- 4. Price & Trial (Sec 7 & 8) -->
        <section id="price" class="pt-16 -mt-12 pb-20">
            <h3 class="text-3xl font-bold text-center mb-6 text-gray-900">🎁 まずは<ruby>効果<rt class="text-xs font-normal">こうか</rt></ruby>を<ruby>実感<rt class="text-xs font-normal">じっかん</rt></ruby>してください！</h3>
            <h4 class="text-4xl font-extrabold text-center text-blue-600 mb-12">「1ヶ<ruby>月<rt class="text-xs font-normal">げつ</rt></ruby>お試しトライアル」のご<ruby>提案<rt class="text-xs font-normal">ていあん</rt></ruby></h4>
            
            <p class="max-w-3xl mx-auto text-center text-gray-700 mb-12 px-4">
                プログラムの<ruby>質<rt class="text-xs font-normal">しつ</rt></ruby>の<ruby>高<rt class="text-xs font-normal">たか</rt></ruby>さを、まずは<ruby>貴機関<rt class="text-xs font-normal">ききかん</rt></ruby>の<ruby>目<rt class="text-xs font-normal">め</rt></ruby>でご<ruby>確認<rt class="text-xs font-normal">かくにん</rt></ruby>ください。<ruby>全<rt class="text-xs font-normal">ぜん</rt></ruby>4<ruby>週間<rt class="text-xs font-normal">しゅうかん</rt></ruby>（<ruby>計<rt class="text-xs font-normal">けい</rt></ruby>20<ruby>時間<rt class="text-xs font-normal">じかん</rt></ruby>）のコースを、<ruby>導入<rt class="text-xs font-normal">どうにゅう</rt></ruby>リスクを<ruby>最小限<rt class="text-xs font-normal">さいしょうげん</rt></ruby>に<ruby>抑<rt class="text-xs font-normal">おさ</rt></ruby>えられる<ruby>特別<rt class="text-xs font-normal">とくべつ</rt></ruby>なトライアル<ruby>料金<rt class="text-xs font-normal">りょうきん</rt></ruby>でご<ruby>提供<rt class="text-xs font-normal">ていきょう</rt></ruby>します。
            </p>

            <div class="max-w-4xl mx-auto grid md:grid-cols-2 gap-8 items-stretch px-4">
                <!-- Regular Plan -->
                <div class="bg-white p-8 rounded-xl shadow-xl border-2 border-gray-300 flex flex-col transform transition duration-300 hover:shadow-2xl">
                    <h5 class="text-2xl font-semibold text-center text-gray-700 mb-6"><ruby>通常<rt class="text-xs font-normal">つうじょう</rt></ruby>プログラム</h5>
                    <div class="text-center mb-6">
                        <span class="text-5xl font-bold">100,000<span class="text-xl font-medium">円</span></span>
                        <span class="block text-gray-600">/ <ruby>受講生<rt class="text-xs font-normal">じゅこうせい</rt></ruby>グループ・<ruby>月<rt class="text-xs font-normal">げつ</rt></ruby></span>
                    </div>
                    <ul class="space-y-3 mb-8 flex-grow text-left">
                        <li class="flex items-center">
                            <span class="text-green-500 mr-2">✔</span> <ruby>講師料<rt class="text-xs font-normal">こうしりょう</rt></ruby>：5,000<ruby>円<rt class="text-xs font-normal">えん</rt></ruby>/<ruby>時<rt class="text-xs font-normal">じ</rt></ruby>
                        </li>
                        <li class="flex items-center">
                            <span class="text-green-500 mr-2">✔</span> <ruby>総額<rt class="text-xs font-normal">そうがく</rt></ruby>：5,000<ruby>円<rt class="text-xs font-normal">えん</rt></ruby> $\times$ 20<ruby>時間<rt class="text-xs font-normal">じかん</rt></ruby>
                        </li>
                        <li class="flex items-center">
                            <span class="text-green-500 mr-2">✔</span> <ruby>現場直結<rt class="text-xs font-normal">げんばちょっけつ</rt></ruby>のオリジナル<ruby>教材<rt class="text-xs font-normal">きょうざい</rt></ruby>（PDF）
                        </li>
                    </ul>
                    <button class="w-full bg-gray-400 text-white py-3 rounded-lg font-semibold cursor-not-allowed opacity-70">（<ruby>本契約<rt class="text-xs font-normal">ほんけいやく</rt></ruby>）</button>
                </div>

                <!-- Trial Plan (Highlighted) -->
                <div class="bg-yellow-50 p-8 rounded-xl shadow-2xl border-4 border-yellow-500 flex flex-col relative overflow-hidden">
                    <div class="absolute top-0 right-0 bg-yellow-400 text-yellow-900 font-bold px-8 py-1 transform translate-x-1/4 rotate-45 translate-y-1/2 shadow-md">
                        <ruby>特別価格<rt class="text-xs font-normal">とくべつかかく</rt></ruby>
                    </div>
                    <h5 class="text-2xl font-bold text-center text-yellow-900 mb-6">💥 1ヶ<ruby>月<rt class="text-xs font-normal">げつ</rt></ruby>トライアル</h5>
                    <div class="text-center mb-6">
                        <span class="text-5xl font-bold text-red-600">89,000<span class="text-xl font-medium">円</span></span>
                        <span class="block text-gray-600">/ <ruby>受講生<rt class="text-xs font-normal">じゅこうせい</rt></ruby>グループ・<ruby>月<rt class="text-xs font-normal">げつ</rt></ruby></span>
                    </div>
                    <ul class="space-y-3 mb-8 flex-grow text-left">
                        <li class="flex items-center">
                            <span class="text-green-500 mr-2">✔</span> <strong class="text-red-600"><ruby>大幅割引<rt class="text-xs font-normal">おおはばわりびき</rt></ruby>！</strong>
                        </li>
                        <li class="flex items-center">
                            <span class="text-green-500 mr-2">✔</span> <ruby>全<rt class="text-xs font-normal">ぜん</rt></ruby>4<ruby>週間<rt class="text-xs font-normal">しゅうかん</rt></ruby>（20<ruby>時間<rt class="text-xs font-normal">じかん</rt></ruby>）の<ruby>全内容<rt class="text-xs font-normal">ぜんないよう</rt></ruby>を<ruby>体験<rt class="text-xs font-normal">たいけん</rt></ruby>
                        </li>
                        <li class="flex items-center">
                            <span class="text-green-500 mr-2">✔</span> <ruby>導入前後<rt class="text-xs font-normal">どうにゅうぜんご</rt></ruby>の<ruby>効果測定<rt class="text-xs font-normal">こうかそくてい</rt></ruby>テスト<ruby>付<rt class="text-xs font-normal">つ</rt></ruby>き
                        </li>
                    </ul>
                    <!-- 変更点: Formspreeに対応させるため、formタグで囲み、ボタンをsubmitに変更 -->
                    <form action="https://formspree.io/f/mldolzwl" method="POST">
                        <!-- トライアルプランの識別情報や連絡先などを隠しフィールドで送ることも可能だが、今回はUI変更のみに留める -->
                        <input type="hidden" name="プラン" value="1ヶ月トライアル">
                        <input type="submit" value="トライアルに申し込む" class="w-full bg-blue-600 hover:bg-blue-700 active:bg-blue-800 text-white py-3 rounded-lg font-semibold text-lg shadow-lg transition duration-300 transform hover:scale-[1.01] focus:outline-none focus:ring-4 focus:ring-blue-300 cursor-pointer">
                    </form>
                </div>
            </div>
            
            <div class="max-w-4xl mx-auto mt-12 px-4">
                <h5 class="text-xl font-semibold text-center mb-6 text-gray-800">トライアルのメリット</h5>
                <div class="grid sm:grid-cols-3 gap-6 text-center">
                    <div class="bg-white p-4 rounded-lg shadow-md border-b-4 border-blue-400">
                        <h6 class="font-semibold text-blue-700">1. <ruby>授業<rt class="text-xs font-normal">じゅぎょう</rt></ruby>の<ruby>質<rt class="text-xs font-normal">しつ</rt></ruby>を<ruby>確認<rt class="text-xs font-normal">かくにん</rt></ruby>できる</h6>
                        <p class="text-sm text-gray-600"><ruby>講師<rt class="text-xs font-normal">こうし</rt></ruby>の<ruby>指導力<rt class="text-xs font-normal">しどうりょく</rt></ruby>やカリキュラムの<ruby>有効性<rt class="text-xs font-normal">ゆうこうせい</rt></ruby>を<ruby>貴機関<rt class="text-xs font-normal">ききかん</rt></ruby>の<ruby>目<rt class="text-xs font-normal">め</rt></ruby>で<ruby>確認<rt class="text-xs font-normal">かくにん</rt></ruby>できます。</p>
                    </div>
                    <div class="bg-white p-4 rounded-lg shadow-md border-b-4 border-blue-400">
                        <h6 class="font-semibold text-blue-700">2. <ruby>受講生<rt class="text-xs font-normal">じゅこうせい</rt></ruby>の<ruby>適応<rt class="text-xs font-normal">てきおう</rt></ruby>を<ruby>判断<rt class="text-xs font-normal">はんだん</rt></ruby></h6>
                        <p class="text-sm text-gray-600"><ruby>受講生<rt class="text-xs font-normal">じゅこうせい</rt></ruby>がこの<ruby>実践的<rt class="text-xs font-normal">じっせんてき</rt></ruby>な<ruby>学習<rt class="text-xs font-normal">がくしゅう</rt></ruby>スタイルに<ruby>適応<rt class="text-xs font-normal">てきおう</rt></ruby>できるかを<ruby>判断<rt class="text-xs font-normal">はんだん</rt></ruby>できます。</p>
                    </div>
                    <div class="bg-white p-4 rounded-lg shadow-md border-b-4 border-blue-400">
                        <h6 class="font-semibold text-blue-700">3. <ruby>導入後<rt class="text-xs font-normal">どうにゅうご</rt></ruby>の<ruby>効果<rt class="text-xs font-normal">こうか</rt></ruby>を<ruby>可視化<rt class="text-xs font-normal">かしか</rt></ruby></h6>
                        <p class="text-sm text-gray-600"><ruby>前後<rt class="text-xs font-normal">ぜんご</rt></ruby>テストにより、<ruby>会話力向上<rt class="text-xs font-normal">かいわりょくこうじょう</rt></ruby>の<ruby>効果<rt class="text-xs font-normal">こうか</rt></ruby>を<ruby>具体的<rt class="text-xs font-normal">ぐたいてき</rt></ruby>にイメージできます。</p>
                    </div>
                </div>
            </div>
        </section>

        <!-- 5. Flow & Effect (Sec 9) -->
        <section id="flow" class="pt-16 -mt-12 pb-20 bg-gray-100 rounded-xl shadow-inner">
            <h3 class="text-3xl font-bold text-center mb-16 text-gray-900">🚀 <ruby>導入<rt class="text-xs font-normal">どうにゅう</rt></ruby>の<ruby>流<rt class="text-xs font-normal">なが</rt></ruby>れと<ruby>期待<rt class="text-xs font-normal">きたい</rt></ruby>される<ruby>効果<rt class="text-xs font-normal">こうか</rt></ruby></h3>

            <div class="max-w-6xl mx-auto grid md:grid-cols-2 gap-12 px-4">
                
                <div>
                    <h4 class="text-2xl font-semibold text-center mb-8 text-gray-800">➡️ トライアル<ruby>導入<rt class="text-xs font-normal">どうにゅう</rt></ruby>の<ruby>流<rt class="text-xs font-normal">なが</rt></ruby>れ</h4>
                    <p class="text-center text-gray-700 mb-8 max-w-lg mx-auto">
                        お<ruby>申<rt class="text-xs font-normal">もう</rt></ruby>し<ruby>込<rt class="text-xs font-normal">こ</rt></ruby>みからトライアル<ruby>実施<rt class="text-xs font-normal">じっし</rt></ruby>、<ruby>効果<rt class="text-xs font-normal">こうか</rt></ruby>の<ruby>確認<rt class="text-xs font-normal">かくにん</rt></ruby>までをスムーズにサポートします。
                    </p>
                    <ol class="space-y-6">
                        <li class="flex items-center">
                            <span class="flex-shrink-0 w-10 h-10 bg-blue-600 text-white rounded-full flex items-center justify-center font-bold text-lg mr-4 shadow-md">1</span>
                            <span class="bg-white p-4 rounded-lg shadow-md flex-grow border border-gray-200"><strong>ご<ruby>検討<rt class="text-xs font-normal">けんとう</rt></ruby>・トライアル<ruby>決定<rt class="text-xs font-normal">けってい</rt></ruby></strong><br><span class="text-sm text-gray-600"><ruby>本提案内容<rt class="text-xs font-normal">ほんていあんないよう</rt></ruby>をご<ruby>確認<rt class="text-xs font-normal">かくにん</rt></ruby>の<ruby>上<rt class="text-xs font-normal">うえ</rt></ruby>、お<ruby>申<rt class="text-xs font-normal">もう</rt></ruby>し<ruby>込<rt class="text-xs font-normal">こ</rt></ruby>みください。</span></span>
                        </li>
                        <li class="flex items-center">
                            <span class="flex-shrink-0 w-10 h-10 bg-blue-600 text-white rounded-full flex items-center justify-center font-bold text-lg mr-4 shadow-md">2</span>
                            <span class="bg-white p-4 rounded-lg shadow-md flex-grow border border-gray-200"><strong><ruby>開講準備<rt class="text-xs font-normal">かいこうじゅんび</rt></ruby></strong><br><span class="text-sm text-gray-600"><ruby>日程調整<rt class="text-xs font-normal">にっていちょうせい</rt></ruby>、<ruby>受講生選定<rt class="text-xs font-normal">じゅこうせいせんてい</rt></ruby>、<ruby>環境構築<rt class="text-xs font-normal">かんきょうこうちく</rt></ruby>を<ruby>行<rt class="text-xs font-normal">おこな</rt></ruby>います。</span></span>
                        </li>
                        <li class="flex items-center">
                            <span class="flex-shrink-0 w-10 h-10 bg-blue-600 text-white rounded-full flex items-center justify-center font-bold text-lg mr-4 shadow-md">3</span>
                            <span class="bg-white p-4 rounded-lg shadow-md flex-grow border border-gray-200"><strong>トライアル1ヶ<ruby>月実施<rt class="text-xs font-normal">げつじっし</rt></ruby></strong><br><span class="text-sm text-gray-600"><ruby>導入前<rt class="text-xs font-normal">どうにゅうまえ</rt></ruby>テスト、<ruby>授業実施<rt class="text-xs font-normal">じゅぎょうじっし</rt></ruby>、<ruby>最終<rt class="text-xs font-normal">さいしゅう</rt></ruby>テストを<ruby>行<rt class="text-xs font-normal">おこな</rt></ruby>います。</span></span>
                        </li>
                        <li class="flex items-center">
                            <span class="flex-shrink-0 w-10 h-10 bg-blue-600 text-white rounded-full flex items-center justify-center font-bold text-lg mr-4 shadow-md">4</span>
                            <span class="bg-white p-4 rounded-lg shadow-md flex-grow border border-gray-200"><strong><ruby>結果共有<rt class="text-xs font-normal">けっかきょうゆう</rt></ruby>・<ruby>本格導入決定<rt class="text-xs font-normal">ほんかくどうにゅうけってい</rt></ruby></strong><br><span class="text-sm text-gray-600"><ruby>効果測定<rt class="text-xs font-normal">こうかそくてい</rt></ruby>の<ruby>結果<rt class="text-xs font-normal">けっか</rt></ruby>を<ruby>共有<rt class="text-xs font-normal">きょうゆう</rt></ruby>し、<ruby>本格導入<rt class="text-xs font-normal">ほんかくどうにゅう</rt></ruby>をご<ruby>判断<rt class="text-xs font-normal">はんだん</rt></ruby>いただきます。</span></span>
                        </li>
                    </ol>
                </div>

                <div>
                    <h4 class="text-2xl font-semibold text-center mb-8 text-gray-800">📈 <ruby>期待<rt class="text-xs font-normal">きたい</rt></ruby>される<ruby>効果<rt class="text-xs font-normal">こうか</rt></ruby></h4>
                    <p class="text-center text-gray-700 mb-8 max-w-lg mx-auto">
                        このプログラムは、<ruby>実習生個人<rt class="text-xs font-normal">じっしゅうせいこじん</rt></ruby>のスキルアップだけでなく、<ruby>貴機関<rt class="text-xs font-normal">ききかん</rt></ruby>のブランド<ruby>価値向上<rt class="text-xs font-normal">かちこうじょう</rt></ruby>にも<ruby>直結<rt class="text-xs font-normal">ちょっけつ</rt></ruby>します。
                    </p>
                    <div class="overflow-x-auto">
                        <table class="w-full min-w-max bg-white rounded-xl shadow-lg overflow-hidden border border-gray-200">
                            <thead class="bg-gray-200 text-gray-700">
                                <tr>
                                    <th class="py-3 px-4 text-left border-b border-gray-300"><ruby>現状<rt class="text-xs font-normal">げんじょう</rt></ruby> (Before)</th>
                                    <th class="py-3 px-4 text-left border-b border-gray-300"><ruby>本<rt class="text-xs font-normal">ほん</rt></ruby>プログラム<ruby>導入後<rt class="text-xs font-normal">どうにゅうご</rt></ruby> (After)</th>
                                </tr>
                            </thead>
                            <tbody class="divide-y divide-gray-100">
                                <tr class="hover:bg-blue-50">
                                    <td class="py-4 px-4 text-gray-600">N5<ruby>知識<rt class="text-xs font-normal">ちしき</rt></ruby>はあるが<ruby>自信<rt class="text-xs font-normal">じしん</rt></ruby>がない</td>
                                    <td class="py-4 px-4 font-semibold text-blue-700"><ruby>会話<rt class="text-xs font-normal">かいわ</rt></ruby>に<ruby>対<rt class="text-xs font-normal">たい</rt></ruby>する<ruby>積極性<rt class="text-xs font-normal">せっきょくせい</rt></ruby>が<ruby>格段<rt class="text-xs font-normal">かくだん</rt></ruby>に<ruby>向上<rt class="text-xs font-normal">こうじょう</rt></ruby></td>
                                </tr>
                                <tr class="hover:bg-blue-50">
                                    <td class="py-4 px-4 text-gray-600"><ruby>来日直後<rt class="text-xs font-normal">らいにちちょくご</rt></ruby>のストレスが<ruby>大<rt class="text-xs font-normal">おお</rt></ruby>きい</td>
                                    <td class="py-4 px-4 font-semibold text-blue-700"><ruby>日本<rt class="text-xs font-normal">にほん</rt></ruby>での<ruby>生活<rt class="text-xs font-normal">せいかつ</rt></ruby>・<ruby>業務<rt class="text-xs font-normal">ぎょうむ</rt></ruby>の<ruby>初期<rt class="text-xs font-normal">しょき</rt></ruby>ストレスを<ruby>軽減<rt class="text-xs font-normal">けいげん</rt></ruby></td>
                                </tr>
                                <tr class="hover:bg-blue-50">
                                    <td class="py-4 px-4 text-gray-600"><ruby>採用後<rt class="text-xs font-normal">さいようご</rt></ruby>の<ruby>定着<rt class="text-xs font-normal">ていちゃく</rt></ruby>に<ruby>不安<rt class="text-xs font-normal">ふあん</rt></ruby>がある</td>
                                    <td class="py-4 px-4 font-semibold text-blue-700"><ruby>日本人<rt class="text-xs font-normal">にほんじん</rt></ruby>との<ruby>信頼関係<rt class="text-xs font-normal">しんらいかんけい</rt></ruby>を<ruby>築<rt class="text-xs font-normal">きず</rt></ruby>きやすく、<ruby>定着率向上<rt class="text-xs font-normal">ていちゃくりつこうじょう</rt></ruby>に<ruby>貢献<rt class="text-xs font-normal">こうけん</rt></ruby></td>
                                </tr>
                            </tbody>
                        </table>
                    </div>
                    <p class="mt-8 p-4 bg-blue-100 text-blue-800 font-bold rounded-lg shadow-md border border-blue-300">
                        <ruby>会話力<rt class="text-xs font-normal">かいわりょく</rt></ruby>の<ruby>高<rt class="text-xs font-normal">たか</rt></ruby>い<ruby>実習生<rt class="text-xs font-normal">じっしゅうせい</rt></ruby>の<ruby>送<rt class="text-xs font-normal">おく</rt></ruby>り<ruby>出<rt class="text-xs font-normal">だ</rt></ruby>しは、<ruby>貴機関<rt class="text-xs font-normal">ききかん</rt></ruby>のブランド<ruby>価値<rt class="text-xs font-normal">かち</rt></ruby>を<ruby>飛躍的<rt class="text-xs font-normal">ひやくてき</rt></ruby>に<ruby>高<rt class="text-xs font-normal">たか</rt></ruby>めます。
                    </p>
                </div>
            </div>
        </section>

    </main>

    <!-- Footer -->
    <footer class="bg-gray-800 text-white py-10 text-center">
        <p>ご<ruby>提案<rt class="text-xs font-normal">ていあん</rt></ruby>：[<ruby>提案者名<rt class="text-xs font-normal">ていあんしゃめい</rt></ruby>/ロゴ]</p>
        <p class="text-sm text-gray-400 mt-2">© 2025 [<ruby>提案者名<rt class="text-xs font-normal">ていあんしゃめい</rt></ruby>]. All rights reserved.</p>
    </footer>

    <script>
        document.addEventListener('DOMContentLoaded', () => {
            
            // --- Tab Switching Logic ---
            const tabButtons = document.querySelectorAll('.tab-btn');
            const tabPanels = document.querySelectorAll('.tab-panel');

            // Function to handle tab activation
            const activateTab = (targetTab) => {
                // Deactivate all buttons and panels
                tabButtons.forEach(btn => btn.classList.remove('active'));
                tabPanels.forEach(panel => panel.classList.remove('active'));

                // Activate clicked button and target panel
                const targetButton = document.querySelector(`.tab-btn[data-tab="${targetTab}"]`);
                const targetPanel = document.getElementById(`tab-${targetTab}`);
                
                if (targetButton && targetPanel) {
                    targetButton.classList.add('active');
                    targetPanel.classList.add('active');
                    
                    // Trigger chart re-render if it's the lesson tab
                    if (targetTab === 'lesson') {
                        // Chart.js doesn't strictly need a redraw on tab switch if properly initiated
                        // but sometimes helps ensure responsiveness
                        if (window.lessonDoughnutChart) {
                             // This is a minimal way to ensure Chart.js re-initializes or re-sizes correctly if needed
                            window.lessonDoughnutChart.resize(); 
                        }
                    }
                }
            };
            
            // Set up click listeners for all tab buttons
            tabButtons.forEach(button => {
                button.addEventListener('click', () => {
                    const targetTab = button.getAttribute('data-tab');
                    activateTab(targetTab);
                });
            });


            // --- Chart.js Doughnut Chart Logic ---
            const lessonChartCanvas = document.getElementById('lessonChart');
            if (lessonChartCanvas) {
                const ctx = lessonChartCanvas.getContext('2d');
                
                // Initialize the chart once and store it globally for potential access (e.g., resize)
                window.lessonDoughnutChart = new Chart(ctx, {
                    type: 'doughnut',
                    data: {
                        labels: [
                            'トピックスの練習 (20分) - インプット',
                            '会話のロールプレイング (20分) - アウトプット',
                            '発表とフィードバック (20分) - アウトプット'
                        ],
                        datasets: [{
                            label: '60分の授業構成',
                            data: [20, 20, 20],
                            backgroundColor: [
                                'rgb(156, 163, 175, 0.7)', // gray-400 for input (subtle)
                                'rgb(59, 130, 246, 0.8)', // blue-500 for core output
                                'rgb(16, 185, 129, 0.8)'  // green-500 for presentation/feedback (crucial output)
                            ],
                            borderColor: [
                                'rgb(75, 85, 99)',
                                'rgb(37, 99, 235)',
                                'rgb(5, 150, 105)'
                            ],
                            borderWidth: 2
                        }]
                    },
                    options: {
                        responsive: true,
                        maintainAspectRatio: false,
                        cutout: '75%', /* Makes it a thin doughnut chart */
                        plugins: {
                            legend: {
                                position: 'bottom',
                                labels: {
                                    padding: 20,
                                    font: {
                                        size: 14
                                    }
                                }
                            },
                            tooltip: {
                                callbacks: {
                                    label: function(context) {
                                        let label = context.label || '';
                                        if (label) {
                                            // Extract minute value from label
                                            const match = label.match(/\((\d+)分\)/);
                                            const minutes = match ? match[1] : context.parsed;
                                            
                                            // Clean up label for tooltip
                                            label = label.split('(')[0].trim(); 
                                            return `${label}: ${minutes}分`;
                                        }
                                        return null;
                                    }
                                }
                            }
                        }
                    }
                });
            }

            // --- Smooth Scroll for Navigation ---
            document.querySelectorAll('a[href^="#"]').forEach(anchor => {
                anchor.addEventListener('click', function (e) {
                    e.preventDefault();
                    const targetId = this.getAttribute('href');
                    const targetElement = document.querySelector(targetId);
                    if(targetElement) {
                        // Adjust scroll to account for fixed header (16 + padding/margin, roughly 90px)
                        const offset = 90; 
                        const elementPosition = targetElement.getBoundingClientRect().top;
                        const offsetPosition = elementPosition + window.pageYOffset - offset;

                        window.scrollTo({
                            top: offsetPosition,
                            behavior: "smooth"
                        });
                    }
                });
            });
        });
    </script>

</body>
</html>
****
