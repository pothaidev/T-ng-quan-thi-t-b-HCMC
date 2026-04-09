<!DOCTYPE html>
<html lang="vi">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width,initial-scale=1.0">
<title>Pepsi HCM – Equipment Tracking Dashboard Q1/2026</title>
<script src="https://cdnjs.cloudflare.com/ajax/libs/Chart.js/4.4.1/chart.umd.js"></script>
<link href="https://fonts.googleapis.com/css2?family=Sora:wght@300;400;500;600;700&family=IBM+Plex+Mono:wght@400;500&display=swap" rel="stylesheet">
<style>
*,*::before,*::after{box-sizing:border-box;margin:0;padding:0}
:root{
  --pepsi-blue:#004B93;--pepsi-red:#ED1C24;--pepsi-light:#EEF4FF;
  --teal:#00B2A0;--teal-l:#E0F7F5;
  --green:#16a34a;--green-l:#dcfce7;
  --red:#dc2626;--red-l:#fee2e2;
  --orange:#ea580c;--orange-l:#ffedd5;
  --amber:#d97706;--amber-l:#fef3c7;
  --gray:#64748b;--gray-l:#f8fafc;
  --border:#e2e8f0;--text:#0f172a;--muted:#94a3b8;
  --white:#ffffff;--shadow:0 1px 8px rgba(0,0,0,.08);--r:10px
}
body{font-family:'Sora',sans-serif;background:#f1f5f9;color:var(--text);font-size:13px;min-height:100vh}

/* HEADER */
.hdr{background:var(--pepsi-blue);padding:0 24px;height:56px;display:flex;align-items:center;justify-content:space-between;position:sticky;top:0;z-index:200;box-shadow:0 2px 12px rgba(0,75,147,.3)}
.hdr-brand{display:flex;align-items:center;gap:12px}
.brand-badge{background:var(--pepsi-red);color:#fff;font-weight:700;font-size:12px;padding:4px 10px;border-radius:6px;letter-spacing:1px}
.hdr-title{color:#fff;font-weight:600;font-size:14px;opacity:.95}
.hdr-meta{color:rgba(255,255,255,.7);font-size:11px;margin-top:2px}
.hdr-right{display:flex;align-items:center;gap:10px}
.ctrl{display:flex;align-items:center;gap:6px;background:rgba(255,255,255,.12);border:1px solid rgba(255,255,255,.2);border-radius:8px;padding:5px 10px;cursor:pointer;transition:.2s}
.ctrl:hover{background:rgba(255,255,255,.2)}
.ctrl label{color:rgba(255,255,255,.6);font-size:10px;cursor:pointer}
.ctrl select{background:transparent;border:none;color:#fff;font-family:'Sora',sans-serif;font-size:12px;font-weight:600;cursor:pointer;outline:none}
.ctrl select option{background:var(--pepsi-blue);color:#fff}
.live-badge{background:var(--teal);color:#fff;padding:4px 12px;border-radius:20px;font-size:11px;font-weight:600;display:flex;align-items:center;gap:5px}
.live-dot{width:6px;height:6px;border-radius:50%;background:#fff;animation:blink 1.5s infinite}
@keyframes blink{0%,100%{opacity:1}50%{opacity:.3}}

/* LAYOUT */
.page{padding:16px 20px 28px}
.row{display:grid;gap:12px;margin-bottom:12px}
.r5{grid-template-columns:repeat(5,1fr)}
.r4{grid-template-columns:repeat(4,1fr)}
.r3{grid-template-columns:repeat(3,1fr)}
.r2{grid-template-columns:1fr 1fr}
.r-7-5{grid-template-columns:7fr 5fr}
.r-6-4{grid-template-columns:6fr 4fr}
.r-4-3-3{grid-template-columns:4fr 3fr 3fr}

/* CARDS */
.card{background:#fff;border-radius:var(--r);box-shadow:var(--shadow);padding:14px 16px;position:relative;overflow:hidden;transition:box-shadow .2s}
.card:hover{box-shadow:0 4px 20px rgba(0,0,0,.12)}
.card-accent{position:absolute;top:0;left:0;right:0;height:3px}
.card-accent.teal{background:linear-gradient(90deg,var(--teal),#00e5d4)}
.card-accent.blue{background:linear-gradient(90deg,var(--pepsi-blue),#3b82f6)}
.card-accent.red{background:linear-gradient(90deg,var(--red),var(--orange))}
.card-accent.green{background:linear-gradient(90deg,var(--green),#84cc16)}
.card-accent.amber{background:linear-gradient(90deg,var(--amber),var(--orange))}
.card-accent.gray{background:linear-gradient(90deg,var(--gray),#cbd5e1)}

.ctitle{font-size:10px;font-weight:600;color:var(--muted);text-transform:uppercase;letter-spacing:.6px;margin-bottom:5px}
.cvalue{font-family:'IBM Plex Mono',monospace;font-size:28px;font-weight:500;color:var(--text);line-height:1.1;margin-bottom:8px}
.cvalue.sm{font-size:20px}
.cvalue.xs{font-size:16px}
.cmeta{display:flex;flex-direction:column;gap:3px}
.cmrow{display:flex;justify-content:space-between;align-items:center;font-size:11px}
.cml{color:var(--muted)}
.cup{color:var(--green);font-weight:600}
.cdn{color:var(--red);font-weight:600}
.camt{color:var(--amber);font-weight:600}

/* Section label */
.sec{font-size:10px;font-weight:600;color:var(--gray);text-transform:uppercase;letter-spacing:1px;margin-bottom:8px;display:flex;align-items:center;gap:8px}
.sec::after{content:'';flex:1;height:.5px;background:var(--border)}

/* Charts */
.ctitle-chart{font-size:12px;font-weight:600;color:var(--text);margin-bottom:8px;text-align:center}
.cw{position:relative;width:100%}

/* Legend */
.legend{display:flex;flex-wrap:wrap;gap:8px;margin-bottom:6px}
.li{display:flex;align-items:center;gap:4px;font-size:10px;color:var(--muted)}
.ld{width:10px;height:10px;border-radius:2px;flex-shrink:0}

/* Table */
table{width:100%;border-collapse:collapse;font-size:11px}
th{text-align:left;padding:6px 8px;font-size:10px;font-weight:600;color:var(--muted);text-transform:uppercase;letter-spacing:.4px;border-bottom:1px solid var(--border)}
th:not(:first-child){text-align:right}
td{padding:6px 8px;border-bottom:.5px solid var(--border);vertical-align:middle}
td:not(:first-child){text-align:right}
tr:last-child td{border-bottom:none}
tr:hover td{background:var(--gray-l)}
.tb{font-weight:600}
.tup{color:var(--green);font-weight:600}
.tdn{color:var(--red);font-weight:600}
.tag{display:inline-block;font-size:9px;padding:1px 5px;border-radius:3px;font-weight:600}
.tag-g{background:var(--green-l);color:var(--green)}
.tag-r{background:var(--red-l);color:var(--red)}
.tag-a{background:var(--amber-l);color:var(--amber)}
.tag-b{background:var(--pepsi-light);color:var(--pepsi-blue)}

/* Progress bar */
.pb-wrap{display:flex;align-items:center;gap:6px}
.pb-bg{flex:1;height:5px;background:var(--border);border-radius:3px;overflow:hidden;min-width:50px}
.pb-fill{height:100%;border-radius:3px;transition:width .6s ease}
.pb-val{font-size:10px;min-width:34px;text-align:right}

/* Issue pills */
.issue-grid{display:grid;grid-template-columns:repeat(5,1fr);gap:6px;margin-top:8px}
.issue-pill{text-align:center;padding:8px 4px;border-radius:8px;cursor:default}
.ip-val{font-family:'IBM Plex Mono',monospace;font-size:18px;font-weight:500}
.ip-lbl{font-size:9px;color:var(--muted);margin-top:2px}

/* CCC pills */
.ccc-row{display:flex;align-items:center;justify-content:center;gap:6px;margin-bottom:10px;flex-wrap:wrap}
.cpill{padding:4px 10px;border-radius:20px;font-size:12px;font-weight:600;display:flex;align-items:center;gap:4px}
.pill-op{font-size:16px;font-weight:700;color:var(--muted)}

/* Filter tabs */
.tabs{display:flex;gap:4px;margin-bottom:10px}
.tab{padding:4px 12px;border-radius:6px;font-size:11px;font-weight:500;cursor:pointer;border:1px solid var(--border);background:transparent;color:var(--muted);transition:.15s}
.tab.on{background:var(--pepsi-blue);color:#fff;border-color:var(--pepsi-blue)}
.tab:hover:not(.on){background:var(--gray-l)}

/* ASM filter */
.filter-row{display:flex;align-items:center;gap:8px;margin-bottom:10px;flex-wrap:wrap}
.filter-row label{font-size:11px;color:var(--muted)}
.filter-row select{font-family:'Sora',sans-serif;font-size:11px;padding:4px 8px;border:1px solid var(--border);border-radius:6px;background:#fff;color:var(--text);outline:none;cursor:pointer}
.filter-row select:focus{border-color:var(--pepsi-blue)}

@media(max-width:1300px){
  .r5{grid-template-columns:repeat(3,1fr)}
  .r-7-5,.r-6-4,.r-4-3-3{grid-template-columns:1fr}
}
</style>
</head>
<body>

<!-- HEADER -->
<div class="hdr">
  <div class="hdr-brand">
    <div class="brand-badge">PEPSI</div>
    <div>
      <div class="hdr-title">Equipment Tracking Dashboard – TP. Hồ Chí Minh</div>
      <div class="hdr-meta">Quý 1 / 2026 &nbsp;·&nbsp; Cập nhật: 31/03/2026 &nbsp;·&nbsp; 21.894 thiết bị</div>
    </div>
  </div>
  <div class="hdr-right">
    <div class="ctrl">
      <label>Xem theo</label>
      <select id="view-sel" onchange="applyFilter()">
        <option value="all">Toàn thị trường</option>
        <option value="HCMC1">HCMC1 – N.V. Phương</option>
        <option value="HCMC2">HCMC2 – B.P.G. Hưng</option>
        <option value="HCMC3">HCMC3 – V.Q. Tuấn</option>
        <option value="HCMC4">HCMC4 – N.V. Khương</option>
        <option value="HCMC5">HCMC5 – Đ.V. Hiếu</option>
        <option value="HCMC6">HCMC6 – P.M. Lý</option>
        <option value="HCMC7">HCMC7 – N.V. Hải</option>
        <option value="AFHM1">AFHM1 – N.V. Nhân</option>
        <option value="AFHM2">AFHM2 – L.T.T. Nguyên</option>
        <option value="MTM">MTM – P.T. Tùng</option>
        <option value="WS">WS – N.T. Thành</option>
      </select>
    </div>
    <div class="live-badge"><div class="live-dot"></div>Q1/2026</div>
  </div>
</div>

<div class="page">

<!-- ROW 1: 5 KPI Cards -->
<div class="sec">Tổng quan thị trường</div>
<div class="row r5" id="kpi-row">
  <div class="card" id="c-total"><div class="card-accent blue"></div>
    <div class="ctitle">Tổng thiết bị</div>
    <div class="cvalue" id="v-total">21.894</div>
    <div class="cmeta">
      <div class="cmrow"><span class="cml">QR tháng</span><span class="cup" id="v-qrt">19.022</span></div>
      <div class="cmrow"><span class="cml">QR quý</span><span class="cup" id="v-qrq">2.872</span></div>
    </div>
  </div>
  <div class="card" id="c-aso"><div class="card-accent teal"></div>
    <div class="ctitle">ASO có tủ</div>
    <div class="cvalue" id="v-aso">19.870</div>
    <div class="cmeta">
      <div class="cmrow"><span class="cml">Thu hồi T3</span><span class="cdn">372 YC</span></div>
      <div class="cmrow"><span class="cml">Lắp mới T3</span><span class="cup">467 YC</span></div>
    </div>
  </div>
  <div class="card" id="c-qr"><div class="card-accent green"></div>
    <div class="ctitle">Hoàn thành QR</div>
    <div class="cvalue" id="v-qr">21.894</div>
    <div class="cmeta">
      <div class="cmrow"><span class="cml">Tỷ lệ</span><span class="cup" id="v-pqr">100%</span></div>
      <div class="cmrow"><span class="cml">Chưa HT</span><span class="cdn" id="v-nqr">0</span></div>
    </div>
  </div>
  <div class="card" id="c-issue"><div class="card-accent red"></div>
    <div class="ctitle">Trạng thái đặc biệt</div>
    <div class="cvalue" id="v-issue">685</div>
    <div class="cmeta">
      <div class="cmrow"><span class="cml">ARR+ETR+VERIFY</span><span class="camt">656</span></div>
      <div class="cmrow"><span class="cml">Unidentify</span><span class="cdn">23</span></div>
    </div>
  </div>
  <div class="card" id="c-net"><div class="card-accent amber"></div>
    <div class="ctitle">ASO Net Addition Q1</div>
    <div class="cvalue" id="v-net">+267</div>
    <div class="cmeta">
      <div class="cmrow"><span class="cml">AOP 2026</span><span class="cml" id="v-aop">1.835</span></div>
      <div class="cmrow"><span class="cml">% vs AOP</span><span class="camt" id="v-paop">14.5%</span></div>
    </div>
  </div>
</div>

<!-- ROW 2: Vol + Issues -->
<div class="row r2" style="margin-bottom:12px">
  <!-- Vol -->
  <div class="card">
    <div class="card-accent green"></div>
    <div class="ctitle-chart">Doanh số Vol (TT & AFH) – T1 → T2 → T3</div>
    <div class="row r3" style="gap:8px;margin-bottom:10px">
      <div style="text-align:center">
        <div style="font-size:10px;color:var(--muted)">Vol T1</div>
        <div style="font-family:'IBM Plex Mono',monospace;font-size:18px;font-weight:500" id="vv1">1.658.117</div>
      </div>
      <div style="text-align:center">
        <div style="font-size:10px;color:var(--muted)">Vol T2</div>
        <div style="font-family:'IBM Plex Mono',monospace;font-size:18px;font-weight:500;color:var(--red)" id="vv2">1.246.113</div>
        <div style="font-size:9px;color:var(--red)">-24.8% vs T1</div>
      </div>
      <div style="text-align:center">
        <div style="font-size:10px;color:var(--muted)">Vol T3</div>
        <div style="font-family:'IBM Plex Mono',monospace;font-size:18px;font-weight:500;color:var(--green)" id="vv3">1.705.613</div>
        <div style="font-size:9px;color:var(--green)">+36.9% vs T2</div>
      </div>
    </div>
    <div class="cw" style="height:160px"><canvas id="volChart" aria-label="Vol chart"></canvas></div>
  </div>

  <!-- Issues breakdown -->
  <div class="card">
    <div class="card-accent red"></div>
    <div class="ctitle-chart">Phân loại trạng thái thiết bị</div>
    <div class="issue-grid">
      <div class="issue-pill" style="background:#fee2e2">
        <div class="ip-val" style="color:var(--red)">347</div>
        <div class="ip-lbl">ARR<br>Thu hồi</div>
      </div>
      <div class="issue-pill" style="background:#fef3c7">
        <div class="ip-val" style="color:var(--amber)">253</div>
        <div class="ip-lbl">VERIFY<br>Đóng cửa</div>
      </div>
      <div class="issue-pill" style="background:#ffedd5">
        <div class="ip-val" style="color:var(--orange)">56</div>
        <div class="ip-lbl">ETR<br>Di dời</div>
      </div>
      <div class="issue-pill" style="background:#ede9fe">
        <div class="ip-val" style="color:#7c3aed">23</div>
        <div class="ip-lbl">UNI<br>Thất lạc</div>
      </div>
      <div class="issue-pill" style="background:#fce7f3">
        <div class="ip-val" style="color:#be185d">6</div>
        <div class="ip-lbl">LEGAL<br>Pháp lý</div>
      </div>
    </div>
    <div class="cw" style="height:110px;margin-top:10px"><canvas id="issueDonut" aria-label="Issues donut"></canvas></div>
  </div>
</div>

<!-- ROW 3: QR timing + Net Addition -->
<div class="row r2" style="margin-bottom:12px">
  <!-- QR Timing -->
  <div class="card">
    <div class="card-accent teal"></div>
    <div class="ctitle-chart">Phân bổ tuần hoàn tất QR tháng – T3/2026</div>
    <div class="legend">
      <div class="li"><div class="ld" style="background:#16a34a"></div>Tuần 1 (1–7/3)</div>
      <div class="li"><div class="ld" style="background:#84cc16"></div>Tuần 2 (8–14/3)</div>
      <div class="li"><div class="ld" style="background:#f59e0b"></div>Tuần 3 (15–21/3)</div>
      <div class="li"><div class="ld" style="background:#ea580c"></div>Tuần 4 (22–27/3)</div>
      <div class="li"><div class="ld" style="background:#94a3b8"></div>Chưa HT</div>
    </div>
    <div class="cw" style="height:170px"><canvas id="timingChart" aria-label="QR timing chart"></canvas></div>
  </div>

  <!-- Net Addition -->
  <div class="card">
    <div class="card-accent amber"></div>
    <div class="ctitle-chart">Net Addition Q1 vs AOP 2026 – Lắp mới theo tháng</div>
    <div class="legend">
      <div class="li"><div class="ld" style="background:#004B93"></div>Tháng 1</div>
      <div class="li"><div class="ld" style="background:#f59e0b"></div>Tháng 2</div>
      <div class="li"><div class="ld" style="background:#16a34a"></div>Tháng 3</div>
      <div class="li"><div class="ld" style="background:#dc2626"></div>Net Add Q1 (âm=đỏ)</div>
    </div>
    <div class="cw" style="height:170px"><canvas id="netChart" aria-label="Net addition chart"></canvas></div>
  </div>
</div>

<!-- ROW 4: ASM Table + VPO -->
<div class="row r-6-4" style="margin-bottom:12px">
  <!-- ASM Full table -->
  <div class="card">
    <div class="card-accent blue"></div>
    <div style="display:flex;justify-content:space-between;align-items:center;margin-bottom:10px">
      <div class="ctitle-chart" style="margin:0">Hiệu suất theo ASM / Manager</div>
      <div class="filter-row" style="margin:0">
        <label>Sắp xếp:</label>
        <select id="asm-sort" onchange="renderASMTable()">
          <option value="total">Tổng tủ</option>
          <option value="pct">% QR</option>
          <option value="issues">Issues</option>
          <option value="v3">Vol T3</option>
        </select>
      </div>
    </div>
    <table id="asm-table">
      <thead>
        <tr>
          <th>ASM</th>
          <th>Tổng tủ</th>
          <th>% QR</th>
          <th>Chưa HT</th>
          <th>Issues</th>
          <th>Vol T3</th>
          <th>% Có DS</th>
        </tr>
      </thead>
      <tbody id="asm-tbody"></tbody>
    </table>
  </div>

  <!-- VPO=0 -->
  <div class="card">
    <div class="card-accent orange"></div>
    <div class="ctitle-chart">Xử lý tủ 0DS T2 (VPO=0)</div>
    <div style="display:flex;gap:16px;margin-bottom:10px">
      <div style="text-align:center">
        <div style="font-size:10px;color:var(--muted)">Cần xử lý</div>
        <div style="font-family:'IBM Plex Mono',monospace;font-size:20px;font-weight:500;color:var(--orange)">591</div>
      </div>
      <div style="text-align:center">
        <div style="font-size:10px;color:var(--muted)">Đã xử lý</div>
        <div style="font-family:'IBM Plex Mono',monospace;font-size:20px;font-weight:500;color:var(--green)">507</div>
      </div>
      <div style="text-align:center">
        <div style="font-size:10px;color:var(--muted)">Còn lại</div>
        <div style="font-family:'IBM Plex Mono',monospace;font-size:20px;font-weight:500;color:var(--red)">84</div>
      </div>
      <div style="text-align:center">
        <div style="font-size:10px;color:var(--muted)">Tỷ lệ XL</div>
        <div style="font-family:'IBM Plex Mono',monospace;font-size:20px;font-weight:500;color:var(--pepsi-blue)">85.8%</div>
      </div>
    </div>
    <table id="vpo-table">
      <thead>
        <tr><th>ASM</th><th>Tổng 0DS</th><th>% XL</th><th>Còn lại</th></tr>
      </thead>
      <tbody id="vpo-tbody"></tbody>
    </table>
  </div>
</div>

<!-- ROW 5: ASO Penetration + SS worst -->
<div class="row r2" style="margin-bottom:12px">
  <!-- ASO Penetration doughnut -->
  <div class="card">
    <div class="card-accent blue"></div>
    <div class="ctitle-chart">ASO Penetration & Net Addition Q1 vs AOP</div>
    <div class="cw" style="height:220px"><canvas id="peneChart" aria-label="Penetration chart"></canvas></div>
  </div>

  <!-- SS worst QR -->
  <div class="card">
    <div class="card-accent red"></div>
    <div style="display:flex;justify-content:space-between;align-items:center;margin-bottom:8px">
      <div class="ctitle-chart" style="margin:0">SS hoàn tất QR trễ nhất (Tuần 4 / chưa HT)</div>
    </div>
    <table id="ss-table">
      <thead>
        <tr><th>SS / AFHE</th><th>ASM</th><th>Tổng tủ</th><th>% QR</th><th>Tủ action trễ</th></tr>
      </thead>
      <tbody id="ss-tbody"></tbody>
    </table>
  </div>
</div>

<!-- ROW 6: Thu hoi + Lap dat -->
<div class="row r2">
  <div class="card">
    <div class="card-accent red"></div>
    <div class="ctitle-chart">Thu hồi T3 – Phân loại (372 yêu cầu)</div>
    <div class="cw" style="height:200px"><canvas id="thChart" aria-label="Thu hoi chart"></canvas></div>
  </div>
  <div class="card">
    <div class="card-accent green"></div>
    <div class="ctitle-chart">Lắp đặt T3 – Phân loại (467 yêu cầu)</div>
    <div class="cw" style="height:200px"><canvas id="ldChart" aria-label="Lap dat chart"></canvas></div>
  </div>
</div>

</div>

<script>
// ══════════════════════════════════════════════════
// DATA
// ══════════════════════════════════════════════════
const ASM_DATA = [
  {name:'HCMC4',full:'HCMC4 – N.V. Khương',   total:3654,aso:3562,report:3654,pct:100.0,arr:46, etrl:0,verify:27,uni:6, etr:14,issues:93, v1:217626,v2:172530,v3:218857,hv3:3617},
  {name:'HCMC2',full:'HCMC2 – B.P.G. Hưng',   total:2924,aso:2756,report:2924,pct:100.0,arr:26, etrl:0,verify:21,uni:3, etr:12,issues:62, v1:170126,v2:121263,v3:154469,hv3:2879},
  {name:'HCMC6',full:'HCMC6 – P.M. Lý',        total:2732,aso:2584,report:2732,pct:100.0,arr:34, etrl:3,verify:52,uni:3, etr:8, issues:100,v1:161250,v2:122303,v3:148914,hv3:2679},
  {name:'HCMC5',full:'HCMC5 – Đ.V. Hiếu',      total:2698,aso:2581,report:2698,pct:100.0,arr:52, etrl:1,verify:6, uni:4, etr:6, issues:69, v1:173950,v2:128336,v3:160623,hv3:2681},
  {name:'HCMC3',full:'HCMC3 – V.Q. Tuấn',      total:2507,aso:2363,report:2507,pct:100.0,arr:35, etrl:0,verify:17,uni:1, etr:5, issues:58, v1:164222,v2:112487,v3:147470,hv3:2474},
  {name:'HCMC7',full:'HCMC7 – N.V. Hải',       total:2135,aso:2065,report:2135,pct:100.0,arr:54, etrl:0,verify:39,uni:2, etr:5, issues:100,v1:0,     v2:0,     v3:143025,hv3:2087},
  {name:'HCMC1',full:'HCMC1 – N.V. Phương',    total:1858,aso:1753,report:1858,pct:100.0,arr:26, etrl:1,verify:13,uni:3, etr:2, issues:45, v1:118109,v2:85112, v3:112680,hv3:1821},
  {name:'AFHM2',full:'AFHM2 – L.T.T. Nguyên',  total:1243,aso:534, report:1243,pct:100.0,arr:33, etrl:0,verify:76,uni:0, etr:3, issues:112,v1:148422,v2:174946,v3:151056,hv3:254},
  {name:'AFHM1',full:'AFHM1 – N.V. Nhân',      total:939, aso:473, report:939, pct:100.0,arr:16, etrl:1,verify:2, uni:0, etr:0, issues:19, v1:10769, v2:8021,  v3:16866, hv3:76},
  {name:'MTM',  full:'MTM – P.T. Tùng',         total:654, aso:649, report:654, pct:100.0,arr:9,  etrl:0,verify:0, uni:0, etr:1, issues:10, v1:0,     v2:0,     v3:0,     hv3:0},
  {name:'WS',   full:'WS – N.T. Thành',         total:550, aso:550, report:550, pct:100.0,arr:16, etrl:0,verify:0, uni:1, etr:0, issues:17, v1:493642,v2:321114,v3:451653,hv3:547},
];

const NET_DATA = [
  {ASM:'AFHM2 – L.T.T. Nguyên',  AOP:205, Q1:-6,   pAOP:-2.9,  pene:19.2, jan:13, feb:7,  mar:4,  vc_total:24},
  {ASM:'AFHM1 – N.V. Nhân',      AOP:189, Q1:33,   pAOP:17.5,  pene:10.6, jan:40, feb:17, mar:29, vc_total:86},
  {ASM:'HCMC1 – N.V. Phương',    AOP:175, Q1:83,   pAOP:47.5,  pene:25.0, jan:32, feb:9,  mar:34, vc_total:75},
  {ASM:'HCMC2 – B.P.G. Hưng',    AOP:251, Q1:-151, pAOP:-60.3, pene:30.2, jan:45, feb:10, mar:35, vc_total:90},
  {ASM:'HCMC3 – V.Q. Tuấn',      AOP:219, Q1:26,   pAOP:11.9,  pene:28.8, jan:27, feb:16, mar:40, vc_total:83},
  {ASM:'HCMC4 – N.V. Khương',    AOP:220, Q1:50,   pAOP:22.7,  pene:34.2, jan:56, feb:22, mar:42, vc_total:120},
  {ASM:'HCMC5 – Đ.V. Hiếu',      AOP:200, Q1:48,   pAOP:24.0,  pene:25.1, jan:69, feb:27, mar:40, vc_total:136},
  {ASM:'HCMC6 – P.M. Lý',        AOP:174, Q1:129,  pAOP:74.0,  pene:26.5, jan:29, feb:13, mar:26, vc_total:68},
  {ASM:'HCMC7 – N.V. Hải',       AOP:202, Q1:50,   pAOP:24.7,  pene:27.7, jan:25, feb:24, mar:64, vc_total:113},
  {ASM:'WS – N.T. Thành',        AOP:0,   Q1:5,    pAOP:null,  pene:36.3, jan:1,  feb:0,  mar:5,  vc_total:6},
];

const VPO_DATA = [
  {ASM:'HCMC7 – N.V. Hải',       total:154, done:140, rate:90.9, remain:14},
  {ASM:'HCMC3 – V.Q. Tuấn',      total:124, done:108, rate:87.1, remain:16},
  {ASM:'HCMC2 – B.P.G. Hưng',    total:83,  done:65,  rate:78.3, remain:18},
  {ASM:'HCMC6 – P.M. Lý',        total:66,  done:51,  rate:77.3, remain:15},
  {ASM:'HCMC1 – N.V. Phương',    total:63,  done:54,  rate:85.7, remain:9},
  {ASM:'HCMC5 – Đ.V. Hiếu',      total:44,  done:41,  rate:93.2, remain:3},
  {ASM:'HCMC4 – N.V. Khương',    total:35,  done:30,  rate:85.7, remain:5},
  {ASM:'AFHM1 – N.V. Nhân',      total:15,  done:11,  rate:73.3, remain:4},
  {ASM:'AFHM2 – L.T.T. Nguyên',  total:7,   done:7,   rate:100,  remain:0},
];

const SS_WORST = [
  {ss:'SS-Nguyễn Văn Xô',         asm:'HCMC6', total:418, pct:100.0, uni:0, note:'27 tủ W4'},
  {ss:'SS-Võ Văn Quang',          asm:'HCMC4', total:641, pct:100.0, uni:3, note:'20 tủ W4'},
  {ss:'SS-Trần Đắc Hưng',         asm:'HCMC4', total:412, pct:100.0, uni:0, note:'18 tủ W4'},
  {ss:'SS-Hoàng Trọng Toản',      asm:'HCMC2', total:411, pct:100.0, uni:0, note:'17 tủ W4'},
  {ss:'SS-Nguyễn Văn Hoàng',      asm:'HCMC7', total:221, pct:100.0, uni:0, note:'11 tủ W4'},
  {ss:'SS-Huỳnh Bá Phương',       asm:'HCMC1', total:194, pct:100.0, uni:0, note:'11 tủ W4'},
  {ss:'Lê Công Hiền',             asm:'AFHM2', total:142, pct:100.0, uni:0, note:'125 tủ W4'},
  {ss:'Lê Trần Diệu Tâm',         asm:'AFHM2', total:231, pct:100.0, uni:0, note:'141 tủ W4'},
  {ss:'Vũ Hoàng Ngân',            asm:'AFHM2', total:107, pct:100.0, uni:0, note:'36 tủ W4'},
  {ss:'SS-Văn Vũ Bảo',            asm:'HCMC1', total:609, pct:100.0, uni:0, note:'6 tủ W4'},
];

const TIMING_T = {W1:15319,W2:2521,W3:687,W4:256,'Chưa HT':97};
const TH_CAT = {
  'ON Thu hồi tài sản':150,
  'OFF Thu hồi tài sản':73,
  'Thu hồi tủ lạnh':52,
  'ON Thu hồi thay thế':38,
  'OFF Thu hồi thay thế':29,
  'Khác (TH thay thế, non sale, route)':30,
};
const LD_CAT = {
  'OFF Lắp đặt tài sản':141,
  'ON Lắp đặt tài sản':135,
  'AFH Lắp đặt tủ lạnh':38,
  'ON Lắp đặt thay thế':37,
  'Lắp đặt tạm thời':35,
  'OFF Lắp đặt thay thế':29,
  'Khác (PMX, ngoài CL)':52,
};

// ══════════════════════════════════════════════════
// CHARTS
// ══════════════════════════════════════════════════
let charts = {};
function destroyChart(id){ if(charts[id]){charts[id].destroy();delete charts[id];} }

const GRID_OPTS = { color:'rgba(0,0,0,.04)' };
const TICK_OPTS = { font:{size:10}, color:'#94a3b8' };

function mkBar(id, labels, datasets, opts={}){
  destroyChart(id);
  charts[id] = new Chart(document.getElementById(id), {
    type:'bar',
    data:{ labels, datasets },
    options:{
      responsive:true, maintainAspectRatio:false,
      plugins:{ legend:{ display:false }, tooltip:{ mode:'index', intersect:false }, ...opts.plugins },
      scales:{
        x:{ grid:{ display:false }, ticks:TICK_OPTS },
        y:{ grid:GRID_OPTS, ticks:TICK_OPTS },
        ...(opts.scales||{})
      },
      ...opts
    }
  });
}

// Vol chart
function buildVolChart(data){
  destroyChart('vol');
  const labels = data.map(d=>d.name);
  charts['vol'] = new Chart(document.getElementById('volChart'),{
    type:'bar',
    data:{labels, datasets:[
      {label:'Vol T1',data:data.map(d=>d.v1),backgroundColor:'rgba(59,130,246,.6)',borderRadius:3,stack:'s'},
      {label:'Vol T3',data:data.map(d=>d.v3),backgroundColor:'rgba(22,163,74,.7)',borderRadius:3,stack:'s2'},
    ]},
    options:{responsive:true,maintainAspectRatio:false,
      plugins:{legend:{display:false},tooltip:{mode:'index',intersect:false}},
      scales:{x:{grid:{display:false},ticks:{font:{size:9},color:'#94a3b8'}},y:{grid:GRID_OPTS,ticks:TICK_OPTS}}}
  });
}

// Issue donut
function buildIssueDonut(){
  destroyChart('iss');
  charts['iss'] = new Chart(document.getElementById('issueDonut'),{
    type:'doughnut',
    data:{
      labels:['ARR','VERIFY','ETR','UNI','LEGAL'],
      datasets:[{data:[347,253,56,23,6],
        backgroundColor:['#dc2626','#f59e0b','#ea580c','#7c3aed','#be185d'],
        borderColor:'#fff',borderWidth:2,hoverOffset:6}]
    },
    options:{responsive:true,maintainAspectRatio:false,cutout:'65%',
      plugins:{legend:{display:false},tooltip:{callbacks:{label:ctx=>`${ctx.label}: ${ctx.parsed}`}}}}
  });
}

// QR Timing
function buildTimingChart(){
  destroyChart('tim');
  const tot = Object.values(TIMING_T).reduce((a,b)=>a+b,0);
  charts['tim'] = new Chart(document.getElementById('timingChart'),{
    type:'bar',
    data:{
      labels:['Tuần 1\n(1–7/3)','Tuần 2\n(8–14/3)','Tuần 3\n(15–21/3)','Tuần 4\n(22–27/3)','Chưa HT'],
      datasets:[{
        data:Object.values(TIMING_T),
        backgroundColor:['#16a34a','#84cc16','#f59e0b','#ea580c','#94a3b8'],
        borderRadius:6, borderSkipped:false,
      }]
    },
    options:{responsive:true,maintainAspectRatio:false,
      plugins:{legend:{display:false},tooltip:{callbacks:{label:ctx=>`${ctx.parsed.y.toLocaleString('vi')} tủ (${(ctx.parsed.y/tot*100).toFixed(1)}%)`}}},
      scales:{x:{grid:{display:false},ticks:{font:{size:10},color:'#94a3b8'}},y:{grid:GRID_OPTS,ticks:TICK_OPTS}}}
  });
}

// Net Addition chart
function buildNetChart(){
  destroyChart('net');
  const d = NET_DATA;
  charts['net'] = new Chart(document.getElementById('netChart'),{
    type:'bar',
    data:{
      labels:d.map(r=>r.ASM.split(' – ')[0]),
      datasets:[
        {label:'Tháng 1',data:d.map(r=>r.jan),backgroundColor:'#004B93',borderRadius:2,stack:'s'},
        {label:'Tháng 2',data:d.map(r=>r.feb),backgroundColor:'#f59e0b',borderRadius:2,stack:'s'},
        {label:'Tháng 3',data:d.map(r=>r.mar),backgroundColor:'#16a34a',borderRadius:2,stack:'s'},
        {label:'Net Add Q1',data:d.map(r=>r.Q1),
          type:'line',borderColor:d.map(r=>r.Q1<0?'#dc2626':'#16a34a'),
          pointBackgroundColor:d.map(r=>r.Q1<0?'#dc2626':'#16a34a'),
          borderWidth:2,pointRadius:5,tension:0.2,stack:undefined,
          segment:{borderColor:ctx=>ctx.p1.parsed.y<0?'#dc2626':'#16a34a'},
        }
      ]
    },
    options:{responsive:true,maintainAspectRatio:false,
      plugins:{legend:{display:false},tooltip:{mode:'index',intersect:false}},
      scales:{
        x:{stacked:true,grid:{display:false},ticks:{font:{size:9}}},
        y:{stacked:true,grid:GRID_OPTS,ticks:TICK_OPTS}
      }}
  });
}

// Penetration chart
function buildPeneChart(){
  destroyChart('pen');
  const d = NET_DATA.filter(r=>r.AOP>0);
  charts['pen'] = new Chart(document.getElementById('peneChart'),{
    type:'bar',
    data:{
      labels:d.map(r=>r.ASM.split(' – ')[0]),
      datasets:[
        {label:'AOP Net Add',data:d.map(r=>r.AOP),backgroundColor:'rgba(148,163,184,.4)',borderRadius:4,borderSkipped:false},
        {label:'Actual Q1',data:d.map(r=>r.Q1),
          backgroundColor:d.map(r=>r.Q1<0?'rgba(220,38,38,.7)':'rgba(22,163,74,.7)'),
          borderRadius:4,borderSkipped:false},
      ]
    },
    options:{responsive:true,maintainAspectRatio:false,
      plugins:{legend:{
        display:true,position:'top',
        labels:{font:{size:10},color:'#64748b',boxWidth:10}
      },
      tooltip:{mode:'index',intersect:false}},
      scales:{x:{grid:{display:false},ticks:{font:{size:9}}},y:{grid:GRID_OPTS,ticks:TICK_OPTS}}}
  });
}

// Thu hoi chart
function buildThChart(){
  destroyChart('th');
  const labels = Object.keys(TH_CAT).map(k=>k.length>18?k.slice(0,18)+'…':k);
  charts['th'] = new Chart(document.getElementById('thChart'),{
    type:'bar',data:{labels,datasets:[{data:Object.values(TH_CAT),
      backgroundColor:['#dc2626','#b91c1c','#ef4444','#f87171','#fca5a5','#94a3b8'],
      borderRadius:5,borderSkipped:false}]},
    options:{indexAxis:'y',responsive:true,maintainAspectRatio:false,
      plugins:{legend:{display:false}},
      scales:{x:{grid:GRID_OPTS,ticks:TICK_OPTS},y:{grid:{display:false},ticks:{font:{size:10}}}}}
  });
}

// Lap dat chart
function buildLdChart(){
  destroyChart('ld');
  const labels = Object.keys(LD_CAT).map(k=>k.length>18?k.slice(0,18)+'…':k);
  charts['ld'] = new Chart(document.getElementById('ldChart'),{
    type:'bar',data:{labels,datasets:[{data:Object.values(LD_CAT),
      backgroundColor:['#16a34a','#15803d','#22c55e','#4ade80','#86efac','#94a3b8'],
      borderRadius:5,borderSkipped:false}]},
    options:{indexAxis:'y',responsive:true,maintainAspectRatio:false,
      plugins:{legend:{display:false}},
      scales:{x:{grid:GRID_OPTS,ticks:TICK_OPTS},y:{grid:{display:false},ticks:{font:{size:10}}}}}
  });
}

// ══════════════════════════════════════════════════
// TABLES
// ══════════════════════════════════════════════════
function renderASMTable(){
  const sortBy = document.getElementById('asm-sort').value;
  const filter = document.getElementById('view-sel').value;
  let data = [...ASM_DATA];
  if(filter !== 'all') data = data.filter(d=>d.name===filter);
  if(sortBy==='total') data.sort((a,b)=>b.total-a.total);
  else if(sortBy==='pct') data.sort((a,b)=>a.pct-b.pct);
  else if(sortBy==='issues') data.sort((a,b)=>b.issues-a.issues);
  else if(sortBy==='v3') data.sort((a,b)=>b.v3-a.v3);

  const tbody = document.getElementById('asm-tbody');
  tbody.innerHTML = data.map(r => {
    const chk = r.total - r.report;
    const pctDS = r.total>0?(r.hv3/r.total*100).toFixed(0):0;
    const pctColor = r.pct>=100?'#16a34a':r.pct>=99?'#84cc16':r.pct>=98?'#f59e0b':'#dc2626';
    const issCol = r.issues>100?'tag-r':r.issues>50?'tag-a':'tag-b';
    const rowBg = r.issues>100?'background:#fff5f5':r.pct<99?'background:#fffbf0':'';
    return `<tr style="${rowBg}">
      <td><strong>${r.name}</strong><br><span style="font-size:9px;color:var(--muted)">${r.full.split(' – ')[1]||''}</span></td>
      <td class="tb">${r.total.toLocaleString('vi')}</td>
      <td>
        <div class="pb-wrap">
          <div class="pb-bg"><div class="pb-fill" style="width:${r.pct}%;background:${pctColor}"></div></div>
          <span class="pb-val" style="color:${pctColor}">${r.pct}%</span>
        </div>
      </td>
      <td class="${chk>0?'tdn':''}">${chk||'—'}</td>
      <td><span class="tag ${issCol}">${r.issues}</span></td>
      <td>${r.v3>0?Math.round(r.v3/1000)+'K':'—'}</td>
      <td style="color:${pctDS>80?'#16a34a':pctDS>50?'#f59e0b':'#dc2626'}">${pctDS}%</td>
    </tr>`;
  }).join('');

  buildVolChart(data);
}

function renderVPOTable(){
  const tbody = document.getElementById('vpo-tbody');
  tbody.innerHTML = VPO_DATA.sort((a,b)=>b.remain-a.remain).map(r=>{
    const pctColor = r.rate>=90?'#16a34a':r.rate>=80?'#f59e0b':'#dc2626';
    return `<tr>
      <td>${r.ASM}</td>
      <td class="tb">${r.total}</td>
      <td>
        <div class="pb-wrap">
          <div class="pb-bg"><div class="pb-fill" style="width:${r.rate}%;background:${pctColor}"></div></div>
          <span class="pb-val" style="color:${pctColor}">${r.rate}%</span>
        </div>
      </td>
      <td class="${r.remain>10?'tdn':r.remain>0?'camt':''}">${r.remain||'✓'}</td>
    </tr>`;
  }).join('');
}

function renderSSTable(){
  const filter = document.getElementById('view-sel').value;
  let data = [...SS_WORST];
  if(filter!=='all') data = data.filter(d=>d.asm===filter||d.asm.includes(filter));
  const tbody = document.getElementById('ss-tbody');
  tbody.innerHTML = data.slice(0,10).map(r=>{
    const pctColor = r.pct<95?'#dc2626':r.pct<98?'#f59e0b':'#16a34a';
    return `<tr>
      <td style="font-size:11px">${r.ss.replace('SS-','')}</td>
      <td><span class="tag tag-b">${r.asm}</span></td>
      <td>${r.total}</td>
      <td style="color:${pctColor};font-weight:600">${r.pct}%</td>
      <td style="font-size:10px;color:var(--orange)">${r.note||'—'}</td>
    </tr>`;
  }).join('');
}

// ══════════════════════════════════════════════════
// FILTER
// ══════════════════════════════════════════════════
function applyFilter(){
  renderASMTable();
  renderSSTable();
}

// ══════════════════════════════════════════════════
// INIT
// ══════════════════════════════════════════════════
function init(){
  renderASMTable();
  renderVPOTable();
  renderSSTable();
  buildIssueDonut();
  buildTimingChart();
  buildNetChart();
  buildPeneChart();
  buildThChart();
  buildLdChart();
}

window.addEventListener('load', init);
</script>
</body>
</html>
