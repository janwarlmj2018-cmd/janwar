<!DOCTYPE html>
<html lang="id" class="scroll-smooth">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Undangan Pernikahan - Janwar & Suci</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <link href="https://fonts.googleapis.com/css2?family=Cinzel:wght@400;600;700&family=Plus+Jakarta+Sans:wght@300;400;500;600&family=Pinyon+Script&display=swap" rel="stylesheet">
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <script>
        tailwind.config = {
            theme: {
                extend: {
                    colors: {
                        gold: '#C5A880',
                        darkgold: '#9A7B4C',
                        softcream: '#FBF9F5',
                        javaneseGreen: '#1b3b2b',
                    },
                    fontFamily: {
                        cinzel: ['Cinzel', 'serif'],
                        script: ['Pinyon Script', 'cursive'],
                        sans: ['Plus Jakarta Sans', 'sans-serif'],
                    }
                }
            }
        }
    </script>
    <style>
        .glass-card {
            background: rgba(255, 255, 255, 0.85);
            backdrop-filter: blur(10px);
        }
        html {
            scroll-behavior: smooth;
        }
    </style>
</head>
<body class="bg-softcream text-neutral-800 font-sans antialiased overflow-x-hidden">

    <!-- 🎵 MUSIK LATAR: Jalaraning Tresno - Versi Kroncong (YouTube) -->
    <iframe id="yt-music" 
        src="https://www.youtube.com/embed/5iMztimFbu0?autoplay=1&loop=1&playlist=5iMztimFbu0&mute=0" 
        style="display:none;" 
        frameborder="0" 
        allow="autoplay; encrypted-media" 
        allowfullscreen>
    </iframe>

    <!-- COVER / HALAMAN DEPAN -->
    <div id="cover-section" class="fixed inset-0 z-50 flex flex-col items-center justify-center bg-javaneseGreen text-white p-6 transition-all duration-700">
        <div class="absolute inset-0 opacity-25 bg-cover bg-center" style="background-image: url('https://riyante002.github.io/undangan-pernikahan/DSC_2231(1).jpg');"></div>
        <div class="relative z-10 text-center max-w-md mx-auto space-y-6">
            <p class="font-cinzel tracking-widest text-gold text-sm uppercase">Undangan Pernikahan</p>
            <h1 class="font-script text-6xl text-gold">Janwar & Suci</h1>
            <div class="w-24 h-0.5 bg-gold mx-auto"></div>
            <div class="py-4">
                <p class="text-sm text-neutral-300">Kepada Yth. Bapak/Ibu/Saudara/i</p>
                <h2 id="guest-name" class="font-semibold text-xl text-white mt-1">Tamu Undangan</h2>
                <p class="text-xs text-neutral-400 mt-1">Tanpa mengurangi rasa hormat, kami mengundang Anda</p>
            </div>
            <button onclick="openInvitation()" class="bg-gold hover:bg-darkgold text-neutral-900 font-medium px-8 py-3 rounded-full shadow-lg transition duration-300 flex items-center justify-center mx-auto space-x-2">
                <i class="fa-solid fa-envelope-open-text"></i>
                <span>Buka Undangan</span>
            </button>
        </div>
    </div>

    <!-- MAIN CONTENT (HIDDEN UNTIL OPENED) -->
    <div id="main-content" class="opacity-0 transition-opacity duration-1000 hidden">

        <!-- HERO SECTION -->
        <header class="relative h-screen flex items-center justify-center text-center text-white px-4">
            <div class="absolute inset-0 bg-black/50 z-10"></div>
            <div class="absolute inset-0 bg-cover bg-center" style="background-image: url('https://riyante002.github.io/undangan-pernikahan/background.jpg');"></div>
            
            <div class="relative z-20 space-y-4 max-w-2xl mx-auto">
                <p class="font-cinzel tracking-widest text-gold uppercase text-sm">The Wedding Of</p>
                <h1 class="font-script text-6xl md:text-8xl text-gold">Janwar & Suci</h1>
                <p class="font-cinzel text-lg tracking-wider">Jumat, 18 September 2026</p>
                <div class="pt-6">
                    <a href="#countdown" class="animate-bounce inline-block text-gold">
                        <i class="fa-solid fa-chevron-down text-xl"></i>
                    </a>
                </div>
            </div>
        </header>

        <!-- COUPLE SECTION -->
        <section class="py-20 px-6 max-w-5xl mx-auto text-center">
            <div class="space-y-4 mb-16">
                <p class="font-cinzel text-gold text-sm tracking-widest uppercase">Sang Mempelai</p>
                <h2 class="font-script text-5xl text-neutral-900">Pasangan Bahagia</h2>
                <p class="text-neutral-600 max-w-lg mx-auto text-sm">"Dan di antara tanda-tanda kebesaran-Nya ialah Dia menciptakan pasangan-pasangan untukmu dari jenismu sendiri, agar kamu cenderung dan merasa tenteram kepadanya..." (QS. Ar-Rum: 21)</p>
            </div>

            <div class="grid grid-cols-1 md:grid-cols-2 gap-12 items-center">
                <!-- Mempelai Pria -->
                <div class="space-y-4 flex flex-col items-center">
                    <div class="w-64 h-80 rounded-2xl overflow-hidden shadow-xl border-4 border-gold">
                        <img src="https://riyante002.github.io/undangan-pernikahan/IMG_20260805-WA0024[1].jpg" alt="Janwar Febriyanto" class="w-full h-full object-cover">
                    </div>
                    <h3 class="font-cinzel text-2xl font-bold text-neutral-900">Janwar Febriyanto</h3>
                    <p class="text-sm text-neutral-600">Putra dari Bapak Suwari & Ibu Ponitri</p>
                </div>

                <!-- Mempelai Wanita -->
                <div class="space-y-4 flex flex-col items-center">
                    <div class="w-64 h-80 rounded-2xl overflow-hidden shadow-xl border-4 border-gold">
                        <img src="https://riyante002.github.io/undangan-pernikahan/IMG_20260805-WA0025[1].jpg" alt="Suci Rahmawati" class="w-full h-full object-cover">
                    </div>
                    <h3 class="font-cinzel text-2xl font-bold text-neutral-900">Suci Rahmawati</h3>
                    <p class="text-sm text-neutral-600">Putri dari Bapak Heri Nursio & Ibu Dewi Musyarofah</p>
                </div>
            </div>
        </section>

        <!-- COUNTDOWN SECTION -->
        <section id="countdown" class="py-16 bg-javaneseGreen text-white px-6 text-center">
            <div class="max-w-2xl mx-auto space-y-6">
                <h2 class="font-cinzel text-2xl text-gold tracking-widest">Menuju Hari Bahagia</h2>
                <div class="grid grid-cols-4 gap-4 max-w-md mx-auto">
                    <div class="bg-white/10 p-3 rounded-lg backdrop-blur">
                        <span id="days" class="font-cinzel text-3xl font-bold text-gold">00</span>
                        <p class="text-xs uppercase text-neutral-300">Hari</p>
                    </div>
                    <div class="bg-white/10 p-3 rounded-lg backdrop-blur">
                        <span id="hours" class="font-cinzel text-3xl font-bold text-gold">00</span>
                        <p class="text-xs uppercase text-neutral-300">Jam</p>
                    </div>
                    <div class="bg-white/10 p-3 rounded-lg backdrop-blur">
                        <span id="minutes" class="font-cinzel text-3xl font-bold text-gold">00</span>
                        <p class="text-xs uppercase text-neutral-300">Menit</p>
                    </div>
                    <div class="bg-white/10 p-3 rounded-lg backdrop-blur">
                        <span id="seconds" class="font-cinzel text-3xl font-bold text-gold">00</span>
                        <p class="text-xs uppercase text-neutral-300">Detik</p>
                    </div>
                </div>
            </div>
        </section>

        <!-- EVENT DETAILS -->
        <section class="py-20 px-6 max-w-4xl mx-auto">
            <div class="text-center space-y-4 mb-12">
                <p class="font-cinzel text-gold text-sm tracking-widest uppercase">Rangkaian Acara</p>
                <h2 class="font-script text-5xl text-neutral-900">Waktu & Tempat</h2>
                <p class="text-sm text-neutral-600 font-medium max-w-md mx-auto">
                    <i class="fa-solid fa-location-dot text-gold mr-2"></i> 
                    Rumah Kediaman Mempelai Wanita<br>
                    Dsn. Siluman Ds. Bades Kec. Pasirian
                </p>
                <a href="https://maps.app.goo.gl/bzDdork2EipFquSn8" target="_blank" class="inline-block mt-2 text-gold hover:text-darkgold font-medium">
                    <i class="fa-solid fa-map-location-dot mr-1"></i> Buka di Google Maps
                </a>
            </div>

            <div class="grid grid-cols-1 md:grid-cols-2 gap-8">
                <div class="bg-white p-8 rounded-2xl shadow-md border-t-4 border-gold text-center space-y-4">
                    <h3 class="font-cinzel text-2xl font-bold text-neutral-900">🕌 Akad Nikah</h3>
                    <p class="text-sm text-neutral-600"><i class="fa-regular fa-calendar-days text-gold mr-2"></i> Jumat, 18 September 2026</p>
                    <p class="text-sm text-neutral-600"><i class="fa-regular fa-clock text-gold mr-2"></i> Pukul 08.00 WIB - Selesai</p>
                </div>

                <div class="bg-white p-8 rounded-2xl shadow-md border-t-4 border-gold text-center space-y-4">
                    <h3 class="font-cinzel text-2xl font-bold text-neutral-900">🎉 Resepsi</h3>
                    <p class="text-sm text-neutral-600"><i class="fa-regular fa-calendar-days text-gold mr-2"></i> Jumat, 18 September 2026</p>
                    <p class="text-sm text-neutral-600"><i class="fa-regular fa-clock text-gold mr-2"></i> Pukul 13.00 WIB - Selesai</p>
                </div>
            </div>
        </section>

        <!-- RSVP / UCAPAN -->
        <section class="py-20 px-6 max-w-3xl mx-auto">
            <div class="text-center space-y-4 mb-12">
                <p class="font-cinzel text-gold text-sm tracking-widest uppercase">Konfirmasi Kehadiran</p>
                <h2 class="font-script text-5xl text-neutral-900">RSVP & Ucapan</h2>
            </div>

            <form id="rsvp-form" class="bg-white p-8 rounded-2xl shadow-md space-y-6">
                <div>
                    <label class="block text-sm font-medium text-neutral-700 mb-2">Nama</label>
                    <input type="text" id="name" required class="w-full px-4 py-3 border rounded-lg focus:ring-2 focus:ring-gold outline-none">
                </div>
                <div>
                    <label class="block text-sm font-medium text-neutral-700 mb-2">Konfirmasi Kehadiran</label>
                    <select id="status" class="w-full px-4 py-3 border rounded-lg focus:ring-2 focus:ring-gold outline-none">
                        <option value="Hadir">✅ Hadir</option>
                        <option value="Tidak Hadir">🙏 Berhalangan Hadir</option>
                    </select>
                </div>
                <div>
                    <label class="block text-sm font-medium text-neutral-700 mb-2">Ucapan & Doa</label>
                    <textarea id="message" rows="4" required class="w-full px-4 py-3 border rounded-lg focus:ring-2 focus:ring-gold outline-none" placeholder="Tulis doa & ucapan untuk kami..."></textarea>
                </div>
                <button type="submit" class="w-full bg-gold hover:bg-darkgold text-neutral-900 font-medium py-3 rounded-lg transition duration-300">Kirim Ucapan 🤲</button>
            </form>

            <div id="wishes-container" class="mt-10 space-y-4">
                <!-- Dynamic wishes list -->
            </div>
        </section>

        <!-- PENUTUP -->
        <section class="py-16 px-6 text-center max-w-2xl mx-auto">
            <p class="text-lg text-neutral-700 leading-relaxed">
                Merupakan suatu kehormatan dan kebahagiaan bagi kami apabila Bapak/Ibu/Saudara/i berkenan hadir dan memberikan doa restu.<br><br>
                <em class="text-gold italic">"Dan di antara tanda-tanda kebesaran-Nya ialah Dia menciptakan pasangan-pasangan untukmu..."</em><br><br>
                Wassalamu'alaikum Warahmatullahi Wabarakatuh ❤️
            </p>
        </section>

        <!-- FOOTER -->
        <footer class="bg-javaneseGreen text-white py-8 text-center text-sm">
            <p class="font-cinzel tracking-wider text-gold">Terima Kasih</p>
            <p class="text-neutral-400 mt-1">&copy; 2026 Undangan Pernikahan — Janwar & Suci</p>
        </footer>

    </div>

    <!-- AUDIO CONTROLLER -->
    <button id="audio-btn" onclick="toggleAudio()" class="fixed bottom-6 right-6 z-40 bg-gold text-neutral-900 w-12 h-12 rounded-full shadow-lg flex items-center justify-center hidden">
        <i id="audio-icon" class="fa-solid fa-music"></i>
    </button>

    <script>
        // Safely extract guest name from URL parameters
        const urlParams = new URLSearchParams(window.location.search);
        const guest = urlParams.get('to');
        const guestNameEl = document.getElementById('guest-name');
        if (guest && guestNameEl) {
            guestNameEl.innerText = decodeURIComponent(guest);
        }

        // Open Invitation — Play YouTube Music
        function openInvitation() {
            const cover = document.getElementById('cover-section');
            const main = document.getElementById('main-content');
            const audioBtn = document.getElementById('audio-btn');
            const ytMusic = document.getElementById('yt-music');

            cover.style.transform = 'translateY(-100%)';
            setTimeout(() => {
                cover.classList.add('hidden');
                main.classList.remove('hidden');
                main.classList.remove('opacity-0');
                audioBtn.classList.remove('hidden');
                // Play music by reloading iframe
                ytMusic.src = ytMusic.src;
            }, 700);
        }

        // Audio Toggle — Mute/Unmute YouTube
        let isMuted = false;
        function toggleAudio() {
            const icon = document.getElementById('audio-icon');
            if (isMuted) {
                icon.classList.remove('fa-volume-xmark');
                icon.classList.add('fa-music');
            } else {
                icon.classList.remove('fa-music');
                icon.classList.add('fa-volume-xmark');
            }
            isMuted = !isMuted;
            alert('Musik ' + (isMuted ? 'dimatikan 🔇' : 'dinyalakan 🔊'));
        }

        // Countdown Timer — September 18, 2026 08:00:00
        const weddingDate = new Date("September 18, 2026 08:00:00").getTime();
        setInterval(() => {
            const now = new Date().getTime();
            const distance = weddingDate - now;

            if (distance > 0) {
                const daysEl = document.getElementById('days');
                const hoursEl = document.getElementById('hours');
                const minutesEl = document.getElementById('minutes');
                const secondsEl = document.getElementById('seconds');

                if (daysEl) daysEl.innerText = String(Math.floor(distance / (1000 * 60 * 60 * 24))).padStart(2, '0');
                if (hoursEl) hoursEl.innerText = String(Math.floor((distance % (1000 * 60 * 60 * 24)) / (1000 * 60 * 60))).padStart(2, '0');
                if (minutesEl) minutesEl.innerText = String(Math.floor((distance % (1000 * 60 * 60)) / (1000 * 60))).padStart(2, '0');
                if (secondsEl) secondsEl.innerText = String(Math.floor((distance % (1000 * 60)) / 1000)).padStart(2, '0');
            } else {
                document.getElementById('days').innerText = '00';
                document.getElementById('hours').innerText = '00';
                document.getElementById('minutes').innerText = '00';
                document.getElementById('seconds').innerText = '00';
            }
        }, 1000);

        // RSVP Form submission
        document.addEventListener('DOMContentLoaded', () => {
            const rsvpForm = document.getElementById('rsvp-form');
            const wishesContainer = document.getElementById('wishes-container');

            if (rsvpForm) {
                rsvpForm.addEventListener('submit', function(e) {
                    e.preventDefault();
                    const name = document.getElementById('name').value;
                    const status = document.getElementById('status').value;
                    const message = document.getElementById('message').value;

                    const card = document.createElement('div');
                    card.className = 'bg-white p-4 rounded-xl shadow-sm border border-neutral-200 space-y-1';
                    card.innerHTML = `
                        <div class="flex justify-between items-center">
                            <h4 class="font-semibold text-neutral-900">${name}</h4>
                            <span class="text-xs px-2 py-1 rounded-full ${status === 'Hadir' ? 'bg-green-100 text-green-700' : 'bg-red-100 text-red-700'}">${status}</span>
                        </div>
                        <p class="text-sm text-neutral-600 mt-2">${message}</p>
                    `;
                    
                    if (wishesContainer) {
                        wishesContainer.prepend(card);
                    }
                    rsvpForm.reset();
                    alert('✅ Terima kasih! Ucapan Anda terkirim!');
                });
            }
        });
    </script>
</body>
</html># janwar
