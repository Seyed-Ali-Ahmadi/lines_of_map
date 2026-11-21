# The Shapes of Rivers & Highways · Iran & Iraq 🌊🛣️

An interactive cartographic exploration of the world's most dramatic river networks and national transit corridors, collapsed into abstract geometric forms.

Inspired by Dr. Dominic Royé's signature dataviz project [The Shapes of Rivers](https://dominicroye.github.io/shapes-of-rivers/).

---

## 🌐 Live Demo

🔗 **[Launch Interactive App](https://seyed-ali-ahmadi.github.io/lines_of_map/)**  
*(Replace with your actual GitHub Pages URL after deployment)*

---

## 🗺️ Datasets Included

1. **Iraq Rivers (19 Major River Courses)**  
   The ancient cradle of civilization, dominated by the **Tigris (*Dijlah*)** and **Euphrates (*Al-Furat*)** systems, along with the **Great Zab**, **Little Zab**, **Diyala (*Sirwan*)**, **Khabur**, and **Al-Gharraf**.
   
2. **Iran Rivers (62 Major River Courses)**  
   Iran's diverse hydrological basins across the Zagros and Alborz ranges, featuring the **Karun** (Iran's most effluent river), **Karkheh**, **Sefid-Rud**, **Aras**, **Zayandeh-Rud**, **Atrak**, **Dez**, and **Mand**.

3. **Iran National Highways (341 Inter-City Corridors)**  
   The primary arterial transit corridors connecting Iranian cities, including the **Tehran – Semnan – Mashhad Expressway (Road 44)**, the **Tehran – Qom – Isfahan – Shiraz spine**, the mountain passes of **Chalus (Road 59)** and **Haraz (Road 77)**, and international border links to Turkey, Iraq, and Central Asia.

---

## ✨ Features & Visual Views

* **Drop View (Rotated North · Equal Length):**  
  Every river and highway is scaled to an equal visual length and rotated so its mouth (or terminus) points straight North ($0^\circ$). This isolates and highlights the meandering geometry and sinuosity index ($S = \text{Actual Length} / \text{Straight-Line Distance}$).
* **Radial View (True Geographic Bearing):**  
  All paths radiate from a shared center $(0,0)$ while preserving their real compass azimuth, illustrating how drainage basins divide across mountain crests or how transport corridors fan out from central hubs.
* **Map View (Real Geographic Alignment):**  
  Rivers and roads return to their authentic geographic coordinates, overlaid with **official sovereign country borders**, **Caspian Sea & Persian Gulf coastlines**, and **major city anchor points**.
* **Major City Hub Filter:**  
  Isolate corridors connected to Iran's key transport hubs: **Tehran**, **Mashhad**, **Isfahan**, **Tabriz**, **Shiraz**, and **Ahvaz**.
* **Interactive Tooltips & Search:**  
  Hover over any line to inspect its name, corridor path, length in km, and sinuosity index. Filter in real time by typing any city or river name.
* **Smooth 60 FPS Transitions:**  
  Hardware-accelerated HTML5 Canvas with smooth cubic easing between all views.

---

## 🚀 How to Deploy on GitHub Pages

This project is completely **self-contained in a single `index.html` file** with zero build steps, zero npm packages, and zero external CDN dependencies.

### Step 1: Create a Repository
1. Go to [GitHub.com](https://github.com) and create a new repository (e.g. `shapes-of-iran`).
2. Make it **Public**.

### Step 2: Upload Files
Upload `index.html` and this `README.md` directly into the repository root:
* `index.html`
* `README.md`

### Step 3: Enable GitHub Pages
1. Go to your repository's **Settings** $\to$ **Pages** (in the left sidebar).
2. Under **Build and deployment** $\to$ **Source**, select **Deploy from a branch**.
3. Under **Branch**, select `main` (or `master`) and folder `/ (root)`.
4. Click **Save**.

Your interactive map will be live at:
```
https://<your-username>.github.io/<your-repo-name>/
```

---

## 🛠️ Data Sources & Methodology

* **Rivers:** [GSriver](https://figshare.com/articles/dataset/GSriver/30119851) (Liu et al., CC BY 4.0), integrating HydroRIVERS, OpenStreetMap, and GRIT. Each river is resampled to 200 equidistant vertices.
* **Borders & Coastlines:** [Natural Earth Vector](https://www.naturalearthdata.com/) 1:50m administrative boundaries and marine coastlines.
* **Highways:** Natural Earth 1:10m Roads and OpenStreetMap, topologically clipped strictly to national sovereign boundaries and tagged with city-to-city corridor names.
* **Rendering Engine:** Vanilla HTML5 Canvas with custom matrix interpolation and 2D rotation transformations.

---

## 📄 License & Credits

* Original concept and methodology: [Dr. Dominic Royé](https://dominicroye.github.io/) ([The Shapes of Rivers](https://dominicroye.github.io/shapes-of-rivers/)).
* River data: GSriver (HydroRIVERS, OSM, GRIT).
* Code license: [MIT License](LICENSE) (Free to use, modify, and distribute).
