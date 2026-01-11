--bg:#f6f8fb;
  --surface:#ffffff;
  --surface2:#f3f6ff;
  --text:#0f172a;
  --muted:#475569;

  --primary:#0ea5a4;     /* teal */
  --primary2:#6366f1;    /* indigo */
  --accent:#f59e0b;      /* amber */

  --border:#e2e8f0;
  --shadow:0 14px 40px rgba(15, 23, 42, .10);

  --radius:18px;
  --max:1200px;

  --font: ui-sans-serif, system-ui, -apple-system, "Segoe UI", Arial, "Noto Sans Arabic", "Noto Sans", sans-serif;
}

*{box-sizing:border-box}
html,body{margin:0;padding:0}
body{
  font-family:var(--font);
  background:
    radial-gradient(1100px 700px at 10% 10%, rgba(14,165,164,.12), transparent 60%),
    radial-gradient(1100px 700px at 90% 15%, rgba(99,102,241,.10), transparent 60%),
    radial-gradient(1000px 650px at 50% 90%, rgba(245,158,11,.10), transparent 60%),
    var(--bg);
  color:var(--text);
  line-height:1.75;
}

a{color:inherit;text-decoration:none}
img{max-width:100%;display:block}
.container{max-width:var(--max);margin:0 auto;padding:0 18px}
.section{padding:76px 0}
.grid{display:grid;gap:18px}

.skip-link{
  position:absolute;left:-999px;top:auto;width:1px;height:1px;overflow:hidden;
}
.skip-link:focus{left:18px;top:12px;width:auto;height:auto;z-index:9999;background:#fff;padding:10px 12px;border-radius:12px;border:1px solid var(--border);box-shadow:var(--shadow)}

.card{
  background:var(--surface);
  border:1px solid var(--border);
  border-radius:var(--radius);
  box-shadow:var(--shadow);
  padding:22px;
}

.card.soft{
  background:linear-gradient(180deg, var(--surface), var(--surface2));
}

.badge{
  display:inline-flex;align-items:center;gap:8px;
  padding:8px 12px;
  border-radius:999px;
  border:1px solid rgba(14,165,164,.25);
  background:rgba(14,165,164,.08);
  color:#0b6b6a;
  font-size:14px;
  font-weight:700;
}

.hr{height:1px;background:var(--border);margin:18px 0}

.btn{
  display:inline-flex;align-items:center;justify-content:center;gap:10px;
  padding:12px 16px;border-radius:14px;border:1px solid var(--border);
  background:#fff;color:var(--text);
  cursor:pointer;transition:.18s transform,.18s box-shadow,.18s opacity;
  font-weight:800;
}
.btn:hover{transform:translateY(-1px);box-shadow:0 10px 24px rgba(15,23,42,.10)}
.btn:focus-visible{outline:3px solid rgba(99,102,241,.25);outline-offset:2px}
.btn.primary{border-color:transparent;color:#fff;background:linear-gradient(90deg,var(--primary),var(--primary2))}
.btn.ghost{background:transparent}
.btn.pill{border-radius:999px}

.nav{
  position:sticky;top:0;z-index:50;
  background:#ffffffcc;
  backdrop-filter: blur(10px);
  border-bottom:1px solid var(--border);
}
.navbar{display:flex;align-items:center;justify-content:space-between;padding:14px 0;gap:14px;flex-wrap:wrap}
.brand{display:flex;align-items:center;gap:12px;font-weight:900;letter-spacing:.2px}
.brand img{width:42px;height:42px;border-radius:14px}
.brand-text{display:flex;flex-direction:column;gap:2px}
.brand-text span{font-size:12px;color:var(--muted);font-weight:700}

.links{display:flex;gap:10px;flex-wrap:wrap}
.link{padding:10px 12px;border-radius:12px;color:var(--muted);border:1px solid transparent}
.link:hover{background:#f1f5f9;color:var(--text);border-color:var(--border)}
.link.active{background:#eef2ff;color:#3730a3;border-color:#e0e7ff}

.nav-actions{display:flex;gap:10px;align-items:center;flex-wrap:wrap}
.menu-btn{display:none}

.hero{
  display:grid;grid-template-columns: 1.15fr .85fr;
  gap:18px;align-items:stretch;
}
.hero h1{font-size:44px;line-height:1.15;margin:12px 0 0;letter-spacing:-.3px}
.hero p{color:var(--muted);margin:14px 0 18px;font-size:16px}
.hero .actions{display:flex;gap:12px;flex-wrap:wrap}
.hero-art{
  background:linear-gradient(135deg,#e0f2fe,#eef2ff 55%,#fef3c7);
  border-radius:var(--radius);
  border:1px solid var(--border);
  box-shadow:var(--shadow);
  padding:22px;
  display:flex;flex-direction:column;justify-content:space-between;
}

.kpis{display:grid;grid-template-columns:repeat(4, minmax(0,1fr));gap:14px}
.kpi{background:#f8fafc;border:1px solid var(--border);border-radius:16px;padding:16px;text-align:center}
.kpi strong{display:block;font-size:18px}
.kpi span{color:var(--muted);font-size:13px}

.products{grid-template-columns:repeat(3,minmax(0,1fr))}
.product{border:1px solid var(--border);border-radius:18px;padding:18px;background:#fff;box-shadow:0 8px 26px rgba(15,23,42,.06)}
.product h3{margin:12px 0 6px}
.product p{margin:0;color:var(--muted)}
.tag{display:inline-flex;align-items:center;gap:8px;padding:6px 10px;border-radius:999px;background:#f1f5f9;border:1px solid var(--border);font-size:13px;font-weight:800;color:#0f172a}

form{display:grid;gap:12px}
label{font-size:14px;color:var(--muted);font-weight:800}
input,textarea,select{
  width:100%;padding:12px 12px;border-radius:14px;border:1px solid var(--border);
  background:#fff;color:var(--text);outline:none;
}
input:focus,textarea:focus,select:focus{border-color:rgba(99,102,241,.50);box-shadow:0 0 0 4px rgba(99,102,241,.12)}
textarea{min-height:140px;resize:vertical}
.two{display:grid;grid-template-columns:1fr 1fr;gap:12px}

.notice{border:1px dashed rgba(15,23,42,.20);background:#f8fafc;border-radius:16px;padding:12px 14px;color:var(--muted)}

.footer{border-top:1px solid var(--border);background:#fff;padding:34px 0}
.footer .row{display:flex;align-items:flex-start;justify-content:space-between;gap:18px;flex-wrap:wrap}
.small{font-size:13px;color:var(--muted)}

.toast{
  position:fixed;bottom:18px;left:18px;background:#fff;border:1px solid var(--border);
  border-radius:16px;padding:12px 14px;box-shadow:var(--shadow);
  min-width:240px;display:none;
}
.toast.show{display:block}

@media (max-width: 960px){
  .hero{grid-template-columns:1fr}
  .kpis{grid-template-columns:repeat(2,minmax(0,1fr))}
  .products{grid-template-columns:repeat(2,minmax(0,1fr))}
}
@media (max-width: 680px){
  .menu-btn{display:inline-flex}
  .links{display:none;width:100%;flex-direction:column;align-items:stretch;padding:10px 0 0}
  .links.open{display:flex}
  .two{grid-template-columns:1fr}
  .products{grid-template-columns:1fr}
  .hero h1{font-size:36px}
