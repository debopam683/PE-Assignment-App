<div align="center">

<img width="1200" height="475" alt="GHBanner" src="https://github.com/user-attachments/assets/0aa67016-6eaf-458a-adb2-6e31a0763ed6" />

  <h1>VoltFlow · Power Electronics Circuit Simulator</h1>

  <p>Interactive visual simulation and real-time waveform analysis for power electronics rectifiers and converters.</p>

</div>

---

## 🚀 Features

- **8 Universal Topologies**: Single-Phase & 3-Phase, Half-Wave & Full-Wave, Diode & Thyristor (SCR) Controlled Rectifiers.
- **Interactive Multi-Channel Oscilloscope**: Real-time waveform viewer for $v_s$, $v_o$, $i_o$, switch drop, and average DC levels with frame-by-frame stepping and slow-motion playback.
- **Dynamic Circuit Schematics**: Vector schematics with terminal binding posts ($L, N, A, B, C, DC+, DC-$), device pin markings ($A, K, G$), and active conduction path illumination.
- **Live Performance Metrics**: Instantaneous calculation of $V_{dc}$, $V_{rms}$, $I_{dc}$, $I_{rms}$, Ripple Factor ($RF$), Form Factor ($FF$), Rectification Efficiency ($\eta$), and PIV.

---

## 🛠️ Local Development

```bash
# 1. Install dependencies
npm install

# 2. Start the local development server
npm run dev
```

Visit `http://localhost:3000` in your browser.

---

## 📦 How to Deploy on GitHub Pages

This repository is already configured with:
1. `base: './'` in `vite.config.ts` (ensures assets load correctly on repository subpaths).
2. An automated GitHub Actions workflow in `.github/workflows/deploy.yml`.

### Step 1: Push code to your GitHub Repository

```bash
git init
git add .
git commit -m "Initial commit of Power Electronics Simulator"
git branch -M main
git remote add origin https://github.com/<your-username>/<your-repo-name>.git
git push -u origin main
```

### Step 2: Enable GitHub Pages in Repository Settings

1. Go to your repository on GitHub.
2. Click on **Settings** (top tab) → **Pages** (in the left sidebar under "Code and automation").
3. Under **Build and deployment** → **Source**, select **GitHub Actions**.

### Step 3: Automated Deployment

- Whenever you push changes to the `main` branch, the workflow will automatically build your app and deploy it.
- Within 1–2 minutes, your live site will be accessible at:
  `https://<your-username>.github.io/<your-repo-name>/`
