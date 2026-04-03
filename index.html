import { useState, useEffect, useRef, useCallback } from "react";

const ADMIN_PASSWORD = "nrk2024";

const DEFAULT_VEHICLES = [
  { id: "v1", brand: "Mercedes-Benz", model: "CLA 45 AMG", price: "42 900€", km: "38 500", year: "2021", hp: "387", seats: "5", image: "https://images.unsplash.com/photo-1618843479313-40f8afb4b4d8?w=800&q=80", description: "CLA 45 AMG en parfait état, full options, toit ouvrant, sièges AMG, système multimédia MBUX." },
  { id: "v2", brand: "BMW", model: "M4 Competition", price: "67 500€", km: "22 000", year: "2022", hp: "510", seats: "4", image: "https://images.unsplash.com/photo-1617814076367-b759c7d7e738?w=800&q=80", description: "M4 Competition xDrive, carbone, head-up display, Harman Kardon." },
  { id: "v3", brand: "Audi", model: "RS3 Sportback", price: "54 900€", km: "31 200", year: "2022", hp: "400", seats: "5", image: "https://images.unsplash.com/photo-1603584173870-7f23fdae1b7a?w=800&q=80", description: "RS3 Sportback, gris Nardo, échappement sport, virtual cockpit." },
  { id: "v4", brand: "Mercedes-Benz", model: "Classe C 63 AMG", price: "49 900€", km: "45 000", year: "2020", hp: "476", seats: "5", image: "https://images.unsplash.com/photo-1563720223185-11003d516935?w=800&q=80", description: "C63 AMG S, V8 biturbo, performance seats, night package." },
  { id: "v5", brand: "Porsche", model: "718 Cayman S", price: "72 000€", km: "18 500", year: "2023", hp: "350", seats: "2", image: "https://images.unsplash.com/photo-1614162692292-7ac56d7f7f1e?w=800&q=80", description: "718 Cayman S, PDK, Sport Chrono, PASM, sièges sport adaptatifs." },
  { id: "v6", brand: "BMW", model: "M2 Competition", price: "52 900€", km: "27 800", year: "2022", hp: "410", seats: "4", image: "https://images.unsplash.com/photo-1555215695-3004980ad54e?w=800&q=80", description: "M2 Competition, boîte manuelle, différentiel actif M, freins M." },
];

const REVIEWS = [
  { name: "Thomas L.", text: "Achat d'une RS3 impeccable. Véhicule conforme à la description, livraison rapide et professionnelle. Je recommande vivement !", date: "Mars 2026" },
  { name: "Julien M.", text: "Excellent service du début à la fin. NRK Prestige m'a trouvé la M4 de mes rêves en un temps record. Merci encore !", date: "Février 2026" },
  { name: "Sophie D.", text: "Très satisfaite de mon achat. La voiture était dans un état irréprochable et le prix très compétitif.", date: "Février 2026" },
  { name: "Karim B.", text: "Un vrai professionnel. Conseils avisés, pas de mauvaises surprises. Ma CLA 45 est parfaite.", date: "Janvier 2026" },
  { name: "Alexandre P.", text: "Service client au top. Réponse rapide, transparence totale sur l'historique du véhicule. Je reviendrai !", date: "Janvier 2026" },
  { name: "Marie-Claire F.", text: "Première fois que j'achète une voiture d'occasion avec autant de confiance. Équipe sérieuse et véhicule impeccable.", date: "Décembre 2025" },
  { name: "Romain G.", text: "Superbe expérience. Livraison à domicile, véhicule préparé comme neuf. Rien à redire.", date: "Décembre 2025" },
  { name: "Nadia K.", text: "Rapport qualité-prix imbattable. Mon Cayman était mieux que ce que j'espérais. Merci NRK !", date: "Novembre 2025" },
  { name: "David R.", text: "Achat en toute sérénité. Garantie incluse, contrôle technique OK, tout était carré.", date: "Novembre 2025" },
  { name: "Laura S.", text: "J'ai comparé plusieurs concessionnaires, NRK Prestige est clairement au-dessus en termes de service.", date: "Octobre 2025" },
  { name: "Mehdi A.", text: "Véhicule en parfait état mécanique et esthétique. Le propriétaire est passionné et ça se voit.", date: "Octobre 2025" },
  { name: "Christophe V.", text: "Deuxième achat chez NRK, toujours aussi satisfait. Fidélité méritée !", date: "Septembre 2025" },
  { name: "Élodie B.", text: "Accompagnement personnalisé pour le financement. Très pratique et arrangeant.", date: "Septembre 2025" },
  { name: "Yannick T.", text: "La M2 Competition que j'ai achetée est une merveille. Entretien suivi, carnet complet.", date: "Août 2025" },
  { name: "Camille H.", text: "Vendeur honnête et transparent. Pas de vice caché, la voiture est exactement comme décrite.", date: "Août 2025" },
  { name: "Fabien L.", text: "Réactivité exemplaire. J'ai posé une question le soir, réponse le lendemain matin. Pro.", date: "Juillet 2025" },
  { name: "Amandine C.", text: "Belle sélection de véhicules premium. On sent la passion automobile. Bravo !", date: "Juillet 2025" },
  { name: "Olivier N.", text: "Transaction fluide, pas de stress. Le véhicule a été préparé aux petits oignons.", date: "Juin 2025" },
  { name: "Sarah M.", text: "Je recommande les yeux fermés. Sérieux, professionnel, et véhicules de qualité.", date: "Juin 2025" },
  { name: "Maxime J.", text: "NRK Prestige, c'est la garantie d'un achat en toute confiance. Merci pour cette C63 sublime !", date: "Mai 2025" },
];

const StarIcon = () => (
  <svg width="16" height="16" viewBox="0 0 24 24" fill="#D4AF37" stroke="none">
    <path d="M12 2l3.09 6.26L22 9.27l-5 4.87 1.18 6.88L12 17.77l-6.18 3.25L7 14.14 2 9.27l6.91-1.01L12 2z"/>
  </svg>
);

const PhoneIcon = () => <svg width="20" height="20" viewBox="0 0 24 24" fill="none" stroke="currentColor" strokeWidth="2"><path d="M22 16.92v3a2 2 0 01-2.18 2 19.79 19.79 0 01-8.63-3.07 19.5 19.5 0 01-6-6 19.79 19.79 0 01-3.07-8.67A2 2 0 014.11 2h3a2 2 0 012 1.72c.127.96.361 1.903.7 2.81a2 2 0 01-.45 2.11L8.09 9.91a16 16 0 006 6l1.27-1.27a2 2 0 012.11-.45c.907.339 1.85.573 2.81.7A2 2 0 0122 16.92z"/></svg>;
const MailIcon = () => <svg width="20" height="20" viewBox="0 0 24 24" fill="none" stroke="currentColor" strokeWidth="2"><path d="M4 4h16c1.1 0 2 .9 2 2v12c0 1.1-.9 2-2 2H4c-1.1 0-2-.9-2-2V6c0-1.1.9-2 2-2z"/><polyline points="22,6 12,13 2,6"/></svg>;
const MapIcon = () => <svg width="20" height="20" viewBox="0 0 24 24" fill="none" stroke="currentColor" strokeWidth="2"><path d="M21 10c0 7-9 13-9 13s-9-6-9-13a9 9 0 0118 0z"/><circle cx="12" cy="10" r="3"/></svg>;
const ClockIcon = () => <svg width="20" height="20" viewBox="0 0 24 24" fill="none" stroke="currentColor" strokeWidth="2"><circle cx="12" cy="12" r="10"/><polyline points="12 6 12 12 16 14"/></svg>;
const ChevronDown = () => <svg width="28" height="28" viewBox="0 0 24 24" fill="none" stroke="currentColor" strokeWidth="2"><polyline points="6 9 12 15 18 9"/></svg>;
const InstagramIcon = () => <svg width="28" height="28" viewBox="0 0 24 24" fill="none" stroke="currentColor" strokeWidth="2"><rect x="2" y="2" width="20" height="20" rx="5" ry="5"/><path d="M16 11.37A4 4 0 1112.63 8 4 4 0 0116 11.37z"/><line x1="17.5" y1="6.5" x2="17.51" y2="6.5"/></svg>;
const TiktokIcon = () => <svg width="28" height="28" viewBox="0 0 24 24" fill="currentColor"><path d="M19.59 6.69a4.83 4.83 0 01-3.77-4.25V2h-3.45v13.67a2.89 2.89 0 01-2.88 2.5 2.89 2.89 0 01-2.89-2.89 2.89 2.89 0 012.89-2.89c.28 0 .54.04.79.1v-3.5a6.37 6.37 0 00-.79-.05A6.34 6.34 0 003.15 15.2a6.34 6.34 0 006.34 6.34 6.34 6.34 0 006.34-6.34V8.71a8.21 8.21 0 004.76 1.52v-3.4a4.85 4.85 0 01-1-.14z"/></svg>;
const PlusIcon = () => <svg width="20" height="20" viewBox="0 0 24 24" fill="none" stroke="currentColor" strokeWidth="2"><line x1="12" y1="5" x2="12" y2="19"/><line x1="5" y1="12" x2="19" y2="12"/></svg>;
const TrashIcon = () => <svg width="16" height="16" viewBox="0 0 24 24" fill="none" stroke="currentColor" strokeWidth="2"><polyline points="3 6 5 6 21 6"/><path d="M19 6v14a2 2 0 01-2 2H7a2 2 0 01-2-2V6m3 0V4a2 2 0 012-2h4a2 2 0 012 2v2"/></svg>;
const MenuIcon = () => <svg width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" strokeWidth="2"><line x1="3" y1="12" x2="21" y2="12"/><line x1="3" y1="6" x2="21" y2="6"/><line x1="3" y1="18" x2="21" y2="18"/></svg>;
const CloseIcon = () => <svg width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" strokeWidth="2"><line x1="18" y1="6" x2="6" y2="18"/><line x1="6" y1="6" x2="18" y2="18"/></svg>;
const DashIcon = () => <svg width="20" height="20" viewBox="0 0 24 24" fill="none" stroke="currentColor" strokeWidth="2"><rect x="3" y="3" width="7" height="7"/><rect x="14" y="3" width="7" height="7"/><rect x="14" y="14" width="7" height="7"/><rect x="3" y="14" width="7" height="7"/></svg>;

function useInView(threshold = 0.15) {
  const ref = useRef(null);
  const [visible, setVisible] = useState(false);
  useEffect(() => {
    const el = ref.current;
    if (!el) return;
    const obs = new IntersectionObserver(([e]) => { if (e.isIntersecting) { setVisible(true); obs.unobserve(el); } }, { threshold });
    obs.observe(el);
    return () => obs.disconnect();
  }, [threshold]);
  return [ref, visible];
}

function AnimatedSection({ children, className = "", delay = 0 }) {
  const [ref, visible] = useInView();
  return (
    <div ref={ref} className={className} style={{ opacity: visible ? 1 : 0, transform: visible ? "translateY(0)" : "translateY(40px)", transition: `all 0.8s cubic-bezier(0.16, 1, 0.3, 1) ${delay}s` }}>
      {children}
    </div>
  );
}

export default function NRKPrestige() {
  const [vehicles, setVehicles] = useState(DEFAULT_VEHICLES);
  const [showAdmin, setShowAdmin] = useState(false);
  const [adminAuth, setAdminAuth] = useState(false);
  const [password, setPassword] = useState("");
  const [mobileMenu, setMobileMenu] = useState(false);
  const [selectedVehicle, setSelectedVehicle] = useState(null);
  const [reviewPage, setReviewPage] = useState(0);
  const [heroLoaded, setHeroLoaded] = useState(false);
  const [scrollY, setScrollY] = useState(0);
  const [newVehicle, setNewVehicle] = useState({ brand: "", model: "", price: "", km: "", year: "", hp: "", seats: "", image: "", description: "" });

  useEffect(() => {
    setTimeout(() => setHeroLoaded(true), 300);
    const handleScroll = () => setScrollY(window.scrollY);
    window.addEventListener("scroll", handleScroll, { passive: true });
    return () => window.removeEventListener("scroll", handleScroll);
  }, []);

  useEffect(() => {
    (async () => {
      try {
        const r = await window.storage.get("nrk_vehicles");
        if (r && r.value) setVehicles(JSON.parse(r.value));
      } catch {}
    })();
  }, []);

  const saveVehicles = async (v) => {
    setVehicles(v);
    try { await window.storage.set("nrk_vehicles", JSON.stringify(v)); } catch {}
  };

  const addVehicle = () => {
    if (!newVehicle.brand || !newVehicle.model) return;
    const v = { ...newVehicle, id: "v" + Date.now() };
    saveVehicles([v, ...vehicles]);
    setNewVehicle({ brand: "", model: "", price: "", km: "", year: "", hp: "", seats: "", image: "", description: "" });
  };

  const deleteVehicle = (id) => saveVehicles(vehicles.filter(v => v.id !== id));

  const reviewsPerPage = 4;
  const totalPages = Math.ceil(REVIEWS.length / reviewsPerPage);
  const currentReviews = REVIEWS.slice(reviewPage * reviewsPerPage, (reviewPage + 1) * reviewsPerPage);

  const scrollTo = (id) => {
    setMobileMenu(false);
    document.getElementById(id)?.scrollIntoView({ behavior: "smooth" });
  };

  const navItems = [
    { label: "Accueil", id: "hero" },
    { label: "Véhicules", id: "vehicles" },
    { label: "Avis", id: "reviews" },
    { label: "Contact", id: "contact" },
  ];

  return (
    <div style={{ background: "#0a0a0a", color: "#e8e8e8", fontFamily: "'Outfit', sans-serif", minHeight: "100vh", overflow: "hidden" }}>
      <link href="https://fonts.googleapis.com/css2?family=Outfit:wght@300;400;500;600;700&family=Playfair+Display:ital,wght@0,400;0,700;1,400&display=swap" rel="stylesheet" />
      <style>{`
        * { margin: 0; padding: 0; box-sizing: border-box; }
        ::selection { background: #D4AF37; color: #000; }
        ::-webkit-scrollbar { width: 6px; }
        ::-webkit-scrollbar-track { background: #111; }
        ::-webkit-scrollbar-thumb { background: #D4AF37; border-radius: 3px; }
        @keyframes fadeInUp { from { opacity: 0; transform: translateY(30px); } to { opacity: 1; transform: translateY(0); } }
        @keyframes slideDown { from { opacity: 0; transform: translateY(-20px); } to { opacity: 1; transform: translateY(0); } }
        @keyframes pulse { 0%, 100% { opacity: 1; } 50% { opacity: 0.5; } }
        @keyframes shimmer { 0% { background-position: -200% 0; } 100% { background-position: 200% 0; } }
        @keyframes float { 0%, 100% { transform: translateY(0); } 50% { transform: translateY(-10px); } }
        @keyframes kenburns { 0% { transform: scale(1.05); } 50% { transform: scale(1.15); } 100% { transform: scale(1.05); } }
        @keyframes textReveal { from { clip-path: inset(0 100% 0 0); } to { clip-path: inset(0 0 0 0); } }
        @keyframes goldLine { from { width: 0; } to { width: 80px; } }
        @keyframes borderGlow { 0%, 100% { border-color: rgba(212,175,55,0.2); } 50% { border-color: rgba(212,175,55,0.5); } }
        .nav-link { position: relative; cursor: pointer; padding: 8px 0; font-size: 14px; font-weight: 500; letter-spacing: 1.5px; text-transform: uppercase; color: #ccc; transition: color 0.3s; }
        .nav-link:hover { color: #D4AF37; }
        .nav-link::after { content: ''; position: absolute; bottom: 0; left: 0; width: 0; height: 1px; background: #D4AF37; transition: width 0.3s; }
        .nav-link:hover::after { width: 100%; }
        .vehicle-card { position: relative; background: #141414; border: 1px solid #222; border-radius: 12px; overflow: hidden; transition: all 0.5s cubic-bezier(0.16, 1, 0.3, 1); cursor: pointer; }
        .vehicle-card:hover { transform: translateY(-8px); border-color: rgba(212,175,55,0.4); box-shadow: 0 20px 60px rgba(0,0,0,0.5), 0 0 30px rgba(212,175,55,0.08); }
        .vehicle-card:hover .vehicle-img { transform: scale(1.08); }
        .vehicle-img { transition: transform 0.7s cubic-bezier(0.16, 1, 0.3, 1); }
        .btn-gold { background: linear-gradient(135deg, #D4AF37, #B8960C); color: #000; border: none; padding: 14px 36px; font-size: 14px; font-weight: 600; letter-spacing: 2px; text-transform: uppercase; cursor: pointer; transition: all 0.3s; font-family: 'Outfit', sans-serif; border-radius: 4px; }
        .btn-gold:hover { background: linear-gradient(135deg, #e6c54b, #D4AF37); transform: translateY(-2px); box-shadow: 0 8px 25px rgba(212,175,55,0.3); }
        .btn-outline { background: transparent; color: #D4AF37; border: 1px solid #D4AF37; padding: 14px 36px; font-size: 14px; font-weight: 600; letter-spacing: 2px; text-transform: uppercase; cursor: pointer; transition: all 0.3s; font-family: 'Outfit', sans-serif; border-radius: 4px; }
        .btn-outline:hover { background: #D4AF37; color: #000; }
        .review-card { background: #141414; border: 1px solid #1e1e1e; border-radius: 12px; padding: 28px; transition: all 0.4s; }
        .review-card:hover { border-color: rgba(212,175,55,0.3); transform: translateY(-4px); }
        .social-btn { width: 64px; height: 64px; border-radius: 50%; border: 1px solid #333; display: flex; align-items: center; justify-content: center; color: #999; transition: all 0.4s; cursor: pointer; background: #141414; }
        .social-btn:hover { border-color: #D4AF37; color: #D4AF37; transform: translateY(-4px); box-shadow: 0 8px 25px rgba(212,175,55,0.15); }
        .input-field { width: 100%; padding: 12px 16px; background: #1a1a1a; border: 1px solid #2a2a2a; border-radius: 6px; color: #e8e8e8; font-family: 'Outfit', sans-serif; font-size: 14px; outline: none; transition: border-color 0.3s; }
        .input-field:focus { border-color: #D4AF37; }
        .input-field::placeholder { color: #555; }
        .modal-overlay { position: fixed; inset: 0; background: rgba(0,0,0,0.85); z-index: 1000; display: flex; align-items: center; justify-content: center; padding: 20px; backdrop-filter: blur(10px); animation: fadeInUp 0.3s; }
        .gold-separator { width: 80px; height: 2px; background: linear-gradient(90deg, transparent, #D4AF37, transparent); margin: 0 auto; }
        .stat-item { text-align: center; padding: 20px; }
        .stat-number { font-family: 'Playfair Display', serif; font-size: 36px; color: #D4AF37; font-weight: 700; }
        .admin-fab { position: fixed; bottom: 24px; right: 24px; z-index: 900; width: 48px; height: 48px; border-radius: 50%; background: #1a1a1a; border: 1px solid #333; color: #999; display: flex; align-items: center; justify-content: center; cursor: pointer; transition: all 0.3s; }
        .admin-fab:hover { border-color: #D4AF37; color: #D4AF37; }
        .page-dot { width: 10px; height: 10px; border-radius: 50%; border: 1px solid #555; background: transparent; cursor: pointer; transition: all 0.3s; }
        .page-dot.active { background: #D4AF37; border-color: #D4AF37; }
        @media (max-width: 768px) {
          .hero-title { font-size: 42px !important; }
          .hero-sub { font-size: 16px !important; }
          .section-title { font-size: 28px !important; }
          .vehicles-grid { grid-template-columns: 1fr !important; }
          .reviews-grid { grid-template-columns: 1fr !important; }
          .contact-grid { grid-template-columns: 1fr !important; }
          .stats-row { flex-direction: column !important; gap: 10px !important; }
          .footer-inner { flex-direction: column !important; text-align: center !important; gap: 20px !important; }
        }
      `}</style>

      {/* NAVBAR */}
      <nav style={{
        position: "fixed", top: 0, left: 0, right: 0, zIndex: 999,
        background: scrollY > 50 ? "rgba(10,10,10,0.95)" : "transparent",
        backdropFilter: scrollY > 50 ? "blur(20px)" : "none",
        borderBottom: scrollY > 50 ? "1px solid #1a1a1a" : "1px solid transparent",
        transition: "all 0.4s", padding: "0 40px"
      }}>
        <div style={{ maxWidth: 1200, margin: "0 auto", display: "flex", alignItems: "center", justifyContent: "space-between", height: 72 }}>
          <div style={{ cursor: "pointer" }} onClick={() => scrollTo("hero")}>
            <span style={{ fontFamily: "'Playfair Display', serif", fontSize: 22, fontWeight: 700, color: "#D4AF37", letterSpacing: 3 }}>NRK</span>
            <span style={{ fontFamily: "'Outfit', sans-serif", fontSize: 11, fontWeight: 300, letterSpacing: 4, color: "#888", marginLeft: 8, textTransform: "uppercase" }}>Prestige</span>
          </div>
          <div style={{ display: "flex", gap: 32, alignItems: "center" }} className="desktop-nav">
            {navItems.map(item => (
              <span key={item.id} className="nav-link" onClick={() => scrollTo(item.id)}>{item.label}</span>
            ))}
          </div>
          <div style={{ display: "none" }} className="mobile-menu-btn">
            <button onClick={() => setMobileMenu(!mobileMenu)} style={{ background: "none", border: "none", color: "#e8e8e8", cursor: "pointer" }}>
              {mobileMenu ? <CloseIcon /> : <MenuIcon />}
            </button>
          </div>
        </div>
        {mobileMenu && (
          <div style={{ padding: "20px 0", borderTop: "1px solid #1a1a1a", animation: "slideDown 0.3s" }}>
            {navItems.map(item => (
              <div key={item.id} style={{ padding: "12px 0", textAlign: "center" }}>
                <span className="nav-link" onClick={() => scrollTo(item.id)}>{item.label}</span>
              </div>
            ))}
          </div>
        )}
      </nav>

      {/* HERO */}
      <section id="hero" style={{ position: "relative", height: "100vh", display: "flex", alignItems: "center", justifyContent: "center", overflow: "hidden" }}>
        <div style={{
          position: "absolute", inset: 0,
          backgroundImage: "url('https://images.unsplash.com/photo-1618843479313-40f8afb4b4d8?w=1600&q=80')",
          backgroundSize: "cover", backgroundPosition: "center",
          animation: "kenburns 25s ease-in-out infinite",
          filter: "brightness(0.3) contrast(1.1)"
        }} />
        <div style={{ position: "absolute", inset: 0, background: "linear-gradient(to bottom, rgba(10,10,10,0.4) 0%, rgba(10,10,10,0.7) 60%, #0a0a0a 100%)" }} />
        
        <div style={{ position: "relative", zIndex: 2, textAlign: "center", padding: "0 20px" }}>
          <div style={{
            opacity: heroLoaded ? 1 : 0, transform: heroLoaded ? "translateY(0)" : "translateY(30px)",
            transition: "all 1.2s cubic-bezier(0.16, 1, 0.3, 1)"
          }}>
            <div style={{ marginBottom: 16 }}>
              <span style={{ fontSize: 13, letterSpacing: 6, textTransform: "uppercase", color: "#D4AF37", fontWeight: 500 }}>Automobile de prestige</span>
            </div>
            <h1 className="hero-title" style={{
              fontFamily: "'Playfair Display', serif", fontSize: 72, fontWeight: 700,
              color: "#fff", lineHeight: 1.05, marginBottom: 8
            }}>
              NRK <span style={{ color: "#D4AF37", fontStyle: "italic" }}>Prestige</span>
            </h1>
            <div style={{ margin: "24px auto", width: 80, height: 2, background: "linear-gradient(90deg, transparent, #D4AF37, transparent)", animation: heroLoaded ? "goldLine 1s ease-out 0.8s both" : "none" }} />
            <p className="hero-sub" style={{
              fontSize: 18, color: "#aaa", fontWeight: 300, maxWidth: 500, margin: "0 auto 40px",
              lineHeight: 1.7, opacity: heroLoaded ? 1 : 0, transition: "opacity 1s 0.6s"
            }}>
              Vente de véhicules d'occasion haut de gamme.<br/>L'excellence automobile à votre portée.
            </p>
          </div>
          <div style={{ display: "flex", gap: 16, justifyContent: "center", flexWrap: "wrap", opacity: heroLoaded ? 1 : 0, transition: "opacity 1s 1s" }}>
            <button className="btn-gold" onClick={() => scrollTo("vehicles")}>Nos Véhicules</button>
            <button className="btn-outline" onClick={() => scrollTo("contact")}>Contact</button>
          </div>
        </div>

        <div onClick={() => scrollTo("vehicles")} style={{
          position: "absolute", bottom: 40, left: "50%", transform: "translateX(-50%)",
          animation: "float 2s ease-in-out infinite", cursor: "pointer", color: "#D4AF37", opacity: 0.7
        }}>
          <ChevronDown />
        </div>
      </section>

      {/* STATS */}
      <section style={{ background: "#0f0f0f", borderTop: "1px solid #1a1a1a", borderBottom: "1px solid #1a1a1a" }}>
        <div className="stats-row" style={{ maxWidth: 1000, margin: "0 auto", display: "flex", justifyContent: "space-around", padding: "40px 20px" }}>
          {[
            { num: "150+", label: "Véhicules vendus" },
            { num: "100%", label: "Clients satisfaits" },
            { num: "5★", label: "Note moyenne" },
            { num: "2020", label: "Depuis" }
          ].map((s, i) => (
            <AnimatedSection key={i} delay={i * 0.1}>
              <div className="stat-item">
                <div className="stat-number">{s.num}</div>
                <div style={{ color: "#777", fontSize: 13, letterSpacing: 1, textTransform: "uppercase", marginTop: 4 }}>{s.label}</div>
              </div>
            </AnimatedSection>
          ))}
        </div>
      </section>

      {/* VEHICLES */}
      <section id="vehicles" style={{ padding: "100px 40px", maxWidth: 1200, margin: "0 auto" }}>
        <AnimatedSection>
          <div style={{ textAlign: "center", marginBottom: 60 }}>
            <span style={{ fontSize: 12, letterSpacing: 5, textTransform: "uppercase", color: "#D4AF37", fontWeight: 500 }}>Notre sélection</span>
            <h2 className="section-title" style={{ fontFamily: "'Playfair Display', serif", fontSize: 42, fontWeight: 700, color: "#fff", marginTop: 12 }}>
              Véhicules Disponibles
            </h2>
            <div className="gold-separator" style={{ marginTop: 20 }} />
          </div>
        </AnimatedSection>

        <div className="vehicles-grid" style={{ display: "grid", gridTemplateColumns: "repeat(auto-fill, minmax(340px, 1fr))", gap: 28 }}>
          {vehicles.map((v, i) => (
            <AnimatedSection key={v.id} delay={i * 0.08}>
              <div className="vehicle-card" onClick={() => setSelectedVehicle(v)}>
                <div style={{ overflow: "hidden", height: 220, background: "#111" }}>
                  <img className="vehicle-img" src={v.image} alt={`${v.brand} ${v.model}`}
                    style={{ width: "100%", height: "100%", objectFit: "cover" }}
                    onError={(e) => { e.target.style.display = "none"; }}
                  />
                </div>
                <div style={{ padding: "20px 24px" }}>
                  <div style={{ display: "flex", justifyContent: "space-between", alignItems: "flex-start", marginBottom: 12 }}>
                    <div>
                      <div style={{ fontSize: 11, color: "#666", letterSpacing: 2, textTransform: "uppercase", marginBottom: 4 }}>{v.brand}</div>
                      <div style={{ fontSize: 20, fontWeight: 600, color: "#fff" }}>{v.model}</div>
                    </div>
                    <div style={{ fontSize: 20, fontWeight: 700, color: "#D4AF37" }}>{v.price}</div>
                  </div>
                  <div style={{ display: "flex", gap: 16, flexWrap: "wrap", marginTop: 16, paddingTop: 16, borderTop: "1px solid #222" }}>
                    {[
                      { icon: "⚡", val: v.km + " km" },
                      { icon: "📅", val: v.year },
                      { icon: "🐎", val: v.hp + " ch" },
                      { icon: "💺", val: v.seats + " pl." },
                    ].map((d, j) => (
                      <div key={j} style={{ fontSize: 12, color: "#888", display: "flex", alignItems: "center", gap: 4 }}>
                        <span style={{ fontSize: 12 }}>{d.icon}</span> {d.val}
                      </div>
                    ))}
                  </div>
                </div>
              </div>
            </AnimatedSection>
          ))}
        </div>
      </section>

      {/* VEHICLE MODAL */}
      {selectedVehicle && (
        <div className="modal-overlay" onClick={() => setSelectedVehicle(null)}>
          <div onClick={e => e.stopPropagation()} style={{
            background: "#141414", borderRadius: 16, maxWidth: 700, width: "100%",
            border: "1px solid #222", overflow: "hidden", maxHeight: "90vh", overflowY: "auto"
          }}>
            <div style={{ position: "relative" }}>
              <img src={selectedVehicle.image} alt={selectedVehicle.model}
                style={{ width: "100%", height: 320, objectFit: "cover" }} />
              <button onClick={() => setSelectedVehicle(null)} style={{
                position: "absolute", top: 16, right: 16, background: "rgba(0,0,0,0.6)", border: "none",
                color: "#fff", width: 36, height: 36, borderRadius: "50%", cursor: "pointer",
                display: "flex", alignItems: "center", justifyContent: "center"
              }}><CloseIcon /></button>
            </div>
            <div style={{ padding: 32 }}>
              <span style={{ fontSize: 11, color: "#D4AF37", letterSpacing: 3, textTransform: "uppercase" }}>{selectedVehicle.brand}</span>
              <h3 style={{ fontFamily: "'Playfair Display', serif", fontSize: 32, color: "#fff", marginTop: 4, marginBottom: 8 }}>{selectedVehicle.model}</h3>
              <div style={{ fontSize: 28, fontWeight: 700, color: "#D4AF37", marginBottom: 24 }}>{selectedVehicle.price}</div>
              <div style={{ display: "grid", gridTemplateColumns: "repeat(4, 1fr)", gap: 12, marginBottom: 24 }}>
                {[
                  { label: "Kilométrage", val: selectedVehicle.km + " km" },
                  { label: "Année", val: selectedVehicle.year },
                  { label: "Puissance", val: selectedVehicle.hp + " ch" },
                  { label: "Places", val: selectedVehicle.seats },
                ].map((d, i) => (
                  <div key={i} style={{ background: "#1a1a1a", borderRadius: 8, padding: 16, textAlign: "center" }}>
                    <div style={{ fontSize: 11, color: "#666", letterSpacing: 1, textTransform: "uppercase", marginBottom: 6 }}>{d.label}</div>
                    <div style={{ fontSize: 16, fontWeight: 600, color: "#fff" }}>{d.val}</div>
                  </div>
                ))}
              </div>
              <p style={{ color: "#999", lineHeight: 1.8, fontSize: 15, marginBottom: 24 }}>{selectedVehicle.description}</p>
              <a href="tel:0761509269" style={{ textDecoration: "none" }}>
                <button className="btn-gold" style={{ width: "100%" }}>Appeler pour réserver</button>
              </a>
            </div>
          </div>
        </div>
      )}

      {/* REVIEWS */}
      <section id="reviews" style={{ padding: "100px 40px", background: "#0f0f0f" }}>
        <div style={{ maxWidth: 1200, margin: "0 auto" }}>
          <AnimatedSection>
            <div style={{ textAlign: "center", marginBottom: 60 }}>
              <span style={{ fontSize: 12, letterSpacing: 5, textTransform: "uppercase", color: "#D4AF37", fontWeight: 500 }}>Témoignages</span>
              <h2 className="section-title" style={{ fontFamily: "'Playfair Display', serif", fontSize: 42, fontWeight: 700, color: "#fff", marginTop: 12 }}>
                Avis de nos Clients
              </h2>
              <div className="gold-separator" style={{ marginTop: 20 }} />
              <div style={{ display: "flex", justifyContent: "center", gap: 4, marginTop: 16 }}>
                {[...Array(5)].map((_, i) => <StarIcon key={i} />)}
                <span style={{ color: "#888", fontSize: 14, marginLeft: 8 }}>5.0 / 5</span>
              </div>
            </div>
          </AnimatedSection>

          <div className="reviews-grid" style={{ display: "grid", gridTemplateColumns: "repeat(auto-fill, minmax(260px, 1fr))", gap: 20 }}>
            {currentReviews.map((r, i) => (
              <AnimatedSection key={reviewPage + "-" + i} delay={i * 0.1}>
                <div className="review-card">
                  <div style={{ display: "flex", gap: 3, marginBottom: 12 }}>
                    {[...Array(5)].map((_, j) => <StarIcon key={j} />)}
                  </div>
                  <p style={{ color: "#bbb", fontSize: 14, lineHeight: 1.7, marginBottom: 16, fontStyle: "italic" }}>"{r.text}"</p>
                  <div style={{ display: "flex", justifyContent: "space-between", alignItems: "center" }}>
                    <div style={{ display: "flex", alignItems: "center", gap: 10 }}>
                      <div style={{ width: 36, height: 36, borderRadius: "50%", background: "linear-gradient(135deg, #D4AF37, #8B7320)", display: "flex", alignItems: "center", justifyContent: "center", fontSize: 14, fontWeight: 600, color: "#000" }}>
                        {r.name.charAt(0)}
                      </div>
                      <span style={{ fontWeight: 500, fontSize: 14 }}>{r.name}</span>
                    </div>
                    <span style={{ color: "#555", fontSize: 12 }}>{r.date}</span>
                  </div>
                </div>
              </AnimatedSection>
            ))}
          </div>

          <div style={{ display: "flex", justifyContent: "center", gap: 10, marginTop: 32 }}>
            {[...Array(totalPages)].map((_, i) => (
              <button key={i} className={`page-dot ${i === reviewPage ? "active" : ""}`} onClick={() => setReviewPage(i)} />
            ))}
          </div>
        </div>
      </section>

      {/* SOCIAL */}
      <section style={{ padding: "80px 40px", borderTop: "1px solid #1a1a1a" }}>
        <div style={{ maxWidth: 600, margin: "0 auto", textAlign: "center" }}>
          <AnimatedSection>
            <span style={{ fontSize: 12, letterSpacing: 5, textTransform: "uppercase", color: "#D4AF37", fontWeight: 500 }}>Suivez-nous</span>
            <h2 className="section-title" style={{ fontFamily: "'Playfair Display', serif", fontSize: 36, fontWeight: 700, color: "#fff", marginTop: 12, marginBottom: 32 }}>
              Nos Réseaux Sociaux
            </h2>
            <div style={{ display: "flex", justifyContent: "center", gap: 24 }}>
              <a href="https://instagram.com/nrkprestige" target="_blank" rel="noopener noreferrer" className="social-btn" title="Instagram">
                <InstagramIcon />
              </a>
              <a href="https://tiktok.com/@nrkprestige" target="_blank" rel="noopener noreferrer" className="social-btn" title="TikTok">
                <TiktokIcon />
              </a>
            </div>
          </AnimatedSection>
        </div>
      </section>

      {/* CONTACT */}
      <section id="contact" style={{ padding: "100px 40px", background: "#0f0f0f" }}>
        <div style={{ maxWidth: 1000, margin: "0 auto" }}>
          <AnimatedSection>
            <div style={{ textAlign: "center", marginBottom: 60 }}>
              <span style={{ fontSize: 12, letterSpacing: 5, textTransform: "uppercase", color: "#D4AF37", fontWeight: 500 }}>Prenez rendez-vous</span>
              <h2 className="section-title" style={{ fontFamily: "'Playfair Display', serif", fontSize: 42, fontWeight: 700, color: "#fff", marginTop: 12 }}>
                Nous Contacter
              </h2>
              <div className="gold-separator" style={{ marginTop: 20 }} />
            </div>
          </AnimatedSection>

          <div className="contact-grid" style={{ display: "grid", gridTemplateColumns: "repeat(2, 1fr)", gap: 20 }}>
            {[
              { icon: <PhoneIcon />, label: "Téléphone", value: "07 61 50 92 69", href: "tel:0761509269" },
              { icon: <MailIcon />, label: "Email", value: "nrkprestige@gmail.com", href: "mailto:nrkprestige@gmail.com" },
              { icon: <MapIcon />, label: "Adresse", value: "33 Rue Joliot Curie, 69780 Mions", href: "https://maps.google.com/?q=33+Rue+Joliot+Curie+69780+Mions" },
              { icon: <ClockIcon />, label: "Horaires", value: "9h30 - 18h30 (sauf dimanche)" },
            ].map((c, i) => (
              <AnimatedSection key={i} delay={i * 0.1}>
                <a href={c.href || "#"} target={c.href?.startsWith("http") ? "_blank" : undefined} rel="noopener noreferrer"
                  style={{ textDecoration: "none", color: "inherit" }}>
                  <div style={{
                    background: "#141414", border: "1px solid #1e1e1e", borderRadius: 12,
                    padding: 28, display: "flex", alignItems: "center", gap: 20,
                    transition: "all 0.4s", cursor: c.href ? "pointer" : "default"
                  }}
                  onMouseEnter={e => { e.currentTarget.style.borderColor = "rgba(212,175,55,0.3)"; e.currentTarget.style.transform = "translateY(-2px)"; }}
                  onMouseLeave={e => { e.currentTarget.style.borderColor = "#1e1e1e"; e.currentTarget.style.transform = "translateY(0)"; }}
                  >
                    <div style={{ width: 48, height: 48, borderRadius: "50%", background: "rgba(212,175,55,0.1)", display: "flex", alignItems: "center", justifyContent: "center", color: "#D4AF37", flexShrink: 0 }}>
                      {c.icon}
                    </div>
                    <div>
                      <div style={{ fontSize: 11, color: "#666", letterSpacing: 2, textTransform: "uppercase", marginBottom: 4 }}>{c.label}</div>
                      <div style={{ fontSize: 15, fontWeight: 500 }}>{c.value}</div>
                    </div>
                  </div>
                </a>
              </AnimatedSection>
            ))}
          </div>

          <AnimatedSection delay={0.4}>
            <div style={{ marginTop: 40, borderRadius: 12, overflow: "hidden", border: "1px solid #1e1e1e" }}>
              <iframe
                src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d2786.8!2d4.955!3d45.67!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x0%3A0x0!2zNDXCsDQwJzEyLjAiTiA0wrA1NycxOC4wIkU!5e0!3m2!1sfr!2sfr!4v1"
                width="100%" height="300" style={{ border: 0, filter: "invert(0.92) hue-rotate(180deg) brightness(0.8) contrast(1.2)" }}
                allowFullScreen loading="lazy"
                title="NRK Prestige - Localisation"
              />
            </div>
          </AnimatedSection>
        </div>
      </section>

      {/* FOOTER */}
      <footer style={{ borderTop: "1px solid #1a1a1a", padding: "40px 40px 24px", background: "#0a0a0a" }}>
        <div className="footer-inner" style={{ maxWidth: 1200, margin: "0 auto", display: "flex", justifyContent: "space-between", alignItems: "center" }}>
          <div>
            <span style={{ fontFamily: "'Playfair Display', serif", fontSize: 20, fontWeight: 700, color: "#D4AF37", letterSpacing: 2 }}>NRK</span>
            <span style={{ fontSize: 10, fontWeight: 300, letterSpacing: 3, color: "#666", marginLeft: 6, textTransform: "uppercase" }}>Prestige</span>
          </div>
          <div style={{ color: "#555", fontSize: 12 }}>
            © {new Date().getFullYear()} NRK Prestige — Tous droits réservés
          </div>
        </div>
      </footer>

      {/* ADMIN FAB */}
      <button className="admin-fab" onClick={() => setShowAdmin(true)} title="Administration">
        <DashIcon />
      </button>

      {/* ADMIN PANEL */}
      {showAdmin && (
        <div className="modal-overlay" onClick={() => { setShowAdmin(false); setAdminAuth(false); setPassword(""); }}>
          <div onClick={e => e.stopPropagation()} style={{
            background: "#141414", borderRadius: 16, maxWidth: 600, width: "100%",
            border: "1px solid #222", maxHeight: "85vh", overflowY: "auto", padding: 32
          }}>
            <div style={{ display: "flex", justifyContent: "space-between", alignItems: "center", marginBottom: 24 }}>
              <h3 style={{ fontFamily: "'Playfair Display', serif", fontSize: 24, color: "#D4AF37" }}>Dashboard Admin</h3>
              <button onClick={() => { setShowAdmin(false); setAdminAuth(false); setPassword(""); }} style={{ background: "none", border: "none", color: "#666", cursor: "pointer" }}><CloseIcon /></button>
            </div>

            {!adminAuth ? (
              <div>
                <p style={{ color: "#888", marginBottom: 16, fontSize: 14 }}>Entrez le mot de passe administrateur</p>
                <input className="input-field" type="password" placeholder="Mot de passe" value={password}
                  onChange={e => setPassword(e.target.value)}
                  onKeyDown={e => { if (e.key === "Enter" && password === ADMIN_PASSWORD) setAdminAuth(true); }}
                />
                <button className="btn-gold" style={{ width: "100%", marginTop: 16 }}
                  onClick={() => { if (password === ADMIN_PASSWORD) setAdminAuth(true); }}>
                  Connexion
                </button>
              </div>
            ) : (
              <div>
                <div style={{ background: "#1a1a1a", borderRadius: 10, padding: 20, marginBottom: 24 }}>
                  <h4 style={{ color: "#D4AF37", fontSize: 14, letterSpacing: 2, textTransform: "uppercase", marginBottom: 16 }}>Ajouter un véhicule</h4>
                  <div style={{ display: "grid", gridTemplateColumns: "1fr 1fr", gap: 10 }}>
                    <input className="input-field" placeholder="Marque *" value={newVehicle.brand} onChange={e => setNewVehicle({ ...newVehicle, brand: e.target.value })} />
                    <input className="input-field" placeholder="Modèle *" value={newVehicle.model} onChange={e => setNewVehicle({ ...newVehicle, model: e.target.value })} />
                    <input className="input-field" placeholder="Prix (ex: 42 900€)" value={newVehicle.price} onChange={e => setNewVehicle({ ...newVehicle, price: e.target.value })} />
                    <input className="input-field" placeholder="Kilométrage" value={newVehicle.km} onChange={e => setNewVehicle({ ...newVehicle, km: e.target.value })} />
                    <input className="input-field" placeholder="Année" value={newVehicle.year} onChange={e => setNewVehicle({ ...newVehicle, year: e.target.value })} />
                    <input className="input-field" placeholder="Chevaux" value={newVehicle.hp} onChange={e => setNewVehicle({ ...newVehicle, hp: e.target.value })} />
                    <input className="input-field" placeholder="Nombre de places" value={newVehicle.seats} onChange={e => setNewVehicle({ ...newVehicle, seats: e.target.value })} />
                    <input className="input-field" placeholder="URL de l'image" value={newVehicle.image} onChange={e => setNewVehicle({ ...newVehicle, image: e.target.value })} />
                  </div>
                  <textarea className="input-field" placeholder="Description du véhicule" rows={3} style={{ marginTop: 10, resize: "vertical" }}
                    value={newVehicle.description} onChange={e => setNewVehicle({ ...newVehicle, description: e.target.value })} />
                  <button className="btn-gold" style={{ width: "100%", marginTop: 12, display: "flex", alignItems: "center", justifyContent: "center", gap: 8 }}
                    onClick={addVehicle}>
                    <PlusIcon /> Ajouter le véhicule
                  </button>
                </div>

                <h4 style={{ color: "#D4AF37", fontSize: 14, letterSpacing: 2, textTransform: "uppercase", marginBottom: 16 }}>
                  Véhicules actuels ({vehicles.length})
                </h4>
                {vehicles.map(v => (
                  <div key={v.id} style={{
                    display: "flex", justifyContent: "space-between", alignItems: "center",
                    padding: "12px 16px", background: "#1a1a1a", borderRadius: 8, marginBottom: 8,
                    border: "1px solid #222"
                  }}>
                    <div>
                      <span style={{ color: "#888", fontSize: 12 }}>{v.brand}</span>
                      <span style={{ fontWeight: 600, marginLeft: 8 }}>{v.model}</span>
                      <span style={{ color: "#D4AF37", marginLeft: 12, fontSize: 14 }}>{v.price}</span>
                    </div>
                    <button onClick={() => deleteVehicle(v.id)} style={{
                      background: "none", border: "1px solid #333", borderRadius: 6, color: "#ff4444",
                      cursor: "pointer", padding: "6px 10px", display: "flex", alignItems: "center", gap: 4, fontSize: 12,
                      transition: "all 0.3s"
                    }}
                    onMouseEnter={e => { e.currentTarget.style.background = "#ff4444"; e.currentTarget.style.color = "#fff"; e.currentTarget.style.borderColor = "#ff4444"; }}
                    onMouseLeave={e => { e.currentTarget.style.background = "none"; e.currentTarget.style.color = "#ff4444"; e.currentTarget.style.borderColor = "#333"; }}
                    >
                      <TrashIcon /> Supprimer
                    </button>
                  </div>
                ))}
                <button onClick={() => { saveVehicles(DEFAULT_VEHICLES); }} style={{
                  background: "none", border: "1px solid #333", color: "#888", padding: "10px 20px",
                  borderRadius: 6, cursor: "pointer", fontSize: 12, marginTop: 12, width: "100%",
                  fontFamily: "'Outfit', sans-serif", transition: "all 0.3s"
                }}
                onMouseEnter={e => { e.currentTarget.style.borderColor = "#D4AF37"; e.currentTarget.style.color = "#D4AF37"; }}
                onMouseLeave={e => { e.currentTarget.style.borderColor = "#333"; e.currentTarget.style.color = "#888"; }}
                >
                  Réinitialiser les véhicules par défaut
                </button>
              </div>
            )}
          </div>
        </div>
      )}
    </div>
  );
}
