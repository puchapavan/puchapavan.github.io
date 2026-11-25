---
layout: page
title: Smart Water Management for Agriculture
description: Deep learning water-level detection, weather forecasting and drought early warning for farm fields, with SMS alerts.
importance: 3
github: https://github.com/puchapavan/Smart-Water-Management-for-Agriculture
---

A machine learning course project that helps farmers decide when to drain or irrigate a field. It combines three models into one decision engine, which sends an SMS alert and shows the status on a dashboard.

- **Water-level detection:** classifies drone images of fields (FloodNet) as low, medium or high water using transfer learning on MobileNetV3.
- **Drought early warning:** predicts drought risk from IMD gridded rainfall data (2015–2025) using the Standardized Precipitation Index and LightGBM.
- **Weather forecast:** a 7-day rainfall forecast from Open-Meteo, mapped to IMD heavy-rain categories.

<div class="row mt-3">
  <div class="col-sm mt-3 mt-md-0">
    {% include figure.liquid loading="eager" path="assets/img/projects/integrated-demo.jpg" title="Integrated demo" class="img-fluid rounded z-depth-1" %}
  </div>
</div>
<div class="caption">The decision engine on three field images, giving FLOOD, PRE-FLOOD and OK alerts.</div>

<div class="row">
  <div class="col-sm mt-3 mt-md-0">
    {% include figure.liquid path="assets/img/projects/drought-risk-map.jpg" title="Drought risk map" class="img-fluid rounded z-depth-1" %}
  </div>
</div>
<div class="caption">Predicted drought risk across India (left) against the actual drought class (right).</div>

**Results**

| Module | Model | Result |
| --- | --- | --- |
| Water-level detection | MobileNetV3-Large | 89.6% accuracy, macro F1 0.79 (simple CNN: 80.5%) |
| Drought early warning | LightGBM | 80.7% accuracy, 79.4% drought recall (baseline: 53.3%) |

**Tools:** Python, deep learning (MobileNetV3 transfer learning), LightGBM, Open-Meteo API, Streamlit, Twilio / Fast2SMS.

**Code:** [github.com/puchapavan/Smart-Water-Management-for-Agriculture](https://github.com/puchapavan/Smart-Water-Management-for-Agriculture)
