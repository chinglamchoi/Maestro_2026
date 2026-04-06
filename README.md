<p align="center">
  <br />
  <img src="https://img.shields.io/badge/太極-Tai_Chi-5b8a72?style=for-the-badge&labelColor=2c2c3a" alt="Tai Chi"/>
  <br /><br />
</p>

<h1 align="center">Maestro</h1>
<p align="center"><em>Virtual Tai Chi Tutor — AI-powered real-time posture correction</em></p>

<p align="center">
  <img src="https://img.shields.io/badge/OpenPose-Computer_Vision-5b8a72?style=flat-square" alt="OpenPose"/>
  <img src="https://img.shields.io/badge/Real--time-Pose_Estimation-7ea8be?style=flat-square" alt="Pose Estimation"/>
  <img src="https://img.shields.io/badge/Hong_Kong-Social_Impact-d4a574?style=flat-square" alt="Social Impact"/>
</p>

<p align="center">
  <a href="#-overview">Overview</a> · 
  <a href="#-motivation">Motivation</a> · 
  <a href="#-how-it-works">How It Works</a> · 
  <a href="#-features">Features</a> · 
  <a href="#-project-history">Project History</a> · 
  <a href="#-references">References</a>
</p>

---

## 🎯 Overview

Maestro is an AI-powered Tai Chi tutor that uses human pose estimation to give **real-time, personalised feedback** on form. Point a camera at yourself while practising, and Maestro compares your posture against expert demonstrations — correcting misalignments instantly through visual and audio cues.

> A private coach at the tap of a button, unconstrained by time, cost, or geography.

---

## 🌏 Motivation

<table>
<tr>
<td width="120" align="center"><h1>10%</h1><sub>of HK elderly show<br/>signs of depression</sub></td>
<td width="120" align="center"><h1>3×</h1><sub>elderly suicide rate<br/>vs. city-wide avg</sub></td>
<td>

In Hong Kong, elderly residents face declining physical and cognitive health alongside deepening intergenerational isolation. Tai Chi — linked by research from Harvard Medical School and HKU to slower dementia progression, reduced depression, and stronger social bonds — is uniquely positioned to address both.

Maestro digitises something elders already love, wrapping it in a platform where grandparents and grandchildren practise together. Rather than asking elderly users to adapt to youth culture, we brought technology to meet them where they are.

</td>
</tr>
</table>

---

## ⚙️ How It Works

Maestro frames Tai Chi correction as two ML tasks: **classification** (identifying which posture the user is attempting) and **discrimination** (determining whether it is executed correctly).

```
📷 Camera feed
 ↓
🦴 Pose estimation (OpenPose) → Skeleton extraction
 ↓
📊 Compare against expert trajectories
 ↓
🟢 Correct → Green overlay + encouragement
🔴 Incorrect → Red highlight + audio correction
```

| Component | Detail |
|:--|:--|
| **Pose Estimation** | OpenPose with Part Affinity Fields (PAFs) for multi-person 2D pose estimation |
| **Personalisation** | PAFs learn body parts independently per user, adapting to different physiques |
| **Feedback** | Red/green skeleton overlay + real-time audio cues |
| **Frontend** | HTML, CSS, JavaScript, Bootstrap |

---

## ✨ Features

| | Feature | Description |
|:--:|:--|:--|
| 🤖 | **AI Posture Correction** | Real-time pose estimation compared against Tai Chi masters |
| 🎨 | **Visual Feedback** | Skeleton overlay with red/green colour coding per joint |
| 🔊 | **Audio Feedback** | Spoken corrections and encouragement during practice |
| 🎵 | **Ambient Audio** | Relaxing background music for a meditative environment |
| 💬 | **Discussion Forum** | Community where masters share guides and beginners ask questions |
| 👨‍👩‍👧‍👦 | **Intergenerational Design** | Video-call practice connecting grandparents and grandchildren |

---

## 📅 Project History

```
2018                    2018–2021                 2021                     Now
  ●━━━━━━━━━━━━━━━━━━━━━━━●━━━━━━━━━━━━━━━━━━━━━━━●━━━━━━━━━━━━━━━━━━━━━━━●
  │                        │                        │                        │
  Conceived idea           CUHK Multimedia Lab      Built & launched         MIT — multimodal AI,
  as secondary student     & NVIDIA Research:       Maestro                  structured reasoning,
  in Hong Kong             video synthesis,                                  AI safety
                           perceptual consistency
```

| Year | Milestone |
|:--|:--|
| **2018** | Conceived the idea as a secondary school student in Hong Kong — 5+ years before the first AI Tai Chi startups. The stack didn't exist: fast models were inaccurate, accurate ones were too slow. |
| **2018–2021** | Worked on underlying bottlenecks. At CUHK Multimedia Lab: contrastive learning for generative models. At NVIDIA Research: contributed to Face Vid2Vid, advancing real-time video synthesis. |
| **2021** | Built and launched Maestro — real-time pose estimation, expert comparison, personalised audio-visual feedback. |
| **Present** | Continuing AI research at MIT. Same conviction: identify what living beings actually need, then build AI to serve that need. |

---

## 📚 References

1. Cao, Z., Hidalgo, G., Simon, T., Wei, S.E., Sheikh, Y. — *OpenPose: Realtime Multi-Person 2D Pose Estimation using Part Affinity Fields* (CVPR 2017)
2. Kendall, A., Grimes, M., Cipolla, R. — *PoseNet: A Convolutional Network for Real-Time 6-DOF Camera Relocalization* (ICCV 2015)
3. Fang, H.-S., Xie, S., Tai, Y.-W., Lu, C. — *RMPE: Regional Multi-Person Pose Estimation* (ICCV 2017)

---

## 📄 License

This project was created for research and social impact purposes.

---

<p align="center">
  <img src="https://img.shields.io/badge/Technology_bridging_generations-2c2c3a?style=for-the-badge" alt="Technology bridging generations"/>
  <br /><br />
  <sub>Built by Choi Ching Lam · Hong Kong</sub>
</p>
