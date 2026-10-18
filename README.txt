====================================================
YOURCLOTHES — VIRTUAL TRY-ON WEBSITE (ALPHA)
====================================================
Owner: Youssef (solo 3D Motion Designer, Morocco)
Built with: OpenCode (GLM) — 100% free tools
Stage: v0.2.2 — hero functional, waiting for 3D model
File: YourClothes/index.html (SINGLE FILE — no install)

----------------------------------------------------
1. L-CONCEPT (li tbi3 bih)
----------------------------------------------------
Client ydkhel height+weight → yjereb jackets/pants/cap/shoes
3la avatar 3D LIVE (drag+zoom) → y5tar size/color → order
via WhatsApp COD. Fit accuracy FIRST, fun second.
Target: clothing brands maghribiya. Ticket: 8,000-15,000 DH
+ retainer maintenance/garments jdad.

----------------------------------------------------
2. DESIGN = MIX DIAL 3 REFERENCES
----------------------------------------------------
- ZYON (olive tracksuit site): structure + mood + nav pill
  top center + icons top right + size circles right + dark
- PLANET BOLD (sneaker pink): pop color world, dots
- JACKET MASTERS (orange puffer): price block with old price
  strike, tagline bottom, left copy+CTA
Font: Space Grotesk (kolchi) + Unbounded (loader ghir)
Logo: YC monogram — Logo.png (tayyar user) → Logo_t.png
  transparent (generated, crop 910x278) f header + favicon

----------------------------------------------------
3. PRODUCTS (3 looks, go daily via arrows/nav/keys)
----------------------------------------------------
1. PUFFER JACKET — $149/$199 — world #e8630a orange
   dots: orange/white/black — sizes S M L XL
2. TRACKSUIT — $349/$399 — world #8a8f66 olive
   dots: olive/black/white
3. SNEAKER SET — $129/$159 — world #e0245e pink
   dots: pink/yellow/black — sizes 40-44

WORLD COLOR = clicking "CHOOSE YOUR COLOR" dots changes
the ENTIRE background (world swap). Light colors auto-flip
UI to dark text (body.light class, luminance > .58).

----------------------------------------------------
4. FEATURES KHDAMIN DABA
----------------------------------------------------
[x] Pill nav (3 products) + carousel arrows + keys -> / <-
[x] Color dots = live world/background swap
[x] Size circles (S M L XL) selected state
[x] Add to cart button (+ Add to cart) → cart items
[x] Cart icon → drawer: items, remove, total, ORDER VIA
    WHATSAPP (auto message b items + total)
[x] Wishlist heart → toggle + badge counter
[x] Search icon → overlay search bar (filter by name,
    Enter = first result, Escape = close)
[x] Account icon → drawer with login form (demo stub)
[x] Socials IG / FB / X / YouTube = clickable SVG icons
    (placeholder URLs: @yourclothes.ma — bdelhom men b3d)
[x] Place order button → wa.me/212600000000 (BDEL NUMBER)
[x] Try it live → studio panel: height/weight sliders +
    recommended size (BMI S/M/L/XL)
[x] Responsive mobile (nav hidden, panels reflow)
[x] Grain overlay + scrim readability + loader
[x] v0.2.3: UI strings unified EN (cart/wishlist/account/search/
    fallback/drawers) — no Darija inside the UI, saraha demo n9ia
[x] v0.2.5: font system — display=Unbounded (H1/price/nav/CTAs/
    sizes/tag), UI=Borela local OTF (Borela/BORELA.otf via
    @font-face, replaced Space Grotesk; note: Borela = 1 weight)
[x] v0.2.5: reviews chip (bottom center, frosted glass) — 6 fake
    positive reviews FR w/ Moroccan names+cities, auto-rotate 4.2s,
    click=next, pause on hover, hidden mobile
[x] v0.2.6: localStorage persist (cart+wishlist survive reload:
    ycCart/ycWish) · gold REC ring on recommended size circle
    (sync w/ studio BMI sliders) · discount % badge (auto from
    price/old) · stock urgency line (● Only N left in SIZE)
[x] v0.3: SECOND THEME VERSION = bento.html (index.html kept
    as v1, untouched). Bento grid layout per user ref image:
    dark textured bg + light streaks bottom, frame radius 38
    w/ matte tiles. Mapping: tlogo=YC logo · rail(pill)=prev/
    next + 3 product dots + socials + account avatar · tstage
    = 3D scene (cwrap for canvas+world tint, overflow trick
    for notch) + eyebrow/H1/para/shopline/stock/tagline/color
    dots · notch on stage left edge = try-on studio toggle ·
    ticons pill = search morph/wishlist/cart/location/theme/
    ORDER(wa) · tside = COLLECTION list (3 rows, active light
    bg) replaces nav pills · tkeys = size KEYS (keyboard look)
    + REC tag + price pill + ADD TO CART · tdeck = fanned
    reviews deck (3 stacked cards, click/auto 5.2s, fly-out).
    Theme toggle (sun/moon) replaces auto-light. Search morph
    same logic. localStorage same keys. MODEL_URL slot same.
    Mobile: frame stacks (rail hidden). JS checked node OK.
[x] v0.3.1 fixes (bento): theme-follows-product = frame aura
    box-shadow + page bottom glow + cwrap tile tint all use
    color-mix(w var(--world)) w/ .6-.7s transitions · reviews
    deck stacking FIXED (pos1/pos2 painted above pos0 w/o
    z-index -> mixed text; now z 3/2/1 + fly z 5 + pos0 re-entry
    dIn animation, opacities .6/.35) · Logo_t.png regenerated
    (full bbox thresh 40 + pad 20 -> 921x285, wordmark
    YOURCLOTHES complete w/ final S, verified on orange comp)
[x] v0.3.2: FULL theme = product color. All surfaces (bg/frame/
    tile/tile2/line, dark+light) now color-mix(var(--world) %,)
    dark base: bg 14% frame 20% tile 25% tile2 34% line 26%
    (light: 16/24/10/20/32) -> yellow product = whole theme
    olive/gold, pink = wine etc. cwrap reverted to var(--tile)
    (tint now lives in :root). Loader/drawer glass stay neutral
    for contrast; active states stay white (brand rule).
[x] v0.3.3: reviews deck = continuous conveyor (was: fly 380ms
    then full innerHTML rebuild = gap/blink between reviews).
    Now: dvi++ first, classes shift pos1->pos0 & pos2->pos1
    (CSS transition slides them), NEW pos2 card dealt in w/
    .enter state removed after double rAF, old card .fly
    removed at 620ms. No innerHTML resets during rotation.
    Interval 5.2s -> 5s. dIn keyframes removed (raced
    transitions). JS checked.
[x] v0.3.4: studio notch (floating ↕ circle on stage left edge,
    read as "stuck mid-screen") REMOVED from stage. Try-on
    studio toggle moved to SIZE tile khead, right of "REC · M"
    (logic: studio drives the size recommendation). khead now
    labe | khright(recTag + iconbtn ctaTry). .notch CSS +
    mobile media notch rule deleted. JS checked.
[x] v0.3.5: SEARCH = IN-CARD MORPH (per user "hole/seamless"
    request). Fixed floating overlay bar (was: bar + X floating
    over/inside icons pill = looked stuck mid-card). Now the
    icons pill IS the bar: click search -> other controls
    (wish/cart/loc/theme/order) collapse to width 0 w/ stagger
    delays (.05-.25s), sFill flex-grows to fill card, magnifier
    icon stays as bar start. Gap 5->0 animated. Click-outside/
    X/Escape/Enter close. Results panel anchored UNDER pill,
    right-aligned to card (top=bottom+8, right+width from
    iconsPill rect). Open/close = click only (no hover). JS OK.
[x] v0.3.6: bento tlogo now uses NEW Logo_sq.png (YC monogram
    only 429x170, auto-split from Logo_t.png via largest
    transparent row gap y190 + bbox pad 14, verified on comp).
    Full wordmark Logo_t.png kept for loader + v1 header (tile
    76px too small for wordmark = was clipped "YOURCLOT").
[x] v0.3.7: drawers + studio = bento tiles now (was: floating
    dark-glass overlays top-right = looked like v1 leftovers,
    acc drawer appeared over COLLECTION while trigger is rail
    avatar). Restyled matte: var(--tile) + line border + big
    soft shadow, no blur. Anchored to triggers via anchorDw():
    accD = above rail avatar (left-aligned), cartD/locD = below
    icons pill (right-aligned), studio = above SIZE tile right
    by !important in mobile media. JS checked.
[x] DEPLOY: Vercel Hobby (free), CLI 64.5.0 installed global,
    login via device flow (GitHub), project "yourclothes"
    (scope vegasander01-9705s-projects), .vercelignore skips
    README.txt. PRODUCTION: https://yourclothes-xi.vercel.app
    (v1 = /, bento = /bento.html — both verified 200, font
    font/otf 200 len 61.8KB, logos 200). Redeploy: vercel
    deploy --prod --yes (in YourClothes dir). NOTE: new GLB
    additions need redeploy. Custom domain later via dashboard.
[x] v0.2.3: logo = YC monogram Logo.png → Logo_t.png transparent
    + favicon (spotlight-noise bg removed programmatically)
[x] v0.2.4: motion pass — entrance choreo (pre→ready), product
    swap slide/blur + h1 word-by-word stagger, sizes/dots pop,
    scene pulse on swap, hover lifts, idle model spin (3D slot)

BOT TAYYAR: REMOVED (user decision — may return later
m3a model). Concepts: bubbles, chat log, reactions fihom ba9i
f git history mn alpha v0.1 l9dima.

La 3dyana: pedestal + giant word "WARM" + floor rings —
REMOVED (user decision). Scene = clean background only.

----------------------------------------------------
5. THE GLB MODEL SLOT (L-BDAQA DYAL MODEL DYALEK)
----------------------------------------------------
Scene fih group fard: MODELSLOT (y = 0, center).
Bach t’inject l model:
1) 7et l file .glb f: YourClothes/models/  (e.g. look1.glb)
2) F index.html lowl dial script, beddel:
   const MODEL_URL = './models/look1.glb'   (daba = null)
Auto: scale to 1.55m height, center, add to slot.
Format: .glb preferred (Blender export GLTF binary).
NOTE: core manual position: m.position.y = -c.y*scale
   (feet at 0). Ila model dyalekma mkyass jib liya w ana
n7tah f slot bi wa7ed tweak dial scale.

----------------------------------------------------
6. NEXT STEPS (ROADMAP)
----------------------------------------------------
[ ] MODEL_URL injection (model dyalek GLB) → PRIORITY 1
[ ] Interactions 3la model: garment swap, color tint
[ ] Bot reactions (maybe) wla fit feedback badge
[ ] Checkout: COD form (nom, tel, ville, adresse) → wa.me
[ ] Products b2 = REAL data + images + sizes DH (madam
    Morocco: prices b DH mchi $, COD f, livraison villes)
[ ] Deploy: Vercel free + domain .com (~150 DH/3am)
[ ] README updated f kol change kbir (l /compact)

----------------------------------------------------
7. NOTES TECHNIQUES
----------------------------------------------------
- Single file: index.html. No build. Open f Chrome immediat.
- CDN: three@0.160.0 (jsdelivr) + Google Fonts.
- WebGL fallback included. DPR capped 2 (mobile perf).
- OrbitControls: target y=1.02, dist 2.4-7, no pan.
- State: S = {h, w, size(index), dot(index)}; P = product idx.
- Colors via CSS vars --world/--world-deep on documentElement.
- body.light class = dark UI text on light backgrounds.
- Ikhtar sizes sotayra: sizes circles animate transform.

Backend? LA. 100% static demo (Vercel-ready). Data hna
(PRODUCTS array f script). F v0.3: lakhar products json.

----------------------------------------------------
8. SNAPSHOT DYAL L-KHDMA (l /compact memory)
----------------------------------------------------
tihya: 3 references f user siftohom (JACKET MASTERS orange
puffer, PLANET pink sneaker BOLD, ZYON olive tracksuit).
Bot removed, WARM giant word removed, pedestal removed,
rings removed. Logo = hanger mark + Unbounded wordmark.
Icons khdamin kamlin (search/wishlist/cart/account/socials
+ YouTube). Cart = WhatsApp order message. Studio = sliders
+ BMI size. User ghadi ydir /compact mn be3d had l-file.

User rules bdihom 3liya:
- Nta (user) director: nta tgol, ana ndir. Similar messages
  daba: "GO" = start, "SF" = check.
- Ma njawboch 3la swel 9bel ma ykml idea dyalek.
- Reply b Darija (latin) m3a terms tech English.
- Thread wahed f marra — nsaliwh wla n9tloh.
- Never download b-la permission + show links lowl.
- Kif tkmel milestone kbir = dir README update (had l-file).
====================================================
END — v0.2.2 — 2026-10-17
====================================================
