## Hi there, I'm Guillaume Bonlieu 👋

**Aerospace Engineering Student | SAR, Remote Sensing & Geospatial Data Science**

I am an engineering student at ISAE-SUPAERO (Master's in Aerospace Engineering, major in Earth Observation), also pursuing an MSc in Operations Research and Optimisation at Université de Toulouse. I am passionate about Earth Observation, satellite imagery and GEOINT, and I specialise in SAR (Synthetic Aperture Radar) processing: building automated pipelines and deep-learning models for remote sensing applications.

🎯 **Seeking a 6-month final-year internship from April 2027.**

### 🛰️ Projects

#### 🔍 [Aletheia](https://github.com/bonlieuguillaume/aletheia): SAR forensics *(Nov. 2026 – present)*

**Detecting tampered and AI-generated Sentinel-1 radar images.** Fake satellite imagery now spreads during conflicts, and SAR is the natural next target: it is used for verification and defence, and its look (speckle, layover, radar shadows) is hard to challenge by eye. Given a SAR image, Aletheia answers two questions: *is it forged?* and *where?*

![A forged Sentinel-1 patch, its ground truth and the predicted map](https://raw.githubusercontent.com/bonlieuguillaume/aletheia/main/docs/figures/readme/hero_example.png)
*A test patch never seen in training: three pastes of different shapes (input | ground truth | predicted map).*

- **Model:** U-Net with a ResNet-34 encoder (PyTorch): a pixel-level map of the tampered regions, and an image-level decision derived from it.
- **Data:** 10 Sentinel-1 IW GRD forest scenes (Amazon, Gran Chaco) preprocessed with SNAP, 2,000 patches split by scene, copy-move forgeries at 3 difficulty levels.
- **v0.1 results** on unseen test scenes: image MCC 0.998, pixel MCC 0.991, one error out of 800 patches per level.
- **Next:** harder forgeries (distant-source copy-move, splicing), then inpainting and generated images.
- Python, PyTorch, Google Colab, pytest + GitHub Actions CI.

#### 🌹 [Rosarium](https://github.com/bonlieuguillaume/rosarium): Sentinel-1 preprocessing toolbox *(June 2026 – present)*

From an area of interest to analysis-ready GeoTIFFs: search the Copernicus CDSE STAC catalogue, download, then pre/post-event backscatter and coherence processing with ESA SNAP, all in fewer than 10 clicks through a webmap. Fully European data and processing chain, no dependency on ASF.

![Rosarium webmap: pre/post product search over a deforestation area](https://raw.githubusercontent.com/bonlieuguillaume/rosarium/main/frontend/rosarium_display.png)
*The webmap: pre-event (blue) and post-event (pink) Sentinel-1 footprints over an area of interest, ready to download and preprocess.*

- Python, ESA SNAP (gpt), Copernicus STAC (CDSE), rclone, Leaflet.

#### 🌊 [Moonfleet](https://github.com/bonlieuguillaume/moonfleet): maritime surveillance *(on pause)*

**Detect vessels anywhere in the ocean from a single command.** From a raw Sentinel-1 product, a SNAP graph runs orbit correction, calibration, speckle filtering, terrain correction, land masking and CFAR ship detection; the detections open in an interactive web map with vessel classes and live filters. Towards dark fleet identification.

![Moonfleet detections over the Strait of Hormuz](https://raw.githubusercontent.com/bonlieuguillaume/moonfleet/main/assets/display/hormuz-detections-cluster.png)
*Vessel detections over the Strait of Hormuz, with the tile footprint overlaid in cyan.*

#### 🛰️ Aerospacelab, Engineering and Business Project *(Oct. 2026 – present)*

Team project for an industrial client on the operating strategies of a spaceborne SAR (acquisition modes, on-board processing, detection algorithms).

### 💼 Experience & Education

- **SERTIT (ICube), Sept. 2025 – Feb. 2026**: SAR image processing internship. Built a Python pipeline for deforestation-related change detection from Sentinel-1, leveraging backscatter and interferometric coherence, and exposed the limitations of C-band SAR for this use.
- **ISAE-SUPAERO (Toulouse)**: Master's in Aerospace Engineering, major in Earth Observation, Defence Certificate. Exchange semester at UNRC (Argentina).
- **Université de Toulouse**: MSc in Operations Research and Optimisation (global, combinatorial and ML optimisation).

### 🛠️ Tech Stack

- **Languages:** Python (primary), basic SQL, Java, C
- **Geospatial & RS:** ESA SNAP, Copernicus (Sentinel-1/2, CDSE, STAC), QGIS, Rasterio, GeoPandas
- **AI & Data Science:** Machine Learning, Deep Learning, PyTorch, Scikit-learn, NumPy
- **Tools:** Conda, Git, GitHub, GitHub Actions, Docker, Google Colab

### 📊 Key Skills

- **SAR imaging:** geometric and radiometric corrections, coregistration, backscatter and coherence analysis, CFAR detection.
- **Geospatial data science:** leveraging data science and deep learning to extract value from geospatial data.
- **Soft skills:** leadership (former association president), problem-solving under pressure, proactive project management.

### 🌍 Languages

- **French:** Native
- **English:** Full Professional Proficiency (C1–C2, Cambridge Proficiency 193/230)
- **Spanish:** Professional Working Proficiency (B2–C1, CELU 3.1/4)
- **Russian:** Basic (A2)

### 📬 Get in Touch

- **LinkedIn:** [linkedin.com/in/guillaumebonlieu](https://linkedin.com/in/guillaumebonlieu)
- **Email:** bonlieuguillaume@gmail.com
- **Location:** Lyon / Toulouse, France

> *"Curious and passionate about how satellite data can solve real-world environmental challenges."*
