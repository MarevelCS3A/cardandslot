# 🎰 Lucky 9 & Slot Machine · Monte Carlo Analysis  
**Stochastic Game Simulation**  
Explore how probability tweaks and payout tuning shape house edge in **Lucky 9** and a **3-reel slot machine**. Run thousands of simulations, then optionally play interactively.

---

## Quick Facts
- 🃏 Lucky 9 with adjustable multipliers  
- 🎰 Slot machine with weighted reels  
- 📈 10,000+ simulations per run  
- 📊 ROI, win rate, and profit charts  

---

## Introduction
This project simulates casino-style games using **Monte Carlo methods** to compare **fair vs. tweaked probability models**.  

I chose **Option 2: Game Simulation** to:  
- Explore probability adjustments in gambling games  
- Measure house edge impacts  
- Visualize outcomes over thousands of plays  

**Project Goal:**  
Simulate Lucky 9 and a weighted slot machine under both fair and tweaked rules, then analyze **win rates, ROI, and house profit**.

---

## Project Overview
The project consists of these steps:  

1. **Define game rules and payout structures** for Lucky 9 and Slot Machine.  
2. **Simulate 10,000+ plays** for both fair and tweaked models.  
3. **Collect outcomes** (win/loss, payouts, player profit, house profit).  
4. **Perform Exploratory Data Analysis (EDA)** using charts.  
5. **Compare fair vs. tweaked models** to quantify house edge.  
6. **Summarize findings and insights**.  

---

## Data Generation / Model Definition

### 🎴 Lucky 9
**How to Play:**  
- Each hand draws **two cards**; totals are modulo 10  
- Player may draw a **third card**  
- Compare player vs. banker: higher total wins; tie returns bet  

**Payout Structure (default)**  

| Outcome | Payout | Example |
|---------|--------|---------|
| Loss    | –1     | Lose bet |
| Tie     | 0      | Push |
| Win     | +2     | ~2:1 multiplier |

**Tweaked Model:**  
- Banker’s probability slightly biased toward high totals  
- Player distribution unchanged  

---

### 🎰 Slot Machine
**How it Works:**  
- 3 reels with weighted symbols: A, B, C, D, 7, BAR  
- Only **triples pay**  
- Rare symbols pay more  
- House edge can be tuned via **reel weights** or forced-win probability  

**Example Triple Payouts:**  

| Symbol | Multiplier |
|--------|-----------|
| A      | 2x        |
| B      | 3x        |
| C      | 5x        |
| D      | 8x        |
| 7      | 15x       |
| BAR    | 25x       |

**Tweaked Model:**  
- Jackpot symbol 7 occurrence reduced  
- Other symbols adjusted to compensate  
- Payouts remain the same  


