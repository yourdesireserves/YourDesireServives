<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">

<title>YourDesireServices</title>

<style>
* {
box-sizing: border-box;
margin: 0;
padding: 0;
font-family: Arial, Helvetica, sans-serif;
}

body {
background: #f7faff;
color: #14213d;
}

/* NAVIGATION */

nav {
height: 75px;
background: white;
display: flex;
align-items: center;
justify-content: space-between;
padding: 0 7%;
border-bottom: 1px solid #e7edf5;
position: sticky;
top: 0;
z-index: 100;
}

.logo {
font-size: 24px;
font-weight: 800;
color: #075bd8;
}

.nav-links {
display: flex;
gap: 28px;
align-items: center;
}

.nav-links a {
text-decoration: none;
color: #253858;
font-weight: 600;
}

.login {
border: 1px solid #075bd8;
padding: 10px 18px;
border-radius: 8px;
color: #075bd8 !important;
}

/* HERO */

.hero {
min-height: 620px;
display: flex;
align-items: center;
padding: 70px 7%;
background:
radial-gradient(circle at 90% 20%, #d9ebff 0%, transparent 30%),
linear-gradient(135deg, #ffffff 0%, #eef6ff 100%);
}

.hero-content {
max-width: 650px;
}

.badge {
display: inline-block;
background: #e2efff;
color: #075bd8;
padding: 9px 15px;
border-radius: 30px;
font-size: 14px;
font-weight: bold;
margin-bottom: 20px;
}

.hero h1 {
font-size: 58px;
line-height: 1.05;
margin-bottom: 22px;
}

.hero h1 span {
color: #075bd8;
}

.hero p {
font-size: 19px;
line-height: 1.7;
color: #667085;
margin-bottom: 32px;
}

.buttons {
display: flex;
gap: 14px;
flex-wrap: wrap;
}

.primary-btn {
background: #075bd8;
color: white;
border: none;
padding: 15px 25px;
border-radius: 9px;
font-size: 16px;
font-weight: bold;
cursor: pointer;
}

.secondary-btn {
background: white;
color: #075bd8;
border: 1px solid #cbd8e8;
padding: 15px 25px;
border-radius: 9px;
font-size: 16px;
font-weight: bold;
cursor: pointer;
}

/* SEARCH */

.search-section {
margin-top: -55px;
padding: 0 7%;
position: relative;
}

.search-box {
background: white;
padding: 15px;
border-radius: 15px;
box-shadow: 0 12px 35px rgba(24, 67, 120, 0.12);
display: flex;
gap: 10px;
max-width: 900px;
margin: auto;
}

.search-box input {
flex: 1;
border: none;
outline: none;
padding: 15px;
font-size: 16px;
}

.search-box button {
background: #075bd8;
color: white;
border: none;
padding: 15px 30px;
border-radius: 9px;
font-weight: bold;
cursor: pointer;
}

/* SERVICES */

.services-section {
padding: 90px 7%;
}

.section-title {
text-align: center;
margin-bottom: 45px;
}

.section-title h2 {
font-size: 36px;
margin-bottom: 12px;
}

.section-title p {
color: #667085;
}

.services {
display: grid;
grid-template-columns:
repeat(auto-fit, minmax(190px, 1fr));
gap: 20px;
}

.service {
background: white;
padding: 30px 20px;
border: 1px solid #e4ebf4;
border-radius: 15px;
text-align: center;
transition: 0.2s;
}

.service:hover {
transform: translateY(-5px);
box-shadow: 0 10px 25px rgba(24, 67, 120, 0.1);
}

.service-icon {
width: 65px;
height: 65px;
margin: auto auto 18px;
border-radius: 14px;
background: #eaf3ff;
display: flex;
justify-content: center;
align-items: center;
font-size: 30px;
}

.service h3 {
margin-bottom: 9px;
}

.service p {
color: #667085;
font-size: 14px;
line-height: 1.5;
}

/* HOW IT WORKS */

.how {
background: #075bd8;
color: white;
padding: 75px 7%;
text-align: center;
}

.how h2 {
font-size: 35px;
margin-bottom: 45px;
}

.steps {
display: grid;
grid-template-columns:
repeat(auto-fit, minmax(200px, 1fr));
gap: 35px;
max-width: 950px;
margin: auto;
}

.step-number {
width: 50px;
height: 50px;
background: white;
color: #075bd8;
border-radius: 50%;
display: flex;
align-items: center;
justify-content: center;
margin: auto auto 15px;
font-weight: bold;
font-size: 20px;
}

.step p {
margin-top: 8px;
opacity: 0.85;
}

/* PROVIDER */

.provider {
padding: 80px 7%;
}

.provider-box {
background: white;
border: 1px solid #e3eaf4;
border-radius: 20px;
padding: 50px;
text-align: center;
max-width: 950px;
margin: auto;
}

.provider-box h2 {
font-size: 34px;
margin-bottom: 15px;
}

.provider-box p {
color: #667085;
margin-bottom: 25px;
}

/* FOOTER */

footer {
background: #101d33;
color: white;
padding: 45px 7%;
text-align: center;
}

footer h3 {
color: #5fa0ff;
margin-bottom: 10px;
}

footer p {
color: #b7c1d1;
}

/* MOBILE */

@media (max-width: 700px) {

.nav-links {
display: none;
}

.hero {
min-height: 560px;
padding-top: 60px;
}

.hero h1 {
font-size: 42px;
}

.hero p {
font-size: 17px;
}

.search-box {
flex-direction: column;
}

.search-box button {
width: 100%;
}

.provider-box {
padding: 35px 20px;
}
}
</style>
</head>

<body>

<!-- NAVIGATION -->

<nav>

<div class="logo">
YourDesireServices
</div>

<div class="nav-links">
<a href="index.html">Home</a>
<a href="services.html">Services</a>
<a href="#how">How It Works</a>
<a href="#provider">Become a Provider</a>
<a href="#" class="login">Log In</a>
</div>

</nav>


<!-- HERO -->

<section class="hero">

<div class="hero-content">

<div class="badge">
Your Services. Your Choice.
</div>

<h1>
Find the right service
<span>for your needs.</span>
</h1>

<p>
YourDesireServices connects customers with
service providers in one convenient place.
Search, discover and book services with ease.
</p>

<div class="buttons">

<button
class="primary-btn"
onclick="goToServices()">
Find a Service
</button>

<button
class="secondary-btn"
onclick="becomeProvider()">
Become a Provider
</button>

</div>

</div>

</section>


<!-- SEARCH -->

<section class="search-section">

<div class="search-box">

<input
id="searchInput"
type="text"
placeholder="What service are you looking for?">

<button onclick="searchService()">
Search
</button>

</div>

</section>


<!-- SERVICES -->

<section class="services-section">

<div class="section-title">

<h2>Explore Services</h2>

<p>
Find professionals for the services you need.
</p>

</div>


<div class="services">

<div class="service">
<div class="service-icon">💇</div>
<h3>Beauty</h3>
<p>Hair, nails, makeup and more.</p>
</div>

<div class="service">
<div class="service-icon">🚗</div>
<h3>Auto</h3>
<p>Repairs, detailing and automotive services.</p>
</div>

<div class="service">
<div class="service-icon">🏠</div>
<h3>Home</h3>
<p>Cleaning, repairs, lawn care and more.</p>
</div>

<div class="service">
<div class="service-icon">🍔</div>
<h3>Food</h3>
<p>Catering, cooks and food services.</p>
</div>

<div class="service">
<div class="service-icon">📦</div>
<h3>Delivery</h3>
<p>Delivery, moving and transportation.</p>
</div>

<div class="service">
<div class="service-icon">💻</div>
<h3>Technology</h3>
<p>Websites, computer help and digital services.</p>
</div>

</div>

</section>


<!-- HOW IT WORKS -->

<section class="how" id="how">

<h2>How YourDesireServices Works</h2>

<div class="steps">

<div class="step">
<div class="step-number">1</div>
<h3>Find a Service</h3>
<p>Search for the service you need.</p>
</div>

<div class="step">
<div class="step-number">2</div>
<h3>Choose a Provider</h3>
<p>Explore available service providers.</p>
</div>

<div class="step">
<div class="step-number">3</div>
<h3>Book</h3>
<p>Choose a convenient date and time.</p>
</div>

<div class="step">
<div class="step-number">4</div>
<h3>Get It Done</h3>
<p>Connect with your service provider.</p>
</div>

</div>

</section>


<!-- PROVIDER -->

<section class="provider" id="provider">

<div class="provider-box">

<h2>Grow Your Business With Us</h2>

<p>
Offer your services to customers looking
for professionals like you.
</p>

<button
class="primary-btn"
onclick="becomeProvider()">
Become a Service Provider
</button>

</div>

</section>


<!-- FOOTER -->

<footer>

<h3>YourDesireServices</h3>

<p>
Connecting customers with service providers.
</p>

<br>

<p>
© 2026 YourDesireServices. All rights reserved.
</p>

</footer>


<script>

function goToServices() {
window.location.href = "services.html";
}

function searchService() {

const service =
document.getElementById("searchInput").value;

if (service.trim() === "") {

alert("Please enter a service to search.");

} else {

window.location.href =
"services.html?search=" +
encodeURIComponent(service);

}

}

function becomeProvider() {

alert(
"Provider registration will be available soon!"
);

}

</script>

</body>
</html>
