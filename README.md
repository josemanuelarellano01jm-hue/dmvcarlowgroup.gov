<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0, maximum-scale=1.0, user-scalable=no">
    <title>DMV Car Low Group | Cloud Verification Portal</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0/css/all.min.css">
    <style>
        @import url('https://fonts.googleapis.com/css2?family=Inter:wght@400;600;800;900&display=swap');
        body { font-family: 'Inter', sans-serif; scroll-behavior: smooth; }
        .tab-active { color: #2563eb; position: relative; font-weight: 900; }
        .tab-active::after { content: ''; position: absolute; bottom: 0; left: 0; width: 100%; height: 4px; background: #2563eb; border-radius: 10px; }
        .verified-stamp {
            position: absolute; top: 50%; left: 50%; transform: translate(-50%, -50%) rotate(-15deg);
            border: 8px solid #16a34a; color: #16a34a; padding: 15px 30px; font-size: 3rem;
            font-weight: 900; text-transform: uppercase; border-radius: 15px;
            background: rgba(255, 255, 255, 0.95); box-shadow: 0 0 30px rgba(0,0,0,0.1);
            pointer-events: none; z-index: 20; opacity: 0.9;
        }
        .animate-fade { animation: fadeIn 0.4s ease-out; }
        @keyframes fadeIn { from { opacity: 0; transform: translateY(15px); } to { opacity: 1; transform: translateY(0); } }
        .loading-overlay {
            position: fixed; inset: 0; background: rgba(255,255,255,0.8);
            display: flex; justify-content: center; items-center; z-index: 100;
        }
        .spinner {
            width: 40px; height: 40px; border: 4px solid #f3f3f3;
            border-top: 4px solid #2563eb; border-radius: 50%;
            animation: spin 1s linear infinite;
        }
        @keyframes spin { 0% { transform: rotate(0deg); } 100% { transform: rotate(360deg); } }
        .hidden { display: none; }
    </style>
</head>
<body class="bg-slate-50 text-slate-900">

    <!-- Loading State -->
    <div id="loading-screen" class="loading-overlay hidden">
        <div class="text-center">
            <div class="spinner mx-auto mb-4"></div>
            <p class="text-[10px] font-black uppercase tracking-widest text-slate-500">Accessing Cloud Database...</p>
        </div>
    </div>

    <!-- Legal Header Strip -->
    <div class="bg-blue-950 text-white py-2 text-[9px] font-black text-center uppercase tracking-[0.3em] px-4">
        FEDERAL DOCUMENTATION COMPLIANCE PORTAL — SECURED CLOUD ACCESS 2026
    </div>

    <!-- Main Header -->
    <header class="bg-white sticky top-0 z-50 shadow-sm border-b">
        <div class="container mx-auto px-6 py-4 flex flex-col md:flex-row justify-between items-center gap-4">
            <div class="flex items-center space-x-4">
                <div class="bg-blue-600 text-white p-2.5 rounded-2xl shadow-lg shadow-blue-200">
                    <i class="fas fa-shield-check text-2xl"></i>
                </div>
                <div>
                    <h1 class="text-xl md:text-2xl font-black italic tracking-tighter uppercase leading-none">
                        DMV <span class="text-blue-600">CAR LOW GROUP</span>
                    </h1>
                    <p class="text-[9px] font-extrabold text-slate-400 tracking-widest uppercase mt-1">Independent Legal Consulting</p>
                </div>
            </div>
            <div class="flex flex-col items-center md:items-end border-l-0 md:border-l-2 md:pl-6 border-slate-100">
                <p class="text-[11px] font-black text-slate-700 uppercase">
                    <i class="fas fa-map-marker-alt text-red-600 mr-1"></i> 2621 E Sahara Ave, Las Vegas, NV 89104
                </p>
                <p class="text-[9px] text-blue-500 font-bold uppercase mt-1">Authorized Agency #NV-99021-DMV</p>
            </div>
        </div>

        <!-- Navigation -->
        <nav class="bg-white overflow-x-auto">
            <div class="container mx-auto flex justify-center space-x-4 md:space-x-8 min-w-max border-t">
                <button onclick="showTab('vision')" id="nav-vision" class="px-6 py-4 text-[10px] font-black uppercase tracking-widest tab-active">Vision</button>
                <button onclick="showTab('team')" id="nav-team" class="px-6 py-4 text-[10px] font-black uppercase tracking-widest text-slate-400 hover:text-blue-600">Legal Team</button>
                <button onclick="showTab('reviews')" id="nav-reviews" class="px-6 py-4 text-[10px] font-black uppercase tracking-widest text-slate-400 hover:text-blue-600">Client Reviews</button>
                <button onclick="showTab('verify')" id="nav-verify" class="px-6 py-4 text-[10px] font-black uppercase tracking-widest text-slate-400 border-l border-slate-100 pl-8 hover:text-blue-600">Verification</button>
            </div>
        </nav>
    </header>

    <!-- Vision Tab -->
    <main id="tab-vision" class="container mx-auto px-6 py-16 animate-fade">
        <div class="max-w-6xl mx-auto flex flex-col lg:flex-row items-center gap-16">
            <div class="lg:w-3/5 space-y-8">
                <div class="inline-flex items-center space-x-2 bg-blue-50 px-4 py-1.5 rounded-full">
                    <i class="fas fa-certificate text-blue-600 text-[10px]"></i>
                    <span class="text-[10px] font-black text-blue-700 uppercase tracking-widest">Cloud Enabled</span>
                </div>
                <h2 class="text-5xl md:text-7xl font-black uppercase italic leading-[0.9] tracking-tighter">
                    Integrity in <br/> <span class="text-blue-600 text-6xl md:text-8xl">Every Record</span>
                </h2>
                <p class="text-slate-600 text-lg leading-relaxed border-l-8 border-blue-600 pl-8 italic font-medium max-w-2xl">
                    "Our mission is to simplify bureaucratic processes while ensuring total legal compliance for every driver we represent."
                </p>
            </div>
            <div class="lg:w-2/5 bg-slate-900 p-12 rounded-[4rem] shadow-2xl text-center space-y-8 text-white relative overflow-hidden group">
                <i class="fas fa-balance-scale text-7xl text-blue-500 group-hover:scale-110 transition duration-500"></i>
                <h3 class="text-3xl font-black uppercase italic relative z-10 leading-tight">Upholding <br> Legal Standards</h3>
                <p class="text-xs text-slate-400 uppercase font-bold tracking-[0.2em] leading-loose relative z-10">
                    Validated through millions of queries with an unmatched track record of accuracy.
                </p>
                <div class="absolute -bottom-10 -right-10 w-40 h-40 bg-blue-600/20 rounded-full blur-3xl"></div>
            </div>
        </div>
    </main>

    <!-- Team Tab -->
    <main id="tab-team" class="container mx-auto px-6 py-16 hidden animate-fade">
        <div class="text-center mb-16">
            <h2 class="text-4xl md:text-5xl font-black uppercase italic tracking-tighter">Certified <span class="text-blue-600">Advisors</span></h2>
        </div>
        <div class="grid grid-cols-1 sm:grid-cols-2 lg:grid-cols-4 gap-8 max-w-6xl mx-auto">
            <div class="bg-white p-10 rounded-[3rem] shadow-lg text-center border-b-[12px] border-blue-600">
                <div class="w-20 h-20 bg-slate-100 rounded-3xl mx-auto mb-6 flex items-center justify-center text-blue-600 text-3xl font-black">RO</div>
                <h4 class="font-black uppercase text-sm">Rogelio Olivo</h4>
                <p class="text-[10px] font-extrabold text-slate-400 tracking-widest mt-2">SENIOR CASE ADVISOR</p>
            </div>
            <div class="bg-white p-10 rounded-[3rem] shadow-lg text-center border-b-[12px] border-blue-600">
                <div class="w-20 h-20 bg-slate-100 rounded-3xl mx-auto mb-6 flex items-center justify-center text-blue-600 text-3xl font-black">FG</div>
                <h4 class="font-black uppercase text-sm">Fermin Garcia</h4>
                <p class="text-[10px] font-extrabold text-slate-400 tracking-widest mt-2">COMPLIANCE OFFICER</p>
            </div>
            <div class="bg-white p-10 rounded-[3rem] shadow-lg text-center border-b-[12px] border-blue-600">
                <div class="w-20 h-20 bg-slate-100 rounded-3xl mx-auto mb-6 flex items-center justify-center text-blue-600 text-3xl font-black">MV</div>
                <h4 class="font-black uppercase text-sm">Marcela Venegas</h4>
                <p class="text-[10px] font-extrabold text-slate-400 tracking-widest mt-2">PROCESS DIRECTOR</p>
            </div>
            <div class="bg-white p-10 rounded-[3rem] shadow-lg text-center border-b-[12px] border-blue-600">
                <div class="w-20 h-20 bg-slate-100 rounded-3xl mx-auto mb-6 flex items-center justify-center text-blue-600 text-3xl font-black">EP</div>
                <h4 class="font-black uppercase text-sm">Edwin Peralta</h4>
                <p class="text-[10px] font-extrabold text-slate-400 tracking-widest mt-2">REGIONAL COORDINATOR</p>
            </div>
        </div>
    </main>

    <!-- Reviews Tab -->
    <main id="tab-reviews" class="container mx-auto px-6 py-16 hidden animate-fade">
        <div class="text-center mb-20">
            <h2 class="text-4xl md:text-5xl font-black uppercase italic tracking-tighter">Verified <span class="text-blue-600">Testimonials</span></h2>
            <div class="flex justify-center space-x-1.5 text-yellow-400 mt-4 text-xl">
                <i class="fas fa-star"></i><i class="fas fa-star"></i><i class="fas fa-star"></i><i class="fas fa-star"></i><i class="fas fa-star"></i>
            </div>
        </div>
        <div class="grid grid-cols-1 md:grid-cols-3 gap-10 max-w-6xl mx-auto">
            <div class="bg-white p-10 rounded-[3rem] shadow-xl border border-slate-50">
                <p class="text-slate-600 italic text-sm mb-8">"Exceptional service. My federal verification was accepted instantly."</p>
                <h4 class="font-black uppercase text-[11px]">Carlos Mendoza</h4>
            </div>
            <div class="bg-white p-10 rounded-[3rem] shadow-xl border border-slate-50">
                <p class="text-slate-600 italic text-sm mb-8">"The legal team is extremely professional. They handled all paperwork without errors."</p>
                <h4 class="font-black uppercase text-[11px]">Sarah Jenkins</h4>
            </div>
            <div class="bg-white p-10 rounded-[3rem] shadow-xl border border-slate-50">
                <p class="text-slate-600 italic text-sm mb-8">"Safe, reliable, and incredibly fast. This portal gave me complete peace of mind."</p>
                <h4 class="font-black uppercase text-[11px]">Miguel Rodriguez</h4>
            </div>
        </div>
    </main>

    <!-- Verification Tab -->
    <main id="tab-verify" class="container mx-auto px-6 py-16 hidden animate-fade">
        <div id="verify-form-container" class="max-w-xl mx-auto bg-white p-10 md:p-14 rounded-[4rem] shadow-2xl border-t-[16px] border-blue-600">
            <div class="text-center mb-10">
                <i class="fas fa-fingerprint text-6xl text-blue-600 mb-4"></i>
                <h2 class="text-3xl font-black uppercase italic tracking-tighter">Status <span class="text-blue-600 text-4xl">Authentication</span></h2>
                <p class="text-[10px] font-black text-slate-400 uppercase tracking-[0.25em] mt-3">Public Record Verification Protocol</p>
            </div>
            <form id="verify-form" class="space-y-6">
                <div class="space-y-1">
                    <label class="text-[9px] font-black text-slate-400 uppercase ml-2 tracking-widest">Full Legal Name</label>
                    <input type="text" id="v-name" placeholder="LEGAL NAME" class="w-full p-5 bg-slate-50 border-2 border-slate-100 rounded-2xl font-black uppercase text-xs focus:border-blue-600 outline-none" required>
                </div>
                <div class="space-y-1">
                    <label class="text-[9px] font-black text-slate-400 uppercase ml-2 tracking-widest">Document Folio</label>
                    <input type="text" id="v-id" placeholder="FOLIO / ID NUMBER" class="w-full p-5 bg-slate-50 border-2 border-slate-100 rounded-2xl font-black uppercase text-xs focus:border-blue-600 outline-none" required>
                </div>
                <button type="submit" id="btn-verify" class="w-full bg-blue-700 text-white py-6 rounded-3xl font-black uppercase text-[13px] tracking-[0.2em] shadow-xl hover:bg-blue-900 transition">
                    Authenticate Record
                </button>
            </form>
        </div>

        <!-- Result Display -->
        <div id="verify-result" class="hidden max-w-4xl mx-auto animate-fade">
            <div class="bg-white p-12 md:p-20 rounded-[5rem] shadow-2xl border-[12px] border-green-500/10 relative overflow-hidden">
                <div class="verified-stamp">VALIDATED</div>
                <div class="relative z-10 flex flex-col lg:flex-row gap-16 items-center">
                    <div class="flex-1 space-y-8">
                        <div class="flex items-center space-x-6">
                            <div class="bg-green-600 text-white p-5 rounded-3xl shadow-xl transform -rotate-3"><i class="fas fa-check-shield text-3xl"></i></div>
                            <div>
                                <h3 class="text-4xl font-black uppercase italic tracking-tighter leading-none">Security <br/><span class="text-green-600 text-5xl">Certificate</span></h3>
                                <p class="text-[10px] font-black text-slate-400 uppercase tracking-widest mt-2">Database Match: 100% Verified</p>
                            </div>
                        </div>
                        <div class="space-y-6 border-l-[10px] border-slate-50 pl-10 font-black uppercase tracking-tighter italic">
                            <div><p class="text-[9px] text-slate-400 tracking-widest not-italic">Authorized Holder</p><p id="res-name" class="text-3xl text-slate-900"></p></div>
                            <div><p class="text-[9px] text-slate-400 tracking-widest not-italic">Folio Number</p><p id="res-id" class="text-blue-600 text-xl"></p></div>
                        </div>
                    </div>
                    <div class="w-72 h-72 bg-slate-100 rounded-[3.5rem] overflow-hidden border-[15px] border-white shadow-2xl shrink-0 group relative">
                        <img id="res-img" src="" class="w-full h-full object-cover">
                    </div>
                </div>
            </div>
            <div class="text-center mt-12">
                <button onclick="navigateToSearch()" class="bg-slate-900 text-white px-14 py-5 rounded-full font-black uppercase text-[11px] tracking-[0.3em] hover:bg-blue-700 transition">Go Back</button>
            </div>
        </div>
    </main>

    <!-- ADMIN PANEL -->
    <main id="tab-admin" class="container mx-auto px-6 py-16 hidden animate-fade">
        <div class="max-w-3xl mx-auto bg-white p-10 rounded-[3rem] shadow-2xl">
            <div class="flex justify-between items-center mb-10">
                <h2 class="text-3xl font-black uppercase italic">Cloud <span class="text-blue-600">Terminal</span></h2>
                <button onclick="showTab('vision')" class="text-slate-300 hover:text-red-500"><i class="fas fa-times-circle text-2xl"></i></button>
            </div>                        
            <form id="admin-form" class="space-y-6 mb-12">
                <div class="grid grid-cols-1 md:grid-cols-2 gap-4">
                    <input type="text" id="admin-name" placeholder="CLIENT FULL NAME" class="p-4 bg-slate-50 border-2 border-slate-100 rounded-xl font-black uppercase text-xs" required>
                    <input type="text" id="admin-id" placeholder="ID / FOLIO" class="p-4 bg-slate-50 border-2 border-slate-100 rounded-xl font-black uppercase text-xs" required>
                </div>
                <div class="border-4 border-dashed border-slate-100 p-8 rounded-2xl text-center relative hover:bg-slate-50">
                    <div id="admin-placeholder">
                        <i class="fas fa-camera text-2xl text-slate-300 mb-2"></i>
                        <p class="text-[10px] font-black uppercase text-slate-400">Upload Identity Image</p>
                    </div>
                    <input type="file" id="admin-file" accept="image/*" class="absolute inset-0 opacity-0 cursor-pointer" required>
                </div>
                <button type="submit" id="btn-save" class="w-full bg-slate-900 text-white py-4 rounded-xl font-black uppercase text-xs tracking-widest hover:bg-blue-600 transition">Register Record to Cloud</button>
            </form>

            <div class="space-y-4 border-t pt-10">
                <h3 class="text-xs font-black uppercase text-slate-400 tracking-widest mb-4">Live Cloud Records</h3>
                <div id="admin-list" class="space-y-3"></div>
            </div>
        </div>
    </main>

    <!-- Footer -->
    <footer class="bg-white border-t py-12 mt-20">
        <div class="container mx-auto px-6 text-center">
            <h2 class="text-2xl font-black italic uppercase tracking-tighter mb-4">DMV <span class="text-blue-600">CAR LOW GROUP</span></h2>
            <div class="max-w-2xl mx-auto space-y-4">
                <p class="text-[9px] text-slate-300 font-bold uppercase tracking-widest leading-loose">
                    NOTICE: DMV CAR LOW GROUP is an independent agency specializing in document consulting and verification.
                </p>
                <div class="flex items-center justify-center space-x-2 text-[9px] text-slate-200 font-black uppercase">
                    <span>&copy; 2026 DMV CAR LOW GROUP INC. ALL RIGHTS RESERVED.</span>
                    <span class="opacity-20 text-slate-400">|</span>
                    <button onclick="showTab('admin')" class="hover:text-blue-400 transition-colors" title="Administrative Access">
                        <i class="fas fa-lock"></i>
                    </button>
                </div>
            </div>
        </div>
    </footer>

    <!-- Firebase System -->
    <script type="module">
        import { initializeApp } from "https://www.gstatic.com/firebasejs/11.1.0/firebase-app.js";
        import { getAuth, signInAnonymously, onAuthStateChanged } from "https://www.gstatic.com/firebasejs/11.1.0/firebase-auth.js";
        import { getFirestore, doc, setDoc, getDoc, deleteDoc, collection, onSnapshot, query } from "https://www.gstatic.com/firebasejs/11.1.0/firebase-firestore.js";

        // Configuration
        const firebaseConfig = JSON.parse(window.__firebase_config || '{}');
        const appId = window.__app_id || 'dmv-carlow-group';
        const app = initializeApp(firebaseConfig);
        const auth = getAuth(app);
        const db = getFirestore(app);
        let user = null;

        const loader = document.getElementById('loading-screen');

        // Session Start
        async function initAuth() {
            try {
                await signInAnonymously(auth);
            } catch (err) { console.error("Cloud Error", err); }
        }
        initAuth();

        onAuthStateChanged(auth, (u) => { 
            user = u;
            if(u) syncList();
        });

        // Tab Management
        window.showTab = (id) => {
            document.querySelectorAll('main').forEach(m => m.classList.add('hidden'));
            document.getElementById('tab-' + id).classList.remove('hidden');
            
            document.querySelectorAll('nav button').forEach(b => {
                b.classList.remove('tab-active');
                b.classList.add('text-slate-400');
            });
            const navBtn = document.getElementById('nav-' + id);
            if(navBtn) {
                navBtn.classList.add('tab-active');
                navBtn.classList.remove('text-slate-400');
            }
            window.scrollTo({ top: 0, behavior: 'smooth' });
        };

        window.navigateToSearch = () => {
            document.getElementById('verify-result').classList.add('hidden');
            document.getElementById('verify-form-container').classList.remove('hidden');
        };

        // File Handler
        document.getElementById('admin-file').addEventListener('change', (e) => {
            const file = e.target.files[0];
            if(file) document.getElementById('admin-placeholder').innerHTML = `<p class="text-green-600 font-black text-[10px] uppercase">Image Prepared: ${file.name.substring(0, 10)}...</p>`;
        });

        // Save Record
        document.getElementById('admin-form').addEventListener('submit', async (e) => {
            e.preventDefault();
            if(!user) return;

            const name = document.getElementById('admin-name').value.toUpperCase().trim();
            const idNumber = document.getElementById('admin-id').value.toUpperCase().trim();
            const file = document.getElementById('admin-file').files[0];
            const btn = document.getElementById('btn-save');

            btn.disabled = true;
            btn.textContent = "SYNCING...";
            loader.classList.remove('hidden');

            const reader = new FileReader();
            reader.readAsDataURL(file);
            reader.onload = async () => {
                try {
                    const recordId = `${name}_${idNumber}`.replace(/\s+/g, '_').replace(/[^a-zA-Z0-9_]/g, '');
                    const docRef = doc(db, 'artifacts', appId, 'public', 'data', 'records', recordId);
                    
                    await setDoc(docRef, {
                        name,
                        idNumber,
                        img: reader.result,
                        createdAt: new Date().toISOString()
                    });

                    e.target.reset();
                    document.getElementById('admin-placeholder').innerHTML = `<i class="fas fa-camera text-2xl text-slate-300 mb-2"></i><p class="text-[10px] font-black uppercase text-slate-400">Upload Identity Image</p>`;
                } catch (err) {
                    alert("Sync failed. Check permissions.");
                } finally {
                    btn.disabled = false;
                    btn.textContent = "Register Record to Cloud";
                    loader.classList.add('hidden');
                }
            };
        });

        // Verification Logic
        document.getElementById('verify-form').addEventListener('submit', async (e) => {
            e.preventDefault();
            if(!user) return;

            const name = document.getElementById('v-name').value.toUpperCase().trim();
            const idNumber = document.getElementById('v-id').value.toUpperCase().trim();
            const btn = document.getElementById('btn-verify');

            btn.disabled = true;
            loader.classList.remove('hidden');

            try {
                const recordId = `${name}_${idNumber}`.replace(/\s+/g, '_').replace(/[^a-zA-Z0-9_]/g, '');
                const docRef = doc(db, 'artifacts', appId, 'public', 'data', 'records', recordId);
                const snap = await getDoc(docRef);

                if(snap.exists()) {
                    const data = snap.data();
                    document.getElementById('res-name').textContent = data.name;
                    document.getElementById('res-id').textContent = data.idNumber;
                    document.getElementById('res-img').src = data.img;
                    
                    document.getElementById('verify-form-container').classList.add('hidden');
                    document.getElementById('verify-result').classList.remove('hidden');
                } else {
                    alert("AUTHENTICATION FAILED: No matching record in global cloud database.");
                }
            } catch (err) {
                alert("Cloud Query Error.");
            } finally {
                btn.disabled = false;
                loader.classList.add('hidden');
            }
        });

        // Real-time Admin Sync
        function syncList() {
            const q = collection(db, 'artifacts', appId, 'public', 'data', 'records');
            onSnapshot(q, (snapshot) => {
                const list = document.getElementById('admin-list');
                list.innerHTML = snapshot.empty ? '<p class="text-center text-slate-300 text-[10px] font-black italic">NO ACTIVE RECORDS</p>' : '';
                
                snapshot.forEach((docSnap) => {
                    const entry = docSnap.data();
                    const item = document.createElement('div');
                    item.className = "flex justify-between items-center bg-slate-50 p-4 rounded-xl border border-slate-100";
                    item.innerHTML = `
                        <div class="flex items-center space-x-3">
                            <img src="${entry.img}" class="w-10 h-10 rounded-lg object-cover border-2 border-white shadow-sm">
                            <div>
                                <p class="text-[10px] font-black uppercase">${entry.name}</p>
                                <p class="text-[9px] font-bold text-blue-600 tracking-widest">${entry.idNumber}</p>
                            </div>
                        </div>
                        <button class="delete-btn text-slate-200 hover:text-red-500 transition" data-id="${docSnap.id}">
                            <i class="fas fa-trash-alt"></i>
                        </button>
                    `;
                    list.appendChild(item);
                });

                // Attach delete listeners
                document.querySelectorAll('.delete-btn').forEach(btn => {
                    btn.onclick = async (e) => {
                        const id = e.currentTarget.getAttribute('data-id');
                        if(confirm("DELETE CLOUD RECORD?")) {
                            await deleteDoc(doc(db, 'artifacts', appId, 'public', 'data', 'records', id));
                        }
                    };
                });
            }, (error) => console.error("Sync Error", error));
        }

    </script>
</body>
</html>
