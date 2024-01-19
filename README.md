<h1>TWO GOOD CO. CLONE</h1>
    <h2>Table of Contents</h2>
    <ul>
        <li><a href="#introduction">Introduction</a></li>
        <li><a href="#features">Features</a></li>
        <li><a href="#installation">Installation</a></li>
        <li><a href="#usage">Usage</a></li>
        <li><a href="#dependencies">Dependencies</a></li>
        <li><a href="#license">License</a></li>
        <li><a href="#acknowledgments">Acknowledgments</a></li>
    </ul>
    <h2 id="introduction">Introduction</h2>
    <p>Welcome to the documentation for Project Name, a web development project that focuses on creating captivating animations and interactive elements for modern web applications. This project utilizes GSAP (GreenSock Animation Platform) and Locomotive Scroll to provide a seamless and visually appealing user experience</p>
    <h2 id="features">Features</h2>
    <p>List the key features of your project. For example:</p>
    <ul>
        <li>Smooth scrolling with Locomotive Scroll.</li>
        <li>Animated navigation bar.</li>
        <li>Video container with play button animation.</li>
        <li>Loading animations.</li>
        <li>Cursor animation.</li>
    </ul>
    <h2 id="installation">Installation</h2>
    <pre>
        <code>
            # Clone the repository
            git clone https://github.com/bitof-KARTIK/TWO-GOOD-CO.-CLONE.git
            # Navigate to the project directory
            cd TWO-GOOD-CO.-CLONE
            # Install dependencies
            # Add any other installation steps as needed
        </code>
    </pre>
    <h2 id="usage">Usage</h2>
    <pre>
        <code>
           <h2>Usage:</h2>
<p>
    Integrating TWO-GOOD-CO.-CLONE into your web project is a straightforward process. Follow the steps below to leverage its features and enhance the visual appeal of your website.
</p>

<h3>1. Installation:</h3>
<p>
    Include the necessary libraries and files in your project. Ensure you have GSAP and Locomotive Scroll properly linked in your HTML file. You can use CDN links or download the libraries and host them locally.
</p>
<script src="https://unpkg.com/gsap@3.9.0/dist/gsap.min.js"></script>
<script src="https://cdn.jsdelivr.net/npm/locomotive-scroll@4.0.0/dist/locomotive-scroll.min.js"></script>
        </code>
    </pre>
    <h2 id="dependencies">Dependencies</h2>
    <ul>
        <li>GSAP (GreenSock Animation Platform)</li>
        <li>Locomotive Scroll</li>
    </ul>
<h3>2. Initialization:</h3>
<p>
    Initialize the Locomotive Scroll instance and set up ScrollTrigger for smooth animations. Ensure your main container has the id "main" for proper scrollerProxy configuration.
</p>
<script>
    function locomotiveAnimations() {
        gsap.registerPlugin(ScrollTrigger);
        const locoScroll = new LocomotiveScroll({
            el: document.querySelector("#main"),
            smooth: true
        });
        ScrollTrigger.addEventListener("refresh", () => locoScroll.update());
        ScrollTrigger.refresh();
    }
    locomotiveAnimations();
</script>
<h3>3. Navigation Bar Animation:</h3>
<p>
    Implement animated navigation bar effects using GSAP. Adjust the trigger elements and animation properties as needed.
</p>
<!-- Add this script after initializing LocomotiveScroll -->
<script>
    function navbarAnimation() {
        gsap.to("#nav-part1 svg", {
            transform: "translateY(-100%)",
            scrollTrigger: {
                trigger: "#page1",
                scroller: "#main",
                start: "top 0%",
                end: "top -5%",
                scrub: true
            }
        });
    }
    navbarAnimation();
</script>

