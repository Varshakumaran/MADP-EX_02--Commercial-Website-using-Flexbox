# Ex02 Commercial Website
## Date: 12-08-2025

## AIM
To create a commercial website using CSS Flexbox.

## ALGORITHM
### STEP 1
Create an HTML file (index.html)

### STEP 2
Create a CSS file (style.css)

### STEP 3
Include a navigation bar with links to different sections.

### STEP 4
Add structured sections for Homepage, Products / Services, About Us, Contact Details and User Account.

### STEP 5
Include social media links at the footer with copyright information.

### STEP 6
Define global styles for fonts, colors, and layout.

### STEP 7
Style the header, navigation bar, and sections.

### STEP 8
Use Flexbox for layout design.

### STEP 9
Add hover effects and transitions for interactivity.

### STEP 10
Add Images and Media.

### STEP 11
Use optimized images for a professional look.

### STEP 12
Open the HTML file in a browser to check layout and functionality.

### STEP 13
Fix styling issues and refine content placement.

### STEP 14
Deploy the website.

### STEP 15
Upload to GitHub Pages for free hosting.

## PROGRAM
```
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Tech Gadgets Website</title>
    <script src="https://cdn.tailwindcss.com"></script>
   
    <link href="https://fonts.googleapis.com/css2?family=Inter:wght@400;600;700&display=swap" rel="stylesheet">
    <style>
        body {
            font-family: 'Inter', sans-serif;
        }
    </style>
</head>
<body class="bg-slate-950 text-slate-100">

    
    <header class="sticky top-0 bg-slate-900 shadow-md z-50">
        
        <nav class="container mx-auto p-4 flex justify-between items-center">
            
            <a href="#" class="text-xl font-bold text-cyan-400 md:text-2xl">GadgetHub</a>
            
            
            <div class="hidden md:flex space-x-6">
                <a href="#home" class="text-sm text-slate-200 hover:text-cyan-400 transition duration-300 font-semibold md:text-base">Home</a>
                <a href="#products" class="text-sm text-slate-200 hover:text-cyan-400 transition duration-300 font-semibold md:text-base">Products</a>
                <a href="#about" class="text-sm text-slate-200 hover:text-cyan-400 transition duration-300 font-semibold md:text-base">About Us</a>
                <a href="#contact" class="text-sm text-slate-200 hover:text-cyan-400 transition duration-300 font-semibold md:text-base">Contact</a>
            </div>

            
            <button id="mobile-menu-button" class="md:hidden text-slate-200 focus:outline-none">
                <svg class="w-6 h-6" fill="none" stroke="currentColor" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg">
                    <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M4 6h16M4 12h16m-7 6h7"></path>
                </svg>
            </button>
        </nav>
        

        <div id="mobile-menu" class="hidden md:hidden bg-slate-900 shadow-lg py-4">
            <a href="#home" class="block py-2 px-4 text-sm text-slate-100 hover:bg-slate-800 transition duration-300">Home</a>
            <a href="#products" class="block py-2 px-4 text-sm text-slate-100 hover:bg-slate-800 transition duration-300">Products</a>
            <a href="#about" class="block py-2 px-4 text-sm text-slate-100 hover:bg-slate-800 transition duration-300">About Us</a>
            <a href="#contact" class="block py-2 px-4 text-sm text-slate-100 hover:bg-slate-800 transition duration-300">Contact</a>
        </div>
    </header>

    
    <main>
        <section id="home" class="bg-gradient-to-br from-slate-900 to-slate-800 text-white py-16 md:py-24 flex items-center justify-center min-h-screen">
            <div class="container mx-auto px-4 flex flex-col-reverse md:flex-row items-center justify-between gap-8">
                <div class="md:w-1/2 text-center md:text-left">
                    <h1 class="text-3xl md:text-5xl font-extrabold leading-tight">Your Source for the Latest Tech Gadgets</h1>
                    <p class="mt-4 md:mt-6 text-base md:text-lg font-light max-w-2xl mx-auto md:mx-0">
                        Discover cutting-edge technology and innovative gadgets for your everyday life.
                    </p>
                    <a href="#products" class="mt-6 inline-block bg-cyan-400 text-slate-950 font-bold py-2 px-6 rounded-full shadow-lg hover:bg-cyan-300 transition duration-300 text-sm md:text-base">
                        Explore Our Products
                    </a>
                </div>
                <div class="md:w-1/2 flex justify-center md:justify-end">
                    <img src="gadget1.avif" alt="A desk setup with various tech gadgets" class="w-full max-w-lg rounded-xl shadow-2xl">
                </div>
            </div>
        </section>

        <section id="products" class="py-12 md:py-20 bg-slate-950">
            <div class="container mx-auto px-4 text-center">
                <h2 class="text-2xl md:text-3xl font-bold text-slate-100">Our Featured Gadgets</h2>
                <p class="mt-2 text-sm text-slate-300 max-w-2xl mx-auto md:text-base">
                    Check out our most popular tech products that are revolutionizing the market.
                </p>
                
                <div class="mt-8 flex flex-wrap justify-center gap-6">
                    <div class="flex-1 min-w-[280px] max-w-sm bg-slate-900 rounded-xl shadow-lg overflow-hidden transition-transform duration-300 hover:scale-105">
                        <img src="gadget2.jpg" alt="Wireless Earbuds" class="w-full h-40 object-cover">
                        <div class="p-4 text-left">
                            <h3 class="text-lg font-bold text-slate-100">Wireless Earbuds</h3>
                            <p class="mt-1 text-xs text-slate-300 md:text-sm">Experience crystal clear audio with our latest noise-canceling earbuds.</p>
                            <div class="mt-2 text-lg font-bold text-cyan-400">$99.99</div>
                            <button class="mt-3 w-full bg-cyan-400 text-slate-950 py-2 rounded-lg font-semibold hover:bg-cyan-300 transition duration-300 text-sm">Add to Cart</button>
                        </div>
                    </div>
                    
                    <div class="flex-1 min-w-[280px] max-w-sm bg-slate-900 rounded-xl shadow-lg overflow-hidden transition-transform duration-300 hover:scale-105">
                        <img src="gadget3.webp" alt="Smartwatch" class="w-full h-40 object-cover">
                        <div class="p-4 text-left">
                            <h3 class="text-lg font-bold text-slate-100">Smartwatch</h3>
                            <p class="mt-1 text-xs text-slate-300 md:text-sm">Track your fitness and stay connected with our sleek and stylish smartwatch.</p>
                            <div class="mt-2 text-lg font-bold text-cyan-400">$199.99</div>
                            <button class="mt-3 w-full bg-cyan-400 text-slate-950 py-2 rounded-lg font-semibold hover:bg-cyan-300 transition duration-300 text-sm">Add to Cart</button>
                        </div>
                    </div>
                    
                    <div class="flex-1 min-w-[280px] max-w-sm bg-slate-900 rounded-xl shadow-lg overflow-hidden transition-transform duration-300 hover:scale-105">
                        <img src="gadget4.webp" alt="Smartwatch" class="w-full h-40 object-cover">
                        <div class="p-4 text-left">
                            <h3 class="text-lg font-bold text-slate-100">Gaming Mouse</h3>
                            <p class="mt-1 text-xs text-slate-300 md:text-sm">Gain a competitive edge with this high-precision gaming mouse.</p>
                            <div class="mt-2 text-lg font-bold text-cyan-400">$59.99</div>
                            <button class="mt-3 w-full bg-cyan-400 text-slate-950 py-2 rounded-lg font-semibold hover:bg-cyan-300 transition duration-300 text-sm">Add to Cart</button>
                        </div>
                    </div>

                    <div class="flex-1 min-w-[280px] max-w-sm bg-slate-900 rounded-xl shadow-lg overflow-hidden transition-transform duration-300 hover:scale-105">
                        <img src="gadget5.webp" alt="Smartwatch" class="w-full h-40 object-cover">
                        <div class="p-4 text-left">
                            <h3 class="text-lg font-bold text-slate-100">Portable Power Bank</h3>
                            <p class="mt-1 text-xs text-slate-300 md:text-sm">Never run out of battery with our high-capacity portable power bank.</p>
                            <div class="mt-2 text-lg font-bold text-cyan-400">$45.00</div>
                            <button class="mt-3 w-full bg-cyan-400 text-slate-950 py-2 rounded-lg font-semibold hover:bg-cyan-300 transition duration-300 text-sm">Add to Cart</button>
                        </div>
                    </div>
                </div>
            </div>
        </section>

        <section id="about" class="py-12 md:py-20 bg-slate-950">
            <div class="container mx-auto px-4 text-center">
                <h2 class="text-2xl md:text-3xl font-bold text-slate-100">About GadgetHub</h2>
                <p class="mt-3 text-sm text-slate-300 md:text-base max-w-4xl mx-auto">
                    At GadgetHub, we are passionate about technology and committed to bringing you the best and newest gadgets on the market. We carefully curate our selection to ensure quality, performance, and innovation. Our team of tech enthusiasts is dedicated to helping you find the perfect device to enhance your digital lifestyle.
                </p>
                <p class="mt-3 text-sm text-slate-300 md:text-base max-w-4xl mx-auto">
                    We believe that technology should be accessible and exciting for everyone.
                </p>
            </div>
        </section>

        <section id="contact" class="py-12 md:py-20 bg-slate-900 text-white">
            <div class="container mx-auto px-4">
                <div class="flex flex-col md:flex-row justify-between gap-8">
                    <div class="md:w-2/3">
                        <h2 class="text-3xl font-bold text-slate-100 md:text-4xl">Contact Us</h2>
                        <p class="mt-1 text-sm text-slate-300 md:text-base">Questions about products or orders? Drop a message.</p>
                        
                        <form action="#" method="POST" class="mt-6">
                            <div class="grid grid-cols-1 md:grid-cols-2 gap-4">
                                <input type="text" id="name" name="name" class="p-2 rounded-lg border-2 border-slate-700 bg-slate-800 text-slate-100 focus:outline-none focus:border-cyan-400 text-sm md:p-3 md:text-base" placeholder="Your name">
                                <input type="email" id="email" name="email" class="p-2 rounded-lg border-2 border-slate-700 bg-slate-800 text-slate-100 focus:outline-none focus:border-cyan-400 text-sm md:p-3 md:text-base" placeholder="Your email">
                            </div>
                            <div class="mt-4">
                                <textarea id="message" name="message" rows="5" class="p-2 w-full rounded-lg border-2 border-slate-700 bg-slate-800 text-slate-100 focus:outline-none focus:border-cyan-400 text-sm md:p-3 md:text-base" placeholder="Your message"></textarea>
                            </div>
                            <div class="mt-6 flex space-x-3">
                                <button type="submit" class="bg-cyan-400 text-slate-950 font-bold py-2 px-6 rounded-lg shadow-lg hover:bg-cyan-300 transition duration-300 text-sm md:py-3 md:px-8 md:text-base">
                                    Send Message</button>
                                <button type="reset" class="bg-transparent text-slate-200 font-bold py-2 px-6 rounded-lg border-2 border-slate-200 hover:bg-slate-200 hover:text-slate-950 transition duration-300 text-sm md:py-3 md:px-8 md:text-base">
                                    Reset</button>
                            </div>
                        </form>
                    </div>

                    <div class="md:w-1/3 md:pl-8">
                        <h3 class="text-xl font-bold text-slate-100 md:text-2xl">Customer Support</h3>
                        <div class="mt-4 space-y-3 text-slate-300 text-sm md:text-base">
                            <p><span class="font-bold">Email:</span> support@pulsetech.com</p>
                            <p><span class="font-bold">Phone:</span> +91 98765 43210</p>
                            <p><span class="font-bold">Address:</span> 12A Tech Park, Bangalore, India</p>
                        </div>
                        <div class="mt-4 flex space-x-3">
                            <a href="#" class="text-slate-400 hover:text-cyan-400 transition-colors duration-300">
                                <svg class="w-5 h-5 md:w-6 md:h-6" fill="currentColor" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg">
                                    <path d="M12 2.163c3.204 0 3.584.012 4.85.07c3.252.148 4.772 1.624 4.908 4.908.058 1.265.07 1.645.07 4.85s-.012 3.584-.07 4.85c-.148 3.252-1.624 4.772-4.908 4.908-1.265.058-1.645.07-4.85.07s-3.584-.012-4.85-.07c-3.252-.148-4.772-1.624-4.908-4.908-.058-1.265-.07-1.645-.07-4.85s.012-3.584.07-4.85c.148-3.252 1.624-4.772 4.908-4.908 1.265-.058 1.645-.07 4.85-.07zm0-2.163c-3.259 0-3.667.014-4.947.072-4.358.2-6.78 2.618-6.98 6.98-.059 1.281-.073 1.689-.073 4.948s.014 3.668.072 4.948c.2 4.358 2.618 6.78 6.98 6.98 1.281.058 1.689.072 4.948.072s3.668-.014 4.948-.072c4.354-.2 6.782-2.618 6.979-6.98.059-1.28.073-1.689.073-4.948s-.014-3.668-.072-4.947c-.196-4.354-2.617-6.78-6.979-6.98-1.281-.059-1.69-.073-4.949-.073zm0 5.838c-3.403 0-6.162 2.759-6.162 6.162s2.759 6.162 6.162 6.162 6.162-2.759 6.162-6.162c0-3.403-2.759-6.162-6.162-6.162zm0 10.162c-2.209 0-4-1.79-4-4s1.79-4 4-4 4 1.79 4 4-1.79 4-4 4zm6.406-11.845c-.796 0-1.441.645-1.441 1.44s.645 1.44 1.441 1.44c.795 0 1.439-.645 1.439-1.44s-.644-1.44-1.439-1.44z"/>
                                </svg>
                            </a>
                            <a href="#" class="text-slate-400 hover:text-cyan-400 transition-colors duration-300">
                                <svg class="w-5 h-5 md:w-6 md:h-6" fill="currentColor" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg">
                                    <path d="M22.25 4.566c-.808.358-1.68.599-2.6.702.93-.559 1.647-1.444 1.984-2.506-.87.516-1.834.894-2.863 1.096-1.76-1.876-4.665-2.022-6.49-.333-1.488 1.41-1.926 3.518-1.077 5.375-3.812-.187-7.22-2.016-9.5-4.782-.497.854-.783 1.846-.783 2.915 0 2.012 1.026 3.784 2.585 4.825-.85-.027-1.65-.262-2.35-.646v.073c0 2.666 1.895 4.887 4.417 5.393-.45.122-.924.188-1.41.188-.344 0-.678-.034-.997-.095.702 2.195 2.738 3.79 5.158 3.834-1.884 1.478-4.26 2.366-6.84 2.366-.445 0-.883-.026-1.314-.078 2.43 1.56 5.314 2.478 8.412 2.478 10.117 0 15.65-8.384 15.65-15.65 0-.238-.005-.476-.013-.712.99-.714 1.848-1.61 2.528-2.628z"/>
                                </svg>
                            </a>
                            <a href="#" class="text-slate-400 hover:text-cyan-400 transition-colors duration-300">
                                <svg class="w-5 h-5 md:w-6 md:h-6" fill="currentColor" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg">
                                    <path d="M19 0h-14c-2.761 0-5 2.239-5 5v14c0 2.761 2.239 5 5 5h14c2.762 0 5-2.239 5-5v-14c0-2.761-2.238-5-5-5zm-11 19h-3v-11h3v11zm-1.5-12.268c-.966 0-1.75-.79-1.75-1.75s.784-1.75 1.75-1.75 1.75.79 1.75 1.75-.784 1.75-1.75 1.75zm13.5 12.268h-3v-5.604c0-3.368-4-3.113-4 0v5.604h-3v-11h3v1.765c1.396-2.586 7-2.777 7 2.476v6.759z"/>
                                </svg>
                            </a>
                        </div>
                    </div>
                </div>
            </div>
        </section>
    </main>

    <footer class="bg-slate-800 text-slate-200 py-6">
        <div class="container mx-auto px-4 flex flex-col md:flex-row justify-between items-center text-center">
            <p class="text-xs md:text-sm">&copy; 2023 GadgetHub, Inc. All rights reserved.</p>

            <div class="mt-3 md:mt-0 flex space-x-4">
                <a href="#" class="text-slate-400 hover:text-cyan-400 transition-colors duration-300">
                    <svg class="w-5 h-5 md:w-6 md:h-6" fill="currentColor" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg">
                        <path d="M12 2.163c3.204 0 3.584.012 4.85.07c3.252.148 4.772 1.624 4.908 4.908.058 1.265.07 1.645.07 4.85s-.012 3.584-.07 4.85c-.148 3.252-1.624 4.772-4.908 4.908-1.265.058-1.645.07-4.85.07s-3.584-.012-4.85-.07c-3.252-.148-4.772-1.624-4.908-4.908-.058-1.265-.07-1.645-.07-4.85s.012-3.584.07-4.85c.148-3.252 1.624-4.772 4.908-4.908 1.265-.058 1.645-.07 4.85-.07zm0-2.163c-3.259 0-3.667.014-4.947.072-4.358.2-6.78 2.618-6.98 6.98-.059 1.281-.073 1.689-.073 4.948s.014 3.668.072 4.948c.2 4.358 2.618 6.78 6.98 6.98 1.281.058 1.689.072 4.948.072s3.668-.014 4.948-.072c4.354-.2 6.782-2.618 6.979-6.98.059-1.28.073-1.689.073-4.948s-.014-3.668-.072-4.947c-.196-4.354-2.617-6.78-6.979-6.98-1.281-.059-1.69-.073-4.949-.073zm0 5.838c-3.403 0-6.162 2.759-6.162 6.162s2.759 6.162 6.162 6.162 6.162-2.759 6.162-6.162c0-3.403-2.759-6.162-6.162-6.162zm0 10.162c-2.209 0-4-1.79-4-4s1.79-4 4-4 4 1.79 4 4-1.79 4-4 4zm6.406-11.845c-.796 0-1.441.645-1.441 1.44s.645 1.44 1.441 1.44c.795 0 1.439-.645 1.439-1.44s-.644-1.44-1.439-1.44z"/>
                    </svg>
                </a>
                <a href="#" class="text-slate-400 hover:text-cyan-400 transition-colors duration-300">
                    <svg class="w-5 h-5 md:w-6 md:h-6" fill="currentColor" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg">
                        <path d="M22.25 4.566c-.808.358-1.68.599-2.6.702.93-.559 1.647-1.444 1.984-2.506-.87.516-1.834.894-2.863 1.096-1.76-1.876-4.665-2.022-6.49-.333-1.488 1.41-1.926 3.518-1.077 5.375-3.812-.187-7.22-2.016-9.5-4.782-.497.854-.783 1.846-.783 2.915 0 2.012 1.026 3.784 2.585 4.825-.85-.027-1.65-.262-2.35-.646v.073c0 2.666 1.895 4.887 4.417 5.393-.45.122-.924.188-1.41.188-.344 0-.678-.034-.997-.095.702 2.195 2.738 3.79 5.158 3.834-1.884 1.478-4.26 2.366-6.84 2.366-.445 0-.883-.026-1.314-.078 2.43 1.56 5.314 2.478 8.412 2.478 10.117 0 15.65-8.384 15.65-15.65 0-.238-.005-.476-.013-.712.99-.714 1.848-1.61 2.528-2.628z"/>
                    </svg>
                </a>
                <a href="#" class="text-slate-400 hover:text-cyan-400 transition-colors duration-300">
                    <svg class="w-5 h-5 md:w-6 md:h-6" fill="currentColor" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg">
                        <path d="M19 0h-14c-2.761 0-5 2.239-5 5v14c0 2.761 2.239 5 5 5h14c2.762 0 5-2.239 5-5v-14c0-2.761-2.238-5-5-5zm-11 19h-3v-11h3v11zm-1.5-12.268c-.966 0-1.75-.79-1.75-1.75s.784-1.75 1.75-1.75 1.75.79 1.75 1.75-.784 1.75-1.75 1.75zm13.5 12.268h-3v-5.604c0-3.368-4-3.113-4 0v5.604h-3v-11h3v1.765c1.396-2.586 7-2.777 7 2.476v6.759z"/>
                    </svg>
                </a>
            </div>
        </div>
    </footer>

    <script>
        document.addEventListener('DOMContentLoaded', function () {
            const mobileMenuButton = document.getElementById('mobile-menu-button');
            const mobileMenu = document.getElementById('mobile-menu');

            mobileMenuButton.addEventListener('click', function () {
                mobileMenu.classList.toggle('hidden');
            });

            const mobileLinks = mobileMenu.querySelectorAll('a');
            mobileLinks.forEach(link => {
                link.addEventListener('click', function () {
                    mobileMenu.classList.add('hidden');
                });
            });
        });
    </script>
</body>
</html>

```

## OUTPUT
<img width="1920" height="1080" alt="Screenshot (116)" src="https://github.com/user-attachments/assets/5933a27f-2c34-4f60-8129-c425339d61a2" />
<img width="1920" height="1080" alt="Screenshot (117)" src="https://github.com/user-attachments/assets/a74ff296-2e31-47a0-b2f2-760b7fd97e06" />
<img width="1920" height="1080" alt="Screenshot (118)" src="https://github.com/user-attachments/assets/56972598-9164-42a8-9250-5d48ae4ea102" />


## RESULT
The program for creating commercial website using CSS Flexbox is executed successfully.
