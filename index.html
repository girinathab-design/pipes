import { useState } from "react";

const products = [
  { id: 1, name: "Schedule 40 PVC Pipe", category: "PVC", size: '1"', price: 415, unit: "per ft", stock: 250, desc: "Standard pressure-rated white PVC for cold water lines" },
  { id: 2, name: "Schedule 80 PVC Pipe", category: "PVC", size: '2"', price: 790, unit: "per ft", stock: 180, desc: "Heavy-duty grey PVC for higher pressure applications" },
  { id: 3, name: "CPVC Hot Water Pipe", category: "CPVC", size: '3/4"', price: 560, unit: "per ft", stock: 120, desc: "Chlorinated PVC rated for hot water up to 200°F" },
  { id: 4, name: "Black Iron Pipe", category: "Iron", size: '1/2"', price: 1080, unit: "per ft", stock: 90, desc: "Threaded black steel for gas and water distribution" },
  { id: 5, name: "Galvanized Steel Pipe", category: "Iron", size: '1"', price: 1290, unit: "per ft", stock: 60, desc: "Zinc-coated for corrosion resistance in wet environments" },
  { id: 6, name: "Type L Copper Pipe", category: "Copper", size: '3/4"', price: 1830, unit: "per ft", stock: 75, desc: "Medium-wall copper for residential water supply" },
  { id: 7, name: "Type K Copper Pipe", category: "Copper", size: '1"', price: 2620, unit: "per ft", stock: 40, desc: "Thick-wall copper for underground and high-pressure use" },
  { id: 8, name: "PEX-A Tubing", category: "PEX", size: '1/2"', price: 265, unit: "per ft", stock: 500, desc: "Flexible cross-linked polyethylene, ideal for radiant heating" },
  { id: 9, name: "PEX-B Tubing", category: "PEX", size: '3/4"', price: 340, unit: "per ft", stock: 400, desc: "More rigid PEX with excellent chlorine resistance" },
  { id: 10, name: "ABS Drain Pipe", category: "ABS", size: '3"', price: 610, unit: "per ft", stock: 200, desc: "Black ABS for DWV (drain, waste, vent) systems" },
  { id: 11, name: "Corrugated Drain Pipe", category: "HDPE", size: '4"', price: 480, unit: "per ft", stock: 300, desc: "Flexible HDPE for underground drainage and French drains" },
  { id: 12, name: "Stainless Steel Pipe", category: "Stainless", size: '2"', price: 3160, unit: "per ft", stock: 30, desc: "Grade 316 stainless for food-grade and marine applications" },
];

const CATS = ["All", "PVC", "CPVC", "Copper", "Iron", "PEX", "ABS", "HDPE", "Stainless"];

const categoryColors = {
  PVC: "#d4f7e0", CPVC: "#fef3c7", Copper: "#fed7aa", Iron: "#e2e8f0",
  PEX: "#dbeafe", ABS: "#f3e8ff", HDPE: "#fce7f3", Stainless: "#ccfbf1",
};
const categoryText = {
  PVC: "#166534", CPVC: "#92400e", Copper: "#9a3412", Iron: "#475569",
  PEX: "#1e40af", ABS: "#6b21a8", HDPE: "#9d174d", Stainless: "#134e4a",
};

const inr = (n) => "₹" + n.toLocaleString("en-IN");

export default function PipesStore() {
  const [cart, setCart] = useState({});
  const [activeCategory, setActiveCategory] = useState("All");
  const [search, setSearch] = useState("");
  const [cartOpen, setCartOpen] = useState(false);
  const [quantities, setQuantities] = useState({});
  const [added, setAdded] = useState({});

  const filtered = products.filter((p) => {
    const matchCat = activeCategory === "All" || p.category === activeCategory;
    const matchSearch =
      p.name.toLowerCase().includes(search.toLowerCase()) ||
      p.category.toLowerCase().includes(search.toLowerCase());
    return matchCat && matchSearch;
  });

  const cartItems = Object.entries(cart).map(([id, qty]) => ({
    ...products.find((p) => p.id === +id),
    qty,
  }));

  const cartTotal = cartItems.reduce((s, i) => s + i.price * i.qty, 0);
  const cartCount = Object.values(cart).reduce((s, v) => s + v, 0);

  const addToCart = (id) => {
    const qty = quantities[id] || 1;
    setCart((c) => ({ ...c, [id]: (c[id] || 0) + qty }));
    setAdded((a) => ({ ...a, [id]: true }));
    setTimeout(() => setAdded((a) => ({ ...a, [id]: false })), 900);
  };

  const removeFromCart = (id) => {
    setCart((c) => { const next = { ...c }; delete next[id]; return next; });
  };

  const setQty = (id, val) => {
    const v = Math.max(1, Math.min(99, +val || 1));
    setQuantities((q) => ({ ...q, [id]: v }));
  };

  return (
    <div style={{ fontFamily: "'Barlow Condensed', sans-serif", background: "#0f1117", minHeight: "100vh", color: "#e8e4dc" }}>
      <link href="https://fonts.googleapis.com/css2?family=Barlow+Condensed:wght@300;400;500;600;700;800&family=Barlow:wght@300;400;500&display=swap" rel="stylesheet" />

      {/* Header */}
      <header style={{ background: "#1a1d27", borderBottom: "2px solid #e87d2b", padding: "0 1.5rem", display: "flex", alignItems: "center", gap: "1.5rem", height: 70, position: "sticky", top: 0, zIndex: 100 }}>
        <div style={{ display: "flex", flexDirection: "column", lineHeight: 1.1 }}>
          <div style={{ display: "flex", alignItems: "center", gap: 8 }}>
            <svg width="28" height="28" viewBox="0 0 32 32" fill="none">
              <rect x="2" y="12" width="28" height="8" rx="2" fill="#e87d2b"/>
              <rect x="10" y="4" width="4" height="8" rx="1" fill="#e87d2b" opacity="0.7"/>
              <rect x="18" y="20" width="4" height="8" rx="1" fill="#e87d2b" opacity="0.7"/>
              <circle cx="10" cy="12" r="3" fill="#f5a052"/>
              <circle cx="22" cy="20" r="3" fill="#f5a052"/>
            </svg>
            <span style={{ fontSize: 24, fontWeight: 800, letterSpacing: 2, color: "#fff", textTransform: "uppercase" }}>AB Pipes</span>
          </div>
          <span style={{ fontSize: 11, color: "#8891a4", letterSpacing: 1, paddingLeft: 36 }}>
            📍 Kallakurichi, Tamil Nadu
          </span>
        </div>

        <input
          type="text"
          placeholder="Search pipes..."
          value={search}
          onChange={(e) => setSearch(e.target.value)}
          style={{ flex: 1, maxWidth: 320, background: "#0f1117", border: "1px solid #2e3142", borderRadius: 6, padding: "8px 14px", color: "#e8e4dc", fontSize: 14, fontFamily: "inherit", outline: "none" }}
        />

        {/* Call button */}
        <a
          href="tel:9003114280"
          style={{ display: "flex", alignItems: "center", gap: 7, background: "#16a34a", borderRadius: 8, padding: "8px 16px", color: "#fff", fontFamily: "inherit", fontWeight: 700, fontSize: 14, textDecoration: "none", letterSpacing: 0.5, flexShrink: 0 }}
        >
          <svg width="16" height="16" viewBox="0 0 24 24" fill="none" stroke="currentColor" strokeWidth="2.5">
            <path d="M22 16.92v3a2 2 0 0 1-2.18 2 19.79 19.79 0 0 1-8.63-3.07A19.5 19.5 0 0 1 4.69 12 19.79 19.79 0 0 1 1.6 3.45 2 2 0 0 1 3.58 1.27h3a2 2 0 0 1 2 1.72c.127.96.361 1.903.7 2.81a2 2 0 0 1-.45 2.11L7.91 8.82a16 16 0 0 0 6.29 6.29l1.27-1.27a2 2 0 0 1 2.11-.45c.907.339 1.85.573 2.81.7A2 2 0 0 1 22 16.92z"/>
          </svg>
          90031 14280
        </a>

        <button
          onClick={() => setCartOpen(!cartOpen)}
          style={{ background: cartCount > 0 ? "#e87d2b" : "#2e3142", border: "none", borderRadius: 8, padding: "8px 16px", cursor: "pointer", display: "flex", alignItems: "center", gap: 8, color: "#fff", fontSize: 15, fontWeight: 600, fontFamily: "inherit", transition: "background 0.2s", flexShrink: 0 }}
        >
          <svg width="18" height="18" viewBox="0 0 24 24" fill="none" stroke="currentColor" strokeWidth="2">
            <circle cx="9" cy="21" r="1"/><circle cx="20" cy="21" r="1"/>
            <path d="M1 1h4l2.68 13.39a2 2 0 0 0 2 1.61h9.72a2 2 0 0 0 2-1.61L23 6H6"/>
          </svg>
          Cart {cartCount > 0 && <span style={{ background: "#fff", color: "#e87d2b", borderRadius: 10, padding: "1px 7px", fontSize: 12, fontWeight: 700 }}>{cartCount}</span>}
        </button>
      </header>

      <div style={{ display: "flex" }}>
        {/* Sidebar */}
        <aside style={{ width: 200, minHeight: "calc(100vh - 70px)", background: "#13151f", padding: "1.5rem 0", flexShrink: 0, borderRight: "1px solid #1e2130" }}>
          <p style={{ padding: "0 1.25rem", fontSize: 11, fontWeight: 700, letterSpacing: 3, color: "#6b7280", textTransform: "uppercase", marginBottom: 8 }}>Material</p>
          {CATS.map((cat) => (
            <button
              key={cat}
              onClick={() => setActiveCategory(cat)}
              style={{ display: "block", width: "100%", textAlign: "left", padding: "8px 1.25rem", background: activeCategory === cat ? "#e87d2b" : "transparent", color: activeCategory === cat ? "#fff" : "#a0a8b8", border: "none", cursor: "pointer", fontSize: 14, fontWeight: activeCategory === cat ? 700 : 400, fontFamily: "inherit", letterSpacing: 0.5, borderLeft: activeCategory === cat ? "3px solid #f5a052" : "3px solid transparent", transition: "all 0.15s" }}
            >
              {cat}
            </button>
          ))}

          <div style={{ margin: "2rem 1.25rem 0", padding: "1rem", background: "#0f1117", borderRadius: 8, border: "1px solid #2e3142" }}>
            <p style={{ fontSize: 11, fontWeight: 700, letterSpacing: 2, color: "#6b7280", textTransform: "uppercase", margin: "0 0 6px" }}>Contact</p>
            <a href="tel:9003114280" style={{ color: "#e87d2b", fontSize: 13, fontWeight: 600, textDecoration: "none", display: "block", marginBottom: 4 }}>📞 90031 14280</a>
            <p style={{ fontSize: 12, color: "#8891a4", margin: 0, lineHeight: 1.6 }}>Kallakurichi, Tamil Nadu</p>
          </div>
        </aside>

        {/* Main */}
        <main style={{ flex: 1, padding: "2rem" }}>
          <div style={{ display: "flex", alignItems: "baseline", gap: 12, marginBottom: "1.5rem" }}>
            <h1 style={{ fontSize: 28, fontWeight: 800, letterSpacing: 1, textTransform: "uppercase", margin: 0, color: "#fff" }}>
              {activeCategory === "All" ? "All Pipes" : `${activeCategory} Pipes`}
            </h1>
            <span style={{ fontSize: 14, color: "#6b7280" }}>{filtered.length} products</span>
          </div>

          <div style={{ display: "grid", gridTemplateColumns: "repeat(auto-fill, minmax(280px, 1fr))", gap: "1.25rem" }}>
            {filtered.map((p) => (
              <div key={p.id} style={{ background: "#1a1d27", border: "1px solid #2e3142", borderRadius: 10, overflow: "hidden", display: "flex", flexDirection: "column" }}>
                <div style={{ height: 5, background: `linear-gradient(90deg, ${categoryText[p.category]}, ${categoryColors[p.category]})` }} />
                <div style={{ padding: "1rem 1.25rem", flex: 1, display: "flex", flexDirection: "column", gap: 8 }}>
                  <div style={{ display: "flex", justifyContent: "space-between", alignItems: "flex-start" }}>
                    <span style={{ fontSize: 11, fontWeight: 700, letterSpacing: 2, textTransform: "uppercase", background: categoryColors[p.category], color: categoryText[p.category], padding: "3px 8px", borderRadius: 4 }}>
                      {p.category}
                    </span>
                    <span style={{ fontSize: 13, color: p.stock > 100 ? "#4ade80" : p.stock > 30 ? "#facc15" : "#f87171", fontWeight: 600 }}>
                      {p.stock > 100 ? "In Stock" : p.stock > 30 ? "Low Stock" : "Critical"}
                    </span>
                  </div>

                  <h2 style={{ margin: 0, fontSize: 17, fontWeight: 700, color: "#fff", lineHeight: 1.3 }}>{p.name}</h2>
                  <p style={{ margin: 0, fontSize: 13, color: "#8891a4", lineHeight: 1.5, flex: 1 }}>{p.desc}</p>

                  <div style={{ display: "flex", gap: 8, marginTop: 4 }}>
                    <span style={{ background: "#0f1117", border: "1px solid #2e3142", borderRadius: 5, padding: "3px 10px", fontSize: 12, color: "#a0a8b8" }}>Size: {p.size}</span>
                    <span style={{ background: "#0f1117", border: "1px solid #2e3142", borderRadius: 5, padding: "3px 10px", fontSize: 12, color: "#a0a8b8" }}>{p.stock} ft avail.</span>
                  </div>

                  <div style={{ display: "flex", alignItems: "center", justifyContent: "space-between", marginTop: 8, paddingTop: 12, borderTop: "1px solid #2e3142" }}>
                    <div>
                      <span style={{ fontSize: 22, fontWeight: 800, color: "#e87d2b" }}>{inr(p.price)}</span>
                      <span style={{ fontSize: 12, color: "#6b7280", marginLeft: 4 }}>{p.unit}</span>
                    </div>
                    <div style={{ display: "flex", alignItems: "center", gap: 6 }}>
                      <input
                        type="number"
                        min={1}
                        max={99}
                        value={quantities[p.id] || 1}
                        onChange={(e) => setQty(p.id, e.target.value)}
                        style={{ width: 50, background: "#0f1117", border: "1px solid #2e3142", borderRadius: 5, padding: "5px 8px", color: "#e8e4dc", fontSize: 13, fontFamily: "inherit", textAlign: "center", outline: "none" }}
                      />
                      <button
                        onClick={() => addToCart(p.id)}
                        style={{ background: added[p.id] ? "#4ade80" : "#e87d2b", border: "none", borderRadius: 6, padding: "6px 14px", color: "#fff", fontFamily: "inherit", fontWeight: 700, fontSize: 13, cursor: "pointer", transition: "background 0.2s", letterSpacing: 0.5 }}
                      >
                        {added[p.id] ? "✓ Added" : "Add"}
                      </button>
                    </div>
                  </div>
                </div>
              </div>
            ))}
          </div>

          {filtered.length === 0 && (
            <div style={{ textAlign: "center", padding: "4rem 2rem", color: "#6b7280" }}>
              <p style={{ fontSize: 20, fontWeight: 600 }}>No pipes found</p>
              <p style={{ fontSize: 14 }}>Try a different search or category</p>
            </div>
          )}
        </main>

        {/* Cart Drawer */}
        {cartOpen && (
          <div style={{ width: 340, background: "#13151f", borderLeft: "1px solid #2e3142", padding: "1.5rem", display: "flex", flexDirection: "column", gap: "1rem", position: "sticky", top: 70, height: "calc(100vh - 70px)", overflowY: "auto" }}>
            <div style={{ display: "flex", alignItems: "center", justifyContent: "space-between" }}>
              <h2 style={{ margin: 0, fontSize: 20, fontWeight: 800, textTransform: "uppercase", letterSpacing: 1, color: "#fff" }}>Your Cart</h2>
              <button onClick={() => setCartOpen(false)} style={{ background: "none", border: "none", color: "#6b7280", cursor: "pointer", fontSize: 20, lineHeight: 1 }}>✕</button>
            </div>

            {cartItems.length === 0 ? (
              <div style={{ textAlign: "center", color: "#6b7280", padding: "2rem 0" }}>
                <svg width="40" height="40" viewBox="0 0 24 24" fill="none" stroke="currentColor" strokeWidth="1.5" style={{ margin: "0 auto 12px", display: "block" }}>
                  <circle cx="9" cy="21" r="1"/><circle cx="20" cy="21" r="1"/>
                  <path d="M1 1h4l2.68 13.39a2 2 0 0 0 2 1.61h9.72a2 2 0 0 0 2-1.61L23 6H6"/>
                </svg>
                <p style={{ fontSize: 15 }}>Cart is empty</p>
              </div>
            ) : (
              <>
                {cartItems.map((item) => (
                  <div key={item.id} style={{ background: "#1a1d27", border: "1px solid #2e3142", borderRadius: 8, padding: "12px 14px" }}>
                    <div style={{ display: "flex", justifyContent: "space-between", alignItems: "flex-start" }}>
                      <div style={{ flex: 1 }}>
                        <p style={{ margin: "0 0 4px", fontSize: 14, fontWeight: 600, color: "#fff" }}>{item.name}</p>
                        <p style={{ margin: 0, fontSize: 12, color: "#6b7280" }}>{item.size} · {item.qty} ft</p>
                      </div>
                      <button onClick={() => removeFromCart(item.id)} style={{ background: "none", border: "none", color: "#f87171", cursor: "pointer", fontSize: 16, padding: "0 0 0 8px" }}>✕</button>
                    </div>
                    <div style={{ display: "flex", justifyContent: "space-between", alignItems: "center", marginTop: 8 }}>
                      <span style={{ fontSize: 12, color: "#8891a4" }}>{inr(item.price)} × {item.qty} ft</span>
                      <span style={{ fontSize: 16, fontWeight: 700, color: "#e87d2b" }}>{inr(item.price * item.qty)}</span>
                    </div>
                  </div>
                ))}

                <div style={{ borderTop: "2px solid #2e3142", paddingTop: "1rem", marginTop: "auto" }}>
                  <div style={{ display: "flex", justifyContent: "space-between", marginBottom: 16 }}>
                    <span style={{ fontSize: 16, fontWeight: 600, color: "#a0a8b8" }}>Subtotal</span>
                    <span style={{ fontSize: 22, fontWeight: 800, color: "#fff" }}>{inr(cartTotal)}</span>
                  </div>
                  <a
                    href="tel:9003114280"
                    style={{ display: "block", width: "100%", background: "#16a34a", border: "none", borderRadius: 8, padding: "12px", color: "#fff", fontSize: 15, fontWeight: 800, textTransform: "uppercase", letterSpacing: 1, cursor: "pointer", fontFamily: "inherit", textAlign: "center", textDecoration: "none", marginBottom: 10, boxSizing: "border-box" }}
                  >
                    📞 Call to Order
                  </a>
                  <button style={{ width: "100%", background: "#e87d2b", border: "none", borderRadius: 8, padding: "12px", color: "#fff", fontSize: 15, fontWeight: 800, textTransform: "uppercase", letterSpacing: 1, cursor: "pointer", fontFamily: "inherit" }}>
                    Checkout →
                  </button>
                </div>
              </>
            )}
          </div>
        )}
      </div>
    </div>
  );
}
