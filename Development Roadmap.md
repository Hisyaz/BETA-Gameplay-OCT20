# Development Roadmap: Next-Gen Lightweight Football Simulation

## Vision & Architecture Principles
Build an authentic, tactical, and fluid football experience that runs at a solid 60 FPS even on low-end and older mobile devices.
- **Authentic Football Realism (Zero Magic, Zero Superpowers)**: Pure grounded, tactile physical football. No giant glowing sci-fi shields, neon magical forcefields, or arcade superpowers. Ball protection is achieved purely through realistic physical body leverage, arm placement, planted studs, and a low center of gravity.
- **Maximum Compatibility & Locked 60 FPS on Budget Phones**: Optimized to run silky-smooth on $50 budget Android devices, older iPhones, and low-spec hardware without garbage collection spikes or thermal throttling. Zero bulky 3D meshes; all visual features (cinematics, replays, player ratings, video ref) are built using lightweight procedural HTML5 Canvas 2D math and pre-allocated zero-allocation buffers.
- **32-Bit Arcade Console Design Constitution**: Pure late-90s / early-2000s 32-bit console visual identity (metallic console gradients, dithered shading, beveled arcade borders, tactile chiseled buttons).
- **Mobile-First UI Without Clutter**: Console-style layouts avoiding vertical/horizontal scrolling on mobile devices and desktop displays; single-screen accessibility with intuitive toggles.
- **Realistic Ball & Match Flow Physics**: Sub-millisecond deterministic game loop with authentic trajectory physics, official IFAB match regulation timing (45m halves, stoppage time calculation, intelligent half/full time whistle logic, extra time & penalty shootouts).
- **Daily Token Budget Calibration**: Strictly 1 Phase = 1 Day's worth of Google AI Studio tokens (~600k–900k tokens over focused engineering turns), guaranteeing a 100% compiled and playable build at the end of each session.

---

# Completed Roadmap Archive (Summary of Phases 1 – 18)

Below is the verified summary of all completed development milestones across the initial development lifecycle:

| Phase | Title | Core Technical Accomplishments |
| :---: | :--- | :--- |
| **Phase 0.5** | **Match Rules, Foul Attribution & Modern Pressing** | Symmetrical foul recognition; strict discrimination between attacking penalty box (penalties) vs. defending box (defensive free kicks); zero friendly-fire tackles; 2026 pressing triggers (backward-facing, sideline traps, loose-ball contest). |
| **Phase 0.6** | **Driven Through-Balls & Camera Suite** | Driven ground through-balls (`W`) with forward leading space vector; delicate chipped long pass over defensive lines (`E + W`); swerving pass (`Q + W`); 3-mode broadcast camera suite (Pitch auto-framing, Ball lock, Player lock). |
| **Phase 1** | **Ball Out-of-Bounds & Set-Piece Attribution** | Robust previous-vs-current segment raycasting distinguishing touchline exits (throw-ins) from endline exits; strict last-touch attribution (attacking touch $\rightarrow$ goal kick; defending deflection/keeper save $\rightarrow$ corner kick). |
| **Phase 2** | **Passing, Shooting & Skill-Chip Delivery** | 4-button canonical control scheme (Short pass `S`, Lead pass `W`, Box cross `D`, Shot `A`); `E` chip modifier suite for scoop chip shots, floating crosses, and lofted passes. |
| **Phase 3** | **Lowered Set-Piece Camera & Aiming Engine** | Immersive pitch-level lowered camera perspective for free kicks and penalties; target aiming reticle with elevation & bend dials; timing-based shot power meter; defensive wall jump duels. |
| **Phase 4** | **Dynamic Team AI, Pressing & Off-Ball Runs** | 2-man pressing traps (Hunter + Trap Closer + Cover Shadow); intelligent teammate support triangles and blindside runs; offside line tracking; zero-allocation mobile AI loops. |
| **Phase 5** | **Canonical Player Stats Architecture** | 18 outfield stats across 6 pillars (Pace, Stamina, Strength; Ball Control, Retention, Dribbling; Short Pass, Long Pass, Crossing; Shooting, Heading, Long Shots; Tackling, Sliding, Interceptions, Marking; Positioning, Composure, Reactions) + 7 Goalkeeper metrics (Saving, Reflexes, Handling, Positioning, Aerial Reach, 1v1, Distribution). |
| **Phase 6** | **Attribute Progression Tiers & Stat Breaks** | 4 canonical tiers (Amateur 40–69, Pro 70–84, Elite 85–94, Pinnacle 95–99) + Stat Break breakthrough traits (>99); duel resolution matrices for speed, dribbling vs. tackling, and aerial battles. |
| **Phase 7** | **Positional Hierarchy & Tactical Playstyles** | 3-tier hierarchy (Primary $\rightarrow$ Sub-Position $\rightarrow$ Playstyle); 16 distinct sub-positions; 28 specialized player playstyles (Poacher, Box-to-Box, Regista, Inverted Fullback, Libero, Sweeper GK, etc.). |
| **Phase 7.5** | **Controls & Ball State Machine Polish** | Progressive charge meter running alongside player cleats; dead-ball collision barriers; touch joystick calibration. |
| **Phase 8** | **Expressive Procedural Animations Suite** | Procedural animation state machine (dribbling cadence, body feints, driven laces strike, trivela, sliding toe poke, bullet header, diving volley, acrobatic GK saves). |
| **Phase 9** | **Scalable 3-Tier Graphics & Retro Filters** | Scalable pipeline (Performance, Balanced, High-End); Quad-Shadow floodlights; zero-lag hardware-accelerated CRT Arcade, VHS 1994, Neo-Geo 16-Bit, and Manga retro filters. |
| **Phase 9.5** | **AI Set-Piece Overhaul & Grounded Realism** | AI throw-in distribution; direct free kick tactical intelligence; subtle anti-magic ball shielding with zero forcefield graphics. |
| **Phase 10** | **Dynamic Stadiums & Match Atmosphere** | 3 stadium tiers (Monumental Grand Arena, Craven Heritage Ground, Ascenso Municipal); rendered city horizon; custom seat color modes; time-of-day lighting. |
| **Phase 11** | **Pitch Dimensions, Weather & Surface Physics** | IFAB pitch dimensions (Compact, Balanced, Expansive, Custom); turf puddles with ball hydroplaning; winter snow with red line markings and orange/yellow balls; Brazilian deep-box nets. |
| **Phase 12** | **Parametric Player Appearance Framework** | Zero-GC 120-byte player appearance contract (skin tones, hairstyles, facial hair, uniform fits, sleeve length, tattoos, physical body scaling 0.92–1.08). |
| **Phase 13** | **Multi-Tier Team Database & Selection Engine** | Drill-down team selection (Clubs, National, Special); randomizer roulette; 4 rating tiers (S, A, B, C); canonical set-piece role specialist assignments. |
| **Phase 13.5** | **Expanded Teams & All-Time Legends** | 2026 World Cup squads, historic South American clubs, Bogotá FC derby, and 7 All-Time Continental Dream Teams. |
| **Phase 14** | **Pre-Match Presentation & Modular Uniforms** | Split-screen presentation layout; 32-bit captain hero sprites; modular kit mixer (shirts, shorts, socks) with automatic anti-clash contrast engine. |
| **Phase 15** | **Dual-Pitch Tactical Game Plan Board** | Side-by-side tactical boards (desktop) and toggleable single pitch (mobile); OVR star ratings; live bench drag-and-drop substitutions; dedicated set-piece role picker. |
| **Phase 16** | **32-Bit Retro Aesthetic & Pitch Drag-and-Drop** | Compact jersey silhouette with squad numbers; interactive pitch drag-and-drop with live positional reclassification; 32-bit metallic console styling across all menus. |
| **Phase 16.5** | **Drop-Zone Grid & Overlap Disambiguation** | 3-tier mechanical pitch partition (ATT, MID, DEF, locked GK sanctuary); multi-role overlap popover (ST/SS, CM/CAM, CM/CDM, LM/LWB, CB/LIB); automatic reversion to 'Basic' playstyle on incompatible positions. |
| **Phase 17** | **Unified Pre-Match Hub & Atmosphere Suite** | 5-button bottom navigation bar (Uniform, Stadium, Tactics, Settings, Kick Off); 3 turf quality grades (Poor, Normal, Pristine); 7 lawn mowing designs; streamlined 3-button in-game pause hub. |
| **Phase 18** | **Mobile Optimization & GC Hardening** | Zero per-frame memory allocations; pre-allocated vector and particle pools; spatial collision partitioning; locked 60 FPS verified on budget smartphones. |

---

# New Development Roadmap: 32-Bit Tactical Simulation & AI Mastery

## Daily Token Budget Profile (1 Phase = 1 Day's Quota)
- **Bounded Engineering Scope**: Each sprint focuses on 1 to 3 designated modules.
- **Non-Breaking Invariant**: Every phase terminates in a fully compiling, zero-regression, playable build.
- **Console-Grade UI Invariant**: All screens follow pristine 32-bit retro styling with **ZERO vertical or horizontal scrolling** across mobile, tablets, and PC desktop viewports.
- **Budget Phone Performance Invariant**: All new systems (ratings, replays, cinematics, match flow state machines) run zero per-frame memory allocation, ensuring steady 60 FPS on $50 hardware.

---

## Phase 0: 32-Bit Console UI Transition, Zero-Scroll Game Plan, Broadcast HUD & Device Profiling [COMPLETED]
*Priority: Architecture Foundation, Zero-Scroll Viewport Constitution, Custom Formation Rules & Hardware Detection*  
*Daily Token Budget Profile: Scope: `src/components/TacticsModal.tsx`, `src/components/PitchCanvas.tsx`, `src/components/PreMatchPresentationModal.tsx`, `src/components/TeamSelectorModal.tsx`, `src/game/formations.ts`, `src/game/specialTeamsData.ts`, `src/App.tsx` | Target: ~750k tokens*

### 0.1 Zero-Scroll Game Plan & Pitch Scale Overhaul
- **Strict Single-Screen Viewport Fit (No Scrolling Anywhere)**:
  - Eliminate all vertical and horizontal page scrolling from the Game Plan / Tactics board on PC desktop, tablet, and mobile devices.
  - Scale down the pitch dimensions and jersey nodes dynamically using CSS `h-full`, `max-h-[calc(100vh-...)]`, and responsive aspect ratios so the tactical board, bench substitutes, team tactics panel, and navigation buttons fit comfortably on a single screen without requiring any mouse scroll or touch swipe.
  - Ensure all squad numbers, names, sub-positions, and attribute tags are crisp, high-contrast, and legible.
- **Authentic 32-Bit Aesthetic Refinement**:
  - Re-theme the Game Plan screen to match authentic 32-bit console UI (metallic steel/slate gradient panels, chiseled gold/cyan bevels, retro font styling, glowing LED status badges, tactile embossed action buttons).

### 0.2 Custom Formation Engine & Structural Validation Rules
- **Freeform Tactical Pitch Customization**:
  - Allow users to freely adjust and create custom formations by dragging and dropping outfield players across the pitch board.
- **Formation Integrity Rules & Enforcement**:
  - Every custom formation **MUST** satisfy the following canonical line minimums to be structurally valid:
    1. **Goalkeeper**: Exactly 1 GK (locked in sanctuary).
    2. **Defenders**: At least **2 Defenders** (`CB`, `LB`, `RB`, `LWB`, `RWB`, `LIB`).
    3. **Midfielders**: At least **2 Midfielders** (`CDM`, `CM`, `CAM`, `LM`, `RM`).
    4. **Attackers**: At least **1 Attacker** (`ST`, `SS`, `CF`, `LW`, `RW`).
  - **Dynamic Invalidation Banner**: If a player drags a lineup into an illegal structure (e.g. 1 defender or 0 attackers):
    - Display an amber/red retro warning: `"⚠️ INVALID FORMATION: Lineup requires at least 2 Defenders, 2 Midfielders, and 1 Attacker!"`
    - **Disable the `[ CONFIRM ]` / `[ PROCEED ]` button** with a locked indicator until the positional balance is restored.

### 0.3 Gameplay HUD & Mobile Controller Viewport Cleansing
- **Broadcast Clean Screen Mandate**:
  - Remove all redundant top navigation and debug buttons during live gameplay (`MATCHDAY`, `TACTICS`, and `GFC` buttons removed from top gameplay bar).
  - Clean top bar layout:
    - **Top-Left**: Broadcast Scoreboard (Home vs Away, score, match timer, team colors).
    - **Top-Right**: "DRAWSTAR TV" retro broadcast network logo.
    - All secondary match indicators (stoppage time, card alerts) must anchor cleanly below these two top elements.
- **Controller-Aware Viewport & Camera Center Offset**:
  - When the on-screen virtual touch controller is visible and solid, the active camera gameplay framing area is bounded strictly to the screen area **ABOVE** the controller overlay.
  - The center of camera focus must never be obscured or occluded beneath the bottom virtual pad or buttons.
- **Input Method Auto-Detection & Key Allocation Suggestions**:
  - On application startup (prior to team selection):
    - Detect current device profile, touch capability, keyboard availability, and connected Gamepads (`navigator.getGamepads()`).
    - **Keyboard / Controller Detected**: Display an automatic suggestion prompt showing recommended button allocations (e.g., Short Pass: `S` / `Cross`, Shoot: `A` / `Square`, Through Ball: `W` / `Triangle`, Long Pass: `D` / `Circle`).
    - Provide an instant toggle: **Hide On-Screen Controller Entirely** when hardware keyboard or joystick is active.
    - **Touchscreen / Mouse Detected**: Enable responsive on-screen virtual joystick and action buttons.
- **Hardware Performance Profiling & Graphic Quality Suggestion**:
  - Auto-benchmark device capacity (GPU renderer string, logical CPU cores, screen DPR, device memory) and suggest an optimal graphics preset:
    - **Performance**: Optimized for budget devices (flat turf, standard lighting, maximum FPS).
    - **Balanced**: Standard shadows and turf patterns.
    - **High**: Quad-shadow floodlights, retro CRT/scanline filtering, pitch detail.

### 0.4 Special Teams Canonical Formations, Starting XI, Substitutes & Playstyles
Align all 7 Special / Continental Dream Teams with their official historical rosters, tactical formations, managers, and philosophies:
1. **CLASSIC SOUTH AMERICA 🌎**: Mario Zagallo | 4-3-3 | Jogo Bonito | Mazurkiewicz GK; Carlos Alberto, Figueroa, Passarella, Nílton Santos; Falcão CDM, Gérson CM, Maradona CAM; Garrincha RW, Pelé SS (biased left), Romário ST. (Subs: Chilavert, Djalma Santos, Nasazzi, Domingos da Guia, Marzolini, Obdulio Varela, Cubillas, Valderrama, Zico, Jairzinho, Kempes).
2. **CLASSIC EUROPE 🇪🇺**: Bob Paisley | 4-4-2 | Counterattack | Yashin GK; Bergomi, Beckenbauer, Baresi, Krol; Rijkaard CDM, Luis Suárez CM, Matthews RM, Best LM; Cruyff SS, Van Basten ST. (Subs: Zoff, Vogts, Scirea, Moore, Brehme, Matthäus, Charlton, Gento, Kopa, Gullit, Eusébio).
3. **MODERN SOUTH AMERICA 🌎**: Luiz Felipe Scolari | 4-2-3-1 (Offensive) | Jogo Bonito | Alisson GK; Cafu, Thiago Silva, Romero, Roberto Carlos; Casemiro CDM, Redondo CM, Kaká CAM; Messi RW, Ronaldinho LW, Ronaldo Nazário ST. (Subs: E. Martínez, Dani Alves, Lúcio, Ayala, Marcelo, Mascherano, Vidal, Riquelme, Di María, Neymar, L. Suárez).
4. **MODERN EUROPE 🇪🇺**: Carlo Ancelotti | 4-3-3 | Counterattack | Neuer GK; Lahm, Ramos, Cannavaro, Maldini; Busquets CDM, Xavi CM, Zidane CAM; Robben RW, Lewandowski ST, C. Ronaldo LW. (Subs: Casillas, Thuram, Van Dijk, Nesta, Alba, Rodri, Modrić, Iniesta, Bale, Mbappé, Henry).
5. **CAF — AFRICA ALL-STARS 🌍**: Stephen Keshi | 4-2-3-1 (Offensive) | Counterattack | Bono GK; Hakimi, Kolo Touré, Kuffour, Asamoah; Essien CDM, Yaya Touré CM, Okocha CAM; Salah RW, Eto’o LW, Weah ST. (Subs: Mendy, Eboué, Koulibaly, Matip, Taiwo, Mikel, Keita, Abedi Pelé, Mahrez, Mané, Drogba).
6. **ASIA / OCEANIA ALL-STARS 🌏**: Choi Kang-hee | 4-4-2 | Long Ball | Schwarzer GK; Mahdavikia, Hong Myung-bo, Kim Min-jae, Nagatomo; Hasebe CDM, Nakata CM, Park Ji-sung RM, Son Heung-min LM; Cahill SS, Rufer ST. (Subs: Ryan, Moore, Yoshida, Emerton, Lee Young-pyo, Jedinak, Ono, Kagawa, Nakamura, Cha Bum-kun, Ali Daei).
7. **CONCACAF LEGENDS 🌎**: Javier Aguirre | 5-3-2 | Catenaccio | Navas GK; Claudio Suárez, Morgan, Duarte CBs; Alphonso Davies LWB, Landon Donovan RWB; Márquez CDM, Bryan Ruiz CM; Mágico González CAM (biased left), David Suazo SS (biased right), Hugo Sánchez ST (center). (Subs: Ochoa, Balboa, Peña, Brooks, Pulisic, Osorio, Edson Álvarez, Dempsey, Blanco, L. Hernández, Chicharito).

---

## Phase 1: Official Match Regulation Flow, Stoppage Time & Intelligent Whistle Engine [COMPLETED]
*Priority: Complete 2-Half Match Engine, Dynamic Stoppage Time, Non-Dangerous Whistle AI & End-Game Hub*  
*Daily Token Budget Profile: Scope: `src/game/engine.ts`, `src/game/matchRules.ts`, `src/components/PauseModal.tsx`, `src/components/EndGameModal.tsx`, `src/types.ts` | Target: ~800k tokens (1 Day's Quota)*

### 1.1 Complete Match Half State Machine & Stoppage Time Mechanics
- **Match Regulation Halves**:
  - Full match consists of two halves of 45:00 simulated match time.
  - **1st Half Kickoff**: Executed by the **Away team**.
  - **2nd Half Kickoff**: Executed by the **Home team** (automatic side swap).
- **Calculated Stoppage Time (Added Time) Engine**:
  - Added time is displayed directly on the broadcast scoreboard banner (`+1'`, `+2'`, etc.).
  - **1st Half Stoppage Time**:
    - Minimum added time: **1 minute**.
    - Additional time added: **+30 seconds** for every substitution or injury occurring in the first half.
    - Accumulated time rounds to whole minute batches (e.g., 2 subs/injuries = +2 minutes).
  - **2nd Half Stoppage Time**:
    - Minimum added time: **2 minutes**.
    - Additional time added: **+30 seconds** per substitution or injury occurring in the 2nd half.
    - Accrued strictly in 1-minute batches (e.g., 2 subs = +3 minutes total).

### 1.2 Context-Aware Intelligent Referee Whistle Engine
- **Non-Dangerous Ending Logic**:
  - The referee does **NOT** blow the half-time or full-time whistle while a team is in an active, dangerous attacking position.
  - If a team possesses the ball inside or directly threatening the opposing penalty box, the referee allows play to continue until:
    - The ball goes out of play (touchline, endline, or goal scored).
    - Defending team clears the ball out of danger.
  - **Penalty Kicks**: If awarded before whistle, the kick must always be taken; whistle cannot blow until the penalty sequence resolves.
  - **Set-Pieces at the Death**:
    - **Corner Kicks**: 70% probability the referee permits the corner to be delivered; 30% whistle is blown before corner is taken.
    - **Free Kicks**: Same 70% / 30% context-aware decision rule based on distance from target goal.

### 1.3 Halftime Transition & Full-Time End-Game Hub
- **Halftime Transition Screen**:
  - Automatically transitions to a specialized 32-bit Pause / Halftime Menu.
  - Prominent primary action: `[ ⏩ START 2ND HALF ]` (teams switch ends, Home team kicks off).
- **Full-Time End-Game Hub**:
  - **Win / Loss Outcome**: Displayed in 32-bit retro victory/defeat banners.
  - **Available Navigation Actions**:
    1. `[ 🔁 REMATCH ]`: Instantly restarts match with the exact same teams, settings, stadium, and tactics/lineups.
    2. `[ 👥 TEAM SELECTION ]`: Returns user directly to the Team Selector modal.
    3. `[ 📊 STATS ]`: Opens match statistics (placeholder scaffold for upcoming phase).
    4. `[ ⭐ RATINGS ]`: Opens player match ratings (placeholder scaffold for upcoming phase).
    5. `[ ⚙️ SETTINGS ]`: Opens match settings.
    6. `[ 🏠 MAIN MENU ]`: Rendered in disabled state for now.
  - **Draw Resolution Options (After 90 Minutes in Draw)**:
    - `[ ⏱️ EXTRA TIME ]`: Initiates two 15-minute extra time periods (ET1 and ET2), followed by penalty shootout if still tied.
    - `[ 🥅 PENALTIES ]`: Skips extra time and transitions immediately to penalty shootout.

---



## Phase 1.5: Immediate Critical Hotfixes, Multi-Player Controller Engine & Side Selection Hub [COMPLETED]
*Priority: Critical Bug Fixes, Input Auto-Binding, Multi-Player Controller Assignment & Full Spectator Mode*  
*Daily Token Budget Profile: Scope: `src/App.tsx`, `src/components/SideSelectModal.tsx`, `src/components/TacticalGamePlanModal.tsx`, `src/components/TacticalPitchBoard.tsx`, `src/components/TeamSelectorModal.tsx`, `src/components/PauseModal.tsx`, `src/game/engine.ts`, `src/types.ts` | Target: ~700–800k tokens*

### 1.5.1 Critical Fix – Tactical Game Plan Blank Screen & Error Boundary Protection
- **Blank Screen Root-Cause & Resolution**:
  - Eliminate unhandled `TypeError` exceptions (`.toUpperCase()` / `.replace()` on undefined player names, tactics, roles, or playstyle strings).
  - Enforce defensive null/undefined fallbacks across all player attribute records, tactical parameters, and specialist roles:
    - `captainId`, `freeKickNearId`, `freeKickLongId`, `penaltyTakerId`, `leftCornerTakerId`, `rightCornerTakerId`.
  - Comprehensive fallback generator: if `initialHomeTeam` or `initialAwayTeam` is partially initialized or corrupted, sanitize starting XI (exactly 11 outfield/GK players) and substitutes array automatically.
  - Safe render guarantee: add a resilient React `ErrorBoundary` wrapper around `TacticalGamePlanModal` that prevents blank screen unmounts and offers an instant "Reset to Defaults" recovery button.

### 1.5.2 Team Selector Immediate Persistence & Roster Synchronization
- **Instant Registration & Elimination of Multiple-Click Lag**:
  - Selecting or swapping a team in `TeamSelectorModal` must immediately trigger authoritative engine updates via `engine.setTeam(side, team)`.
  - Instantly re-generate pitch player instances, kit colors, formations, and playstyles in real-time without requiring multiple clicks or swaps to take effect.
  - Bidirectional sync: active selections in `PreMatchPresentationModal`, `TeamSelectorModal`, and `MatchEngine` remain strictly in lockstep across both home and away sides.

### 1.5.3 Hardware Profiler Input Auto-Binding
- **Immediate Binding of Profiler Recommendation to Settings**:
  - When the user confirms an input recommendation in `DeviceProfilerModal` (`keyboard`, `gamepad`, or `touch`), that choice is directly bound as Player 1's active input mode and saved to persistent settings.
  - Fixes the bug where selecting "Keyboard" on the initial recommendation screen still left the team playing autonomously under CPU control until manually adjusted in settings.
  - Automatic UI deck adaptation: choosing `keyboard` or `gamepad` automatically hides the virtual on-screen touch controller; choosing `touch` ensures the virtual arcade console is active and visible.

### 1.5.4 32-Bit Side Choice Screen (Select Side / Controller Assignment)
- **Position in Startup Flow**: `Device Profiler` ➔ **`Side Select`** ➔ `Team Selector` ➔ `Captain Presentation` ➔ `Match`.
- **3-Zone Interactive Arcade Slot Board**:
  - **LEFT**: [ HOME TEAM ]
  - **MIDDLE**: [ SPECTATOR (CPU vs CPU) ]
  - **RIGHT**: [ AWAY TEAM ]
- **1st Player (1P) Controller Card**:
  - Rendered in vibrant 32-bit Blue (`#38bdf8`) with pixel gamepad icon and "1P" badge.
  - Movable freely between Home, Spectator, and Away via tactile left/right buttons, keyboard navigation, or direct slot clicking.
- **Multi-Player Support (Up to 4 Players: 1P, 2P, 3P, 4P)**:
  - `[ + ADD NEW PLAYER ]` button dynamically adds:
    - **2P** (Amber `#f59e0b`)
    - **3P** (Emerald `#10b981`)
    - **4P** (Purple `#a855f7`)
  - Any player card can be removed (`[ × ]`) or repositioned across the 3 slots (e.g. 1P + 2P co-op on Home, or 1P Home vs 2P Away, or all in Spectator).
- **Logical Non-Overlapping Keyboard Assignments**:
  - **1P (Blue)**:
    - Movement: `ArrowUp`, `ArrowDown`, `ArrowLeft`, `ArrowRight`
    - Actions: `S` (Pass), `A` (Shoot), `W` (Through Ball), `D` (Cross / Long Pass), `Q` (Ball Shield / Switch), `E` (Special / Sprint / Chip)
  - **2P (Amber)**:
    - Movement: `I` (Up), `K` (Down), `J` (Left), `L` (Right)
    - Actions: `U` (Pass), `O` (Shoot), `Y` (Through Ball), `P` (Cross / Long Pass), `H` (Shield / Switch), `N` (Special / Sprint)
  - **3P (Emerald)**:
    - Movement: Numpad `8` (Up), Numpad `5` (Down), Numpad `4` (Left), Numpad `6` (Right)
    - Actions: Numpad `1` (Pass), Numpad `2` (Shoot), Numpad `3` (Through Ball), Numpad `0` (Cross), Numpad `7` (Shield), Numpad `9` (Special)
  - **4P (Purple)**:
    - Movement: `T` (Up), `G` (Down), `F` (Left), `H` (Right)
    - Actions: `Z` (Pass), `X` (Shoot), `C` (Through Ball), `V` (Cross), `B` (Shield), `R` (Special / Sprint)
- **Gamepad / Joystick Hardware Assignment**:
  - If gamepads are connected (`navigator.getGamepads()`), each player card allows toggling between Keyboard and Gamepad (Pad 1, Pad 2, Pad 3, Pad 4).
- **Touchpad / Mobile Touch Restriction**:
  - Touchpad / virtual touch controls are **strictly restricted to 1 player maximum** to prevent multi-touch gesture conflicts.
- **Autonomous Spectator Mode**:
  - Any team with 0 human assigned players is 100% controlled by autonomous match AI.
  - When all active players are placed in the Middle (Spectator) slot, the match runs in full broadcast CPU vs CPU mode with automatic kickoff and active broadcast camera tracking.
- **Mid-Match Side Switching via Pause Menu**:
  - Added dedicated `[ 🎮 SIDE ]` button in `PauseModal.tsx`.
  - Allows players to dynamically reassign sides, join, leave, or enter Spectator mode mid-match without resetting play or losing match state.

---

## Phase 2: Startup Flow Overhaul, Captain Menu & Difficulty Tiers [COMPLETED]
*Priority: Correct Entry Point, 32-Bit Captain Hub, Difficulty Scaling Foundation*  
*Daily Token Budget Profile: Scope: `src/App.tsx`, `src/components/TeamSelectorModal.tsx`, `src/components/PreMatchPresentationModal.tsx`, `src/game/ai.ts`, difficulty settings in UnifiedSettingsModal | Target: ~700–800k tokens (1 Day's Quota)*

### 2.1 Correct Application Entry Sequence
- Application **must** start at **Team Selector** (never jump straight into a live match).
- After both teams are confirmed → transition into the **Captain Presentation Menu**.
- Remove every remaining "PES" / "Pro Evolution" string or stylistic reference from UI copy, comments, and asset labels.

### 2.2 32-Bit Captain Presentation Menu (Mobile-First, Zero-Scroll)
- Layout rules (strict single-screen, no scrolling):
  - Local team captain + kit on the **left**.
  - Away team captain + kit on the **right**.
  - On vertical mobile: show **only the local team**; add a top-right button `[ VIEW OTHER TEAM ]` that swaps the entire panel to the away side (uniform, tactics summary, stadium name).
  - On horizontal / desktop: both sides visible simultaneously.
- Bottom button row (single horizontal line, equally spaced, tactile 32-bit bevels):
  - `[ UNIFORM ]` | `[ TACTICS ]` | **`[ START ]`** (larger, centred) | `[ STADIUM ]` | `[ SETTINGS ]`
- Each button opens a dedicated, self-contained console-style sub-panel (no nested scrolling).
- START launches the match with currently selected teams, formations, playstyles, stadium and difficulty.

### 2.3 Five Difficulty Tiers (AI Effectiveness Scaling)
Add to Settings (and persist):
1. **Standing** – AI almost stationary, very slow reactions, high error rate (tutorial / casual).
2. **Easy** – Current baseline behaviour with relaxed decision timers.
3. **Normal** – Solid modern decisions, reasonable compactness, occasional mistakes.
4. **Elite** – Tight shape, aggressive but clean pressing, rare mistakes; only high-rated players consistently outplay them.
5. **Legend** – Near-perfect positioning, anticipation and decision-making; player must play almost perfectly to win.

Difficulty multiplies:
- AI reaction delay
- Cover-shadow tightness
- Pass error probability (still gated by player stats)
- Press intensity and recovery run commitment
- GK decision quality

---

## Phase 3: Goalkeeper Mechanical Mastery & Dual Control / AI Symmetry [COMPLETED]
*Priority: Full GK Control Scheme + Identical AI Logic*  
*Daily Token Budget Profile: Scope: `src/game/ai.ts`, `src/game/engine.ts`, `src/game/sprites.ts`, controller mapping | Target: ~750k tokens*

### 3.1 Human Goalkeeper Control Mapping (Ball State Aware)
- **Without ball**:
  - Short Pass → sprint full speed toward the ball.
  - Long Pass → spread / star shape to occupy maximum 1v1 blocking space.
  - Cross → high dive / jump in stick direction, aiming top corners, opposite-hand reach.
  - Shoot → low dive aiming bottom corner.
  - No input after opponent shot → automatic dive (medium height/power).
  - Ball Shield (Q) → high jump to catch (corners / crosses).
  - Special (E) → punch clear instead of catch.
- **With ball**: behaves exactly like an outfield player (same pass / clear / throw options).

### 3.2 AI Goalkeeper Uses Identical Decision Tree
- AI GK evaluates the same action set under the same conditions.
- Catch vs Punch decision driven by ball power, curve, and Handling / Reflexes attributes.
- 1v1 star-spread, high/low dives and recovery positioning scale with difficulty tier.

### 3.3 Procedural GK Sprite & Animation Hooks
- Lightweight procedural frames for dive, star-spread, catch, punch, distribution.
- No heavy sprite sheets; keep memory footprint mobile-safe.

---

## Phase 4: Modern Compact Positioning Foundation (AI Core – Part 1) [COMPLETED]
*Priority: 2026 Compactness, Block Height, Shape Maintenance*  
*Daily Token Budget Profile: Scope: `src/game/ai.ts`, `src/game/tactics.ts`, `src/game/formations.ts`, `src/game/pitchGrid.ts` | Target: ~800k tokens*

**Research grounding (2026 tactics)**: Teams keep vertical distance between the highest attacker and deepest defender typically 25–35 m. Mid-block is the default recovery shape. High press is selective and short; low block is used deliberately. Entire unit shifts together.

### 4.1 Vertical Compactness Engine
- Target vertical span (first attacker → last defender) clamped to 25–35 m depending on tactical playstyle and current phase of play.
- High-press phase: back line pushes higher; attackers stay connected.
- Mid-block phase: default recovery shape, compact central corridor.
- Low-block phase: attackers drop deeper to protect the box; no idle high strikers.

### 4.2 Synchronised Block Movement
- Entire team treated as a single elastic unit relative to ball X/Y.
- When the block shifts left/right or up/down, every line (defence, midfield, attack) moves together while preserving relative spacing.
- Difficulty scales how tightly and how quickly the block re-forms after a transition.

### 4.3 Rest-Defence & Transition Safety
- Always leave a minimum number of players behind the ball (rest defence) based on formation and playstyle.
- After losing possession, counter-press trigger window (first 3–5 seconds) is intensity-scaled by difficulty and tactical instructions.

### 4.4 Direct Implementation Notes (Token-Efficient)
- Extend existing role / sub-position system; do not rewrite formation data.
- Use pre-allocated target-position buffers; zero new allocations per frame.
- Expose a single `updateTeamBlockShape(team, ball, phase, difficulty)` entry point.

---

## Phase 4.5: Hotfix – Controller Auto-Binding, Side Selection Control Profile & Advanced Cursor Switching [COMPLETED & VERIFIED]
*Priority: Zero-Friction Match Startup, Authoritative Side Select Device Binding, Single/Team Scope, 3m Proximity Double-Tap Switching*  
*Daily Token Budget Profile: Scope: `src/components/SideSelectModal.tsx`, `src/components/PauseModal.tsx`, `src/components/ControllerSettingsModal.tsx`, `src/game/engine.ts`, `src/types.ts` | Target: ~600k tokens*

### 4.5.1 Instant Controller Auto-Binding & Settings Cleanup
- **Side Selection Authoritative Binding**:
  - The side selection step authoritatively registers and binds the user's active control device (Keyboard WASD, Keyboard Arrows, Gamepad index, or Touch) directly into `GameEngine` upon confirming sides.
  - Fix the match-start movement freeze bug: eliminate the requirement to pause, enter System Settings, and re-select the controller. Matches start immediately with active player responsiveness.
  - **Remove from System Settings**: Strip redundant controller selection menus from the in-game Settings/Pause modal to avoid state conflicts; controller assignment belongs strictly to Side Select.

### 4.5.2 Control Scope: Team vs. Single Player Lock
- Add control scope selection directly inside the Side Selection modal:
  1. **All Team** (Default): User controls the ball carrier when in possession and shifts between outfield players.
  2. **Single Player** (Fixed Lock): User selects and locks onto a specific outfield player or goalkeeper for the entire match (cursor switching disabled).
- When "Single Player" is selected, cursor switching settings are completely hidden and disabled.

### 4.5.3 Cursor Change Logic: Manual vs. Automatic
- Expose **Cursor Change** option in Side Selection (only visible when "All Team" mode is active):
  1. **Manual Mode** (Tactical Default):
     - In possession: Cursor automatically follows the ball carrier.
     - On pass / cross / shot: Cursor transfers to the targeted teammate receiver receiving the ball trajectory.
     - On interception / loose ball: Cursor switches to the teammate closest to the ball.
     - Without the ball: Cursor **never** auto-switches; player only changes when pressing the "Player Switch" button (Q / L1 / LB), which targets the teammate closest to the ball.
  2. **Automatic Mode**:
     - On-ball behavior is identical to Manual (controls carrier, pass transfer, loose ball capture).
     - Without the ball: Game engine automatically switches cursor to the defender closest to the ball at all times.

### 4.5.4 3-Meter Proximity Protection & Double-Tap Override
- **3-Meter Proximity Guard (< 3m / ~71 px)**:
  - Applies to **both** Manual and Automatic switching modes.
  - Prevents erratic or disorienting micro-switches between adjacent cluster defenders: the engine will **not** switch cursor to any candidate teammate situated less than 3 meters away from the currently controlled player.
  - In Automatic mode, if the closest defender is under 3 meters away, the switch is suppressed and the current player remains under user control.
- **Double-Tap Player Switch Override**:
  - If the user explicitly double-taps the "Player Switch" button within a 300 ms window, the 3-meter proximity guard is bypassed, executing an immediate micro-switch to that adjacent teammate.

---

## Phase 5: Advanced AI Positioning, Line Intermingling & Role Fluidity (AI Core – Part 2) [COMPLETED & VERIFIED]
*Priority: Realistic Occupation of Space, Modern Interlocking Lines*  
*Daily Token Budget Profile: Scope: `src/game/ai.ts`, `src/game/tactics.ts`, `src/game/formations.ts` | Target: ~800k tokens*

### 5.1 Line Intermingling Rules
- Forwards actively occupy and shadow opposition centre-backs / defensive midfielders (not stuck on their own half).
- Midfield line interlocks with both the defensive and attacking thirds according to playstyle (e.g. box-to-box vs holding).
- Full-backs / wing-backs tuck inside or push high based on tactical instructions and ball location.

### 5.2 Positional Roles Drive Off-Ball Behaviour
- Every AI player continuously evaluates its assigned Primary Role + Sub-Position + Playstyle to decide:
  - Support run type (underlap, overlap, blind-side, drop into pocket)
  - Cover shadow target
  - When to step out vs hold the line
- Higher Positioning / Reactions attributes = earlier, more accurate arrival at the optimal spot.

### 5.3 Difficulty-Scaled Anticipation
- Standing / Easy: delayed reaction, larger positioning errors.
- Normal: solid modern shape.
- Elite / Legend: near-perfect reading of ball trajectory and opponent intention; only the very best human play consistently beats them.

### 5.4 Implementation Guardrails
- Re-use existing `evaluatePlayerRoleFit` and pitch-grid helpers.
- Keep all calculation inside the already zero-allocation AI tick.
- Unit-test compactness and intermingling distances on a few canonical formations (4-3-3, 4-2-3-1, 3-5-2, 5-3-2).

---

## Phase 6: AI Decision Quality, Passing Logic, Clean Defending & Anti-Spam [COMPLETED & VERIFIED]
*Priority: Intelligent Choices, Stat-Grounded Errors, Modern Pressing Intensity*  
*Daily Token Budget Profile: Scope: `src/game/ai.ts`, `src/game/ballPhysics.ts`, `src/game/engine.ts` | Target: ~750–800k tokens*

### 6.1 Decision-Making Hierarchy
- AI chooses the highest-value available action under pressure:
  1. Safe progressive pass into free pocket
  2. Cross-field switch when wing is overloaded
  3. Controlled clearance only when no progressive option exists
- Eliminate the current “20 back-passes between two CBs” loop. Under pressure the AI must play forward or switch.

### 6.2 Pass / Cross / Shot Accuracy Strictly Stat-Driven
- Miss probability is a function of Short Pass / Long Pass / Crossing / Shooting attributes + pressure + fatigue + difficulty multiplier.
- A 90-rated passer under light pressure almost never misses a simple pass; a 45-rated player under high press frequently does.
- Long-range power shots and switches travel the full required distance (see Phase 7); distance only reduces aiming precision, not velocity.

### 6.3 Clean Tackling & Foul Calibration
- Good defenders (high Tackling + Positioning) preferentially use standing tackles and toe-pokes.
- Sliding tackles reserved for last-ditch or specific aggressive philosophies.
- Fouls become rare on Elite/Legend; more common only on low-defending-stat players or when the tactical instruction is ultra-aggressive.

### 6.4 Modern Pressing Intensity
- Every opponent in possession should feel 1–2 markers within realistic distance (modern “always under pressure” principle).
- Press triggers and recovery runs scale with difficulty and the team’s chosen playstyle (High Press vs Mid Block vs Low Block).

---

## Phase 7: True Long-Range Ball Flight, Cambio de Frente & Physics Polish [COMPLETED & VERIFIED]
*Priority: Authentic Trajectory Distance & Cross-Field Switches*  
*Daily Token Budget Profile: Scope: `src/game/ballPhysics.ts`, `src/game/engine.ts`, `src/game/physics.ts`, `src/game/playerActions.ts` | Target: ~650–750k tokens*

### 7.1 Extended Flight Curve
- 80–95 % power shots / long passes from three-quarter pitch must reach the penalty area / goal with remaining pace (> 18–35 px/f).
- Aerodynamic drag is realistic; high-velocity soccer balls enter the drag crisis where narrow turbulent wakes preserve velocity; distance makes aiming harder, it does not kill velocity.
- Backspin generates positive aerodynamic Magnus lift ($+z$), keeping driven balls and switches in prolonged flight before dipping cleanly into target pockets.

### 7.2 Automatic “Cambio de Frente” (Switch of Play)
- High-power cross aimed from one wing toward the opposite flank is automatically interpreted as a flat switch.
- Ball receives appropriate leading space vector ahead of the opposite winger / fullback so they can take it in stride.
- User control automatically transfers to the receiving winger sprinting onto the ball.

### 7.3 Consistency with Existing Chip / Driven / Swerve Modifiers
- Preserves the current E / Q modifier suite across all actions:
  - E: Delicate chip / floating loft with soft backspin landing.
  - Q: High Magnus lateral curvature bending around defensive lines.
  - Full synergy with Phase 6 Stat Breaks (Thunderbolt Cannon, Radar Telemetry, Guided Whip, Deadly Assassin, Laser Ping).

---

## Phase 8: Procedural Dribbling Animation Tiers, On-Ball Acceleration & Ginga [COMPLETED & VERIFIED]
*Priority: Fluid On-Ball Locomotion, Skill Differentiation*  
*Daily Token Budget Profile: Scope: `src/game/animationEngine.ts`, `src/game/sprites.ts`, `src/game/ginga.ts` | Target: ~750–850k tokens*

### 8.1 Six Dribbling Animation Tiers
| Attribute Band | Tier Name          | Animation Character                     |
|----------------|--------------------|-----------------------------------------|
| 40–59          | Amateur            | Heavy, upright, slow turns              |
| 60–69          | Semi-Pro           | Basic close control                     |
| 70–79          | Pro                | Sharper cuts, better body feints        |
| 80–89          | Elite              | Quick step-overs, rapid direction change|
| 90–99          | World Class        | Fluid, low centre of gravity, explosive |
| 100+ (Stat Break) | Unique           | Signature / exaggerated elite moves     |

### 8.2 On-Ball Physics Separation
- Top speed still governed by Pace.
- Acceleration while on the ball and turn radius governed by Dribbling + Ball Control.
- Higher tiers unlock faster, cleaner animations for step-overs and skill moves.

### 8.3 Ginga Thresholds
- Effective only with Ball Control ≥ 70 **and** Dribbling ≥ 70.
- At 90+ on both attributes it becomes highly reliable.
- Below threshold: high failure / loss-of-possession chance.

### 8.4 Supporting Animations
- Lightweight procedural improvements for standing tackle, sliding tackle, shooting follow-through (no heavy new sprite sheets).

---

## Phase 9: Aerial Anticipation, Headers, Volleys & Rebound Reflexes
*Priority: Reading Flight Paths & Winning the Second Ball*  
*Daily Token Budget Profile: Scope: `src/game/ai.ts`, `src/game/ballPhysics.ts`, `src/game/animationEngine.ts` | Target: ~700–800k tokens*

### 9.1 Drop-Zone Prediction
- AI calculates expected landing zone of aerial balls.
- Positioning attribute determines how early the player starts moving to the optimal spot.
- Interceptions attribute helps defenders arrive first to clear.

### 9.2 Header / Volley / Clearance Animations
- Procedural header (directed / glancing / power), volley, and defensive clearance frames.
- Timing window scales with Reactions and Heading / Volleying attributes.

### 9.3 Rebound & Second-Ball Reflexes
- Reflexes attribute shortens reaction time to deflections and loose balls in the box.
- Higher difficulty AI wins a larger share of second balls.

---

## Phase 10: Live Player Rating Engine (SofaScore Model) & Match MVP
*Priority: Zero-Allocation Live Analytics*  
*Daily Token Budget Profile: Scope: `src/game/playerRatings.ts` (new), `src/game/engine.ts`, HUD components, EndGameModal | Target: ~700k tokens*

### 10.1 Live Rating Core
- Every player starts at 6.0.
- Pre-allocated rating array; zero GC pressure.
- Positive / negative event matrix (pass, dribble, shot, tackle, foul, card, goal, own-goal, clean-sheet contribution, etc.).
- Human player’s live rating shown as a small floating badge (bottom-right, above controller).

### 10.2 End-Game Board & MVP
- Full team ratings list.
- Highest-rated player receives Match MVP gold star treatment.
- Subbed players’ ratings freeze at the moment of substitution.

---

## Phase 11: Dynamic Stadiums & Match Atmosphere
*Priority: Living Stadium Audio, Dynamic Crowd Chants & Contextual Intensity*  
*Daily Token Budget Profile: Scope: `src/game/crowdRenderer.ts`, `src/game/audio.ts`, `src/game/stadiumRenderer.ts` | Target: ~700–800k tokens*

### 11.1 Dynamic Crowd Acoustics & Reactivity
- Crowd reaction scales with match context (near misses, last-minute goals, high-tackle derby intensity).
- Contextual home-crowd cheering, away booing, and dynamic goal celebrations.
- Authentic soundscapes depending on stadium capacity and architecture (intimate vs massive stadium resonance).

### 11.2 Visual Crowd & Banner Immersion
- Dynamic crowd density matching team reputation and match stakes.
- Procedural ultra-low-cost animated crowd sprites waving club-colored scarves and banners.
- Flashbulb pops in stands during night matches and penalty shootouts.

### 11.3 Kickoff Stadium Selector & 6 Crowd Attendance Levels
- **Pre-Match Kickoff Integration (`[ STADIUM ]` option)**:
  - Accessible directly in the Pre-Match Captain Presentation Screen under `[ STADIUM ]`.
  - Added interactive **Crowd Level** selection with 6 distinct attendance tiers:
    1. **Empty**: 0% attendance. Behind-closed-doors ghost match; hollow echo acoustics, ball strikes reverberate across bare concrete terraces, zero crowd singing, audible player and coach shouting.
    2. **Small**: ~15–20% attendance. Sparse supporter pockets; polite isolated applause, distant shouts, minimal acoustic pressure.
    3. **Few**: ~35–45% attendance. Modest localized turnout; sporadic cheers, scattered fan murmurs, moderate reaction to chances.
    4. **Half**: ~50–65% attendance. Solid half-capacity hum; collective gasps on close attempts, energetic goal roar.
    5. **Crowded**: ~80–95% attendance. Near capacity; loud sustained wall-of-sound chanting, intense home advantage roar, deafening whistles on fouls.
    6. **Packet**: 100%+ attendance (to the brim / over-capacity final). Over-top capacity like a continental or World Cup final; packed standing room, maximum acoustic pressure, thunderous reverberation, constant seismic chants, flares/confetti, and deafening stadium roar.
- **Dynamic Audio & Visual Coupling**:
  - Modulates procedural grandstand crowd density and ultras flag/banner density in real-time.
  - Dynamically scales audio volume, reverb, cheer intensity, and reactive chants.

---

## Phase 12: Pitch Dimensions, Weather & Surface Physics
*Priority: Turf Micro-Physics, Tactical Pitch Dimensions & Dynamic Weather Engine*  
*Daily Token Budget Profile: Scope: `src/game/turfPhysics.ts`, `src/game/weatherEngine.ts`, `src/game/pitchDimensions.ts` | Target: ~700–800k tokens*

### 12.1 Pitch Dimension Presets & Tactical Impact
- Standard, Wide (wing play advantage), Narrow (midfield congestion), Long, and Short pitch presets.
- Formation spacing scales proportionately with pitch boundary dimensions.

### 12.2 Atmospheric Weather Engine & Surface Physics
- Dynamic weather conditions: Dry, Rain, Heavy Rain, Snow, and Fog.
- Wet surface physics: increased ground-skid on fast passes, water-spray particles on sliding tackles, mud patches affecting bounce restitution.

---


## Phase 13: 32-Bit Main Menu System, Procedural Stadium Engine & Team Home Venues
*Priority: 32-Bit Main Menu Launch Hub, Complete Stadium Data Architecture, 5 Stand Grades, Wall Tier vs Multi-Tier Mechanics, Procedural Pitch Renderer & Team Home Venue Binding*  
*Daily Token Budget Profile: Scope: `src/components/MainMenuModal.tsx`, `src/types/stadium.ts`, `src/game/stadiumRenderer.ts`, `src/game/teamDatabase.ts`, `src/App.tsx` | Target: ~750–850k tokens (1 Day's Quota)*

### 13.1 32-Bit Arcade Main Menu (Launch Screen)
- **Top-Level Application Entry Point**:
  - Main Menu loads first on launch before entering Kick Off or Editor.
  - Authentic 32-bit console visual design (chiseled metallic steel panels, cyan/gold LED backlit badges, embossed action buttons).
  - 3 Primary Options:
    1. **`[ ⚽ KICK OFF ]`**: Initiates match flow $\rightarrow$ Side Select $\rightarrow$ Team Selector $\rightarrow$ Captain Menu $\rightarrow$ Matchday.
    2. **`[ ⚙️ SETTINGS ]`**: Opens the Unified Game Settings modal (Graphics, Controls, Audio, Match Rules).
    3. **`[ 🛠️ EDITOR ]`**: Opens a dedicated 2-option editing portal:
       - **`[ 👥 TEAMS ]`**: Edit team tactical game plans, formations, playstyles, and assign official **Home Stadium** with custom venue settings.
       - **`[ 🏟️ STADIUMS ]`**: Launches the Stadium Creator & Inspector suite (Phase 14).

### 13.2 Data-Driven Stadium Architecture & 5 Architectural Stand Grades
Stadiums are lightweight, serializable JSON configuration objects with procedural Canvas 2D math (zero bulky 3D meshes, zero GC pressure on budget devices):

1. **Four Architectural Shapes**:
   - `Round` (Maracanã / Estadio Olímpico bowl).
   - `Oval` (Elongated athletics bowl).
   - `Square` (8 stands: 4 straight main stands + 4 independent corner stands).
   - `Rectangular` (Classic English box ground: elongated East/West touchline stands + 4 corner stands).
2. **Five Stand Architectural Grades (Quality / Luxury / Finish Level)**:
   - **Grade 1 – Municipal**: Exposed rough cinder blocks, weathered timber benches, basic utilitarian perimeter, rustic grassroots aesthetic.
   - **Grade 2 – Classic**: Traditional English red-brick masonry, painted structural steel trusses, standard stadium plastic fold-down seats.
   - **Grade 3 – Industrial**: Heavy corrugated steel cladding, exposed industrial I-beams, raw galvanized metal finish.
   - **Grade 4 – Modern**: Smooth pre-cast architectural concrete, cantilevered sweeping roofs, high-grade ergonomic bucket seats, clean glass balustrades.
   - **Grade 5 – Futuristic**: Anodized aero-aluminum cladding, translucent tensile ETFE composite roofs, illuminated VIP seating, continuous panoramic LED ribbon fascia boards.
3. **Multi-Tier Stacking vs Wall Tier Architecture**:
   - **Standard Stacked Tiers (1 to 4 Decks)**:
     - Independent stacked spectator tiers separated by fascia balconies and vomitories.
     - Each tier has customizable size: `"small"`, `"medium"`, `"large"`.
     - Each tier visually stacks directly on top of the lower tier, scaling stand height, depth, and capacity in real-time.
   - **Wall Tier (Single Gigantic Dortmund-Style Kop / "Die Gelbe Wand")**:
     - A massive, steep, continuous single terrace without intermediate deck dividers spanning the entire stand height.
     - 3 Wall Tier Sizes:
       - `"large"`: Occupies the full height, depth, and volume equivalent to a 4-tier stand of large tiers.
       - `"medium"`: Scaled ~20% smaller than Large.
       - `"small"`: Scaled ~40% smaller than Large.
4. **"No Stand" Option & Fused Surroundings-Driven Backdrops**:
   - Any stand can be configured as `"none"` (`No Stand`), allowing authentic asymmetric or modest 2-sided/3-sided grounds (e.g., Gibraltar's Victoria Stadium beside the rock/runway, Braga's granite quarry, Oxford United's 3-sided stadium).
   - Stand capacity contribution = 0.
   - **Fused Surroundings Binding**: The available side background variants for "No Stand" are directly determined by the stadium's global **Surroundings** (selected in Step 1 Structure):
     - **Small City**: `Mall`, `Parking Lot`, `Apartment Buildings`, `Small Houses` (plus `Wall`).
     - **Beach**: `Beach Seaside`, `Apartment Buildings`, `Small Houses` (plus `Wall`).
     - **Big City**: `Skyscrapers / Downtown Avenue`, `Apartment Buildings`, `Mall`, `Metro Rail Overpass` (plus `Wall`).
     - **Nature**: `Mountain / Forest`, `Open Alpine Hills`, `Lake / Valley` (plus `Wall`).
     - **Airport** (Gibraltar style): `Runway Tarmac with Aircraft`, `Hangars & Control Tower`, `Freight Depot` (plus `Wall`).
     - **Railroad**: `Multi-Track Train Depot`, `Freight Railyard`, `Industrial Gantries` (plus `Wall`).
     - **Parking Lot**: `Paved Parking Bays & Team Buses`, `Perimeter Tree Boulevard` (plus `Wall`).
     - **Marine Floating**: `Open Ocean Water`, `Floating Pontoons & Pier`, `Harbor Marina` (plus `Wall`).
   - **Universal Wall Rule**: `"Wall"` is **always available** across all surrounding types.
     - When `"Wall"` is chosen as the background: the separate perimeter finish sub-option is disabled and replaced directly with:
       - Wall Size: `"low"`, `"medium"`, `"tall"`.
       - Wall Material: `"brick"`, `"concrete"`, `"stone"`, `"timber"`, `"metal cladding"`.
     - When any other contextual backdrop variant is chosen: the user selects a **Perimeter Finish** in front of the background (`"none"`, `"small fence"`, `"big fence"`, `"chainlink steel fence (big)"`, `"brick wall"`, `"concrete wall"`).
5. **Decoupled Fence & Perimeter Barrier Specification**:
   - Barrier Size: `"none"` | `"small"` | `"medium"` | `"big"` | `"huge"`.
   - Barrier Material: `"brick"` | `"cement"` | `"wood"` | `"chain link steel"` | `"aluminum picket"`.
6. **Seat Styles & Patterns**:
   - 4 distinct seat styles: `"plastic_bench"`, `"classic_bucket"`, `"tip_up_padded"`, `"vip_leather"`.
   - 5 seat patterns: `"solid"`, `"perStand"`, `"horizontalBands"`, `"verticalStripes"`, `"lowerUpper"` with 1 to 4 colors.
7. **Athletics Running Track**:
   - `hasTrack`: boolean (strictly exclusive to `Round` and `Oval` stadiums; omitted on `Square` and `Rectangular`).
8. **Lighting Model**:
   - Floodlight towers / pylons / roof banks with daytime sunlight pools and night lighting.
9. **Eight Outside Environment Surroundings (Structure Step)**:
   - Configured in the initial stadium structure setup alongside Shape.
   - `Nature`, `Parking Lot` (Camp Nou style), `Small City`, `Big City`, `Airport`, `Railroad`, `Beach`, `Marine Floating`.
10. **FIFA Qualification & Capacity Mathematical Models**:
    - Capacity calculated additively per stand based on shape, tier count/sizes, or wall tier dimensions (0 for No Stand).
    - Qualification Category computed dynamically:
      - `National`: Capacity < 15,000, basic municipal/classic finishes (2nd division/grassroots standard).
      - `First Division`: Capacity 15,000–35,000, industrial/modern finishes, standard floodlights (top-flight league standard).
      - `Continental`: Capacity 35,000–60,000, modern finishes, high-power floodlights (UCL, UEL, Copa Libertadores standard).
      - `World`: Capacity 60,000+, modern/futuristic finishes, premium lighting, pristine turf (World Cup Finals standard).

### 13.3 Live Matchday Procedural Stadium Renderer
- **Unified Procedural Canvas 2D Pipeline**:
  - Draws any configured stadium directly onto the pitch canvas at a locked 60 FPS on budget phones.
  - Matches the exact visual fidelity of the Stadium Creator preview ("What You See Is What You Get").
  - Architectural shadow volumes: circular soft pool for Round/Oval, angular envelope for Square/Rectangular.
  - Pitch-level rendering of open ends ("No Stand" fences, background houses, mountains, runways, or perimeter walls tied to surroundings).
  - Zero per-frame memory allocations; geometry and path data pre-computed at match start.

### 13.4 Team Home Stadium Binding & Kickoff Integration (13.6 Overrides)
- **Team-Specific Home Venue Registry**:
  - In `EDITOR -> TEAMS`: assign any registered stadium from the global stadium list as that team's official home venue.
  - Customize team venue overrides: `pitchPattern`, `netStyle`, `pitchSizePreset`, `turfQuality`, `fanColors`, `bannerMessages`, `sponsors`.
- **Kickoff Automatic Selection & Locking**:
  - In `KICK OFF`: when a team is chosen as Home, its official Home Stadium is selected automatically by default.
  - In the pre-match stadium selector, a prominent gold `[ HOME ]` option appears when the home team has a designated venue.
  - When `[ HOME ]` is selected, pitch pattern, net style, turf quality, and pitch dimensions are locked to the team's official venue settings.
  - When a neutral stadium is selected from the stadium list, pitch pattern, net style, and pitch dimensions remain user-configurable.

---

## Phase 14: Interactive 32-Bit Stadium Creator & Stand Camera Director Suite
*Priority: Real-Time Visual WYSIWYG Editor, Stand-by-Stand Focused Camera Director, Step-by-Step Console Wizard & Live FIFA Qualification HUD*  
*Daily Token Budget Profile: Scope: `src/components/StadiumCreatorModal.tsx`, stand camera inspector hooks, seat customizer, registry persistence | Target: ~750–850k tokens (1 Day's Quota)*

### 14.1 Visual WYSIWYG Real-Time Matchday Preview
- The Stadium Creator renders the stadium in real-time using the exact same procedural Canvas 2D renderer used in live matches.
- Base stadium initializes with lowest tier (Tier 1) in Small size across all stands, with stacked tiers visible immediately.

### 14.2 Persistent Bottom-Left 32-Bit HUD Box (Qualification & Capacity)
- Displayed on the bottom-left at all times in a chiseled 32-bit metallic console box:
  1. **"Qualification"**: Real-time FIFA stadium category indicator:
     - `National` $\rightarrow$ `First Division` $\rightarrow$ `Continental` $\rightarrow$ `World`.
     - Accrued dynamically based on current capacity, stand architectural grades, floodlights, and turf quality.
  2. **"Capacity"**: Real-time numerical capacity meter summing each stand's selected tier, wall, or "no stand" contribution.

### 14.3 Step-by-Step Creation Wizard & Dynamic Camera Director
1. **Step 1: Structure, Shape & Surroundings**:
   - **Shape Selection** (`Round`, `Oval`, `Square`, `Rectangular`): Camera in full-stadium framing.
   - **Surroundings Selection** (`Small City`, `Beach`, `Big City`, `Nature`, `Airport`, `Railroad`, `Parking Lot`, `Marine Floating`):
     - **Dynamic Camera Shift to Aerial Sky-Cam**: When the cursor/focus moves to **Surroundings**, the camera smoothly shifts to the high-altitude **Aerial Sky-Cam view**, showcasing the 32-bit bird's-eye canvas view of the stadium bowl set within the surrounding landscape!
     - The selected surroundings also determine the available background subsections when configuring "No Stand" later.
   - **Athletics Running Track**: Appears immediately after Shape selection **only if Round or Oval is selected**; omitted for Square/Rectangular.
2. **Step 2: Stand-by-Stand Focus Camera & Chiseled Inspector**:
   - Clicking Next automatically shifts camera to focus directly on the **East Stand** first.
   - Previous / Next stand navigation (`East` $\leftrightarrow$ `South` $\leftrightarrow$ `West` $\leftrightarrow$ `North`, plus 4 corner stands for Square/Rectangular) with smooth real-time camera tracking.
   - Vertical list of stand parameters (navigate top-to-bottom); within each parameter, cycle options horizontally (left-to-right):
     - **Stand Type & Tiers**:
       - Standard Tiers: 1–4 stacked tiers with per-tier size (`small`, `medium`, `large`).
       - Wall Tier: Dortmund-style single tall tier with size (`small` [-40%], `medium` [-20%], `large` [full 4-tier equivalent]).
       - No Stand: Disables stand seating (0 capacity). Contextual Backgrounds are dynamically populated from the stadium's **Surroundings**:
         - *Small City* $\rightarrow$ `Mall`, `Parking Lot`, `Apartment Buildings`, `Small Houses`, or `Wall`.
         - *Beach* $\rightarrow$ `Beach Seaside`, `Apartment Buildings`, `Small Houses`, or `Wall`.
         - *Big City* $\rightarrow$ `Skyscrapers / Downtown Avenue`, `Apartment Buildings`, `Mall`, `Metro Rail Overpass`, or `Wall`.
         - *Nature* $\rightarrow$ `Mountain / Forest`, `Open Alpine Hills`, `Lake / Valley`, or `Wall`.
         - *Airport* $\rightarrow$ `Runway Tarmac with Aircraft`, `Hangars & Control Tower`, `Freight Depot`, or `Wall`.
         - *Railroad* $\rightarrow$ `Multi-Track Train Depot`, `Freight Railyard`, `Industrial Gantries`, or `Wall`.
         - *Parking Lot* $\rightarrow$ `Paved Parking Bays & Team Buses`, `Perimeter Tree Boulevard`, or `Wall`.
         - *Marine Floating* $\rightarrow$ `Open Ocean Water`, `Floating Pontoons & Pier`, `Harbor Marina`, or `Wall`.
       - **Wall Background Rule**: `"Wall"` is **always available** regardless of surrounding type. If `Wall` is chosen, Perimeter Finish is disabled and replaced directly with Wall Size (`low`, `medium`, `tall`) and Wall Material (`brick`, `concrete`, `stone`, `timber`, `metal cladding`).
       - If a non-Wall backdrop is chosen: Perimeter Finish is selectable (`none`, `small fence`, `big fence`, `chainlink steel fence (big)`, `brick wall`, `concrete wall`).
     - **Stand Architectural Grade**: 5 grades (`Municipal`, `Classic`, `Industrial`, `Modern`, `Futuristic`).
     - **Stand Structure Colors**: Primary and secondary structural colors.
     - **Roof Inspector**: When cursor reaches Roof, camera tilts/pans higher to showcase the roof structure (style, design 1-3, material, color).
     - **Fence / Barrier Inspector**: When cursor reaches Fence, camera dips down to pitch level to showcase barrier Size (`none`, `small`, `medium`, `big`, `huge`) and Material (`brick`, `cement`, `wood`, `chain link steel`, `aluminum picket`).
3. **Step 3: Stand Completion & Satisfaction Confirmation**:
   - Under the Next / Previous stand buttons, a `[ COMPLETE STANDS ]` button triggers an arcade modal:
     *"Are you satisfied with the current stand design?"*
   - Confirming locks stand architecture and advances to stadium-wide aesthetic styling.
4. **Step 4: Full-Stadium Pan – Seat Color, Pattern & Styles**:
   - Camera pans out to frame the entire stadium bowl.
   - Select Seat Pattern (`solid`, `perStand`, `horizontalBands`, `verticalStripes`, `lowerUpper`) and 1–4 colors.
   - Select from **4 distinct seat styles** (`plastic_bench`, `classic_bucket`, `tip_up_padded`, `vip_leather`).
5. **Step 5: Floodlights & Final Registry Save**:
   - Configure lighting setup (number of banks, power, placement, day/night).
   - Name stadium and save into the persistent global stadium registry.

---

## Phase 15: Aerial Sky-Cam Broadcast Presentation & Dual-Layer Outside Environment Engine
*Priority: 32-Bit Bird's-Eye Stadium Sky-Cam, Seamless Pitch Cam Swoop Transition & Dual-Perspective Outside Environments*  
*Daily Token Budget Profile: Scope: `src/game/skyCamRenderer.ts`, `src/game/environmentRenderer.ts`, pre-match camera transition director | Target: ~750–850k tokens (1 Day's Quota)*

### 15.1 Dual-Perspective Outside Surroundings Engine
Every outside environment provides both pitch-level horizon graphics and aerial bird's-eye canvas graphics:
1. **Nature**: Alpine green hills, forest canopies, open sky.
2. **Parking Lot (Camp Nou Style)**: Asphalt parking bays, parked cars, team buses, pedestrian boulevards, perimeter trees.
3. **Small City**: Suburban townhomes, neighborhood streets, red-brick commercial buildings.
4. **Big City**: Dense metropolitan skyscrapers, arterial highways, elevated rail lines.
5. **Airport (Gibraltar Style)**: Adjacent tarmac runway, hangars, taxiways, control tower, taxiing aircraft.
6. **Railroad**: Multi-track train depot, freight railyard, industrial gantries, moving train sprites.
7. **Beach**: Sandy coastline, turquoise ocean surf, palm trees, seaside promenade.
8. **Marine Floating**: Ocean water envelope, floating pontoons, harbor boats, perimeter buoys.

### 15.2 32-Bit High-Altitude Aerial Sky-Cam Renderer
- Procedural bird's-eye canvas renderer capturing the full stadium footprint, outer facade cladding, roof geometry, parking/surroundings, and central pitch (inspired by Camp Nou aerial reference).
- Accessible in Stadium Creator as an Aerial Inspector mode and in pre-match presentation.

### 15.3 Seamless Pre-Match Sky-Cam to Pitch-Cam Zoom Swoop
- Matchday presentation begins with the Aerial Sky-Cam framing the stadium and its surrounding environment.
- As teams line up, the camera initiates a smooth, cinema-grade zoom-in swoop, transitioning seamlessly through the roofline down to the standard broadcast pitch view before the referee blows the kickoff whistle.

---

## Phase 16: IFAB Linesman Offside Engine & VideoRef (VIR)
*Priority: Law 11 Correctness + Lightweight Review Presentation*  
*Daily Token Budget Profile: Scope: `src/game/engine.ts`, offside helpers, simple referee cut-scene | Target: ~650–750k tokens*

### 16.1 Autonomous Assistant Referee
- Two-player offside ray-cast (IFAB Law 11).
- Correct exceptions (own half, ball played backward, throw-in, etc.).
- Animated sideline linesman with flag.

### 16.2 Toggleable VideoRef
- Optional short referee-monitor style review for tight offside / penalty decisions.
- Fully skippable; can be disabled in Graphics settings for performance.

---

## Phase 17: Lightweight Cinematics Suite & Slow-Mo Replay Buffer
*Priority: Presentation Polish Without Performance Cost*  
*Daily Token Budget Profile: Scope: circular frame buffer, simple cut-scene triggers | Target: ~700k tokens*

### 17.1 Zero-Allocation Replay Ring Buffer
- 300-frame circular buffer of essential state (player positions, ball, camera).
- Automatic slow-mo on goals, penalties, red cards, tight offsides.
- Instant any-key skip.

### 17.2 Future Entrance Cinematic Hook (data only this phase)
- Prepare data structures and timing hooks for a later “players walking onto the pitch” entrance using the larger captain models.
- Do **not** implement the full cinematic yet; only the plumbing so a future phase can drop it in cleanly.

---

## Master Development Execution Order (Updated)

| Phase | Title | Focus | Status / Notes |
| :---: | :--- | :--- | :--- |
| **0** | 32-Bit UI, Zero-Scroll Game Plan, Broadcast HUD & Device Profiling | Architecture & UI | **COMPLETED** |
| **1** | Match Regulation Halves, Stoppage Time, Whistle AI & End-Game Hub | Match Flow | **COMPLETED** |
| **1.5** | Immediate Critical Hotfixes, Multi-Player Engine & Side Selection Hub | Hotfixes & Multiplayer | **COMPLETED** |
| **2** | Startup Flow, Captain Menu, Difficulty Tiers (5) | Entry Point & Settings | **COMPLETED** |
| **3** | Goalkeeper Mechanical Mastery & Dual Control/AI | Goalkeeping | **COMPLETED** |
| **4** | Modern Compact Positioning Foundation (AI Part 1) | AI Positioning | **COMPLETED** |
| **4.5** | Controller Auto-Binding, Side Selection Profile & Advanced Switching | Controls & Switching | **COMPLETED & VERIFIED** |
| **5** | Advanced Positioning, Line Intermingling & Role Fluidity (AI Part 2) | AI Positioning | **COMPLETED & VERIFIED** |
| **6** | AI Decision Quality, Passing Logic, Clean Defending | AI Decisions | **COMPLETED & VERIFIED** |
| **7** | Long-Range Ball Flight & Cambio de Frente | Physics | **COMPLETED & VERIFIED** |
| **8** | Dribbling Animation Tiers, On-Ball Accel, Ginga | Locomotion | NEXT |
| **9** | Aerial Anticipation, Headers, Volleys | Aerial | |
| **10** | Live Player Rating Engine & Match MVP | Analytics | |
| **11** | Dynamic Stadiums & Match Atmosphere | Atmosphere | 6 Crowd Levels in Kickoff |
| **12** | Pitch Dimensions, Weather & Surface Physics | Turf & Weather | |
| **13** | 32-Bit Main Menu System, Procedural Stadium Engine & Team Home Venues | Main Menu & Venues | Recalibrated (1 Day Quota) |
| **14** | Interactive 32-Bit Stadium Creator & Stand Camera Director Suite | Stadium Editor & HUD | Recalibrated (1 Day Quota) |
| **15** | Aerial Sky-Cam Broadcast Presentation & Dual Outside Environment Engine | Sky-Cam & Surroundings | Recalibrated (1 Day Quota) |
| **16** | IFAB Linesman Offside & VideoRef (VIR) | Rules | |
| **17** | Lightweight Cinematics & Replay Buffer | Presentation | |

---

**Token Discipline Reminder**  
1 Phase = strictly 1 Day's worth of Google AI Studio tokens (~700k–850k tokens). Every phase terminates in a fully compiled, zero-regression build. Zero-scroll console UI invariant across all viewports. Zero per-frame memory allocation for sustained 60 FPS on budget devices.
Every phase is deliberately scoped to one focused Google AI Studio free-tier day. Each phase ends with a compilable, playable build. Prefer extending existing zero-allocation systems over introducing new heavy abstractions. Mobile 60 FPS and single-screen 32-bit UI remain non-negotiable constraints for every change.


