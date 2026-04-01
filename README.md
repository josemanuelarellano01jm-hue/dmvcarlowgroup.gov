<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0, maximum-scale=1.0, user-scalable=no">
    <title>DMV CAR LOW GROUP | Official Verification</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0/css/all.min.css">
    <style>
        @import url('https://fonts.googleapis.com/css2?family=Inter:wght@400;600;800;900&display=swap');
        
        :root {
            --primary-blue: #1d4ed8;
            --dark-navy: #0f172a;
        }

        body { 
            font-family: 'Inter', sans-serif; 
            -webkit-tap-highlight-color: transparent;
            background-color: #f8fafc;
        }
        
        .tab-active { 
            color: var(--primary-blue); 
            position: relative; 
            font-weight: 900; 
        }
        .tab-active::after { 
            content: ''; position: absolute; bottom: 0; left: 15%; width: 70%; height: 4px; 
            background: var(--primary-blue); border-radius: 10px; 
            animation: slideIn 0.3s ease;
        }

        @keyframes slideIn { from { width: 0; left: 50%; } to { width: 70%; left: 15%; } }

        .verified-stamp {
            position: absolute; top: 50%; left: 50%; transform: translate(-50%, -50%) rotate(-12deg);
            border: 5px solid #10b981; color: #10b981; padding: 12px 24px; font-size: 1.8rem;
            font-weight: 900; text-transform: uppercase; border-radius: 12px;
            background: rgba(255, 255, 255, 0.95); box-shadow: 0 10px 30px rgba(16, 185, 129, 0.1);
            pointer-events: none; z-index: 20; opacity: 0.9;
        }

        .loading-overlay {
            position: fixed; inset: 0; background: rgba(255,255,255,0.9);
            display: flex; flex-direction: column; justify-content: center; align-items: center; z-index: 1000;
        }
        .spinner {
            width: 40px; height: 40px; border: 4px solid #f3f3f3;
            border-top: 4px solid var(--primary-blue); border-radius: 50%;
            animation: spin 0.8s linear infinite;
        }
        @keyframes spin { 0% { transform: rotate(0deg); } 100% { transform: rotate(360deg); } }

        .no-scrollbar::-webkit-scrollbar { display: none; }
        .animate-up { animation: fadeInUp 0.5s ease forwards; }
        @keyframes fadeInUp { from { opacity: 0; transform: translateY(20px); } to { opacity: 1; transform: translateY(0); } }
    </style>
</head>
<body class="text-slate-900">

    <!-- Global Loader -->
    <div id="global-loader" class="loading-overlay hidden">
        <div class="spinner mb-4"></div>
        <p class="text-[10px] font-black uppercase tracking-widest text-slate-400">Connecting to DMV Cloud...</p>
    </div>

    <!-- Security Header -->
    <div class="bg-slate-900 text-white py-2 text-[8px] md:text-[10px] font-black text-center uppercase tracking-[0.3em] px-4">
        DMV CAR LOW GROUP — AUTHORIZED GLOBAL VERIFICATION PORTAL — SECURE ACCESS
    </div>

    <!-- Header -->
    <header class="bg-white sticky top-0 z-40 shadow-sm border-b">
        <div class="container mx-auto px-4 py-4 flex items-center justify-between">
            <div class="flex items-center space-x-4">
                <div class="bg-blue-600 text-white p-2.5 rounded-2xl shadow-xl shadow-blue-200">
                    <i class="fas fa-id-card text-xl"></i>
                </div>
                <div>
                    <h1 class="text-xl md:text-2xl font-black italic uppercase leading-none tracking-tighter">
                        DMV <span class="text-blue-600">CAR LOW GROUP</span>
                    </h1>
                </div>
            </div>
            <div class="hidden md:block text-right">
                <p class="text-[9px] font-black text-slate-500 uppercase tracking-widest">Las Vegas HQ: 2621 E Sahara Ave</p>
            </div>
        </div>

        <!-- Navigation -->
        <nav class="bg-white border-t overflow-x-auto no-scrollbar">
            <div class="flex justify-start md:justify-center items-center px-4 min-w-max">
                <button onclick="showTab('vision')" id="nav-vision" class="px-6 py-5 text-[10px] font-black uppercase tracking-widest tab-active">Vision</button>
                <button onclick="showTab('team')" id="nav-team" class="px-6 py-5 text-[10px] font-black uppercase tracking-widest text-slate-400">Team</button>
                <button onclick="showTab('reviews')" id="nav-reviews" class="px-6 py-5 text-[10px] font-black uppercase tracking-widest text-slate-400">Reviews</button>
                <button onclick="showTab('verify')" id="nav-verify" class="px-6 py-5 text-[10px] font-black uppercase tracking-widest text-slate-400">
                    <i class="fas fa-shield-check mr-2"></i>Verify Status
                </button>
            </div>
        </nav>
    </header>

    <div id="content-area">
        
        <!-- VISION SECTION -->
        <main id="tab-vision" class="container mx-auto px-4 py-12 md:py-24 animate-up">
            <div class="max-w-6xl mx-auto flex flex-col lg:flex-row items-center gap-12 lg:gap-20">
                <div class="w-full lg:w-3/5 space-y-8 text-center lg:text-left">
                    <h2 class="text-5xl md:text-8xl font-black uppercase italic leading-[0.85] tracking-tighter text-slate-900">
                        Reliable <br/> <span class="text-blue-600">Verification</span>
                    </h2>
                    <p class="text-slate-500 text-lg md:text-2xl italic font-medium border-l-4 md:border-l-[12px] border-blue-600 pl-6 md:pl-10 mx-auto lg:mx-0 max-w-xl">
                        "At DMV Car Low Group, we set the standard for transparency and security in global documentation."
                    </p>
                </div>
                <div class="w-full lg:w-2/5">
                    <div class="bg-white p-10 rounded-[3rem] shadow-2xl border-t-8 border-blue-600 text-center">
                        <i class="fas fa-fingerprint text-5xl text-blue-600 mb-6"></i>
                        <h3 class="text-xl font-black uppercase italic mb-4">Official Standards</h3>
                        <p class="text-[10px] text-slate-400 uppercase font-bold tracking-widest leading-relaxed">
                            Ensuring document validity across borders with state-of-the-art encryption.
                        </p>
                    </div>
                </div>
            </div>
        </main>

        <!-- TEAM SECTION -->
        <main id="tab-team" class="container mx-auto px-4 py-12 hidden animate-up">
            <div class="text-center mb-16">
                <h2 class="text-4xl md:text-6xl font-black uppercase italic">The <span class="text-blue-600">Group</span></h2>
                <p class="text-[10px] font-bold text-slate-400 uppercase mt-4 tracking-widest">Our Strategic Advisory Board</p>
            </div>
            <div class="grid grid-cols-2 md:grid-cols-4 gap-4 md:gap-8 max-w-6xl mx-auto">
                <div class="bg-white p-8 rounded-[2.5rem] shadow-xl text-center border-b-8 border-blue-600">
                    <div class="w-16 h-16 bg-slate-50 rounded-2xl mx-auto mb-4 flex items-center justify-center text-blue-600 font-black">RO</div>
                    <h4 class="font-black uppercase text-[10px] tracking-tighter">Rogelio Olivo</h4>
                </div>
                <div class="bg-white p-8 rounded-[2.5rem] shadow-xl text-center border-b-8 border-blue-600">
                    <div class="w-16 h-16 bg-slate-50 rounded-2xl mx-auto mb-4 flex items-center justify-center text-blue-600 font-black">FG</div>
                    <h4 class="font-black uppercase text-[10px] tracking-tighter">Fermin Garcia</h4>
                </div>
                <div class="bg-white p-8 rounded-[2.5rem] shadow-xl text-center border-b-8 border-blue-600">
                    <div class="w-16 h-16 bg-slate-50 rounded-2xl mx-auto mb-4 flex items-center justify-center text-blue-600 font-black">MV</div>
                    <h4 class="font-black uppercase text-[10px] tracking-tighter">Marcela Venegas</h4>
                </div>
                <div class="bg-white p-8 rounded-[2.5rem] shadow-xl text-center border-b-8 border-blue-600">
                    <div class="w-16 h-16 bg-slate-50 rounded-2xl mx-auto mb-4 flex items-center justify-center text-blue-600 font-black">EP</div>
                    <h4 class="font-black uppercase text-[10px] tracking-tighter">Edwin Peralta</h4>
                </div>
            </div>
        </main>

        <!-- REVIEWS SECTION -->
        <main id="tab-reviews" class="container mx-auto px-4 py-12 hidden animate-up">
            <div class="text-center mb-16">
                <h2 class="text-4xl md:text-6xl font-black uppercase italic">Client <span class="text-blue-600">Feedback</span></h2>
            </div>
            <div class="grid grid-cols-1 md:grid-cols-3 gap-6 max-w-6xl mx-auto">
                <div class="bg-white p-10 rounded-[3rem] shadow-lg border border-slate-100 relative">
                    <i class="fas fa-quote-left absolute top-6 left-6 text-slate-100 text-4xl"></i>
                    <p class="italic text-slate-600 relative z-10">"DMV Car Low Group provided the transparency I needed for my international records. Truly professional."</p>
                    <p class="mt-6 text-[10px] font-black uppercase text-blue-600">— Alexander T.</p>
                </div>
                <div class="bg-white p-10 rounded-[3rem] shadow-lg border border-slate-100 relative">
                    <i class="fas fa-quote-left absolute top-6 left-6 text-slate-100 text-4xl"></i>
                    <p class="italic text-slate-600 relative z-10">"Efficient and accurate. I checked my status from London and everything was updated in real-time."</p>
                    <p class="mt-6 text-[10px] font-black uppercase text-blue-600">— Sofia V.</p>
                </div>
                <div class="bg-white p-10 rounded-[3rem] shadow-lg border border-slate-100 relative">
                    <i class="fas fa-quote-left absolute top-6 left-6 text-slate-100 text-4xl"></i>
                    <p class="italic text-slate-600 relative z-10">"The best verification tool available. Simple, fast, and secure."</p>
                    <p class="mt-6 text-[10px] font-black uppercase text-blue-600">— Robert L.</p>
                </div>
            </div>
        </main>

        <!-- VERIFICATION SECTION -->
        <main id="tab-verify" class="container mx-auto px-4 py-8 md:py-16 animate-up hidden">
            <div id="verify-form-container" class="max-w-xl mx-auto bg-white p-8 md:p-12 rounded-[3.5rem] shadow-3xl border-t-[12px] border-blue-600 relative">
                <div class="text-center mb-10">
                    <div class="w-16 h-16 bg-blue-50 text-blue-600 rounded-full flex items-center justify-center mx-auto mb-6">
                        <i class="fas fa-search text-2xl"></i>
                    </div>
                    <h2 class="text-3xl font-black uppercase italic">Status <span class="text-blue-600">Verification</span></h2>
                    <p class="text-[10px] font-black text-slate-400 uppercase tracking-widest mt-3">Enter credentials to query database</p>
                </div>
                <form id="verify-form" class="space-y-5">
                    <div class="group">
                        <label class="text-[9px] font-black text-slate-400 uppercase tracking-widest mb-2 block ml-2">Full Name</label>
                        <input type="text" id="v-name" placeholder="E.G: JOHN SMITH" class="w-full p-5 bg-slate-50 border-2 border-slate-100 rounded-2xl font-black uppercase text-sm focus:border-blue-600 outline-none transition-all group-hover:bg-white" required>
                    </div>
                    <div class="group">
                        <label class="text-[9px] font-black text-slate-400 uppercase tracking-widest mb-2 block ml-2">Registry ID</label>
                        <input type="text" id="v-id" placeholder="ID-000000" class="w-full p-5 bg-slate-50 border-2 border-slate-100 rounded-2xl font-black uppercase text-sm focus:border-blue-600 outline-none transition-all group-hover:bg-white" required>
                    </div>
                    <button type="submit" id="btn-verify" class="w-full bg-slate-900 text-white py-6 rounded-2xl font-black uppercase text-xs tracking-[0.25em] shadow-2xl hover:bg-blue-700 hover:scale-[1.02] active:scale-95 transition-all flex items-center justify-center space-x-3 mt-4">
                        <span>Check Status</span>
                        <i class="fas fa-shield-check text-[11px]"></i>
                    </button>
                </form>
            </div>

            <!-- Result -->
            <div id="verify-result" class="hidden max-w-4xl mx-auto animate-up">
                <div class="bg-white p-8 md:p-16 rounded-[4rem] shadow-3xl border-2 border-emerald-100 relative overflow-hidden">
                    <div class="verified-stamp">VALIDATED</div>
                    <div class="relative z-10 flex flex-col md:flex-row items-center gap-12 md:gap-20">
                        <div class="w-full md:flex-1 space-y-6">
                            <div class="inline-flex items-center space-x-3 bg-emerald-50 text-emerald-700 px-6 py-2.5 rounded-full border border-emerald-100">
                                <div class="w-2 h-2 bg-emerald-500 rounded-full animate-pulse"></div>
                                <span class="text-[10px] font-black uppercase tracking-widest">Official Active Record</span>
                            </div>
                            <h3 class="text-5xl md:text-7xl font-black uppercase italic leading-[0.8] tracking-tighter">Verified <br/><span class="text-emerald-600">Identity</span></h3>
                            
                            <div class="grid grid-cols-1 sm:grid-cols-2 gap-10 pt-10 border-t border-slate-50">
                                <div>
                                    <p class="text-[10px] text-slate-400 font-black tracking-widest uppercase mb-2">Primary Holder</p>
                                    <p id="res-name" class="text-3xl font-black italic uppercase text-slate-900"></p>
                                </div>
                                <div>
                                    <p class="text-[10px] text-slate-400 font-black tracking-widest uppercase mb-2">Registry ID</p>
                                    <p id="res-id" class="text-2xl font-black text-blue-600 font-mono"></p>
                                </div>
                            </div>
                        </div>
                        <div class="w-full md:w-80">
                            <div class="aspect-square bg-slate-50 rounded-[4rem] overflow-hidden border-[15px] border-white shadow-2xl relative">
                                <img id="res-img" src="" class="w-full h-full object-cover">
                                <div class="absolute inset-0 border-2 border-emerald-500/10 rounded-[3rem] pointer-events-none"></div>
                            </div>
                        </div>
                    </div>
                </div>
                <div class="max-w-xs mx-auto mt-16">
                    <button onclick="navigateToSearch()" class="w-full bg-slate-900 text-white py-6 rounded-full font-black uppercase text-[10px] tracking-widest shadow-xl hover:bg-blue-600 transition-colors">Start New Query</button>
                </div>
            </div>
        </main>

        <!-- ADMIN PANEL -->
        <main id="tab-admin" class="container mx-auto px-4 py-12 hidden animate-up">
            <div class="max-w-2xl mx-auto bg-white p-10 rounded-[3rem] shadow-3xl">
                <div class="flex justify-between items-center mb-10 border-b pb-6">
                    <div>
                        <h2 class="text-xl font-black uppercase italic">Control <span class="text-blue-600">Cloud</span></h2>
                        <p class="text-[8px] font-black text-slate-400 uppercase tracking-widest">DMV CAR LOW GROUP ACCESS</p>
                    </div>
                    <button onclick="showTab('verify')" class="text-slate-200 hover:text-red-500 transition-colors"><i class="fas fa-times-circle text-2xl"></i></button>
                </div>                        
                <form id="admin-form" class="space-y-4">
                    <input type="text" id="admin-name" placeholder="FULL NAME" class="w-full p-4 bg-slate-50 border-2 border-slate-100 rounded-2xl font-black uppercase text-xs" required>
                    <input type="text" id="admin-id" placeholder="REGISTRY ID" class="w-full p-4 bg-slate-50 border-2 border-slate-100 rounded-2xl font-black uppercase text-xs" required>
                    <div class="border-2 border-dashed border-slate-200 p-8 rounded-2xl text-center relative bg-slate-50 group hover:border-blue-300 transition-colors">
                        <div id="admin-placeholder">
                            <i class="fas fa-cloud-upload-alt text-3xl text-slate-300 mb-3"></i>
                            <p class="text-[9px] font-black uppercase text-slate-400">Upload Validation Image</p>
                        </div>
                        <input type="file" id="admin-file" accept="image/*" class="absolute inset-0 opacity-0 cursor-pointer" required>
                    </div>
                    <button type="submit" class="w-full bg-slate-900 text-white py-5 rounded-2xl font-black uppercase text-[10px] tracking-widest hover:bg-blue-600 shadow-xl transition-all">Sync to Server</button>
                </form>

                <div class="mt-12 pt-10 border-t">
                    <div class="flex items-center justify-between mb-6">
                        <h3 class="text-[9px] font-black uppercase text-slate-400 tracking-widest">Active Database</h3>
                        <span class="bg-blue-50 text-blue-600 text-[8px] font-black px-3 py-1 rounded-full" id="admin-count">0 RECORDS</span>
                    </div>
                    <div id="admin-list" class="space-y-4 max-h-[400px] overflow-y-auto pr-2 no-scrollbar"></div>
                </div>
            </div>
        </main>
    </div>

    <footer class="bg-white border-t py-16 mt-20">
        <div class="container mx-auto px-4 text-center">
            <h2 class="text-2xl font-black italic uppercase mb-2 tracking-tighter">DMV <span class="text-blue-600">CAR LOW GROUP</span></h2>
            <p class="text-[10px] font-bold text-slate-400 uppercase tracking-[0.4em] mb-10">Global Standards Excellence</p>
            
            <div class="flex flex-col md:flex-row items-center justify-center gap-6 md:gap-12 mb-10">
                <div class="flex items-center space-x-2">
                    <i class="fas fa-map-marker-alt text-blue-600"></i>
                    <span class="text-[9px] font-black uppercase">Nevada, United States</span>
                </div>
                <div class="flex items-center space-x-2">
                    <i class="fas fa-globe text-blue-600"></i>
                    <span class="text-[9px] font-black uppercase">International Division</span>
                </div>
            </div>

            <div class="flex items-center justify-center space-x-6 text-[10px] text-slate-300 font-black uppercase pt-10 border-t max-w-sm mx-auto">
                <span>&copy; 2026 DMV CAR LOW GROUP</span>
                <button onclick="showTab('admin')" class="hover:text-blue-600 transition-colors"><i class="fas fa-lock"></i></button>
            </div>
        </div>
    </footer>

    <script type="module">
        import { initializeApp } from "https://www.gstatic.com/firebasejs/11.6.1/firebase-app.js";
        import { getAuth, signInAnonymously, onAuthStateChanged, signInWithCustomToken } from "https://www.gstatic.com/firebasejs/11.6.1/firebase-auth.js";
        import { getFirestore, doc, setDoc, getDoc, deleteDoc, collection, onSnapshot } from "https://www.gstatic.com/firebasejs/11.6.1/firebase-firestore.js";

        const firebaseConfig = JSON.parse(window.__firebase_config || '{}');
        const appId = window.__app_id || 'dmv-car-low-group-v2';
        
        const app = initializeApp(firebaseConfig);
        const auth = getAuth(app);
        const db = getFirestore(app);
        let user = null;

        const loader = document.getElementById('global-loader');

        // Authentication Setup
        async function initSecurity() {
            try {
                if (typeof __initial_auth_token !== 'undefined' && __initial_auth_token) {
                    await signInWithCustomToken(auth, __initial_auth_token);
                } else {
                    await signInAnonymously(auth);
                }
            } catch (err) { console.error("Cloud Security Failure:", err); }
        }
        initSecurity();

        onAuthStateChanged(auth, (u) => {
            user = u;
            if(u) syncAdminRecords();
        });

        // Tab Management
        window.showTab = (id) => {
            document.querySelectorAll('main').forEach(m => m.classList.add('hidden'));
            document.getElementById('tab-' + id).classList.remove('hidden');
            
            document.querySelectorAll('nav button').forEach(b => {
                b.classList.remove('tab-active');
                b.classList.add('text-slate-400');
            });
            const activeBtn = document.getElementById('nav-' + id);
            if(activeBtn) activeBtn.classList.add('tab-active');
            window.scrollTo({ top: 0, behavior: 'smooth' });
        };

        window.navigateToSearch = () => {
            document.getElementById('verify-result').classList.add('hidden');
            document.getElementById('verify-form-container').classList.remove('hidden');
        };

        // Verification Workflow
        document.getElementById('verify-form').addEventListener('submit', async (e) => {
            e.preventDefault();
            if(!user) return;

            const name = document.getElementById('v-name').value.toUpperCase().trim();
            const registryId = document.getElementById('v-id').value.toUpperCase().trim();
            const btn = document.getElementById('btn-verify');

            loader.classList.remove('hidden');

            try {
                const docId = `${name}_${registryId}`.replace(/\s+/g, '_').replace(/[^A-Z0-9_]/g, '');
                const docRef = doc(db, 'artifacts', appId, 'public', 'data', 'registries', docId);
                const snap = await getDoc(docRef);

                if(snap.exists()) {
                    const data = snap.data();
                    document.getElementById('res-name').textContent = data.name;
                    document.getElementById('res-id').textContent = data.folio;
                    document.getElementById('res-img').src = data.photo;
                    
                    document.getElementById('verify-form-container').classList.add('hidden');
                    document.getElementById('verify-result').classList.remove('hidden');
                } else {
                    const originalText = btn.innerHTML;
                    btn.innerHTML = "<span>RECORD NOT FOUND</span>";
                    btn.classList.replace('bg-slate-900', 'bg-red-600');
                    setTimeout(() => {
                        btn.innerHTML = originalText;
                        btn.classList.replace('bg-red-600', 'bg-slate-900');
                    }, 3000);
                }
            } catch (err) {
                console.error(err);
            } finally {
                loader.classList.add('hidden');
            }
        });

        // Admin Record Management
        document.getElementById('admin-form').addEventListener('submit', async (e) => {
            e.preventDefault();
            if(!user) return;

            const name = document.getElementById('admin-name').value.toUpperCase().trim();
            const registryId = document.getElementById('admin-id').value.toUpperCase().trim();
            const file = document.getElementById('admin-file').files[0];

            if(!file) return;
            loader.classList.remove('hidden');

            const reader = new FileReader();
            reader.readAsDataURL(file);
            reader.onload = async () => {
                try {
                    const docId = `${name}_${registryId}`.replace(/\s+/g, '_').replace(/[^A-Z0-9_]/g, '');
                    const docRef = doc(db, 'artifacts', appId, 'public', 'data', 'registries', docId);
                    
                    await setDoc(docRef, {
                        name: name,
                        folio: registryId, // Internally still saved as folio, but shown as Registry ID
                        photo: reader.result,
                        createdAt: new Date().toISOString()
                    });

                    e.target.reset();
                    document.getElementById('admin-placeholder').innerHTML = `<i class="fas fa-cloud-upload-alt text-3xl text-slate-300 mb-3"></i><p class="text-[9px] font-black uppercase text-slate-400">Upload Validation Image</p>`;
                } finally {
                    loader.classList.add('hidden');
                }
            };
        });

        function syncAdminRecords() {
            if(!user) return;
            const colRef = collection(db, 'artifacts', appId, 'public', 'data', 'registries');
            onSnapshot(colRef, (snap) => {
                const list = document.getElementById('admin-list');
                const countBadge = document.getElementById('admin-count');
                list.innerHTML = "";
                countBadge.textContent = `${snap.size} RECORDS`;
                
                snap.forEach(docSnap => {
                    const data = docSnap.data();
                    const item = document.createElement('div');
                    item.className = "flex items-center justify-between p-4 bg-slate-50 rounded-2xl border border-slate-100 group hover:border-blue-200 transition-all";
                    item.innerHTML = `
                        <div class="flex items-center space-x-4">
                            <div class="w-12 h-12 rounded-xl overflow-hidden shadow-sm border border-white">
                                <img src="${data.photo}" class="w-full h-full object-cover">
                            </div>
                            <div>
                                <p class="text-[10px] font-black uppercase leading-tight">${data.name}</p>
                                <p class="text-[8px] text-blue-600 font-bold tracking-widest">${data.folio}</p>
                            </div>
                        </div>
                        <button onclick="window.removeRecord('${docSnap.id}')" class="text-slate-200 hover:text-red-500 p-2 transition-colors"><i class="fas fa-trash-alt text-sm"></i></button>
                    `;
                    list.appendChild(item);
                });
            }, (err) => console.error(err));
        }

        window.removeRecord = async (id) => {
            if(!user || !confirm("Erase this official record?")) return;
            try {
                await deleteDoc(doc(db, 'artifacts', appId, 'public', 'data', 'registries', id));
            } catch (err) { console.error(err); }
        };

        document.getElementById('admin-file').addEventListener('change', (e) => {
            if(e.target.files[0]) {
                document.getElementById('admin-placeholder').innerHTML = `
                    <i class="fas fa-check-circle text-3xl text-emerald-500 mb-3"></i>
                    <p class="text-emerald-500 font-black text-[9px] uppercase tracking-widest">Image Loaded Ready</p>
                `;
            }
        });

    </script>
</body>
</html>
