---
layout: single
title: Book Log
---
<style>
  :root{
    --bg:#0f1724; --card:#0b1220; --muted:#9aa4b2; --accent:#60a5fa; --glass: rgba(255,255,255,0.03);
    --card-radius:12px;
  }
  html,body{height:100%;margin:0;font-family:Inter,ui-sans-serif,system-ui,-apple-system,"Segoe UI",Roboto,"Helvetica Neue",Arial;color:#e6eef6;background:linear-gradient(180deg,#071029 0%, #071827 100%);-webkit-font-smoothing:antialiased}
  .container{max-width:980px;margin:36px auto;padding:20px}
  .heading{display:flex;align-items:center;gap:12px;margin-bottom:18px}
  .title{font-size:20px;font-weight:700}
  .subtitle{color:var(--muted);font-size:13px}
  /* Tabs */
  .tabs{background:var(--glass);padding:6px;border-radius:999px;display:flex;gap:6px;align-items:center;margin-bottom:18px}
  .tab{border:0;padding:8px 14px;border-radius:999px;background:transparent;color:var(--muted);cursor:pointer;font-weight:600}
  .tab[aria-selected="true"]{background:linear-gradient(90deg, rgba(96,165,250,0.18), rgba(96,165,250,0.08));color:var(--accent);box-shadow:0 6px 18px rgba(9,14,23,0.6) inset}
  /* Panels */
  .panel{display:none;padding-top:6px}
  .panel[data-visible="true"]{display:block}
  /* Card/list */
  .card{background:linear-gradient(180deg, rgba(255,255,255,0.02), rgba(255,255,255,0.01));border-radius:var(--card-radius);padding:12px;border:1px solid rgba(255,255,255,0.03);margin-bottom:10px}
  .item{display:flex;align-items:flex-start;gap:12px;cursor:pointer;padding:8px;border-radius:10px}
  .item:focus,.item:hover{outline:none;background:linear-gradient(90deg, rgba(96,165,250,0.03), transparent)}
  .item-head{flex:1;display:flex;flex-direction:column;gap:6px}
  .meta{display:flex;align-items:center;gap:10px;font-size:13px;color:var(--muted)}
  .title-line{display:flex;align-items:center;gap:8px}
  .item-title{font-weight:700;color:#e6f3ff}
  .date{font-size:12px;color:var(--muted)}
  /* rating stars */
  .stars{display:inline-block;position:relative;font-size:14px;line-height:1}
  .stars .empty{color:#1f2a3a}
  .stars .filled{position:absolute;left:0;top:0;overflow:hidden;white-space:nowrap;color:#ffd05a}
  /* expand content */
  .detail{padding:10px 12px;border-left:3px solid rgba(96,165,250,0.06);margin-top:8px;background:rgba(255,255,255,0.01);border-radius:8px;display:none}
  .detail.show{display:block}
  .small{font-size:12px;color:var(--muted)}
  /* helper */
  .hint{font-size:12px;color:var(--muted);margin-top:6px}
  /* responsive */
  @media (max-width:640px){
    .container{padding:12px}
    .title{font-size:18px}
  }
</style>
<hr>
