# 🌿 AI in Ayurveda — Prakriti Research Site

A static research website presenting data analysis from the **AI in Ayurveda** study, comparing human and AI-generated Prakriti (Ayurvedic constitutional type) survey responses.

🔗 **Live Site:** [ankitas134.github.io/prakriti-research](https://ankitas134.github.io/prakriti-research)  
🔗 **Main App Repo:** [github.com/ankitas134/Prakriti](https://github.com/ankitas134/Prakriti) 

---

## 📊 What This Site Shows

| Section | What It Covers |
|---|---|
| Key Findings | 6 standout insights from the data |
| Dosha Distribution | Human vs AI breakdown by dosha, gender, age |
| Human vs AI Divergence | Per-question comparison showing where AI data diverges |
| Symptom Heatmap | Alignment between reported symptoms and self-identified Prakriti |
| Discordance Study | Doctor-told vs self-assessment agreement rate |
| Methodology | How data was collected and analysed |

---

## 📁 File Structure

```
prakriti-research/
├── index.html            ← Static research website (all-in-one)
├── prakriti_tagged.csv   ← Full dataset with source column (human/ai_generated)
├── analytics_data.json   ← Pre-computed analytics used by the charts
└── README.md
```

---

## 📂 Dataset: `prakriti_tagged.csv`

The dataset contains **189 responses** (61 human + 128 AI-generated) across 18 survey questions.

| Column | Description |
|---|---|
| `Timestamp` | Submission time (human responses only) |
| `Gender` | Male / Female / Prefer not to say |
| `Age(Number)` | Participant age |
| `Q1–Q15` | Physical, physiological, psychological, lifestyle questions |
| `Q16` | Prior Prakriti assessment by a doctor |
| `Q17` | Frequent health issues (symptom cluster) |
| `Q18` | Self-assessed primary Prakriti |
| **`source`** | `human` (rows 1–61) or `ai_generated` (rows 62–189) |

---

## 🔑 Key Findings

- **AI data distributes doshas in a perfect 33.3/33.3/33.3 split** — humans show natural skew (Pitta 41.7%, Vata 36.7%, Kapha 21.7%)
- **68.9% of humans chose "Medium/Well-built" body frame** — AI data shows only 35.9%
- **Female Kapha is only 10% in humans** — AI shows 35.6%, completely missing this gender-dosha pattern
- **90% agreement** between doctor-diagnosed and self-assessed Prakriti
- **AI symptom-Prakriti alignment is perfectly diagonal** (zero cross-dosha responses) — impossible in real populations
- **Anxiety/nervousness dominates human stress responses** (42.6%) — AI distributes all three equally

---

## 🚀 Deploying on GitHub Pages

This is a **100% static site** — no server needed. Deploy in 3 steps:

1. Create a new repo called `prakriti-research`
2. Push all files to the `main` branch
3. Go to **Settings → Pages → Source → main branch / root**

Your site will be live at `https://your-username.github.io/prakriti-research`

---

## 🔗 Related

- **Main Prakriti App** (Flask + ML): [github.com/ankitas134/Prakriti](https://github.com/ankitas134/Prakriti)
- Built as part of the *AI in Ayurveda* research project
- Data collected for educational and research purposes only · Participant identities not disclosed
