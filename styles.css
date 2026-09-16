document.addEventListener('DOMContentLoaded', () => {
    // Initialize Lucide Icons
    if (window.lucide) {
        lucide.createIcons();
    }

    // Mobile Menu Toggle
    const menuBtn = document.querySelector('.menu');
    const navMenu = document.querySelector('.nav nav');

    if (menuBtn && navMenu) {
        menuBtn.addEventListener('click', () => {
            navMenu.classList.toggle('active');
        });

        // Close the mobile menu after tapping a link
        navMenu.querySelectorAll('a').forEach((link) => {
            link.addEventListener('click', () => {
                navMenu.classList.remove('active');
            });
        });

        // Close the mobile menu if the viewport is resized back to desktop
        window.addEventListener('resize', () => {
            if (window.innerWidth > 800) {
                navMenu.classList.remove('active');
            }
        });
    }

    // Force all reveal and hero elements to stay visible permanently (prevents invisible items)
    if (typeof gsap !== 'undefined') {
        gsap.set('.hero-title, .hero-copy, .eyebrow, .circle-link, .reveal', {
            opacity: 1,
            visibility: 'visible',
            y: 0
        });
    }

    // Floating Hero Cards Animation Loops
    if (typeof gsap !== 'undefined' && typeof ScrollTrigger !== 'undefined') {
        gsap.registerPlugin(ScrollTrigger);

        gsap.to('.card-one', {
            y: -14,
            duration: 3,
            repeat: -1,
            yoyo: true,
            ease: 'power1.inOut'
        });

        gsap.to('.card-two', {
            y: 12,
            duration: 3.5,
            repeat: -1,
            yoyo: true,
            ease: 'power1.inOut',
            delay: 0.5
        });

        gsap.to('.card-three', {
            y: -10,
            duration: 2.8,
            repeat: -1,
            yoyo: true,
            ease: 'power1.inOut',
            delay: 1
        });
    }
});
