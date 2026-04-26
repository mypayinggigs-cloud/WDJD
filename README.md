<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>What Did Jesus Do? | Pastor Chidi Shekinah</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0/css/all.min.css">
    <link href="https://fonts.googleapis.com/css2?family=Playfair+Display:ital,wght@0,400;0,700;1,400&family=Inter:wght@300;400;600&display=swap" rel="stylesheet">
    <style>
        :root {
            --cream: #FDFBF7;
            --latte: #E2D1C3;
            --mocha: #8D7765;
            --espresso: #3E2F26;
        }

        body {
            font-family: 'Inter', sans-serif;
            background-color: var(--cream);
            color: var(--espresso);
            overflow-x: hidden;
            scroll-behavior: smooth;
        }

        .serif { font-family: 'Playfair Display', serif; }

        /* 3D BOOK PORTRAIT ENGINE */
        .book-stage {
            perspective: 2000px;
            width: 100%;
            height: 500px;
            display: flex;
            justify-content: center;
            align-items: center;
        }

        .book-3d {
            width: 300px;
            height: 450px;
            position: relative;
            transform-style: preserve-3d;
            transform: rotateY(-30deg) rotateX(10deg);
            box-shadow: 20px 40px 60px rgba(0,0,0,0.25);
            transition: transform 0.5s ease;
        }

        .book-3d:hover {
            transform: rotateY(-15deg) rotateX(5deg);
        }

        /* Front Cover */
        .book-side-front {
            position: absolute;
            width: 100%;
            height: 100%;
            background: url('https://api.typedream.com/v0/document/public/0d01d5aa-dbc6-4638-ac24-88ba35ff483b_ChatGPT_Image_Apr_25_2026_12_42_53_AM_png.png') center/cover;
            transform: translateZ(25px);
            z-index: 10;
            border-radius: 2px 4px 4px 2px;
        }

        /* Spine (The Bleed) */
        .book-side-spine {
            position: absolute;
            width: 50px;
            height: 100%;
            left: -25px;
            background: #2a1f18; /* Deep brown matching the cover's shadow tones */
            transform: rotateY(-90deg);
            z-index: 5;
            display: flex;
            align-items: center;
            justify-content: center;
        }

        .spine-label {
            color: var(--latte);
            transform: rotate(90deg);
            white-space: nowrap;
            font-size: 14px;
            text-transform: uppercase;
            letter-spacing: 3px;
            font-weight: bold;
            opacity: 0.8;
        }

        /* Page Edges */
        .book-side-pages {
            position: absolute;
            width: 48px;
            height: 98%;
            top: 1%;
            right: -24px;
            background: linear-gradient(90deg, #e0e0e0 0%, #ffffff 20%, #e0e0e0 40%, #ffffff 60%, #e0e0e0 80%, #ffffff 100%);
            transform: rotateY(90deg);
            z-index: 4;
        }

        /* Back Cover */
        .book-side-back {
            position: absolute;
            width: 100%;
            height: 100%;
            background: url('https://api.typedream.com/v0/document/public/08a39495-be21-4029-bc8f-0a8ca71decd0_ChatGPT_Image_Apr_25_2026_12_30_31_AM_png.png') center/cover;
            transform: translateZ(-25px) rotateY(180deg);
            z-index: 1;
        }

        /* Reader Experience - Chapter Format */
        .book-page-layout {
            background: white;
            box-shadow: 0 15px 50px rgba(0,0,0,0.05);
            max-width: 850px;
            margin: 0 auto;
            padding: 4rem;
            border: 1px solid var(--latte);
            position: relative;
        }

        .cta-button {
            background-color: var(--espresso);
            color: var(--cream);
            transition: all 0.4s ease;
        }

        .cta-button:hover {
            background-color: var(--mocha);
            transform: translateY(-2px);
            box-shadow: 0 10px 20px rgba(62, 47, 38, 0.2);
        }

        .section-milk {
            background: linear-gradient(180deg, var(--cream) 0%, #F5F1EB 100%);
        }

    </style>
</head>
<body>

    <!-- Nav -->
    <nav class="fixed w-full z-50 bg-white/90 backdrop-blur-md border-b border-latte px-8 py-5 flex justify-between items-center">
        <div class="text-2xl font-bold serif italic tracking-tighter text-espresso">WDJD.</div>
        <div class="hidden md:flex space-x-10 text-xs font-bold uppercase tracking-widest text-espresso/60">
            <a href="#about" class="hover:text-mocha transition-colors">The Book</a>
            <a href="#read" class="hover:text-mocha transition-colors">Read Excerpt</a>
            <a href="#vision" class="hover:text-mocha transition-colors">Ekklesia.app</a>
        </div>
        <a href="#order" class="cta-button px-8 py-2.5 rounded-full text-xs font-bold">BUY NOW</a>
    </nav>

    <!-- Hero -->
    <section class="min-h-screen flex items-center pt-24 pb-12 px-6 section-milk">
        <div class="max-w-7xl mx-auto w-full grid grid-cols-1 lg:grid-cols-2 gap-16 items-center">
            <div class="space-y-8 order-2 lg:order-1">
                <span class="text-mocha font-bold tracking-[0.4em] uppercase text-xs block">Official Release</span>
                <h1 class="text-6xl lg:text-8xl serif leading-[0.9] text-espresso">What Did <br><span class="italic text-mocha">Jesus</span> Do?</h1>
                <p class="text-xl text-gray-500 max-w-lg leading-relaxed">
                    Rediscover the heart and power of the gospel. A transformative exploration of the life of Christ by <span class="text-espresso font-bold italic">Pastor Chidi Shekinah</span>.
                </p>
                <div class="flex flex-col sm:row space-y-4 sm:space-y-0 sm:space-x-4 pt-4">
                    <a href="#order" class="cta-button px-12 py-5 rounded-2xl text-center font-bold text-lg">Purchase on KDP</a>
                    <a href="#vision" class="border-2 border-espresso px-12 py-5 rounded-2xl text-center font-bold text-lg hover:bg-espresso hover:text-white transition-all text-espresso">The Ekklesia Vision</a>
                </div>
            </div>

            <!-- THE 3D BOOK PORTRAIT -->
            <div class="order-1 lg:order-2 book-stage">
                <div class="book-3d">
                    <div class="book-side-front"></div>
                    <div class="book-side-spine">
                        <div class="spine-label">What Did Jesus Do?</div>
                    </div>
                    <div class="book-side-pages"></div>
                    <div class="book-side-back"></div>
                </div>
            </div>
        </div>
    </section>

    <!-- Quote -->
    <section id="about" class="bg-white py-32 border-y border-latte/30">
        <div class="max-w-3xl mx-auto px-6 text-center">
            <h2 class="serif text-4xl lg:text-5xl italic leading-tight text-espresso">
                "It is possible to have church without Christ... The Church was not built on activity. It was built on Christ."
            </h2>
            <div class="w-16 h-1 bg-mocha mx-auto mt-12 mb-8"></div>
            <p class="text-lg text-gray-400 font-semibold uppercase tracking-widest">A Call Back to Reality</p>
        </div>
    </section>

    <!-- Reading Excerpt -->
    <section id="read" class="py-32 px-6 bg-cream">
        <div class="text-center mb-16">
            <h3 class="serif text-4xl lg:text-5xl">The Tragedy of a <br>Christless Church</h3>
            <p class="text-mocha font-bold uppercase tracking-widest text-xs mt-4">Excerpt: Chapter Four</p>
        </div>

        <div class="book-page-layout rounded-sm">
            <div class="max-w-2xl mx-auto prose prose-brown">
                <p class="text-xl mb-8 font-light leading-relaxed">There is a reality that must be faced with honesty. It is possible to have church without Christ. This statement may sound extreme, but if we are willing to look closely, we will see that it is not far from the truth in many places today.</p>
                
                <p class="mb-8 italic text-espresso font-semibold">There is activity. There is structure. There is passion. But there is not always a clear revelation of Christ.</p>
                
                <p class="mb-12">And this is the tragedy. Because the Church was not built on activity. It was built on Christ.</p>

                <h4 class="serif text-2xl mb-6">When Presence Is Replaced by Performance</h4>
                <p class="mb-8">One of the subtle dangers in the Christian journey is the replacement of presence with performance. Over time, it is easy to shift from knowing Christ to doing things for Him.</p>

                <div class="bg-cream p-10 border-l-4 border-mocha my-12 shadow-sm italic">
                    “And this is eternal life, that they may know You, the only true God, and Jesus Christ whom You have sent.”
                    <p class="mt-4 text-sm font-bold not-italic">— John 17:3</p>
                </div>

                <p class="mb-8">Notice the contradiction. These people were active in ministry. They prophesied. They cast out demons. Yet Jesus says, <span class="font-bold underline text-espresso">“I never knew you.”</span> The issue was not activity. It was relationship.</p>
                
                <div class="text-center mt-20">
                    <p class="text-gray-400 italic mb-6">Experience the full revelation...</p>
                    <a href="#order" class="cta-button px-10 py-4 rounded-xl inline-block font-bold">Get Your Copy on Amazon</a>
                </div>
            </div>
        </div>
    </section>

    <!-- Vision Section -->
    <section id="vision" class="py-32 bg-espresso text-cream">
        <div class="max-w-7xl mx-auto px-6 grid grid-cols-1 lg:grid-cols-2 gap-20 items-center">
            <div class="space-y-8">
                <h2 class="serif text-5xl lg:text-6xl">Ekklesia.app</h2>
                <p class="text-lg opacity-80 leading-relaxed">
                    We are building a state-of-the-art Christian resource app. A digital ecosystem featuring up to <span class="text-mocha font-bold">50 Bible School courses</span>—Basic, Intermediary, and Advanced—designed to empower church workers and global leadership.
                </p>
                <div class="bg-white/5 border border-white/10 p-10 rounded-3xl">
                    <h4 class="serif text-2xl mb-4">Support This Project</h4>
                    <p class="text-sm opacity-60 mb-8">Join us in making state-of-the-art theological training accessible to every leader, everywhere.</p>
                    <button onclick="openPaystack()" class="w-full bg-mocha hover:bg-white hover:text-espresso transition-all py-5 rounded-2xl font-bold text-lg shadow-xl">
                        DONATE VIA PAYSTACK <i class="fas fa-heart ml-2"></i>
                    </button>
                </div>
            </div>
            <div class="relative">
                <div class="w-full aspect-square bg-mocha/10 rounded-[4rem] border border-mocha/20 flex flex-col justify-center items-center text-center p-12">
                    <i class="fas fa-scroll text-6xl text-mocha mb-6"></i>
                    <h3 class="serif text-3xl">50 Courses</h3>
                    <p class="opacity-50 mt-2">Comprehensive Leadership Training</p>
                </div>
            </div>
        </div>
    </section>

    <!-- Footer -->
    <footer class="bg-white pt-24 pb-12 border-t border-latte">
        <div class="max-w-7xl mx-auto px-8">
            <div class="flex flex-col md:flex-row justify-between items-start mb-20 gap-12">
                <div class="max-w-sm">
                    <h2 class="serif text-3xl italic text-espresso mb-6">WDJD.</h2>
                    <p class="text-gray-400 leading-relaxed text-sm">
                        Helping believers rediscover the heart and power of the gospel by looking deeply at the life and teachings of Jesus.
                    </p>
                </div>
                <div class="flex flex-wrap gap-20">
                    <div>
                        <h5 class="text-[10px] uppercase font-bold tracking-widest text-espresso/40 mb-6">The Book</h5>
                        <ul class="text-sm space-y-4 text-gray-500">
                            <li><a href="#about" class="hover:text-mocha">About</a></li>
                            <li><a href="#read" class="hover:text-mocha">Excerpt</a></li>
                            <li><a href="#order" class="hover:text-mocha">KDP Store</a></li>
                        </ul>
                    </div>
                    <div>
                        <h5 class="text-[10px] uppercase font-bold tracking-widest text-espresso/40 mb-6">Author</h5>
                        <p class="text-sm font-bold italic text-espresso">Pastor Chidi Shekinah</p>
                    </div>
                </div>
            </div>
            <div class="border-t border-latte pt-12 flex flex-col md:row justify-between items-center text-[10px] uppercase tracking-[0.3em] font-bold text-gray-300">
                <p>© 2024 Pastor Chidi Shekinah. All Rights Reserved.</p>
                <div class="mt-6 md:mt-0 flex space-x-10">
                    <a href="#">Privacy</a>
                    <a href="#">Terms</a>
                </div>
            </div>
        </div>
    </footer>

    <script>
        const PAYSTACK_LINK = "https://paystack.com/pay/your-link"; 
        const KDP_LINK = "https://amazon.com/";

        function openPaystack() {
            window.open(PAYSTACK_LINK, '_blank');
        }

        // Animate book slightly on scroll
        window.addEventListener('scroll', () => {
            const book = document.querySelector('.book-3d');
            const scroll = window.scrollY;
            const rotation = -30 + (scroll / 100);
            if (rotation < -10) {
                book.style.transform = `rotateY(${rotation}deg) rotateX(10deg)`;
            }
        });
    </script>
</body>
</html>
