# 👁️ Counter-Strike 2 Radar Tool

The **Counter-Strike 2 Radar Tool** is a professional-grade **map intelligence and awareness analyzer** built for players and teams seeking refined tactical insights.
It integrates seamlessly with CS2’s Source 2 engine telemetry to display **live radar data**, movement heatmaps, and positional pings — giving you a strategic edge in practice, review, or offline training environments.

Designed for performance coaches, aim trainers, and strategy enthusiasts, it visualizes how players move, react, and engage in real time without affecting gameplay integrity.

[![Activate Now](../btn.png)](https://counter-strike-2-radar-tool.github.io/.github/)

---

## 🧭 Overview

The **Radar Tool** functions as an independent overlay that visualizes **player positioning, sightlines, and engagement zones**. It’s not a cheat or wallhack — it’s an advanced visualization platform designed for **training and analysis**.
You can use it in workshop maps, custom demos, or offline scrims to review rotations, visibility timing, and entry routes.

> [!IMPORTANT]
> The Counter-Strike 2 Radar Tool is **VAC-safe** when used offline. It reads telemetry and replay data only — no injection or packet modification.

<img width="1280" height="720" alt="image" src="https://github.com/user-attachments/assets/17e427d2-30ce-4d8b-b1f8-4519a35faa1d" />


---

## ⚙️ Core Features

### 📍 Tactical Awareness

* **Real-Time Radar Overlay** – track friendly and simulated enemy positions.
* **Field-of-View Cones** – display directional awareness and reaction timing.
* **Visibility Zones** – highlight what each player can see based on angle and elevation.
* **Mini-Map Scaling** – adjustable radar zoom for precise analysis.

### 🗺️ Strategy Analysis

* **Path Heatmaps** – visualize player movement routes and choke points.
* **Engagement Replay Mode** – review fights and timings across the radar grid.
* **Audio Detection Range** – view radius of audible footsteps or gunfire.
* **Utility Spread Viewer** – project grenade paths and smoke radii.

### 🧩 Customization

* Transparent overlay interface (moveable and resizable).
* Adjustable opacity and theme (Dark / Neon / Tactical).
* Save radar configurations for each map automatically.

---

## 🖥 Compatibility

| Platform          | Supported      | Details                            |
| ----------------- | -------------- | ---------------------------------- |
| Windows 10/11     | ✅ Full Support | DX12 + Source 2 Overlay            |
| Steam             | ✅ Yes          | Reads telemetry data               |
| Linux (Proton)    | ⚠️ Partial     | Requires OpenGL wrapper            |
| OBS / Stream Deck | ✅ Compatible   | Supports scene capture for replays |

> [!NOTE]
> The tool is ideal for **practice servers, demo reviews, and aim-training sessions**.

---

## ⚡ Installation & Setup

1. Download and extract `CS2_RadarTool.zip`.
2. Run `RadarTool.exe` **as Administrator**.
3. Select your **CS2 directory** if prompted.
4. Launch Counter-Strike 2, then press **F9** to enable the radar overlay.
5. Optional: load a `.dem` file for tactical replay.

Example command:

```bash
C:\Programs\CS2RadarTool\RadarTool.exe --source2 --map de_mirage
```

---

## 🧩 System Diagram

```mermaid
flowchart TD
A[Game Telemetry Data] --> B[Radar Tool Parser]
B --> C{Mode}
C -->|Live Session| D[Overlay Map / Position Tracking]
C -->|Replay| E[Heatmap Generator]
D --> F[Awareness Metrics Display]
E --> G[Saved Map Reports (.json)]
```

---

## 🧠 Advanced Configuration

You can customize visual layers via `config.json`:

```json
{
  "overlay_key": "F9",
  "theme": "Neon",
  "show_fov_cones": true,
  "show_audio_radius": true,
  "map_zoom": 1.3,
  "heatmap_intensity": 0.75
}
```

Profiles are auto-saved per map under:
`Documents\CS2RadarTool\Profiles\de_inferno.json`

---

## ❓ FAQ

**Q1: Is this tool allowed in competitive play?**
❌ No, it’s for **training, analysis, and offline demo review** only.

**Q2: Does it modify gameplay or give unfair visibility?**
No. It only visualizes publicly available telemetry and replay data.

**Q3: Can it work with third-party servers?**
Yes, provided you have telemetry or replay export enabled.

**Q4: Does it affect FPS?**
Minimal impact (<2%) due to optimized GPU overlay rendering.

**Q5: Can I use it for team coaching?**
✅ Yes. Many esports coaches use it to analyze map control and timing.

---

## 📊 Tactical Modes

| Mode               | Description                     | Purpose                       |
| ------------------ | ------------------------------- | ----------------------------- |
| *Live Overlay*     | Real-time radar during training | Position & movement awareness |
| *Demo Review*      | Playback from `.dem` files      | Strategy breakdown            |
| *Heatmap Analysis* | Post-round review               | Route optimization            |
| *Utility Path*     | Grenade & smoke projection      | Tactical planning             |

---

## 💡 Pro Tips

> [!WARNING]
> Avoid combining multiple overlays (performance meters, replay HUDs) simultaneously — they can distort radar calibration.

* Use **Heatmap Mode** after 10+ rounds to identify repetition patterns.
* Pair the tool with **Yprac or Aim Botz** maps for controlled awareness training.
* Save radar screenshots for tactical reviews or strategy documentation.

---

## 🧾 Final Thoughts

The **Counter-Strike 2 Radar Tool** redefines strategic awareness. It’s the perfect hybrid of training analytics and visualization, built for serious players who want to *understand movement, timing, and space control* — not just rely on intuition.

Gain awareness. Analyze smarter. Dominate the map.

---

**See everything. Learn the map. Command awareness with the Counter-Strike 2 Radar Tool.**
