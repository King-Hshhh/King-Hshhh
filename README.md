<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>FutureLeadersHub</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            margin: 0;
            padding: 0;
            background-color: #f0f0f0;
        }
        header {
            background-color: #4CAF50;
            color: white;
            padding: 1rem;
            text-align: center;
        }
        nav {
            margin: 1rem;
            text-align: center;
        }
        nav a {
            margin: 0 1rem;
            text-decoration: none;
            color: #4CAF50;
        }
        .container {
            padding: 2rem;
            background-color: white;
            margin: 2rem auto;
            width: 80%;
            box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
        }
        .section-title {
            font-size: 1.5rem;
            margin-bottom: 1rem;
        }
        .mentor {
            display: flex;
            align-items: center;
            margin: 1rem 0;
        }
        .mentor img {
            border-radius: 50%;
            margin-right: 1rem;
        }
        .testimonials, .contact-section {
            background-color: #e0e0e0;
            padding: 1rem;
            margin: 2rem 0;
        }
        .hidden {
            display: none;
        }
    </style>
</head>
<body>

<header>
    <h1>FutureLeadersHub</h1>
    <p>Empower Your Future</p>
</header>

<nav>
    <a href="#get-started">Get Started</a>
    <a href="#learn-more">Learn More</a>
    <a href="#meet-mentors">Meet The Mentors</a>
    <a href="#testimonials">Testimonials</a>
    <a href="#contact">Contact Us</a>
</nav>

<div class="container" id="get-started">
    <h2 class="section-title">Get Started</h2>
    <p>At FutureLeadersHub, we connect youth with mentors and educational resources to unlock their full potential. Discover opportunities, gain guidance, and lead the way.</p>
    <button onclick="toggleSection('learn-more')">Learn More</button>
</div>

<div class="container hidden" id="learn-more">
    <h2 class="section-title">Comprehensive Support</h2>
    <p>FutureLeadersHub offers a range of programs and resources designed to support your academic and career growth. From mentorship to leadership development, we have everything you need to succeed.</p>
    <ul>
        <li>Mentor Profiles: Connect with experienced mentors who can provide guidance and support in your chosen field.</li>
        <li>Academic Support: Access resources and programs to help you excel in your studies and achieve your academic goals.</li>
        <li>Career Guidance: Receive advice and resources to help you navigate your career path and achieve professional success.</li>
    </ul>
</div>

<div class="container" id="meet-mentors">
    <h2 class="section-title">Meet Our Mentors</h2>
    <div class="mentor">
        <img src="mentor1.jpg" alt="Aphiwe Nkosi" width="100">
        <div>
            <h3>Aphiwe Nkosi</h3>
            <p>Career Coach</p>
        </div>
    </div>
    <div class="mentor">
        <img src="mentor2.jpg" alt="Samantha Lee" width="100">
        <div>
            <h3>Samantha Lee</h3>
            <p>Academic Advisor</p>
        </div>
    </div>
    <div class="mentor">
        <img src="mentor3.jpg" alt="Thapelo" width="100">
        <div>
            <h3>Thapelo</h3>
            <p>Leadership Trainer</p>
        </div>
    </div>
    <div class="mentor">
        <img src="mentor4.jpg" alt="Emily Davis" width="100">
        <div>
            <h3>Emily Davis</h3>
            <p>Mentorship Coordinator</p>
        </div>
    </div>
</div>

<div class="container testimonials" id="testimonials">
    <h2 class="section-title">Testimonials</h2>
    <p>FutureLeadersHub has been a game-changer for me. The mentorship and resources have helped me excel in my studies and plan my career path.</p>
    <p><strong>Jordan Brown</strong> - April 20, 2024</p>
    <p>The support and guidance I've received from my mentor have been invaluable. I feel more confident and prepared for my future.</p>
    <p><strong>Taylor Smith</strong> - June 15, 2024</p>
    <p>FutureLeadersHub offers amazing resources and programs. It's a fantastic platform for any young person looking to grow and succeed.</p>
    <p><strong>Casey Lee</strong> - May 10, 2024</p>
</div>

<div class="container contact-section" id="contact">
    <h2 class="section-title">Contact Us</h2>
    <p>Have questions or need support? Reach out to us, and we'll be happy to help.</p>
    <h3>General Inquiries</h3>
    <p>For any general questions or information, feel free to contact us.</p>
    <button onclick="sendEmail('info@futureleadershub.com')">Email Us</button>
    <h3>Support</h3>
    <p>Need assistance? Our support team is here to help you with any issues or questions.</p>
    <button onclick="sendEmail('support@futureleadershub.com')">Get Support</button>
    <h3>Join Our Team</h3>
    <p>Interested in becoming a mentor or joining our team? Contact us to learn more.</p>
    <button onclick="sendEmail('join@futureleadershub.com')">Apply Now</button>
</div>

<script>
    function toggleSection(sectionId) {
        var section = document.getElementById(sectionId);
        if (section.classList.contains('hidden')) {
            section.classList.remove('hidden');
        } else {
            section.classList.add('hidden');
        }
    }

    function sendEmail(email) {
        window.location.href = 'mailto:' + email;
    }
</script>

</body>
</html>
