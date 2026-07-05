# 3D Temporal Barchart Visualization Engine

An advanced data visualization pipeline built with Python and Plotly to track categorical variance and feature distribution changes across a multi-year chronological baseline. 

This repository acts as a public open-source demonstration module featuring a custom, optimized 3D animation rendering layout.

## 🚀 Live Interactive Showcase
The primary interactive deployment is available as a web asset hosted natively via GitHub Pages. Click the link below to evaluate the timeline progression using full interactive speed tracking controls:

👉 **[Launch Live Interactive 3D Playback Dashboard](https://baseljarmak.github.io/BI-dashboard-plotly-dash/index.html)**

*Features a live programmatic canvas, multi-dimensional tracking meshes, and dynamic timeline frame skipping via a web-integrated player controller.*

---

## 🛠️ System Overview & Architecture

This processing engine evaluates structural changes within isolated datasets over time. The application layer cleanses specialized multi-column flat data, extracts categorical variables, and projects volumetric calculations using an automated coordinate mesh network.

### Key Functional Implementations:
1. **Dynamic Data Padding:** Evaluates multi-period timelines and injects structural zero-padded baseline records (`"any"`) for missing chronological steps to prevent vector shape mismatch errors between dynamic animation layers.
2. **Volumetric Mesh Generation (`go.Mesh3d`):** Dynamically plots 8-point coordinates (\(x, y, z\)) mapping to a spatial block layout representing volumetric trends.
3. **Decoupled Keyframes:** Generates lightweight layout state packages containing dynamic scene structural indices to avoid rendering bottlenecks over large network paths.

---

## 💻 Script Reference

The analysis component reads localized tracking spreadsheets, isolates target metrics via Pandas filter pipelines, and formats a sequential frame matrix:

```python
# Core logic snippet mapping temporal transitions
fig = go.Figure()

# Compile tracking states down the data period queue
fig.update(frames=[
    go.Frame(data=(data_period_names[i]['trace'])) 
    for i in range(0, len(data_period_names))
])
```

---

## 📚 Acknowledgments & Credits

*   **Core 3D Engine Architecture:** The programmatic mathematical layout mapping individual arrays into physical 3D box coordinates (`go.Mesh3d`) is built upon and adapted from the open-source base logic developed by [Serge Tochilov](https://github.com/serge-tochilov/barchart3d-plotly).
*   **Data Layout Extensions:** Upgraded to support continuous sequential looping, interactive animation state keys, dynamic column tracking calculations, and automated multi-period structural data alignment.

---

## 📝 License and Usage Notice

This repository represents a filtered, public view of core analytical code modules. Enterprise components, proprietary upstream database connection strings, and financial metrics are stripped and maintained within private enterprise repositories.
