
smartrepair/
  index.html
  about.html
  contact.html
  css/
    style.css
  js/
    app.js
    i18n.js
  assets/
    hero.jpg   
css/style.css
:root{
  --bg:#0b1220;
  --card:#111a2b;
  --text:#eaf0ff;
  --muted:#b9c6e4;
  --accent:#4f8cff;
  --accent2:#22c55e;
  --danger:#ef4444;
  --border:rgba(255,255,255,.12);
  --shadow: 0 10px 30px rgba(0,0,0,.35);
  --radius:16px;
*{box-sizing:border-box}
html,body{margin:0;padding:0}
body{
  font-family: system-ui, -apple-system, Segoe UI, Roboto, Arial, sans-serif;
  background: radial-gradient(1200px 600px at 15% 0%, #152241 0%, var(--bg) 55%);
  color:var(--text);
  line-height:1.6;
a{color:inherit;text-decoration:none}
img{max-width:100%;display:block}
.container{max-width:1100px;margin:0 auto;padding:0 18px}
.section{padding:44px 0}
.grid{display:grid;gap:18px}
.card{
  background: linear-gradient(180deg, rgba(255,255,255,.04), rgba(255,255,255,.02));
  border:1px solid var(--border);
  border-radius: var(--radius);
  box-shadow: var(--shadow);
  padding:18px;
.btn{
  display:inline-flex;align-items:center;justify-content:center;
  gap:10px;
  border:1px solid var(--border);
  background: rgba(255,255,255,.06);
  color:var(--text);
  padding:10px 14px;
  border-radius: 12px;
  cursor:pointer;
  transition:.18s ease;
  font-weight:600;
.btn:hover{transform:translateY(-1px);background: rgba(255,255,255,.10)}
.btn.primary{background: var(--accent); border-color: transparent}
.btn.primary:hover{background:#3b7bff}
.btn.success{background: var(--accent2); border-color: transparent}
.btn.danger{background: var(--danger); border-color: transparent}
.badge{
  display:inline-flex;align-items:center;gap:8px;
  border:1px solid var(--border);
  padding:6px 10px;border-radius:999px;
  color:var(--muted);
  background: rgba(255,255,255,.04);
  font-size: 13px;
  position:sticky;top:0;z-index:50;
  backdrop-filter: blur(10px);
  background: rgba(11,18,32,.72);
  border-bottom:1px solid var(--border);
.nav-inner
  display:flex;align-items:center;justify-content:space-between;
  padding:14px 0;
.brand
  display:flex;align-items:center;gap:10px;
  font-weight:800;letter-spacing:.2px;
.brand-mark{
  width:34px;height:34px;border-radius:10px;
  background: linear-gradient(135deg, var(--accent), #8b5cf6);
  box-shadow: 0 8px 25px rgba(79,140,255,.25);
.nav-links{
  display:flex;align-items:center;gap:12px;
.nav-links a{
  padding:8px 10px;border-radius:10px;
  color:var(--muted);
.nav-links a.active, .nav-links a:hover
  background: rgba(255,255,255,.06);
  color:var(--text);
.nav-actions{display:flex;align-items:center;gap:10px}
.icon-btn
  border:1px solid var(--border);
  background: rgba(255,255,255,.04);
  color:var(--text);
  padding:8px 10px;
  border-radius: 12px;
  cursor:pointer;
.hamburger{display:none}
.mobile-panel{display:none}
.hero
  display:grid;
  grid-template-columns: 1.15fr .85fr;
  gap:18px;
  align-items:stretch;
.hero h1{font-size:42px;line-height:1.15;margin:0 0 10px}
.hero p{color:var(--muted);margin:0 0 16px}
.hero-media{
  border-radius: var(--radius);
  overflow:hidden;
  border:1px solid var(--border);
  background:#0a1020;
  min-height: 320px;
  display:flex;align-items:center;justify-content:center;
.hero-media img{width:100%;height:100%;object-fit:cover}
.kpis{display:flex;flex-wrap:wrap;gap:10px;margin-top:12px}
.cards-3{grid-template-columns: repeat(3, 1fr)}
.cards-2{grid-template-columns: repeat(2, 1fr)}
label{display:block;margin:10px 0 6px;color:var(--muted);font-size:14px}
input, textarea, select{
  width:100%;
  background: rgba(255,255,255,.05);
  border:1px solid var(--border);
  border-radius: 12px;
  padding:10px 12px;
  color:var(--text);
  outline:none;
textarea{min-height:110px;resize:vertical}
small.help{color:var(--muted)}
.row{display:grid;grid-template-columns:1fr 1fr;gap:12px}
.notice{
  margin-top:10px;
  padding:10px 12px;
  border-radius: 12px;
  border:1px solid var(--border);
  background: rgba(255,255,255,.04);
  color: var(--muted);
.notice.ok{border-color: rgba(34,197,94,.35); color:#c9ffd8}
.notice.err{border-color: rgba(239,68,68,.35); color:#ffd1d1}
.footer{
  border-top:1px solid var(--border);
  padding:18px 0;
  color:var(--muted);
  font-size:14px;
.video{
  aspect-ratio: 16/9;
  width:100%;
  border-radius: var(--radius);
  overflow:hidden;
  border:1px solid var(--border);
.video iframe{width:100%;height:100%;border:0}
/* RTL support */
html[dir="rtl"] body{
  font-family: "Segoe UI", Tahoma, Arial, sans-serif;
html[dir="rtl"] .nav-links{gap:12px}
html[dir="rtl"] .row{direction:rtl}
/* Responsive */
@media (max-width: 900px){
  .hero{grid-template-columns: 1fr}
  .cards-3{grid-template-columns: 1fr}
  .cards-2{grid-template-columns: 1fr}
@media (max-width: 760px){
  .nav-links{display:none}
  .hamburger{display:inline-flex}
  .mobile-panel{
    display:none;
    border-top:1px solid var(--border);
    padding:12px 0;
  .mobile-panel.open{display:block}
  .mobile-panel a{
    display:block;
    padding:10px 10px;
    border-radius: 12px;
    color:var(--muted);
  .mobile-panel a:hover{background: rgba(255,255,255,.06); color:var(--text)}
  .nav-actions{gap:8px}
js/i18n.js
const I18N = {
  en: {
    brand: "SmartRepair",
    navHome: "Home",
    navAbout: "About",
    navContact: "Contact",
    navLogin: "Login",
    navRegister: "Register",
    navLogout: "Logout",
    langBtn: "AR",
    heroTag: "Fast booking. Transparent tracking.",
    heroTitle: "Repair booking made simple.",
    heroText: "Book your phone or laptop repair, track the status, and share feedback—all in one place.",
    ctaBook: "Book Repair",
    ctaLearn: "Learn More",
    kpi1: "Same-day options",
    kpi2: "Status tracking",
    kpi3: "Secure login",
    servicesTitle: "Services",
    s1Title: "Phone Screen Repair",
    s1Text: "Quick screen replacement with quality parts.",
    s2Title: "Battery Replacement",
    s2Text: "Improve battery health and device uptime.",
    s3Title: "Laptop Diagnostics",
    s3Text: "Identify issues and estimate repair costs.",
    howTitle: "How it works",
    h1: "Create an account",
    h1t: "Register and keep your bookings in one place.",
    h2: "Submit your request",
    h2t: "Describe the issue and choose a service.",
    h3: "Track and review",
    h3t: "Follow repair status and leave feedback.",
    authTitle: "User Authentication",
    authText: "Register or login to access booking and personalized features.",
    loginTitle: "Login",
    registerTitle: "Register",
    name: "Full Name",
    email: "Email",
    password: "Password",
    confirmPassword: "Confirm Password",
    submitLogin: "Sign In",
    submitRegister: "Create Account",
    aboutTitle: "About SmartRepair",
    aboutText:
      "SmartRepair is a lightweight web platform for repair booking, user authentication, and customer feedback. It improves service transparency by providing a simple, structured flow for users and repair shops.",
    aboutBul1: "Clean and responsive UI (mobile-first).",
    aboutBul2: "Local authentication using browser storage (for academic demo).",
    aboutBul3: "Feedback collection with ratings and timestamps.",
    contactTitle: "Contact & Feedback",
    contactText: "Send us your message or feedback. We review every submission.",
    message: "Message",
    rating: "Rating",
    submitFeedback: "Submit Feedback",
    footer: "Academic project template. Data stored locally in your browser.",
    bookNotice: "Demo booking button: You can extend it later with a booking form."
  ar: {
    brand: "سمارت ريبير",
    navHome: "الرئيسية",
    navAbout: "من نحن",
    navContact: "تواصل معنا",
    navLogin: "تسجيل دخول",
    navRegister: "إنشاء حساب",
    navLogout: "تسجيل خروج",
    langBtn: "EN",
    heroTag: "حجز سريع. تتبع واضح.",
    heroTitle: "حجز صيانة الأجهزة أصبح أسهل.",
    heroText: "احجز صيانة هاتفك أو لابتوبك، تتبع حالة الإصلاح، وأرسل ملاحظاتك—كل ذلك في مكان واحد.",
    ctaBook: "احجز صيانة",
    ctaLearn: "اعرف المزيد",
    kpi1: "خيارات نفس اليوم",
    kpi2: "تتبع الحالة",
    kpi3: "تسجيل آمن",
    servicesTitle: "الخدمات",
    s1Title: "تصليح شاشة الهاتف",
    s1Text: "استبدال سريع للشاشة مع قطع عالية الجودة.",
    s2Title: "تبديل البطارية",
    s2Text: "تحسين عمر البطارية ووقت التشغيل.",
    s3Title: "تشخيص اللابتوب",
    s3Text: "تحديد المشكلة وتقدير تكلفة الإصلاح.",
    howTitle: "كيف يعمل الموقع",
    h1: "أنشئ حساباً",
    h1t: "سجل واحتفظ بكل حجوزاتك في مكان واحد.",
    h2: "أرسل طلبك",
    h2t: "صف المشكلة واختر الخدمة المناسبة.",
    h3: "تتبع وقيّم",
    h3t: "تابع الحالة واترك ملاحظاتك.",
    authTitle: "توثيق المستخدم",
    authText: "يمكنك التسجيل أو تسجيل الدخول للوصول للميزات الخاصة.",
    loginTitle: "تسجيل الدخول",
    registerTitle: "إنشاء حساب",
    name: "الاسم الكامل",
    email: "البريد الإلكتروني",
    password: "كلمة المرور",
    confirmPassword: "تأكيد كلمة المرور",
    submitLogin: "دخول",
    submitRegister: "إنشاء الحساب",
    aboutTitle: "من نحن - سمارت ريبير",
    aboutText:
    aboutBul1: "واجهة نظيفة ومتجاوبة (مناسبة للموبايل).",
    aboutBul2: "توثيق محلي باستخدام تخزين المتصفح (للعرض الأكاديمي).",
    aboutBul3: "جمع الملاحظات مع تقييم وتاريخ الإرسال.",
    contactTitle: "التواصل والتغذية الراجعة",
    contactText: "أرسل لنا رسالتك أو ملاحظاتك. نراجع كل إرسال.",
    message: "الرسالة",
    rating: "التقييم",
    submitFeedback: "إرسال الملاحظة",
    footer: "قالب مشروع أكاديمي. يتم حفظ البيانات محلياً في المتصفح.",
    bookNotice: "زر الحجز تجريبي: يمكنك لاحقاً إضافة نموذج حجز كامل."
function getLang(){
  return localStorage.getItem("lang") || "en";
function setLang(lang){
  localStorage.setItem("lang", lang);
function applyLang(lang){
  const dict = I18N[lang];
  document.documentElement.lang = lang;
  document.documentElement.dir = (lang === "ar") ? "rtl" : "ltr";
  document.querySelectorAll("[data-i18n]").forEach(el=>{
    const key = el.getAttribute("data-i18n");
    if(dict[key] !== undefined) el.textContent = dict[key];
  });
  document.querySelectorAll("[data-i18n-placeholder]").forEach(el=>{
    const key = el.getAttribute("data-i18n-placeholder");
    if(dict[key] !== undefined) el.setAttribute("placeholder", dict[key]);
  });
  const langBtn = document.getElementById("langBtn");
  if(langBtn) langBtn.textContent = dict.langBtn;
document.addEventListener("DOMContentLoaded", ()=>{
  applyLang(getLang());
});
js/app.js
function $(id){ return document.getElementById(id); }
function getUsers(){
  return JSON.parse(localStorage.getItem("users") || "[]");
function setUsers(users){
  localStorage.setItem("users", JSON.stringify(users));
function setCurrentUser(user){
  localStorage.setItem("currentUser", JSON.stringify(user));
function getCurrentUser(){
  return JSON.parse(localStorage.getItem("currentUser") || "null");
function clearCurrentUser(){
  localStorage.removeItem("currentUser");
function showNotice(el, type, msg){
  if(!el) return;
  el.className = "notice " + (type === "ok" ? "ok" : "err");
  el.textContent = msg;
  el.style.display = "block";
function updateAuthUI(){
  const user = getCurrentUser();
  const loginLink = $("navLogin");
  const regLink = $("navRegister");
  const logoutBtn = $("logoutBtn");
  const userBadge = $("userBadge");
  if(user){
    if(loginLink) loginLink.style.display = "none";
    if(regLink) regLink.style.display = "none";
    if(logoutBtn) logoutBtn.style.display = "inline-flex";
    if(userBadge){
      userBadge.style.display = "inline-flex";
      userBadge.textContent = user.name;
  }else{
    if(loginLink) loginLink.style.display = "inline-flex";
    if(regLink) regLink.style.display = "inline-flex";
    if(logoutBtn) logoutBtn.style.display = "none";
    if(userBadge) userBadge.style.display = "none";
function bindNavbar(){
  const burger = $("burger");
  const panel = $("mobilePanel");
  if(burger && panel){
    burger.addEventListener("click", ()=>{
      panel.classList.toggle("open");
    });
  const langBtn = $("langBtn");
  if(langBtn){
    langBtn.addEventListener("click", ()=>{
      const cur = getLang();
      const next = (cur === "en") ? "ar" : "en";
      setLang(next);
      applyLang(next);
    });
  const logoutBtn = $("logoutBtn");
  if(logoutBtn){
    logoutBtn.addEventListener("click", ()=>{
      clearCurrentUser();
      updateAuthUI();
function bindAuthForms(){
  const loginForm = $("loginForm");
  const regForm = $("registerForm");
  if(loginForm){
    loginForm.addEventListener("submit", (e)=>{
      e.preventDefault();
      const email = $("loginEmail").value.trim().toLowerCase();
      const password = $("loginPassword").value;
      const users = getUsers();
      const user = users.find(u => u.email === email && u.password === password);
      const notice = $("loginNotice");
      if(!user){
        showNotice(notice, "err", (getLang()==="ar") ? "بيانات الدخول غير صحيحة." : "Invalid login credentials.");
        return;
      setCurrentUser({name:user.name, email:user.email});
      showNotice(notice, "ok", (getLang()==="ar") ? "تم تسجيل الدخول بنجاح." : "Logged in successfully.");
      updateAuthUI();
      loginForm.reset();
    });
  if(regForm){
    regForm.addEventListener("submit", (e)=>{
      e.preventDefault();
      const name = $("regName").value.trim();
      const email = $("regEmail").value.trim().toLowerCase();
      const pass = $("regPassword").value;
      const confirm = $("regConfirm").value;
      const notice = $("registerNotice");
      if(pass.length < 6){
        showNotice(notice, "err", (getLang()==="ar") ? "كلمة المرور يجب أن تكون 6 أحرف على الأقل." : "Password must be at least 6 characters.");
        return;
      if(pass !== confirm){
        showNotice(notice, "err", (getLang()==="ar") ? "كلمتا المرور غير متطابقتين." : "Passwords do not match.");
        return;
      const users = getUsers();
      if(users.some(u=>u.email === email)){
        showNotice(notice, "err", (getLang()==="ar") ? "هذا البريد مسجل مسبقاً." : "Email is already registered.");
        return;
      users.push({name, email, password: pass});
      setUsers(users);
      showNotice(notice, "ok", (getLang()==="ar") ? "تم إنشاء الحساب بنجاح." : "Account created successfully.");
      regForm.reset();
function bindFeedbackForm(){
  const form = $("feedbackForm");
  if(!form) return;
  form.addEventListener("submit", (e)=>{
    e.preventDefault();
    const name = $("fbName").value.trim();
    const email = $("fbEmail").value.trim();
    const rating = $("fbRating").value;
    const message = $("fbMessage").value.trim();
    const notice = $("feedbackNotice");
    if(!name || !email || !message){
      showNotice(notice, "err", (getLang()==="ar") ? "يرجى ملء جميع الحقول المطلوبة." : "Please fill all required fields.");
      return;
    const list = JSON.parse(localStorage.getItem("feedback") || "[]");
    list.push({
      name, email, rating,
      message,
      createdAt: new Date().toISOString()
    });
    localStorage.setItem("feedback", JSON.stringify(list));

    showNotice(notice, "ok", (getLang()==="ar") ? "تم إرسال ملاحظتك بنجاح." : "Feedback submitted successfully.");
    form.reset();
  });
function markActiveNav(){
  const path = location.pathname.split("/").pop() || "index.html";
  document.querySelectorAll(".nav-links a").forEach(a=>{
    const href = a.getAttribute("href");
    if(href === path) a.classList.add("active");
  });
  document.querySelectorAll("#mobilePanel a").forEach(a=>{
    const href = a.getAttribute("href");
    if(href === path) a.style.background = "rgba(255,255,255,.06)";
  });
document.addEventListener("DOMContentLoaded", ()=>{
  bindNavbar();
  bindAuthForms();
  bindFeedbackForm();
  updateAuthUI();
  markActiveNav();
});
index.html
<!doctype html>
<html lang="en" dir="ltr">
<head>
  <meta charset="utf-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1" />
  <title>SmartRepair</title>
  <link rel="stylesheet" href="css/style.css" />
</head>
<body>
  <header class="nav">
    <div class="container">
      <div class="nav-inner">
        <a class="brand" href="index.html">
          <span class="brand-mark"></span>
          <span data-i18n="brand">SmartRepair</span>
        </a>
        <nav class="nav-links">
          <a href="index.html" data-i18n="navHome">Home</a>
          <a href="about.html" data-i18n="navAbout">About</a>
          <a href="contact.html" data-i18n="navContact">Contact</a>
        </nav>
        <div class="nav-actions">
          <span id="userBadge" class="badge" style="display:none;"></span>
          <a id="navLogin" class="btn" href="#auth" data-i18n="navLogin">Login</a>
          <a id="navRegister" class="btn" href="#auth" data-i18n="navRegister">Register</a>
          <button id="logoutBtn" class="btn danger" style="display:none;" data-i18n="navLogout">Logout</button>
          <button id="langBtn" class="icon-btn">AR</button>
          <button id="burger" class="icon-btn hamburger">☰</button>
        </div>
      </div>
      <div id="mobilePanel" class="mobile-panel">
        <a href="index.html" data-i18n="navHome">Home</a>
        <a href="about.html" data-i18n="navAbout">About</a>
        <a href="contact.html" data-i18n="navContact">Contact</a>
      </div>
    </div>
  </header>
  <main>
    <section class="section">
      <div class="container hero">
        <div class="card">
          <span class="badge" data-i18n="heroTag">Fast booking. Transparent tracking.</span>
          <h1 data-i18n="heroTitle">Repair booking made simple.</h1>
          <p data-i18n="heroText">
            Book your phone or laptop repair, track the status, and share feedback—all in one place.
          </p>
          <div style="display:flex; gap:10px; flex-wrap:wrap;">
            <button class="btn primary" id="bookBtn" data-i18n="ctaBook">Book Repair</button>
            <a class="btn" href="about.html" data-i18n="ctaLearn">Learn More</a>
          </div>
          <div class="notice" id="bookNotice" style="display:none; margin-top:12px;" data-i18n="bookNotice">
            Demo booking button: You can extend it later with a booking form.
          </div>
          <div class="kpis">
            <span class="badge" data-i18n="kpi1">Same-day options</span>
            <span class="badge" data-i18n="kpi2">Status tracking</span>
            <span class="badge" data-i18n="kpi3">Secure login</span>
          </div>
        </div>
        <div class="hero-media">
          <img src="assets/hero.jpg" alt="Repair service" />
        </div>
      </div>
    </section>
    <section class="section">
      <div class="container">
        <h2 style="margin:0 0 12px" data-i18n="servicesTitle">Services</h2>
        <div class="grid cards-3">
          <div class="card">
            <h3 style="margin:0 0 8px" data-i18n="s1Title">Phone Screen Repair</h3>
            <p style="margin:0;color:var(--muted)" data-i18n="s1Text">Quick screen replacement with quality parts.</p>
          </div>
          <div class="card">
            <h3 style="margin:0 0 8px" data-i18n="s2Title">Battery Replacement</h3>
            <p style="margin:0;color:var(--muted)" data-i18n="s2Text">Improve battery health and device uptime.</p>
          </div>
          <div class="card">
            <h3 style="margin:0 0 8px" data-i18n="s3Title">Laptop Diagnostics</h3>
            <p style="margin:0;color:var(--muted)" data-i18n="s3Text">Identify issues and estimate repair costs.</p>
          </div>
        </div>
      </div>
    </section>
    <section class="section">
      <div class="container">
        <h2 style="margin:0 0 12px" data-i18n="howTitle">How it works</h2>
        <div class="grid cards-3">
          <div class="card">
            <h3 style="margin:0 0 8px" data-i18n="h1">Create an account</h3>
            <p style="margin:0;color:var(--muted)" data-i18n="h1t">Register and keep your bookings in one place.</p>
          </div>
          <div class="card">
            <h3 style="margin:0 0 8px" data-i18n="h2">Submit your request</h3>
            <p style="margin:0;color:var(--muted)" data-i18n="h2t">Describe the issue and choose a service.</p>
          </div>
          <div class="card">
            <h3 style="margin:0 0 8px" data-i18n="h3">Track and review</h3>
            <p style="margin:0;color:var(--muted)" data-i18n="h3t">Follow repair status and leave feedback.</p>
          </div>
        </div>
      </div>
    </section>
    <section class="section" id="auth">
      <div class="container">
        <div class="card">
          <h2 style="margin:0 0 8px" data-i18n="authTitle">User Authentication</h2>
          <p style="margin:0 0 14px;color:var(--muted)" data-i18n="authText">
            Register or login to access booking and personalized features.
          </p>
          <div class="grid cards-2">
            <div class="card">
              <h3 style="margin:0 0 10px" data-i18n="loginTitle">Login</h3>
              <form id="loginForm">
                <label data-i18n="email">Email</label>
                <input id="loginEmail" type="email" required placeholder="email@example.com" />
                <label data-i18n="password">Password</label>
                <input id="loginPassword" type="password" required />
                <button class="btn primary" type="submit" style="margin-top:12px" data-i18n="submitLogin">Sign In</button>
                <div id="loginNotice" class="notice" style="display:none"></div>
              </form>
            </div>
            <div class="card">
              <h3 style="margin:0 0 10px" data-i18n="registerTitle">Register</h3>
              <form id="registerForm">
                <label data-i18n="name">Full Name</label>
                <input id="regName" type="text" required />
                <label data-i18n="email">Email</label>
                <input id="regEmail" type="email" required placeholder="email@example.com" />
                <div class="row">
                  <div>
                    <label data-i18n="password">Password</label>
                    <input id="regPassword" type="password" required />
                  </div>
                  <div>
                    <label data-i18n="confirmPassword">Confirm Password</label>
                    <input id="regConfirm" type="password" required />
                  </div>
                </div>
                <small class="help">Min 6 characters</small>
                <button class="btn success" type="submit" style="margin-top:12px" data-i18n="submitRegister">Create Account</button>
                <div id="registerNotice" class="notice" style="display:none"></div>
              </form>
            </div>
          </div>
        </div>
      </div>
    </section>
    <section class="section">
      <div class="container">
        <div class="card">
          <h2 style="margin:0 0 12px">Media</h2>
          <div class="video">
            <iframe
              src="https://www.youtube.com/embed/1wfeqDyMUx4"
              title="How device repair works"
              allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture"
              allowfullscreen>
            </iframe>
          </div>
        </div>
      </div>
    </section>
  </main>
  <footer class="footer">
    <div class="container" data-i18n="footer">Academic project template. Data stored locally in your browser.</div>
  </footer>
  <script src="js/i18n.js"></script>
  <script src="js/app.js"></script>
  <script>
    document.getElementById("bookBtn").addEventListener("click", ()=>{
      const n = document.getElementById("bookNotice");
      n.style.display = "block";
    });
  </script>
</body>
</html>
about.html
<!doctype html>
<html lang="en" dir="ltr">
<head>
  <meta charset="utf-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1" />
  <title>About - SmartRepair</title>
  <link rel="stylesheet" href="css/style.css" />
</head>
<body>
  <header class="nav">
    <div class="container">
      <div class="nav-inner">
        <a class="brand" href="index.html">
          <span class="brand-mark"></span>
          <span data-i18n="brand">SmartRepair</span>
        </a>
        <nav class="nav-links">
          <a href="index.html" data-i18n="navHome">Home</a>
          <a href="about.html" data-i18n="navAbout">About</a>
          <a href="contact.html" data-i18n="navContact">Contact</a>
        </nav>
        <div class="nav-actions">
          <span id="userBadge" class="badge" style="display:none;"></span>
          <a id="navLogin" class="btn" href="index.html#auth" data-i18n="navLogin">Login</a>
          <a id="navRegister" class="btn" href="index.html#auth" data-i18n="navRegister">Register</a>
          <button id="logoutBtn" class="btn danger" style="display:none;" data-i18n="navLogout">Logout</button>
          <button id="langBtn" class="icon-btn">AR</button>
          <button id="burger" class="icon-btn hamburger">☰</button>
        </div>
      </div>
      <div id="mobilePanel" class="mobile-panel">
        <a href="index.html" data-i18n="navHome">Home</a>
        <a href="about.html" data-i18n="navAbout">About</a>
        <a href="contact.html" data-i18n="navContact">Contact</a>
      </div>
    </div>
  </header>
  <main class="section">
    <div class="container">
      <div class="card">
        <h1 style="margin:0 0 10px" data-i18n="aboutTitle">About SmartRepair</h1>
        <p style="margin:0;color:var(--muted)" data-i18n="aboutText"></p>
        <div class="grid cards-3" style="margin-top:14px;">
          <div class="card"><span data-i18n="aboutBul1"></span></div>
          <div class="card"><span data-i18n="aboutBul2"></span></div>
          <div class="card"><span data-i18n="aboutBul3"></span></div>
        </div>
      </div>
    </div>
  </main>
  <footer class="footer">
    <div class="container" data-i18n="footer">Academic project template. Data stored locally in your browser.</div>
  </footer>
  <script src="js/i18n.js"></script>
  <script src="js/app.js"></script>
</body>
</html>
contact.html
<!doctype html>
<html lang="en" dir="ltr">
<head>
  <meta charset="utf-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1" />
  <title>Contact - SmartRepair</title>
  <link rel="stylesheet" href="css/style.css" />
</head>
<body>
  <header class="nav">
    <div class="container">
      <div class="nav-inner">
        <a class="brand" href="index.html">
          <span class="brand-mark"></span>
          <span data-i18n="brand">SmartRepair</span>
        </a>
        <nav class="nav-links">
          <a href="index.html" data-i18n="navHome">Home</a>
          <a href="about.html" data-i18n="navAbout">About</a>
          <a href="contact.html" data-i18n="navContact">Contact</a>
        </nav>
        <div class="nav-actions">
          <span id="userBadge" class="badge" style="display:none;"></span>
          <a id="navLogin" class="btn" href="index.html#auth" data-i18n="navLogin">Login</a>
          <a id="navRegister" class="btn" href="index.html#auth" data-i18n="navRegister">Register</a>
          <button id="logoutBtn" class="btn danger" style="display:none;" data-i18n="navLogout">Logout</button>
          <button id="langBtn" class="icon-btn">AR</button>
          <button id="burger" class="icon-btn hamburger">☰</button>
        </div>
      </div>
      <div id="mobilePanel" class="mobile-panel">
        <a href="index.html" data-i18n="navHome">Home</a>
        <a href="about.html" data-i18n="navAbout">About</a>
        <a href="contact.html" data-i18n="navContact">Contact</a>
      </div>
    </div>
  </header>
  <main class="section">
    <div class="container">
      <div class="card">
        <h1 style="margin:0 0 8px" data-i18n="contactTitle">Contact & Feedback</h1>
        <p style="margin:0 0 14px;color:var(--muted)" data-i18n="contactText"></p>
        <form id="feedbackForm">
          <div class="row">
            <div>
              <label data-i18n="name">Full Name</label>
              <input id="fbName" type="text" required />
            </div>
            <div>
              <label data-i18n="email">Email</label>
              <input id="fbEmail" type="email" required placeholder="email@example.com" />
            </div>
          </div>
          <div class="row">
            <div>
              <label data-i18n="rating">Rating</label>
              <select id="fbRating">
                <option value="5">5</option>
                <option value="4">4</option>
                <option value="3" selected>3</option>
                <option value="2">2</option>
                <option value="1">1</option>
              </select>
            </div>
            <div>
              <label>&nbsp;</label>
              <small class="help">You can add phone number field if required.</small>
            </div>
          </div>
          <label data-i18n="message">Message</label>
          <textarea id="fbMessage" required></textarea>
          <button class="btn success" type="submit" style="margin-top:12px" data-i18n="submitFeedback">Submit Feedback</button>
          <div id="feedbackNotice" class="notice" style="display:none"></div>
        </form>
      </div>
    </div>
  </main>
  <footer class="footer">
    <div class="container" data-i18n="footer">Academic project template. Data stored locally in your browser.</div>
  </footer>
  <script src="js/i18n.js"></script>
  <script src="js/app.js"></script>
</body>
</html>
