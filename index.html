<!DOCTYPE html>
<html lang="id">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1">
<title>Absensi Online KB RA At Tibyan</title>
<link rel="icon" href="logo.png">
<style>
  *{box-sizing:border-box}
  body{margin:0;font-family:Arial,sans-serif;background:#f5f5f5;padding:16px}
  .wrap{max-width:480px;margin:auto}
  .card{background:#fff;border-radius:14px;padding:20px;margin-bottom:14px;box-shadow:0 2px 10px rgba(0,0,0,.1)}
  .head{background:#2196F3;color:#fff;border-radius:14px;padding:18px;margin-bottom:14px}
  .head.kepsek{background:#5e35b1}
  .head h2{margin:0 0 6px}
  h2,h3{margin-top:0}
  input[type=text],input[type=password]{width:100%;padding:12px;margin-bottom:12px;border:1px solid #ccc;border-radius:6px;font-size:15px}
  input[type=month],input[type=date]{width:100%;padding:10px;border:1px solid #ccc;border-radius:6px;font-size:15px}
  button{width:100%;padding:13px;border:0;border-radius:8px;background:#2196F3;color:#fff;font-size:15px;margin-top:8px;cursor:pointer}
  button:disabled{background:#999}
  button.red{background:#e53935} button.green{background:#43a047} button.gray{background:#757575} button.purple{background:#5e35b1}
  button.mini{width:auto;margin:0;padding:8px 10px;font-size:14px}
  .msg{margin-top:10px;text-align:center;font-size:14px}
  .err{color:#d32f2f} .ok{color:#2e7d32} .info{color:#1976D2}
  .hidden{display:none}
  video{width:100%;border-radius:10px;background:#000;transform:scaleX(-1)}
  #preview{width:100%;border-radius:10px;background:#000;max-height:320px;object-fit:contain}
  .siswa{display:flex;align-items:center;gap:6px;padding:10px 0;border-bottom:1px solid #eee}
  .siswa .nm{flex:1;font-size:15px}
  .siswa small{display:block;font-size:11px;color:#888}
  .siswa small.ok2{color:#2e7d32}
  .st-Belum{color:#d32f2f}
  select{padding:8px;border-radius:6px;border:1px solid #ccc;font-size:14px}
  select.full{width:100%;margin-bottom:8px;padding:10px;font-size:15px}
  .bar{display:flex;gap:8px}.bar button{margin-top:0}
  #scanLog{margin-top:10px;font-size:14px;max-height:180px;overflow:auto}
  #scanLog div{padding:6px 0;border-bottom:1px solid #eee}
  .judul{text-align:center;margin-bottom:18px}
  .judul .atas{font-size:22px;font-weight:bold;color:#2196F3;margin:0}
  .judul .bawah{font-size:22px;font-weight:bold;color:#2196F3;margin:4px 0 0}
  .judul hr{border:0;border-top:2px solid #e3f2fd;margin:14px 0 0}
  .logo-login{display:block;margin:0 auto 10px;width:150px;height:150px;object-fit:contain}
  details{border:1px solid #eee;border-radius:8px;padding:8px 10px;margin-top:8px}
  summary{cursor:pointer;font-size:14px;line-height:1.5}
</style>
</head>
<body>
<div class="wrap">

  <!-- PILIHAN MASUK -->
  <div id="vPilih" class="card">
    <img src="logo.png" class="logo-login" alt="Logo sekolah" onerror="this.style.display='none'">
    <div class="judul">
      <p class="atas">Absensi Online</p>
      <p class="bawah">KB RA At Tibyan</p>
      <hr>
    </div>
    <p style="text-align:center;font-size:14px;color:#555;margin:0 0 6px">Masuk sebagai</p>
    <button onclick="pilih('vLogin')">👤 Guru</button>
    <button class="purple" onclick="pilih('vKLogin')">🏫 Kepala Sekolah</button>
    <button class="gray" onclick="bukaWali()">👪 Wali Murid</button>
    <div id="srvStatus" class="msg" style="font-size:12px"></div>
  </div>

  <!-- LOGIN GURU -->
  <div id="vLogin" class="card hidden">
    <h3 style="text-align:center;margin-bottom:14px">Login Guru</h3>
    <input type="text" id="user" placeholder="Username" autocomplete="username">
    <input type="password" id="pass" placeholder="Password" autocomplete="current-password">
    <button id="btnLogin" onclick="doLogin()">LOGIN</button>
    <div id="loginMsg" class="msg"></div>
    <button class="gray" onclick="pilih('vPilih')">Kembali</button>
  </div>

  <!-- LOGIN KEPALA SEKOLAH -->
  <div id="vKLogin" class="card hidden">
    <h3 style="text-align:center;margin-bottom:14px">Login Kepala Sekolah</h3>
    <input type="text" id="kUser" placeholder="Username" autocomplete="username">
    <input type="password" id="kPass" placeholder="Password" autocomplete="current-password">
    <button class="purple" id="btnK" onclick="loginKepsek()">LOGIN</button>
    <div id="kLoginMsg" class="msg"></div>
    <button class="gray" onclick="pilih('vPilih')">Kembali</button>
  </div>

  <!-- LOGIN WALI MURID -->
  <div id="vWali" class="card hidden">
    <h3 style="text-align:center">Wali Murid</h3>
    <p style="font-size:14px;color:#555;text-align:center">Masukkan nama anak dan Kode Wali dari sekolah.</p>
    <input type="text" id="wNama" placeholder="Nama anak (sesuai data sekolah)">
    <input type="text" id="wKode" placeholder="Kode Wali" autocapitalize="characters" autocomplete="off">
    <button class="gray" id="btnWali" onclick="loginWali()">LIHAT ABSENSI</button>
    <div id="wMsg" class="msg"></div>
    <button onclick="pilih('vPilih')">Kembali</button>
  </div>

  <!-- REKAP UNTUK WALI MURID -->
  <div id="vWaliHasil" class="card hidden">
    <h3 id="wJudul">Absensi</h3>
    <div id="wInfo" style="font-size:14px;color:#555;margin-bottom:8px"></div>
    <input type="month" id="wBulan">
    <button onclick="muatRekapWali()">Tampilkan</button>
    <div id="wrMsg" class="msg"></div>
    <div id="wrRingkas" style="margin-top:10px;font-size:15px;font-weight:bold"></div>
    <div id="wrList" style="margin-top:8px"></div>
    <button class="red" onclick="keluarWali()">Keluar</button>
  </div>

  <!-- DASHBOARD KEPALA SEKOLAH -->
  <div id="vKepsek" class="hidden">
    <div class="head kepsek">
      <h2>Dashboard Kepala Sekolah</h2>
      <div>Selamat datang, <b id="kNama"></b></div>
    </div>
    <div class="card">
      <h3>Ringkasan Absensi</h3>
      <input type="date" id="kTanggal">
      <button class="purple" onclick="muatRingkasan()">Tampilkan</button>
      <button onclick="bukaKRekap()">📊 Rekap Siswa</button>
      <div id="kMsg" class="msg"></div>
      <div id="kTotal" style="margin-top:10px;font-size:15px;font-weight:bold"></div>
      <div id="kList"></div>
    </div>
    <button class="red" onclick="logout()">🚪 Keluar</button>
  </div>

  <!-- REKAP SISWA (KEPALA SEKOLAH) -->
  <div id="vKRekap" class="card hidden">
    <h3>📊 Rekap Siswa</h3>
    <select id="krKelas" class="full" onchange="isiSiswaK()"></select>
    <select id="krSiswa" class="full"></select>
    <input type="month" id="krBulan">
    <button class="purple" onclick="muatKRekap()">Tampilkan</button>
    <div id="krMsg" class="msg"></div>
    <div id="krRingkas" style="margin-top:10px;font-size:15px;font-weight:bold"></div>
    <div id="krList" style="margin-top:8px"></div>
    <button class="gray" onclick="show('vKepsek')">Kembali</button>
  </div>

  <!-- KAMERA (daftar wajah murid / scan absen) -->
  <div id="vCam" class="card hidden">
    <h3 id="camTitle"></h3>
    <p id="camDesc" style="font-size:14px;color:#555"></p>
    <video id="video" playsinline muted class="hidden"></video>
    <img id="preview" class="hidden">
    <input type="file" id="fileCam" accept="image/*" capture="user" class="hidden">
    <button id="btnCam" onclick="startCam()">📷 Aktifkan Kamera</button>
    <button id="btnSnap" class="green hidden" onclick="snap()">✅ Ambil Sampel Wajah</button>
    <button id="btnFile" class="gray" onclick="document.getElementById('fileCam').click()">Pakai aplikasi kamera HP</button>
    <button class="red" onclick="closeCam()">Selesai</button>
    <div id="camMsg" class="msg"></div>
    <div id="scanLog"></div>
  </div>

  <!-- REKAP SISWA (GURU) -->
  <div id="vRekap" class="card hidden">
    <h3>📊 Rekap Siswa</h3>
    <select id="rkSiswa" class="full"></select>
    <input type="month" id="rkBulan">
    <button onclick="muatRekap()">Tampilkan</button>
    <div id="rkMsg" class="msg"></div>
    <div id="rkRingkas" style="margin-top:10px;font-size:15px;font-weight:bold"></div>
    <div id="rkList" style="margin-top:8px"></div>
    <button class="gray" onclick="show('vDash')">Kembali</button>
  </div>

  <!-- DASHBOARD GURU -->
  <div id="vDash" class="hidden">
    <div class="head">
      <h2>Dashboard Guru</h2>
      <div>Selamat datang, <b id="dNama"></b></div>
      <div>Kelas: <b id="dKelas"></b> &nbsp;|&nbsp; <span id="dTgl"></span></div>
    </div>
    <div class="card">
      <h3>Absensi Siswa</h3>
      <button class="green" onclick="mulaiScan()">📸 Scan Wajah Murid</button>
      <button onclick="bukaRekap()">📊 Rekap Siswa</button>
      <div class="bar" style="margin-top:8px">
        <button class="gray" onclick="setSemua('Hadir')">Semua Hadir</button>
        <button class="gray" onclick="muatSiswa()">Muat Ulang</button>
      </div>
      <div id="listSiswa" style="margin-top:10px">Memuat...</div>
      <button onclick="simpanManual()">💾 Simpan Manual</button>
      <div id="dashMsg" class="msg"></div>
      <button class="gray" id="btnUlang" style="display:none" onclick="bicara(S.lastUcapan)">🔊 Ulangi Suara</button>
    </div>
    <button class="red" onclick="logout()">🚪 Keluar</button>
  </div>

</div>

<script src="https://cdn.jsdelivr.net/npm/@vladmandic/face-api@1.7.12/dist/face-api.js"></script>
<script>
// ===== URL WEB APP APPS SCRIPT (berakhiran /exec) =====
var API_URL = "https://script.google.com/macros/s/AKfycbzyknrk3xLIRahq-A4TqlqCFW-y6fd_8VjXQBIPYcnG1jvHIWgVLNX_rCheCd88hwGR/exec";
// ======================================================

var MODEL_URL = "https://cdn.jsdelivr.net/npm/@vladmandic/face-api@1.7.12/model/";
var THRESHOLD = 0.5;   // makin kecil makin ketat (0.4 - 0.6)
var MARGIN = 0.03;     // selisih minimal dengan murid terdekat kedua
var S = { token:"", nama:"", kelas:"", mode:"", target:"", siswa:[], samples:[],
          selesai:{}, hitung:{}, scanning:false, lastUcapan:"" };
var K = { token:"", nama:"", kelas:[] };
var W = { token:"", nama:"", kelas:"" };
var modelsReady = false, stream = null;
var $ = function(id){ return document.getElementById(id); };
var wait = function(ms){ return new Promise(function(r){ setTimeout(r, ms); }); };

var VIEWS = ["vPilih","vLogin","vKLogin","vWali","vWaliHasil","vKepsek","vKRekap","vCam","vDash","vRekap"];
function show(id){
  VIEWS.forEach(function(v){ $(v).classList.add("hidden"); });
  $(id).classList.remove("hidden");
}
function say(el, text, cls){ el.className = "msg " + (cls||""); el.textContent = text; }
function pilih(id){
  ["loginMsg","kLoginMsg","wMsg"].forEach(function(m){ say($(m),"",""); });
  show(id);
}
function apiSiap(el){
  if(API_URL.indexOf("https://script.google.com/") !== 0){ say(el,"API_URL belum diisi di index.html","err"); return false; }
  return true;
}

// ==========================================
// KOMUNIKASI KE APPS SCRIPT
// (text/plain supaya tidak kena pemeriksaan CORS preflight)
// ==========================================
function api(action, data){
  var body = Object.assign({ action: action }, data || {});
  return fetch(API_URL, {
    method: "POST",
    headers: { "Content-Type": "text/plain;charset=utf-8" },
    body: JSON.stringify(body)
  }).then(function(r){ return r.json(); });
}
function galat(e){
  return "Gagal terhubung ke server. Cek internet / URL API. (" + (e && e.message ? e.message : e) + ")";
}
function sesiHabis(r){ return r && String(r.message).indexOf("Sesi habis") >= 0; }

// cek apakah API_URL terhubung ke script yang benar (tampil di layar pilihan masuk)
function cekServer(){
  var el = $("srvStatus");
  if(API_URL.indexOf("https://script.google.com/") !== 0){
    el.textContent = "API_URL belum diisi."; el.className = "msg err"; return;
  }
  el.textContent = "Memeriksa server..."; el.className = "msg info";
  fetch(API_URL).then(function(r){ return r.text(); }).then(function(t){
    if(t.indexOf("At Tibyan") >= 0){
      el.textContent = "Server tersambung"; el.className = "msg ok";
    } else if(t.indexOf("Attibyan") >= 0){
      el.textContent = "Server LAMA terdeteksi. Ganti API_URL dengan URL deployment script Absensi Attibyan.";
      el.className = "msg err";
    } else {
      el.textContent = "Server membalas, tapi bukan API absensi. Periksa API_URL.";
      el.className = "msg err";
    }
  }).catch(function(){
    el.textContent = "Server tidak terjangkau. Periksa internet atau pengaturan akses (Anyone).";
    el.className = "msg err";
  });
}

// ==========================================
// SUARA
// ==========================================
if("speechSynthesis" in window){
  speechSynthesis.onvoiceschanged = function(){ speechSynthesis.getVoices(); };
}
var audioCtx = null;

// harus dipanggil dari tap pengguna agar bunyi diizinkan HP
function initAudio(){
  try{
    var AC = window.AudioContext || window.webkitAudioContext;
    if(!AC) return;
    if(!audioCtx) audioCtx = new AC();
    if(audioCtx.state === "suspended") audioCtx.resume();
  }catch(e){}
}

// bunyi "tit-tit" cadangan (dipakai kalau bunyi.mp3 gagal diputar)
function titSintesis(){
  try{
    if(!audioCtx) return;
    if(audioCtx.state === "suspended") audioCtx.resume();

    var t = audioCtx.currentTime;

    var master = audioCtx.createGain();
    master.gain.value = 2.5;

    var comp = audioCtx.createDynamicsCompressor();
    comp.threshold.value = -30;
    comp.knee.value = 0;
    comp.ratio.value = 20;
    comp.attack.value = 0.001;
    comp.release.value = 0.05;

    master.connect(comp);
    comp.connect(audioCtx.destination);

    [[2000, 0], [2600, 0.19]].forEach(function(n){
      var f = n[0], mulai = t + n[1];
      ["square", "sawtooth"].forEach(function(jenis){
        var o = audioCtx.createOscillator();
        var g = audioCtx.createGain();
        o.type = jenis;
        o.frequency.value = f;
        g.gain.setValueAtTime(0.0001, mulai);
        g.gain.exponentialRampToValueAtTime(1.0, mulai + 0.005);
        g.gain.setValueAtTime(1.0, mulai + 0.12);
        g.gain.exponentialRampToValueAtTime(0.0001, mulai + 0.16);
        o.connect(g); g.connect(master);
        o.start(mulai); o.stop(mulai + 0.17);
      });
    });
  }catch(e){}
}

// bunyi dari file mp3 (bunyi.mp3 di folder yang sama dengan index.html)
var audioTit = new Audio("bunyi.mp3");
audioTit.preload = "auto";
audioTit.volume = 1.0;
var JEDA_SUARA = 1000;   // jeda (milidetik) antara bunyi tit dan ucapan nama

function tit(){
  try{
    audioTit.currentTime = 0;
    var p = audioTit.play();
    if(p && p.catch) p.catch(function(){ titSintesis(); });
  }catch(e){ titSintesis(); }
}
function unlockSuara(){
  initAudio();
  try{
    audioTit.muted = true;
    var p = audioTit.play();
    if(p && p.then){
      p.then(function(){ audioTit.pause(); audioTit.currentTime = 0; audioTit.muted = false; })
       .catch(function(){ audioTit.muted = false; });
    }
  }catch(e){}
  if(!("speechSynthesis" in window)) return;
  var u = new SpeechSynthesisUtterance(" ");
  u.volume = 0;
  speechSynthesis.speak(u);
}
function buatUtter(teks){
  var u = new SpeechSynthesisUtterance(teks);
  u.lang = "id-ID";
  u.rate = 0.9;
  u.pitch = 1.1;
  u.volume = 1;

  var daftar = speechSynthesis.getVoices().filter(function(x){
    return x.lang && x.lang.toLowerCase().replace("_","-").indexOf("id") === 0;
  });
  daftar.sort(function(a,b){ return (a.localService?1:0) - (b.localService?1:0); });
  if(daftar[0]) u.voice = daftar[0];
  return u;
}
function bicara(teks){
  if(!teks || !("speechSynthesis" in window)) return;
  speechSynthesis.cancel();
  speechSynthesis.speak(buatUtter(teks));
}
function bicaraAntri(teks){
  if(!teks || !("speechSynthesis" in window)) return;
  speechSynthesis.speak(buatUtter(teks));
}
function susunUcapan(r){
  var h = r.hasil || [];
  var waktu = ", tanggal " + r.tanggalTeks + ", pukul " + r.jam +
              (r.menit === 0 ? " tepat." : " lewat " + r.menit + " menit.");
  if(h.length <= 3){
    return h.map(function(x){ return x.nama + " " + x.status.toLowerCase(); }).join(", ") + waktu;
  }
  var hitung = {};
  h.forEach(function(x){ hitung[x.status] = (hitung[x.status]||0) + 1; });
  var ringkas = Object.keys(hitung).map(function(k){
    return hitung[k] + " " + k.toLowerCase();
  }).join(", ");
  return "Absensi " + h.length + " siswa berhasil disimpan. " + ringkas + waktu;
}

// ==========================================
// LOGIN GURU
// ==========================================
function doLogin(){
  unlockSuara();
  var u = $("user").value.trim(), p = $("pass").value.trim();
  if(!u || !p){ say($("loginMsg"),"Username dan Password wajib diisi","err"); return; }
  if(!apiSiap($("loginMsg"))) return;
  $("btnLogin").disabled = true; say($("loginMsg"),"Memproses login...","info");
  api("login", { username:u, password:p })
    .then(function(r){
      $("btnLogin").disabled = false;
      if(!r || r.status !== "success"){ say($("loginMsg"), (r&&r.message)||"Login gagal","err"); return; }
      S.token = r.token; S.nama = r.namaGuru; S.kelas = r.kelas;
      sessionStorage.setItem("sesi", JSON.stringify({ role:"guru", token:S.token, nama:S.nama, kelas:S.kelas }));
      $("pass").value = "";
      openDash();
    })
    .catch(function(e){
      $("btnLogin").disabled = false; say($("loginMsg"), galat(e), "err");
    });
}

// keluar (guru / kepala sekolah). pesan = alasan, mis. sesi habis
function logout(pesan){
  stopCam();
  if("speechSynthesis" in window) speechSynthesis.cancel();
  sessionStorage.removeItem("sesi");
  S.token = ""; S.siswa = []; S.lastUcapan = "";
  K.token = ""; K.nama = ""; K.kelas = [];
  $("btnUlang").style.display = "none";
  say($("dashMsg"),"","");
  if(typeof pesan === "string"){ show("vLogin"); say($("loginMsg"), pesan, "err"); }
  else { show("vPilih"); say($("loginMsg"),"",""); }
}

// ==========================================
// LOGIN KEPALA SEKOLAH
// ==========================================
function loginKepsek(){
  var u = $("kUser").value.trim(), p = $("kPass").value.trim();
  if(!u || !p){ say($("kLoginMsg"),"Username dan Password wajib diisi","err"); return; }
  if(!apiSiap($("kLoginMsg"))) return;
  $("btnK").disabled = true; say($("kLoginMsg"),"Memproses login...","info");
  api("loginKepsek", { username:u, password:p })
    .then(function(r){
      $("btnK").disabled = false;
      if(!r || r.status !== "success"){ say($("kLoginMsg"), (r&&r.message)||"Login gagal","err"); return; }
      K.token = r.token; K.nama = r.nama;
      sessionStorage.setItem("sesi", JSON.stringify({ role:"kepsek", token:K.token, nama:K.nama }));
      $("kPass").value = "";
      openKepsek();
    })
    .catch(function(e){
      $("btnK").disabled = false; say($("kLoginMsg"), galat(e), "err");
    });
}

// pulihkan sesi kalau halaman di-refresh
(function(){
  try{
    var o = JSON.parse(sessionStorage.getItem("sesi") || "null");
    if(!o || !o.token) return;
    if(o.role === "kepsek"){ K.token = o.token; K.nama = o.nama; openKepsek(); }
    else { S.token = o.token; S.nama = o.nama; S.kelas = o.kelas; openDash(); }
  }catch(e){}
})();

// ==========================================
// DASHBOARD KEPALA SEKOLAH
// ==========================================
function openKepsek(){
  show("vKepsek");
  $("kNama").textContent = K.nama;
  $("kTanggal").value = "";
  muatRingkasan();
}

function muatRingkasan(){
  say($("kMsg"),"Memuat...","info");
  api("kepsekRingkasan", { token:K.token, tanggal:$("kTanggal").value })
    .then(function(r){
      if(r.status !== "success"){
        if(sesiHabis(r)){ logout(r.message); return; }
        say($("kMsg"), r.message, "err"); return;
      }
      say($("kMsg"),"","");
      $("kTanggal").value = r.tanggal;
      K.kelas = r.kelas;
      renderRingkasan();
    })
    .catch(function(e){ say($("kMsg"), galat(e), "err"); });
}

function renderRingkasan(){
  var tot = { Hadir:0, Izin:0, Sakit:0, Alpa:0, Belum:0 }, jml = 0;
  K.kelas.forEach(function(k){
    Object.keys(tot).forEach(function(s){ tot[s] += k.hitung[s]; });
    jml += k.siswa.length;
  });
  $("kTotal").textContent = "Seluruh kelas (" + jml + " murid): Hadir " + tot.Hadir + " | Izin " + tot.Izin +
                            " | Sakit " + tot.Sakit + " | Alpa " + tot.Alpa + " | Belum " + tot.Belum;

  var box = $("kList"); box.innerHTML = "";
  K.kelas.forEach(function(k){
    var d = document.createElement("details");
    var sm = document.createElement("summary");
    var h = k.hitung;
    sm.textContent = k.kelas + " (" + k.siswa.length + " murid) — Hadir " + h.Hadir + ", Izin " + h.Izin +
                     ", Sakit " + h.Sakit + ", Alpa " + h.Alpa + ", Belum " + h.Belum;
    d.appendChild(sm);
    k.siswa.forEach(function(x){
      var row = document.createElement("div"); row.className = "siswa";
      var a = document.createElement("div"); a.className = "nm"; a.textContent = x.nama;
      var b = document.createElement("div");
      b.textContent = x.status ? (x.status + (x.jam ? " (" + x.jam + ")" : "")) : "Belum absen";
      if(!x.status) b.className = "st-Belum";
      row.appendChild(a); row.appendChild(b); d.appendChild(row);
    });
    box.appendChild(d);
  });
}

// ---------- rekap siswa (kepala sekolah) ----------
function bukaKRekap(){
  if(!K.kelas.length){ say($("kMsg"),"Data kelas belum termuat.","err"); return; }
  var sel = $("krKelas"); sel.innerHTML = "";
  K.kelas.forEach(function(k, i){
    var op = document.createElement("option");
    op.value = i; op.textContent = k.kelas; sel.appendChild(op);
  });
  var d = new Date();
  $("krBulan").value = d.getFullYear() + "-" + ("0" + (d.getMonth()+1)).slice(-2);
  $("krRingkas").textContent = ""; $("krList").innerHTML = "";
  say($("krMsg"),"","");
  isiSiswaK();
  show("vKRekap");
}

function isiSiswaK(){
  var k = K.kelas[Number($("krKelas").value)];
  var sel = $("krSiswa"); sel.innerHTML = "";
  if(!k) return;
  k.siswa.forEach(function(s){
    var op = document.createElement("option");
    op.value = s.nama; op.textContent = s.nama; sel.appendChild(op);
  });
}

function muatKRekap(){
  var k = K.kelas[Number($("krKelas").value)];
  var nama = $("krSiswa").value, bulan = $("krBulan").value;
  if(!k || !nama || !bulan){ say($("krMsg"),"Pilih kelas, siswa, dan bulan.","err"); return; }
  say($("krMsg"),"Memuat...","info");
  api("kepsekRekap", { token:K.token, nama:nama, kelas:k.kelas, bulan:bulan })
    .then(function(r){
      if(r.status !== "success"){
        if(sesiHabis(r)){ logout(r.message); return; }
        say($("krMsg"), r.message, "err"); return;
      }
      say($("krMsg"),"","");
      tampilRekap(r, $("krRingkas"), $("krList"));
    })
    .catch(function(e){ say($("krMsg"), galat(e), "err"); });
}

// tampilan rekap bersama (kepala sekolah, guru, wali)
function tampilRekap(r, elRingkas, elList){
  var h = r.hitung;
  elRingkas.textContent = r.nama + ": Hadir " + h.Hadir + "  |  Izin " + h.Izin +
                          "  |  Sakit " + h.Sakit + "  |  Alpa " + h.Alpa;
  elList.innerHTML = "";
  if(!r.list.length){ elList.textContent = "Belum ada catatan absen di bulan ini."; return; }
  r.list.forEach(function(x){
    var row = document.createElement("div"); row.className = "siswa";
    var a = document.createElement("div"); a.className = "nm"; a.textContent = x.tanggal;
    var b = document.createElement("div"); b.textContent = x.status + " (" + x.jam + ")";
    row.appendChild(a); row.appendChild(b); elList.appendChild(row);
  });
}

// ==========================================
// WALI MURID (hanya melihat)
// ==========================================
function bukaWali(){
  say($("wMsg"),"","");
  show("vWali");
}

function loginWali(){
  var n = $("wNama").value.trim(), k = $("wKode").value.trim();
  if(!n || !k){ say($("wMsg"),"Nama anak dan Kode Wali wajib diisi.","err"); return; }
  if(!apiSiap($("wMsg"))) return;
  $("btnWali").disabled = true; say($("wMsg"),"Memeriksa...","info");
  api("loginWali", { nama:n, kode:k })
    .then(function(r){
      $("btnWali").disabled = false;
      if(!r || r.status !== "success"){ say($("wMsg"), (r&&r.message)||"Gagal masuk.","err"); return; }
      W.token = r.token; W.nama = r.nama; W.kelas = r.kelas;
      $("wKode").value = "";
      $("wJudul").textContent = "Absensi " + r.nama;
      $("wInfo").textContent = "Kelas " + r.kelas;
      var d = new Date();
      $("wBulan").value = d.getFullYear() + "-" + ("0" + (d.getMonth()+1)).slice(-2);
      $("wrRingkas").textContent = ""; $("wrList").innerHTML = "";
      say($("wrMsg"),"","");
