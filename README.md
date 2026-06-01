<!DOCTYPE html>
<html lang="az">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Baku Electronics — Marketinq Departamenti Portalı</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link href="https://fonts.googleapis.com/css2?family=Montserrat:wght@400;600;700;800&family=Inter:wght@300;400;500;600;700&display=swap" rel="stylesheet">
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.5.1/css/all.min.css">
    
    <script>
        tailwind.config = {
            theme: {
                extend: {
                    colors: {
                        be: {
                            red: '#e30a17', // Rəsmi Baku Electronics Qırmızısı
                            dark: '#0f172a',
                            slate: '#1e293b',
                            light: '#f8fafc',
                            card: '#ffffff',
                            border: '#e2e8f0'
                        }
                    },
                    fontFamily: {
                        sans: ['Inter', 'sans-serif'],
                        heading: ['Montserrat', 'sans-serif'],
                    }
                }
            }
        }
    </script>
    <style>
        html {
            scroll-behavior: smooth;
        }
        /* Custom scrollbar */
        ::-webkit-scrollbar {
            width: 8px;
        }
        ::-webkit-scrollbar-track {
            background: #f1f1f1;
        }
        ::-webkit-scrollbar-thumb {
            background: #cbd5e1;
            border-radius: 4px;
        }
        ::-webkit-scrollbar-thumb:hover {
            background: #e30a17;
        }
    </style>
</head>
<body class="bg-be-light text-be-dark font-sans min-h-screen flex flex-col">

    <header class="sticky top-0 z-50 bg-white/95 backdrop-blur-md border-b border-be-border shadow-sm">
        <div class="max-w-7xl mx-auto px-6 h-20 flex items-center justify-between">
            <a href="#" class="flex items-center gap-3">
                <span class="text-be-red text-2xl font-black tracking-tighter uppercase font-heading">
                    BAKU <span class="bg-be-red text-white px-2 py-0.5 rounded ml-1">ELECTRONICS</span>
                </span>
            </a>
            <div class="hidden lg:flex items-center gap-3 text-sm text-slate-500 font-medium">
                <span class="px-3 py-1 bg-red-50 text-be-red font-semibold rounded-full text-xs uppercase tracking-wider">Daxili Portal</span>
                <span class="border-l border-slate-200 h-4 mx-2"></span>
                <span><i class="fa-solid fa-phone text-be-red mr-1"></i> Rəsmi Dəstək: *1414</span>
            </div>
        </div>
    </header>

    <section class="relative bg-gradient-to-br from-be-dark via-[#131c2e] to-be-dark text-white py-16 px-6 overflow-hidden">
        <div class="absolute inset-0 bg-[radial-gradient(circle_at_top_right,rgba(227,10,23,0.15),transparent_40%)]"></div>
        <div class="max-w-7xl mx-auto relative z-10 text-center lg:text-left lg:flex lg:items-center lg:justify-between gap-12">
            <div class="max-w-3xl space-y-6">
                <span class="inline-flex items-center gap-2 px-3 py-1 rounded-full bg-be-red/10 border border-be-red/30 text-be-red text-xs font-bold uppercase tracking-wider">
                    <span class="w-2 h-2 rounded-full bg-be-red animate-ping"></span> Struktur və Komanda Kataloqu
                </span>
                <h1 class="font-heading font-extrabold text-4xl sm:text-5xl lg:text-6xl text-white tracking-tight leading-tight">
                    Marketinq <br class="hidden sm:inline"> Departamenti
                </h1>
                <p class="text-slate-300 text-base sm:text-lg max-w-2xl leading-relaxed">
                    Baku Electronics-in brend dəyərini ucaldan, müştəri kommunikasiyasını və rəqəmsal inkişaf dinamikasını idarə edən çevik komandamızla tanış olun.
                </p>
            </div>
            <div class="mt-8 lg:mt-0 grid grid-cols-2 gap-4 w-full lg:w-auto shrink-0 max-w-sm mx-auto lg:mx-0">
                <div class="p-5 bg-white/5 border border-white/10 rounded-xl text-center backdrop-blur-sm">
                    <p class="text-be-red text-3xl font-extrabold font-heading">39</p>
                    <p class="text-slate-400 text-xs uppercase tracking-wider mt-1 font-semibold">Peşəkar Kadr</p>
                </div>
                <div class="p-5 bg-white/5 border border-white/10 rounded-xl text-center backdrop-blur-sm">
                    <p class="text-be-red text-3xl font-extrabold font-heading">7</p>
                    <p class="text-slate-400 text-xs uppercase tracking-wider mt-1 font-semibold">Aktiv Şöbə</p>
                </div>
            </div>
        </div>
    </section>

    <section class="py-10 px-6 bg-white border-b border-be-border sticky top-20 z-40 shadow-sm">
        <div class="max-w-7xl mx-auto flex flex-col lg:flex-row lg:items-center justify-between gap-6">
            
            <div class="flex items-center gap-2 overflow-x-auto pb-2 lg:pb-0 no-scrollbar -mx-6 px-6 lg:mx-0 lg:px-0">
                <button onclick="filterDepartment('all')" id="btn-all" class="dept-btn px-4 py-2 text-xs font-bold uppercase tracking-wider rounded-lg transition-all duration-300 shrink-0 bg-be-red text-white shadow-md shadow-be-red/10">
                    Hamısı
                </button>
                <button onclick="filterDepartment('management')" id="btn-management" class="dept-btn px-4 py-2 text-xs font-bold uppercase tracking-wider rounded-lg transition-all duration-300 shrink-0 bg-slate-100 text-slate-600 hover:bg-slate-200">
                    Rəhbərlik
                </button>
                <button onclick="filterDepartment('pm_unit')" id="btn-pm_unit" class="dept-btn px-4 py-2 text-xs font-bold uppercase tracking-wider rounded-lg transition-all duration-300 shrink-0 bg-slate-100 text-slate-600 hover:bg-slate-200">
                    PM Unit
                </button>
                <button onclick="filterDepartment('growth_unit')" id="btn-growth_unit" class="dept-btn px-4 py-2 text-xs font-bold uppercase tracking-wider rounded-lg transition-all duration-300 shrink-0 bg-slate-100 text-slate-600 hover:bg-slate-200">
                    Growth
                </button>
                <button onclick="filterDepartment('mar_com')" id="btn-mar_com" class="dept-btn px-4 py-2 text-xs font-bold uppercase tracking-wider rounded-lg transition-all duration-300 shrink-0 bg-slate-100 text-slate-600 hover:bg-slate-200">
                    Kommunikasiya
                </button>
                <button onclick="filterDepartment('smm')" id="btn-smm" class="dept-btn px-4 py-2 text-xs font-bold uppercase tracking-wider rounded-lg transition-all duration-300 shrink-0 bg-slate-100 text-slate-600 hover:bg-slate-200">
                    SMM
                </button>
                <button onclick="filterDepartment('design')" id="btn-design" class="dept-btn px-4 py-2 text-xs font-bold uppercase tracking-wider rounded-lg transition-all duration-300 shrink-0 bg-slate-100 text-slate-600 hover:bg-slate-200">
                    Dizayn
                </button>
                <button onclick="filterDepartment('crm')" id="btn-crm" class="dept-btn px-4 py-2 text-xs font-bold uppercase tracking-wider rounded-lg transition-all duration-300 shrink-0 bg-slate-100 text-slate-600 hover:bg-slate-200">
                    CRM
                </button>
            </div>

            <div class="relative w-full lg:w-80">
                <span class="absolute left-4 top-1/2 -translate-y-1/2 text-slate-400">
                    <i class="fa-solid fa-magnifying-glass"></i>
                </span>
                <input type="text" id="searchInput" onkeyup="searchTeam()" placeholder="Ad, soyad və ya vəzifə axtar..." class="w-full bg-slate-50 border border-be-border pl-11 pr-4 py-3 rounded-lg focus:outline-none focus:ring-2 focus:ring-be-red/20 focus:border-be-red transition-all text-sm placeholder:text-slate-400">
            </div>

        </div>
    </section>

    <main class="flex-grow py-16 px-6">
        <div class="max-w-7xl mx-auto">
            
            <div id="teamGrid" class="grid grid-cols-1 sm:grid-cols-2 md:grid-cols-3 lg:grid-cols-4 gap-8">
                </div>

            <div id="noResults" class="hidden text-center py-20">
                <div class="text-slate-300 text-6xl mb-4">
                    <i class="fa-regular fa-face-frown"></i>
                </div>
                <h3 class="font-heading font-bold text-xl text-slate-700">Axtarışa uyğun heç kim tapılmadı</h3>
                <p class="text-slate-400 text-sm mt-1">Zəhmət olmasa daxil etdiyiniz parametrləri yenidən yoxlayın.</p>
            </div>

        </div>
    </main>

    <footer class="bg-be-dark text-white border-t border-be-border/10 py-10 px-6 mt-auto">
        <div class="max-w-7xl mx-auto flex flex-col md:flex-row items-center justify-between gap-6 text-sm text-slate-400">
            <div class="flex items-center gap-3">
                <span class="text-be-red text-lg font-bold tracking-tighter uppercase font-heading">BAKU ELECTRONICS</span>
                <span class="text-slate-600">|</span>
                <span>© 2026 Marketinq Departamenti. Bütün hüquqlar qorunur.</span>
            </div>
            <div class="flex items-center gap-6">
                <span>Daxili Rabitə: <strong>*1414</strong></span>
                <span class="w-1.5 h-1.5 rounded-full bg-be-red"></span>
                <a href="mailto:marketing@bakuelectronics.az" class="hover:text-be-red transition-colors text-white">marketing@bakuelectronics.az</a>
            </div>
        </div>
    </footer>

    <div id="copyAlert" class="fixed bottom-6 right-6 z-50 bg-slate-900 text-white px-5 py-3 rounded-xl shadow-2xl flex items-center gap-3 transform translate-y-20 opacity-0 pointer-events-none transition-all duration-300">
        <span class="text-emerald-400 text-lg"><i class="fa-solid fa-circle-check"></i></span>
        <span class="text-sm font-medium">Əlaqə məlumatı kopyalandı!</span>
    </div>

    <script>
        // Bütün şöbələrin və əməkdaşların tam məlumat bazası
        // PDF-dəki fotoları yerləşdirmək üçün "image" bölməsinə müvafiq URL-i daxil edə bilərsiniz.
        const teamData = [
            // DEPARTAMENT RƏHBƏRLİYİ
            {
                id: 1,
                name: "Aslan Həsənli",
                role: "Departament Direktoru",
                deptKey: "management",
                deptName: "Departament Rəhbərliyi",
                phone: "+994 (55) 000-00-00", 
                internal: "1001",
                email: "a.hasanli@bakuelectronics.az",
                image: "" 
            },
            // PM UNIT
            {
                id: 2,
                name: "Ayla İsmayılzadə",
                role: "Şöbə Müdiri",
                deptKey: "pm_unit",
                deptName: "PM Unit (Layihə İdarəetmə)",
                phone: "+994 (55) 000-00-00",
                internal: "1101",
                email: "a.ismayilzade@bakuelectronics.az",
                image: ""
            },
            {
                id: 3,
                name: "Nəzrin İmaməliyeva",
                role: "Baş Menecer",
                deptKey: "pm_unit",
                deptName: "PM Unit (Layihə İdarəetmə)",
                phone: "+994 (55) 000-00-00",
                internal: "1102",
                email: "n.imamaliyeva@bakuelectronics.az",
                image: ""
            },
            {
                id: 4,
                name: "Səadət Ağabalayeva",
                role: "Menecer",
                deptKey: "pm_unit",
                deptName: "PM Unit (Layihə İdarəetmə)",
                phone: "+994 (55) 000-00-00",
                internal: "1103",
                email: "s.agabalayeva@bakuelectronics.az",
                image: ""
            },
            {
                id: 5,
                name: "Sevil Qədirova",
                role: "Kiçik Menecer",
                deptKey: "pm_unit",
                deptName: "PM Unit (Layihə İdarəetmə)",
                phone: "+994 (55) 000-00-00",
                internal: "1104",
                email: "s.qadirova@bakuelectronics.az",
                image: ""
            },
            {
                id: 6,
                name: "Jalə Balayeva",
                role: "Koordinator",
                deptKey: "pm_unit",
                deptName: "PM Unit (Layihə İdarəetmə)",
                phone: "+994 (55) 000-00-00",
                internal: "1105",
                email: "j.balayeva@bakuelectronics.az",
                image: ""
            },
            {
                id: 7,
                name: "Leyla Həsənova",
                role: "Seven Space — Brend Menecer",
                deptKey: "pm_unit",
                deptName: "PM Unit (Layihə İdarəetmə)",
                phone: "+994 (55) 000-00-00",
                internal: "1106",
                email: "l.hasanova@bakuelectronics.az",
                image: ""
            },
            {
                id: 8,
                name: "Emil Nəcəfli",
                role: "MotoVerse — Brend Menecer",
                deptKey: "pm_unit",
                deptName: "PM Unit (Layihə İdarəetmə)",
                phone: "+994 (55) 000-00-00",
                internal: "1107",
                email: "e.najafli@bakuelectronics.az",
                image: ""
            },
            // GROWTH UNIT
            {
                id: 9,
                name: "Ərtunc Behbudlu",
                role: "Şöbə Rəhbəri",
                deptKey: "growth_unit",
                deptName: "Growth Unit",
                phone: "+994 (55) 000-00-00",
                internal: "1201",
                email: "e.behbudlu@bakuelectronics.az",
                image: ""
            },
            {
                id: 10,
                name: "Aytəkin Salmanova",
                role: "Baş Mütəxəssis",
                deptKey: "growth_unit",
                deptName: "Growth Unit",
                phone: "+994 (55) 000-00-00",
                internal: "1202",
                email: "a.salmanova@bakuelectronics.az",
                image: ""
            },
            {
                id: 11,
                name: "Qərənfil Yaqubova",
                role: "Baş Mütəxəssis",
                deptKey: "growth_unit",
                deptName: "Growth Unit",
                phone: "+994 (55) 000-00-00",
                internal: "1203",
                email: "q.yaqubova@bakuelectronics.az",
                image: ""
            },
            {
                id: 12,
                name: "Nicat Rəşidli",
                role: "Mütəxəssis",
                deptKey: "growth_unit",
                deptName: "Growth Unit",
                phone: "+994 (55) 000-00-00",
                internal: "1204",
                email: "n.rashidli@bakuelectronics.az",
                image: ""
            },
            {
                id: 13,
                name: "Emin Əzimov",
                role: "Mütəxəssis",
                deptKey: "growth_unit",
                deptName: "Growth Unit",
                phone: "+994 (55) 000-00-00",
                internal: "1205",
                email: "e.azimov@bakuelectronics.az",
                image: ""
            },
            // MARKETİNQ KOMMUNİKASİYALARI
            {
                id: 14,
                name: "Nigar Mehdiyeva",
                role: "Şöbə Rəhbəri",
                deptKey: "mar_com",
                deptName: "Marketinq Kommunikasiyaları",
                phone: "+994 (55) 000-00-00",
                internal: "1301",
                email: "n.mehdiyeva@bakuelectronics.az",
                image: ""
            },
            {
                id: 15,
                name: "İmran Səyyaflı",
                role: "Baş Mütəxəssis",
                deptKey: "mar_com",
                deptName: "Marketinq Kommunikasiyaları",
                phone: "+994 (55) 000-00-00",
                internal: "1302",
                email: "i.sayyafli@bakuelectronics.az",
                image: ""
            },
            {
                id: 16,
                name: "Nərmin Aşırzadə",
                role: "Aparıcı Mütəxəssis",
                deptKey: "mar_com",
                deptName: "Marketinq Kommunikasiyaları",
                phone: "+994 (55) 000-00-00",
                internal: "1303",
                email: "n.ashirzade@bakuelectronics.az",
                image: ""
            },
            {
                id: 17,
                name: "Orxan Məmməzadə",
                role: "Aparıcı Mütəxəssis",
                deptKey: "mar_com",
                deptName: "Marketinq Kommunikasiyaları",
                phone: "+994 (55) 000-00-00",
                internal: "1304",
                email: "o.mammadov@bakuelectronics.az",
                image: ""
            },
            {
                id: 18,
                name: "Nərgiz Qurbanova",
                role: "Mütəxəssis",
                deptKey: "mar_com",
                deptName: "Marketinq Kommunikasiyaları",
                phone: "+994 (55) 000-00-00",
                internal: "1305",
                email: "n.qurbanova@bakuelectronics.az",
                image: ""
            },
            {
                id: 19,
                name: "Səmayə İbrahimli",
                role: "Mütəxəssis",
                deptKey: "mar_com",
                deptName: "Marketinq Kommunikasiyaları",
                phone: "+994 (55) 000-00-00",
                internal: "1306",
                email: "s.ibrahimli@bakuelectronics.az",
                image: ""
            },
            {
                id: 20,
                name: "Səbinə Səlimova",
                role: "Kiçik Mütəxəssis",
                deptKey: "mar_com",
                deptName: "Marketinq Kommunikasiyaları",
                phone: "+994 (55) 000-00-00",
                internal: "1307",
                email: "s.salimova@bakuelectronics.az",
                image: ""
            },
            // SMM QRUPU
            {
                id: 21,
                name: "Könül Həsənova",
                role: "Qrup Rəhbəri",
                deptKey: "smm",
                deptName: "SMM Qrupu",
                phone: "+994 (55) 000-00-00",
                internal: "1401",
                email: "k.hasanova@bakuelectronics.az",
                image: ""
            },
            {
                id: 22,
                name: "Almaz Məmmədli",
                role: "Mütəxəssis",
                deptKey: "smm",
                deptName: "SMM Qrupu",
                phone: "+994 (55) 000-00-00",
                internal: "1402",
                email: "a.mammadli@bakuelectronics.az",
                image: ""
            },
            {
                id: 23,
                name: "Gülnur Hüseynova",
                role: "Təcrübəçi",
                deptKey: "smm",
                deptName: "SMM Qrupu",
                phone: "+994 (55) 000-00-00",
                internal: "", // DAXİLİ NÖMRƏSİ OLMAYAN 1-Cİ ƏMƏKDAŞ
                email: "g.huseynova@bakuelectronics.az",
                image: ""
            },
            {
                id: 24,
                name: "Kamil Tukanov",
                role: "Təcrübəçi",
                deptKey: "smm",
                deptName: "SMM Qrupu",
                phone: "+994 (55) 000-00-00",
                internal: "", // DAXİLİ NÖMRƏSİ OLMAYAN 2-Cİ ƏMƏKDAŞ
                email: "k.tukanov@bakuelectronics.az",
                image: ""
            },
            // DİZAYN ŞÖBƏSİ
            {
                id: 25,
                name: "Nigar Rüstəmova",
                role: "Şöbə Rəhbəri",
                deptKey: "design",
                deptName: "Dizayn Şöbəsi",
                phone: "+994 (55) 000-00-00",
                internal: "1501",
                email: "n.rustamova@bakuelectronics.az",
                image: ""
            },
            {
                id: 26,
                name: "Rəsul Azəroğlu",
                role: "Baş Qrafik Dizayner",
                deptKey: "design",
                deptName: "Dizayn Şöbəsi",
                phone: "+994 (55) 000-00-00",
                internal: "1502",
                email: "r.azeroglu@bakuelectronics.az",
                image: ""
            },
            {
                id: 27,
                name: "Nicat Alməmmədov",
                role: "Aparıcı Dizayner",
                deptKey: "design",
                deptName: "Dizayn Şöbəsi",
                phone: "+994 (55) 000-00-00",
                internal: "1503",
                email: "n.almammadov@bakuelectronics.az",
                image: ""
            },
            {
                id: 28,
                name: "Günel Nəsibova",
                role: "Aparıcı Dizayner",
                deptKey: "design",
                deptName: "Dizayn Şöbəsi",
                phone: "+994 (55) 000-00-00",
                internal: "1504",
                email: "g.nasibova@bakuelectronics.az",
                image: ""
            },
            {
                id: 29,
                name: "Aytən Cabbarova",
                role: "Qrafik Dizayner",
                deptKey: "design",
                deptName: "Dizayn Şöbəsi",
                phone: "+994 (55) 000-00-00",
                internal: "1505",
                email: "a.cabbarova@bakuelectronics.az",
                image: ""
            },
            {
                id: 30,
                name: "Saray Quliyeva",
                role: "Kiçik Dizayner",
                deptKey: "design",
                deptName: "Dizayn Şöbəsi",
                phone: "+994 (55) 000-00-00",
                internal: "1506",
                email: "s.quliyeva@bakuelectronics.az",
                image: ""
            },
            {
                id: 31,
                name: "Aysun Xəlilova",
                role: "Kiçik Dizayner",
                deptKey: "design",
                deptName: "Dizayn Şöbəsi",
                phone: "+994 (55) 000-00-00",
                internal: "1507",
                email: "a.khalilova@bakuelectronics.az",
                image: ""
            },
            // MOTION & COPYWRITING
            {
                id: 32,
                name: "Elvar Ağayev",
                role: "Baş Motion Dizayner",
                deptKey: "design",
                deptName: "Dizayn / Motion",
                phone: "+994 (55) 000-00-00",
                internal: "1508",
                email: "e.agayev@bakuelectronics.az",
                image: ""
            },
            {
                id: 33,
                name: "Zeyd Sadıqov",
                role: "Motion Dizayner",
                deptKey: "design",
                deptName: "Dizayn / Motion",
                phone: "+994 (55) 000-00-00",
                internal: "1509",
                email: "z.sadiqov@bakuelectronics.az",
                image: ""
            },
            {
                id: 34,
                name: "Aytac Qasımova",
                role: "Baş Copywriter",
                deptKey: "design",
                deptName: "Copywriting",
                phone: "+994 (55) 000-00-00",
                internal: "1510",
                email: "a.qasimova@bakuelectronics.az",
                image: ""
            },
            {
                id: 35,
                name: "Həsən Həsənov",
                role: "Kiçik Copywriter",
                deptKey: "design",
                deptName: "Copywriting",
                phone: "+994 (55) 000-00-00",
                internal: "1511",
                email: "h.hasanov@bakuelectronics.az",
                image: ""
            },
            // CRM ŞÖBƏSİ
            {
                id: 36,
                name: "Aydan Şahəliyeva",
                role: "CRM Mütəxəssis",
                deptKey: "crm",
                deptName: "CRM Şöbəsi",
                phone: "+994 (55) 000-00-00",
                internal: "1601",
                email: "a.shahaliyeva@bakuelectronics.az",
                image: ""
            },
            {
                id: 37,
                name: "Simuzər İsmətzadə",
                role: "CRM Analitik",
                deptKey: "crm",
                deptName: "CRM Şöbəsi",
                phone: "+994 (55) 000-00-00",
                internal: "1602",
                email: "s.ismatzade@bakuelectronics.az",
                image: ""
            },
            {
                id: 38,
                name: "Ləman Həsənova",
                role: "Kiçik Mütəxəssis",
                deptKey: "crm",
                deptName: "CRM Şöbəsi",
                phone: "+994 (55) 000-00-00",
                internal: "1603",
                email: "l.hasanova@bakuelectronics.az",
                image: ""
            },
            {
                id: 39,
                name: "Esmira Əhmədova",
                role: "Junior Analitik",
                deptKey: "crm",
                deptName: "CRM Şöbəsi",
                phone: "+994 (55) 000-00-00",
                internal: "1604",
                email: "e.ahmadova@bakuelectronics.az",
                image: ""
            }
        ];

        let currentFilter = 'all';

        // Əməkdaş inisiallarını yaradan funksiya
        function getInitials(name) {
            const parts = name.split(' ');
            if(parts.length >= 2) {
                return (parts[0][0] + parts[1][0]).toUpperCase();
            }
            return name[0].toUpperCase();
        }

        // Qradiyent arxa fon rəngləri (şəkil tapılmayanda aktiv olur)
        const gradients = [
            'from-red-500 to-rose-600',
            'from-rose-500 to-orange-600',
            'from-slate-700 to-slate-900',
            'from-be-red to-red-800'
        ];

        function getGradient(id) {
            return gradients[id % gradients.length];
        }

        // Komandanı ekrana render etmək
        function renderTeam(filteredData) {
            const grid = document.getElementById('teamGrid');
            const noResults = document.getElementById('noResults');
            grid.innerHTML = '';

            if (filteredData.length === 0) {
                noResults.classList.remove('hidden');
                grid.classList.add('hidden');
                return;
            } else {
                noResults.classList.add('hidden');
                grid.classList.remove('hidden');
            }

            filteredData.forEach(member => {
                const initials = getInitials(member.name);
                const bgGradient = getGradient(member.id);

                let avatarHTML = '';
                if(member.image) {
                    avatarHTML = `<img src="${member.image}" alt="${member.name}" class="w-full h-full object-cover group-hover:scale-105 transition-transform duration-500">`;
                } else {
                    avatarHTML = `
                        <div class="w-full h-full bg-gradient-to-br ${bgGradient} text-white flex items-center justify-center font-heading font-extrabold text-3xl tracking-wider select-none">
                            ${initials}
                        </div>
                    `;
                }

                // Daxili nömrə şərti yoxlanılır (Əgər yoxdursa HTML bloku daxil edilmir)
                let internalPhoneHTML = '';
                if(member.internal) {
                    internalPhoneHTML = `
                        <div class="flex items-center justify-between text-slate-300 group/item">
                            <span class="text-xs font-medium truncate pr-2"><i class="fa-solid fa-square-phone text-be-red mr-2"></i>Daxili: ${member.internal}</span>
                            <button onclick="copyToClipboard('${member.internal}')" class="text-slate-400 hover:text-white transition-colors text-sm shrink-0">
                                <i class="fa-regular fa-copy"></i>
                            </button>
                        </div>
                    `;
                }

                const card = document.createElement('div');
                card.className = "group bg-be-card border border-be-border rounded-2xl overflow-hidden shadow-sm hover:shadow-xl hover:border-be-red/30 transition-all duration-300 flex flex-col";
                card.innerHTML = `
                    <div class="relative h-60 w-full overflow-hidden bg-slate-100 shrink-0">
                        ${avatarHTML}
                        
                        <div class="absolute inset-0 bg-slate-950/90 backdrop-blur-sm opacity-0 group-hover:opacity-100 transition-all duration-300 flex flex-col justify-center px-6 space-y-3">
                            <span class="text-xs font-bold text-be-red uppercase tracking-wider">Əlaqə Vasitələri</span>
                            
                            <div class="flex items-center justify-between text-slate-300 group/item">
                                <span class="text-xs font-medium truncate pr-2"><i class="fa-solid fa-phone text-be-red mr-2"></i>${member.phone}</span>
                                <button onclick="copyToClipboard('${member.phone}')" class="text-slate-400 hover:text-white transition-colors text-sm shrink-0">
                                    <i class="fa-regular fa-copy"></i>
                                </button>
                            </div>

                            ${internalPhoneHTML}

                            <div class="flex items-center justify-between text-slate-300 group/item">
                                <span class="text-xs font-medium truncate pr-2"><i class="fa-solid fa-envelope text-be-red mr-2"></i>${member.email}</span>
                                <button onclick="copyToClipboard('${member.email}')" class="text-slate-400 hover:text-white transition-colors text-sm shrink-0">
                                    <i class="fa-regular fa-copy"></i>
                                </button>
                            </div>

                            <a href="mailto:${member.email}" class="w-full py-2 mt-2 bg-be-red hover:bg-be-red/90 text-white font-bold text-xs uppercase tracking-wider rounded-lg transition-colors text-center inline-block">
                                Məktub Göndər <i class="fa-solid fa-paper-plane ml-1"></i>
                            </a>
                        </div>
                    </div>

                    <div class="p-6 flex-grow flex flex-col justify-between">
                        <div>
                            <span class="inline-block text-[10px] uppercase font-extrabold text-be-red tracking-wider px-2 py-1 rounded bg-red-50 mb-3 border border-red-100">
                                ${member.deptName}
                            </span>
                            <h3 class="font-heading font-bold text-lg text-slate-800 line-clamp-1 mb-1">${member.name}</h3>
                            <p class="text-slate-500 text-sm font-medium leading-relaxed">${member.role}</p>
                        </div>
                    </div>
                `;
                grid.appendChild(card);
            });
        }

        // Departament Filtrləməsi
        function filterDepartment(deptKey) {
            currentFilter = deptKey;
            
            document.querySelectorAll('.dept-btn').forEach(btn => {
                btn.className = "dept-btn px-4 py-2 text-xs font-bold uppercase tracking-wider rounded-lg transition-all duration-300 shrink-0 bg-slate-100 text-slate-600 hover:bg-slate-200";
            });

            const activeBtn = document.getElementById(`btn-${deptKey}`);
            if(activeBtn) {
                activeBtn.className = "dept-btn px-4 py-2 text-xs font-bold uppercase tracking-wider rounded-lg transition-all duration-300 shrink-0 bg-be-red text-white shadow-md shadow-be-red/10";
            }

            applyFilters();
        }

        // Süzgəc funksiyası
        function applyFilters() {
            const query = document.getElementById('searchInput').value.toLowerCase().trim();
            
            const filtered = teamData.filter(member => {
                const matchDept = (currentFilter === 'all' || member.deptKey === currentFilter);
                const matchSearch = (
                    member.name.toLowerCase().includes(query) ||
                    member.role.toLowerCase().includes(query) ||
                    member.deptName.toLowerCase().includes(query)
                );
                return matchDept && matchSearch;
            });

            renderTeam(filtered);
        }

        // Canlı Axtarış
        function searchTeam() {
            applyFilters();
        }

        // Panoya Kopyalama funksiyası
        function copyToClipboard(text) {
            navigator.clipboard.writeText(text).then(() => {
                const alertBox = document.getElementById('copyAlert');
                alertBox.classList.remove('translate-y-20', 'opacity-0', 'pointer-events-none');
                alertBox.classList.add('translate-y-0', 'opacity-100');
                
                setTimeout(() => {
                    alertBox.classList.add('translate-y-20', 'opacity-0', 'pointer-events-none');
                    alertBox.classList.remove('translate-y-0', 'opacity-100');
                }, 2000);
            });
        }

        // Səhifə yüklənəndə ilk render
        window.onload = () => {
            renderTeam(teamData);
        }
    </script>
</body>
</html>
