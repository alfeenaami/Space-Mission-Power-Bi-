# Space Mission Timeline Explorer
### A Comprehensive Power BI Dashboard | 1957 - 2025

## 🌌 About the Project

This project analyzes **4,451 space missions** launched by **65 companies** across **18 countries** — covering everything from the Soviet Sputnik era to modern SpaceX launches.

The dashboard answers key questions:
- 🌍 Which country dominated space exploration?
- 🏢 Which company launched the most missions?
- 📅 How did space launches evolve over decades?
- 🚀 Which rockets are most reliable?
- 💰 How much did space missions cost?
- ✅ What is the overall mission success rate?

---

## 📁 Dataset Information

| Property | Details |
|---|---|
| **Source** | Kaggle — All Space Missions from 1957 |
| **Extended** | Manually added 2020-2025 missions |
| **Total Records** | 4,451 missions |
| **Date Range** | 1957 to 2025 |
| **Companies** | 65 unique space agencies |
| **Countries** | 18 countries |
| **Launch Sites** | 50 unique sites |
| **Rockets** | 384 unique rocket variants |

### Original Columns:
| Column | Description |
|---|---|
| Company Name | Space agency or company |
| Location | Launch site details |
| Datum | Launch date and time |
| Detail | Rocket name and mission name |
| Status Rocket | Active or Retired |
| Rocket | Cost in $ million |
| Status Mission | Success / Failure / Partial Failure / Prelaunch Failure |

---

## 🗃️ Data Model

The project uses a **Star Schema** data model with:
- **1 Fact Table**
- **5 Dimension Tables**
- **5 One-to-Many Relationships**

```
DimDate ─────────┐
DimCompany ──────┤
DimLocation ─────┼──→ FactMission (Center)
DimRocket ───────┤
DimStatus ───────┘
```

## 🔑 Key Insights

```
🏆 Most Missions    → RVSN USSR with 1,777 missions (40% of all launches!)
✅ Success Rate     → 89.69% overall mission success
❌ Failed Missions  → 353 total failures
🌍 Top Country     → USA with 1,428 missions
🇷🇺 Close Second   → Russia with 1,400 missions
🇰🇿 Baikonur       → Kazakhstan with 707 launches
📈 Peak Era        → 1960s-1980s Space Race
📉 Biggest Drop    → 1991 USSR Collapse
💰 Most Expensive  → NASA SLS Artemis I at $4.1 Billion
💸 Most Efficient  → SpaceX Falcon 9 at $55M per launch
📊 YOY Growth      → +22.52% in recent years
🚀 Modern Leader   → SpaceX with highest success rate
```

---

## 🛠️ Tools Used

| Tool | Purpose |
|---|---|
| Microsoft Power BI Desktop | Dashboard development |
| Microsoft Excel | Data preparation and merging |
| Microsoft PowerPoint | Background design |
| DAX | Data Analysis Expressions |
| Power Query (M Language) | Data cleaning and transformation |
| Kaggle | Dataset source |

---

## 🎓 Learnings

```
📌 Star Schema Data Modeling
📌 Power Query — Data cleaning, merging, splitting
📌 DAX Time Intelligence Functions
📌 Advanced DAX (RANKX, SWITCH, VAR)
📌 Dashboard UI/UX Design
📌 Color Theory in Data Visualization
📌 Storytelling with Data
📌 Bookmark and Navigation tricks
📌 Decomposition Tree Analysis
📌 Conditional Formatting
```

## 📁 Dataset
Source: Kaggle
Dataset:**🔗https://www.kaggle.com/datasets/agirlcoding/all-space-missions-from-1957



