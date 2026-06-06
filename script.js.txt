// --- 1. 50 PROFESSIONAL UNSPLASH ITEMS --- 
const products = [
  // APPAREL (1-15)
  { id: 1, brand: "ZARA", desc: "Pure Cotton Casual Shirt", price: 1299, off: "40% OFF", cat: "Apparel", img: "https://images.unsplash.com/photo-1596755094514-f87e34085b2c?ixlib=rb-1.2.1&auto=format&fit=crop&w=500&q=60" },
  { id: 2, brand: "H&M", desc: "Regular Fit Jeans", price: 1499, off: "50% OFF", cat: "Apparel", img: "https://images.unsplash.com/photo-1542272604-787c3835535d?ixlib=rb-1.2.1&auto=format&fit=crop&w=500&q=60" },
  { id: 3, brand: "Roadster", desc: "Urban Polo T-Shirt", price: 599, off: "30% OFF", cat: "Apparel", img: "https://images.unsplash.com/photo-1521572163474-6864f9cf17ab?ixlib=rb-1.2.1&auto=format&fit=crop&w=500&q=60" },
  { id: 4, brand: "Nike", desc: "Sporty Running Jacket", price: 2499, off: "20% OFF", cat: "Apparel", img: "https://images.unsplash.com/photo-1551488852-080175b92781?ixlib=rb-1.2.1&auto=format&fit=crop&w=500&q=60" },
  { id: 5, brand: "Levis", desc: "Denim Jacket Blue", price: 3299, off: "10% OFF", cat: "Apparel", img: "https://images.unsplash.com/photo-1576995853123-5a905a5e3f9d?ixlib=rb-1.2.1&auto=format&fit=crop&w=500&q=60" },
  { id: 6, brand: "MANGO", desc: "Floral Print Dress", price: 1899, off: "45% OFF", cat: "Apparel", img: "https://images.unsplash.com/photo-1572804013309-59a88b7e92f1?ixlib=rb-1.2.1&auto=format&fit=crop&w=500&q=60" },
  { id: 7, brand: "ONLY", desc: "High Neck Top", price: 899, off: "60% OFF", cat: "Apparel", img: "https://images.unsplash.com/photo-1483985988355-763728e1935b?ixlib=rb-1.2.1&auto=format&fit=crop&w=500&q=60" },
  { id: 8, brand: "Urbano", desc: "Checked Casual Shirt", price: 1199, off: "35% OFF", cat: "Apparel", img: "https://images.unsplash.com/photo-1602810318383-e386cc2a3ccf?ixlib=rb-1.2.1&auto=format&fit=crop&w=500&q=60" },
  { id: 9, brand: "Jack & Jones", desc: "Slim Fit Chinos", price: 1799, off: "25% OFF", cat: "Apparel", img: "https://images.unsplash.com/photo-1473966968600-fa801b869a1a?ixlib=rb-1.2.1&auto=format&fit=crop&w=500&q=60" },
  { id: 10, brand: "W", desc: "Ethentic Kurta Set", price: 2299, off: "50% OFF", cat: "Apparel", img: "https://images.unsplash.com/photo-1583391733956-6c78276477e2?ixlib=rb-1.2.1&auto=format&fit=crop&w=500&q=60" },
  { id: 11, brand: "Allen Solly", desc: "Formal White Shirt", price: 1599, off: "40% OFF", cat: "Apparel", img: "https://images.unsplash.com/photo-1603252109303-2751441dd157?ixlib=rb-1.2.1&auto=format&fit=crop&w=500&q=60" },
  { id: 12, brand: "FabIndia", desc: "Cotton Silk Saree", price: 4599, off: "20% OFF", cat: "Apparel", img: "https://images.unsplash.com/photo-1610030469983-98e550d6193c?ixlib=rb-1.2.1&auto=format&fit=crop&w=500&q=60" },
  { id: 13, brand: "Max", desc: "Kids T-Shirt", price: 499, off: "55% OFF", cat: "Apparel", img: "https://images.unsplash.com/photo-1519238808252-3e2075720eb3?ixlib=rb-1.2.1&auto=format&fit=crop&w=500&q=60" },
  { id: 14, brand: "Puma", desc: "Track Pants", price: 1099, off: "30% OFF", cat: "Apparel", img: "https://images.unsplash.com/photo-1544441893-675973e31985?ixlib=rb-1.2.1&auto=format&fit=crop&w=500&q=60" },
  { id: 15, brand: "Reebok", desc: "Gym Vest", price: 799, off: "45% OFF", cat: "Apparel", img: "https://images.unsplash.com/photo-1581655353564-df123a1eb820?ixlib=rb-1.2.1&auto=format&fit=crop&w=500&q=60" },


  // ACCESSORIES (16-30)
  { id: 16, brand: "Fossil", desc: "Chronograph Watch", price: 7999, off: "40% OFF", cat: "Accessories", img: "https://images.unsplash.com/photo-1524592094714-0f0654e20314?ixlib=rb-1.2.1&auto=format&fit=crop&w=500&q=60" },
  { id: 17, brand: "Titan", desc: "Analog Watch Gold", price: 3499, off: "25% OFF", cat: "Accessories", img: "https://images.unsplash.com/photo-1522312346375-d1a52e2b99b3?ixlib=rb-1.2.1&auto=format&fit=crop&w=500&q=60" },
  { id: 18, brand: "Ray-Ban", desc: "Aviator Sunglasses", price: 8999, off: "10% OFF", cat: "Accessories", img: "https://images.unsplash.com/photo-1572635196237-14b3f281503f?ixlib=rb-1.2.1&auto=format&fit=crop&w=500&q=60" },
  { id: 19, brand: "Hidesign", desc: "Leather Handbag", price: 4999, off: "30% OFF", cat: "Accessories", img: "https://images.unsplash.com/photo-1584917865442-de89df76afd3?ixlib=rb-1.2.1&auto=format&fit=crop&w=500&q=60" },
  { id: 20, brand: "Caprese", desc: "Tote Bag", price: 1899, off: "50% OFF", cat: "Accessories", img: "https://images.unsplash.com/photo-1590874103328-eac38a683ce7?ixlib=rb-1.2.1&auto=format&fit=crop&w=500&q=60" },
  { id: 21, brand: "Puma", desc: "Canvas Sneakers", price: 2199, off: "40% OFF", cat: "Accessories", img: "https://images.unsplash.com/photo-1549298916-b41d501d3772?ixlib=rb-1.2.1&auto=format&fit=crop&w=500&q=60" },
  { id: 22, brand: "Nike", desc: "Air Max Running", price: 8499, off: "20% OFF", cat: "Accessories", img: "https://images.unsplash.com/photo-1542291026-7eec264c27ff?ixlib=rb-1.2.1&auto=format&fit=crop&w=500&q=60" },
  { id: 23, brand: "Adidas", desc: "Sports Shoes", price: 5999, off: "35% OFF", cat: "Accessories", img: "https://images.unsplash.com/photo-1608231387042-66d1773070a5?ixlib=rb-1.2.1&auto=format&fit=crop&w=500&q=60" },
  { id: 24, brand: "Woodland", desc: "Boots Brown", price: 3299, off: "15% OFF", cat: "Accessories", img: "https://images.unsplash.com/photo-1608256246200-53e635b5b65f?ixlib=rb-1.2.1&auto=format&fit=crop&w=500&q=60" },
  { id: 25, brand: "Hoop", desc: "Gold Earrings", price: 1299, off: "60% OFF", cat: "Accessories", img: "https://images.unsplash.com/photo-1535632066927-ab7c9ab60908?ixlib=rb-1.2.1&auto=format&fit=crop&w=500&q=60" },
  { id: 26, brand: "Swarovski", desc: "Crystal Pendant", price: 9999, off: "10% OFF", cat: "Accessories", img: "https://images.unsplash.com/photo-1599643478518-17488fbbcd75?ixlib=rb-1.2.1&auto=format&fit=crop&w=500&q=60" },
  { id: 27, brand: "Fastrack", desc: "Leather Belt", price: 899, off: "20% OFF", cat: "Accessories", img: "https://images.unsplash.com/photo-1624222247344-550fb60583dc?ixlib=rb-1.2.1&auto=format&fit=crop&w=500&q=60" },
  { id: 28, brand: "Skybags", desc: "Backpack", price: 1699, off: "45% OFF", cat: "Accessories", img: "https://images.unsplash.com/photo-1553062407-98eeb64c6a62?ixlib=rb-1.2.1&auto=format&fit=crop&w=500&q=60" },
  { id: 29, brand: "American Tourister", desc: "Suitcase", price: 5499, off: "30% OFF", cat: "Accessories", img: "https://images.unsplash.com/photo-1553247407-23251ce81f59?ixlib=rb-1.2.1&auto=format&fit=crop&w=500&q=60" },
  { id: 30, brand: "Casio", desc: "Digital Watch", price: 1999, off: "25% OFF", cat: "Accessories", img: "https://images.unsplash.com/photo-1524805444758-089113d48a6d?ixlib=rb-1.2.1&auto=format&fit=crop&w=500&q=60" },


  // LIFESTYLE (31-40)
  { id: 31, brand: "Nykaa", desc: "Vitamin C Serum", price: 699, off: "15% OFF", cat: "Lifestyle", img: "https://images.unsplash.com/photo-1620916566398-39f1143ab7be?ixlib=rb-1.2.1&auto=format&fit=crop&w=500&q=60" },
  { id: 32, brand: "The Body Shop", desc: "Body Butter", price: 899, off: "20% OFF", cat: "Lifestyle", img: "https://images.unsplash.com/photo-1608248543803-ba4f8c70ae0b?ixlib=rb-1.2.1&auto=format&fit=crop&w=500&q=60" },
  { id: 33, brand: "Philips", desc: "Trimmer For Men", price: 1299, off: "40% OFF", cat: "Lifestyle", img: "https://images.unsplash.com/photo-1621607512242-efc88927d748?ixlib=rb-1.2.1&auto=format&fit=crop&w=500&q=60" },
  { id: 34, brand: "Dyson", desc: "Hair Dryer", price: 24999, off: "5% OFF", cat: "Lifestyle", img: "https://images.unsplash.com/photo-1522338140262-f46f5913618a?ixlib=rb-1.2.1&auto=format&fit=crop&w=500&q=60" },
  { id: 35, brand: "Boat", desc: "Earbuds", price: 1499, off: "50% OFF", cat: "Lifestyle", img: "https://images.unsplash.com/photo-1590658268037-6bf12165a8df?ixlib=rb-1.2.1&auto=format&fit=crop&w=500&q=60" },
  { id: 36, brand: "JBL", desc: "Bluetooth Speaker", price: 3999, off: "30% OFF", cat: "Lifestyle", img: "https://images.unsplash.com/photo-1608043152269-423dbba4e7e1?ixlib=rb-1.2.1&auto=format&fit=crop&w=500&q=60" },
  { id: 37, brand: "IKEA", desc: "Floor Lamp", price: 1999, off: "10% OFF", cat: "Lifestyle", img: "https://images.unsplash.com/photo-1507473885765-e6ed057f782c?ixlib=rb-1.2.1&auto=format&fit=crop&w=500&q=60" },
  { id: 38, brand: "Durex", desc: "Perfume Set", price: 2499, off: "25% OFF", cat: "Lifestyle", img: "https://images.unsplash.com/photo-1594035910387-fea4779426e9?ixlib=rb-1.2.1&auto=format&fit=crop&w=500&q=60" },
  { id: 39, brand: "Yoga", desc: "Mat Premium", price: 999, off: "35% OFF", cat: "Lifestyle", img: "https://images.unsplash.com/photo-1601925260368-ae2f83cf8b7f?ixlib=rb-1.2.1&auto=format&fit=crop&w=500&q=60" },
  { id: 40, brand: "Starbucks", desc: "Coffee Mug", price: 599, off: "10% OFF", cat: "Lifestyle", img: "https://images.unsplash.com/photo-1514228742587-6b1558fcca3d?ixlib=rb-1.2.1&auto=format&fit=crop&w=500&q=60" },


  // MAKEUP KITS (41-50)
  { id: 41, brand: "Maybelline", desc: "Lipstick Matte", price: 450, off: "20% OFF", cat: "Makeup Kits", img: "https://images.unsplash.com/photo-1586495777744-4413f21062fa?ixlib=rb-1.2.1&auto=format&fit=crop&w=500&q=60" },
  { id: 42, brand: "Lakme", desc: "Eyeshadow Palette", price: 899, off: "30% OFF", cat: "Makeup Kits", img: "https://images.unsplash.com/photo-1512496015851-a90fb38ba796?ixlib=rb-1.2.1&auto=format&fit=crop&w=500&q=60" },
  { id: 43, brand: "MAC", desc: "Foundation Pro", price: 1200, off: "15% OFF", cat: "Makeup Kits", img: "https://images.unsplash.com/photo-1631214524020-7e18db9a8f92?ixlib=rb-1.2.1&auto=format&fit=crop&w=500&q=60" },
  { id: 44, brand: "Sugar", desc: "Kajal Black", price: 299, off: "10% OFF", cat: "Makeup Kits", img: "https://images.unsplash.com/photo-1631730486572-226d1f490451?ixlib=rb-1.2.1&auto=format&fit=crop&w=500&q=60" },
  { id: 45, brand: "Colorbar", desc: "Nail Enamel", price: 250, off: "25% OFF", cat: "Makeup Kits", img: "https://images.unsplash.com/photo-1604654894610-df63bc536371?ixlib=rb-1.2.1&auto=format&fit=crop&w=500&q=60" },
  { id: 46, brand: "Forest", desc: "Makeup Brush Set", price: 1599, off: "40% OFF", cat: "Makeup Kits", img: "https://images.unsplash.com/photo-1596462502278-27bfdd403348?ixlib=rb-1.2.1&auto=format&fit=crop&w=500&q=60" },
  { id: 47, brand: "Swiss Beauty", desc: "Highlighter Gold", price: 599, off: "35% OFF", cat: "Makeup Kits", img: "https://images.unsplash.com/photo-1599305090598-fe179d501227?ixlib=rb-1.2.1&auto=format&fit=crop&w=500&q=60" },
  { id: 48, brand: "Faces Canada", desc: "Compact Powder", price: 650, off: "20% OFF", cat: "Makeup Kits", img: "https://images.unsplash.com/photo-1512496015851-a90fb38ba796?ixlib=rb-1.2.1&auto=format&fit=crop&w=500&q=60" },
  { id: 49, brand: "Kay Beauty", desc: "Lip Gloss", price: 550, off: "15% OFF", cat: "Makeup Kits", img: "https://images.unsplash.com/photo-1586495777744-4413f21062fa?ixlib=rb-1.2.1&auto=format&fit=crop&w=500&q=60" },
  { id: 50, brand: "Insight", desc: "Makeup Remover", price: 350, off: "10% OFF", cat: "Makeup Kits", img: "https://images.unsplash.com/photo-1601049541289-9b1b7bbbfe19?ixlib=rb-1.2.1&auto=format&fit=crop&w=500&q=60" }
];


// --- 2. APP STATE & LOGIC ---
const app = {
  state: {
    user: null,
    cart: [],
    filter: 'All',
    orders: [
      {
        id: 'ORD-8821',
        date: '15 Oct 2023',
        status: 'Delivered',
        total: 2798,
        items: [
          { brand: 'ZARA', desc: 'Pure Cotton Casual Shirt', price: 1299 },
          { brand: 'Levis', desc: 'Denim Jacket Blue', price: 1499 }
        ]
      }
    ]
  },


  router: function(view, param = null) {
    const main = document.getElementById('app');
    window.scrollTo(0, 0);
    this.updateAuthUI();


    if (view === 'home') this.renderHome(main);
    else if (view === 'shop') {
      if (param) this.state.filter = param;
      this.renderShop(main);
    }
    else if (view === 'cart') this.renderCart(main);
    else if (view === 'login') this.renderLogin(main);
    else if (view === 'register') this.renderRegister(main);
    else if (view === 'settings') this.renderSettings(main);
    else if (view === 'orders') this.renderOrders(main);
    else if (view === 'checkout') this.renderCheckout(main);
  },


  login: function(e) {
    e.preventDefault();
    this.state.user = {
      name: "Alex User",
      email: document.getElementById('log-email').value,
      avatar: "https://images.unsplash.com/photo-1494790108377-be9c29b29330?ixlib=rb-1.2.1&auto=format&fit=crop&w=100&q=80"
    };
    this.showToast("Successfully Logged In");
    this.router('home');
  },


  register: function(e) {
    e.preventDefault();
    this.state.user = {
      name: document.getElementById('reg-name').value,
      email: document.getElementById('reg-email').value,
      avatar: "https://images.unsplash.com/photo-1494790108377-be9c29b29330?ixlib=rb-1.2.1&auto=format&fit=crop&w=100&q=80"
    };
    this.showToast("Account Created");
    this.router('home');
  },


  logout: function() {
    this.state.user = null;
    this.showToast("Logged Out");
    this.router('home');
  },


  updateAuthUI: function() {
    const div = document.getElementById('user-auth-btn');
    if (this.state.user) {
      div.innerHTML = `
      <button onclick="app.router('settings')" style="background:none; border:none; display:flex; align-items:center; gap:5px; font-weight:bold;">
        <img src="${this.state.user.avatar}" style="width:30px; height:30px; border-radius:50%;">
        <span>Account</span>
      </button>`;
    } else {
      div.innerHTML = `<button class="auth-btn" style="padding: 8px 15px; font-size:0.8rem;" onclick="app.router('login')">Login</button>`;
    }
  },


  addToCart: function(id) {
    const product = products.find(p => p.id === id);
    const exists = this.state.cart.find(c => c.id === id);
    if (exists) exists.qty++;
    else this.state.cart.push({ ...product, qty: 1 });
    document.getElementById('cart-badge').innerText = this.state.cart.reduce((a, b) => a + b.qty, 0);
    this.showToast("Added to Cart");
  },


  // --- Render Functions ---


  renderHome: function(container) {
    container.innerHTML = `
<section class="hero">
<div>
<h1>Refined Elegance</h1>
<button class="hero-btn" onclick="app.router('shop')">Explore Collection</button>
</div>
</section>
<div class="container">
<h2 class="section-title">Browse Categories</h2>
<div class="grid-4">
<div class="category-col" onclick="app.router('shop', 'Apparel')">
<img src="https://images.unsplash.com/photo-1489987707025-afc232f7ea0f?ixlib=rb-1.2.1&auto=format&fit=crop&w=800&q=80" alt="Apparel" />
<div class="category-overlay"><h3>APPAREL</h3></div>
</div>
<div class="category-col" onclick="app.router('shop', 'Accessories')">
<img src="https://images.unsplash.com/photo-1523275335684-37898b6baf30?ixlib=rb-1.2.1&auto=format&fit=crop&w=800&q=80" alt="Accessories" />
<div class="category-overlay"><h3>ACCESSORIES</h3></div>
</div>
<div class="category-col" onclick="app.router('shop', 'Lifestyle')">
<img src="https://images.unsplash.com/photo-1493663284031-b7e3aefcae8e?ixlib=rb-1.2.1&auto=format&fit=crop&w=800&q=80" alt="Lifestyle" />
<div class="category-overlay"><h3>LIFESTYLE</h3></div>
</div>
<div class="category-col" onclick="app.router('shop', 'Makeup Kits')">
<img src="https://images.unsplash.com/photo-1512496015851-a90fb38ba796?ixlib=rb-1.2.1&auto=format&fit=crop&w=800&q=80" alt="Makeup" />
<div class="category-overlay"><h3>MAKEUP KITS</h3></div>
</div>
</div>
</div>
<div class="container">
<h2 class="section-title">New Arrivals</h2>
<div class="grid-4">
${products.slice(0, 4).map(p => this.createCard(p)).join('')}
</div>
</div>`;
  },


  renderShop: function(container) {
    const filtered = this.state.filter === 'All' ? products : products.filter(p => p.cat === this.state.filter);
    const categories = ['All', 'Apparel', 'Accessories', 'Lifestyle', 'Makeup Kits'];
    const filtersHTML = categories.map(cat =>
      `<button onclick="app.state.filter='${cat}'; app.router('shop')" style="padding:8px 16px; margin:5px; border:1px solid #ddd; background:${this.state.filter===cat?'#222':'white'}; color:${this.state.filter===cat?'white':'#222'}; border-radius:20px;">${cat}</button>`
    ).join('');
    container.innerHTML = `
<div class="container" style="padding-top:40px;">
<div style="text-align:center; margin-bottom:30px;">
<h2>${this.state.filter} Collection</h2>
<div style="margin-top:20px;">${filtersHTML}</div>
</div>
<div class="grid-4">
${filtered.map(p => this.createCard(p)).join('')}
</div>
</div>`;
  },


  createCard: function(p) {
    return `
<div class="product-card">
<div class="p-img-container">
<img src="${p.img}" alt="${p.desc}">
</div>
<div class="p-info">
<div class="p-cat">${p.cat}</div>
<div class="p-brand">${p.brand}</div>
<div class="p-name">${p.desc}</div>
<div style="display:flex; justify-content:center; align-items:center; gap:5px;">
<div class="p-price">₹${p.price}</div>
<div class="p-off">${p.off}</div>
</div>
<button class="add-btn" onclick="app.addToCart(${p.id})">ADD TO CART</button>
</div>
</div>`;
  },


  renderLogin: function(c) {
    c.innerHTML = `
<div class="auth-box">
<h2 style="margin-bottom:20px;">Login</h2>
<form onsubmit="app.login(event)">
<div class="form-group"><label>Email</label><input type="email" id="log-email" required></div>
<div class="form-group"><label>Password</label><input type="password" required></div>
<button type="submit" class="auth-btn">LOGIN</button>
</form>
<div class="switch-link">New here? <span onclick="app.router('register')">Create Account</span></div>
</div>`;
  },


  renderRegister: function(c) {
    c.innerHTML = `
<div class="auth-box">
<h2 style="margin-bottom:20px;">Register</h2>
<form onsubmit="app.register(event)">
<div class="form-group"><label>Full Name</label><input type="text" id="reg-name" required></div>
<div class="form-group"><label>Email</label><input type="email" id="reg-email" required></div>
<div class="form-group"><label>Password</label><input type="password" required></div>
<button type="submit" class="auth-btn">REGISTER</button>
</form>
<div class="switch-link">Already have account? <span onclick="app.router('login')">Login</span></div>
</div>`;
  },


  renderSettings: function(c) {
    if (!this.state.user) return app.router('login');
    c.innerHTML = `
<div class="container">
<h2 class="section-title" style="text-align:left;">My Account</h2>
<div class="settings-container">
<div class="profile-card">
<img src="${this.state.user.avatar}" class="profile-pic" />
<h3>${this.state.user.name}</h3>
<p style="color:#888;">${this.state.user.email}</p>
<div class="settings-nav">
<div onclick="app.router('orders')">Order History</div>
<div onclick="alert('Profile Settings')">Profile Settings</div>
<div onclick="app.logout()" style="color:red;">Logout</div>
</div>
</div>
<div class="settings-content">
<h3>Account Settings</h3>
<p style="color:#888; margin:10px 0 20px;">Manage your account details and preferences.</p>
<div class="form-group"><label>Full Name</label><input type="text" value="${this.state.user.name}"></div>
<div class="form-group"><label>Email</label><input type="text" value="${this.state.user.email}" disabled></div>
<div class="form-group"><label>New Password</label><input type="password"></div>
<button class="auth-btn" onclick="app.showToast('Settings Saved')">Save Changes</button>
</div>
</div>
</div>`;
  },


  renderOrders: function(c) {
    if (!this.state.user) return app.router('login');
    const ordersHTML = this.state.orders.length === 0
      ? `<div style="text-align:center; padding:40px; color:#888;">No orders yet.</div>`
      : this.state.orders.map(order => `
<div class="order-card">
<div class="order-header">
<span class="order-id">#${order.id}</span>
<span class="order-status">${order.status}</span>
</div>
<div class="order-date">Placed on ${order.date}</div>
<ul class="order-items-list">
${order.items.map(item => `<li><span>${item.brand} ${item.desc}</span> <span>₹${item.price}</span></li>`).join('')}
</ul>
<div class="order-total">Total: ₹${order.total}</div>
</div>`).join('');
    c.innerHTML = `
<div class="container">
<h2 class="section-title" style="text-align:left; margin-top:50px;">Order History</h2>
<div class="orders-container">
${ordersHTML}
</div>
</div>`;
  },


  renderCart: function(c) {
    if (this.state.cart.length === 0) {
      c.innerHTML = `<div class="container" style="text-align:center; padding:50px;"><h3>Your Cart is Empty</h3></div>`;
      return;
    }
    const total = this.state.cart.reduce((a, b) => a + b.price * b.qty, 0);
    c.innerHTML = `
<div class="container" style="padding-top:50px;">
<h2>Shopping Cart</h2>
<div style="background:white; padding:20px; margin-top:20px; box-shadow:var(--shadow);">
${this.state.cart.map(item => `
<div style="display:flex; justify-content:space-between; align-items:center; border-bottom:1px solid #eee; padding:15px 0;">
<div style="display:flex; align-items:center; gap:15px;">
<img src="${item.img}" style="width:50px; height:50px; border-radius:4px;">
<b>${item.brand} ${item.desc}</b>
</div>
<div>${item.qty} x ₹${item.price}</div>
</div>
`).join('')}
<div style="text-align:right; margin-top:20px; font-size:1.2rem; font-weight:bold;">
Total: ₹${total}
</div>
<div style="text-align:right; margin-top:10px;">
<button class="auth-btn" onclick="app.router('checkout')">Checkout</button>
</div>
</div>
</div>`;
  },


  renderCheckout: function(c) {
    if (!this.state.user) {
      this.showToast("Please Login First");
      return this.router('login');
    }
    c.innerHTML = `
<div class="container" style="padding-top:50px;">
<h2>Secure Checkout</h2>
<div class="auth-box" style="margin:30px auto; text-align:left;">
<div class="form-group"><label>Shipping Address</label><input type="text" placeholder="Street Address"></div>
<div class="form-group"><label>City</label><input type="text"></div>
<button class="auth-btn" onclick="app.placeOrder()">Pay & Place Order</button>
</div>
</div>`;
  },


  placeOrder: function() {
    const total = this.state.cart.reduce((a, b) => a + b.price * b.qty, 0);
    const newOrder = {
      id: 'ORD-' + Math.floor(Math.random() * 10000),
      date: new Date().toLocaleDateString(),
      status: 'Processing',
      total: total,
      items: [...this.state.cart]
    };
    this.state.orders.unshift(newOrder);
    this.state.cart = [];
    document.getElementById('cart-badge').innerText = '0';
    this.showToast('Order Placed Successfully!');
    this.router('orders');
  },


  showToast: function(msg) {
    const t = document.getElementById("toast");
    t.innerText = msg;
    t.className = "show";
    setTimeout(() => {
      t.className = t.className.replace("show", "");
    }, 3000);
  }
};


// Initialize the app
app.router('home');