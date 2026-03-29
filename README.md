# 📊 Experiment 2: Upper Confidence Bound (UCB) Algorithm for Ad Optimization

**Name:** Sanad Naqvi
**Roll No:** 221A023

---

## 🎯 Aim

To implement the **Upper Confidence Bound (UCB) algorithm** and compare its performance with random ad selection in order to maximize total reward.

---

## 📌 Problem Statement

The goal is to determine the most effective advertisement among multiple options by maximizing user clicks using a reinforcement learning approach.

---

## 📖 Theory

### 🔹 Multi-Armed Bandit Problem

This problem represents a scenario where an agent must choose between multiple options (ads), each having an unknown reward distribution.

### 🔹 Exploration vs Exploitation

* **Exploration:** Trying different ads to gather information
* **Exploitation:** Selecting the best-known ad to maximize reward

### 🔹 Upper Confidence Bound (UCB)

UCB is a strategy that balances exploration and exploitation by selecting the ad with the highest upper confidence bound.

UCB formula:

```
Upper Bound = Average Reward + √( (3/2 * log(n+1)) / Number of Selections )
```

---

## 🛠️ Implementation

### 🔹 Libraries Used

* numpy
* matplotlib
* pandas
* random
* math

### 🔹 Dataset

* Ads Optimisation dataset
* Contains 10 ads and 10,000 rounds
* Each value represents whether the ad was clicked (1) or not (0)

### 🔹 Steps

1. Imported dataset using pandas
2. Implemented **Random Selection** strategy
3. Calculated total reward for random ads
4. Implemented **UCB Algorithm**:

   * Initialized selection counters and rewards
   * Calculated upper bound for each ad
   * Selected ad with highest UCB value
5. Updated rewards and selection count
6. Compared performance with random selection

---

## 📊 Results

* **Total Reward (Random Selection):** 1206

* **Total Reward (UCB):** 2178

* UCB significantly outperformed random selection by choosing better ads over time.

* Most selected ads:

  * Ad 5 selected highest number of times
  * Other ads selected based on performance

---


## ✅ Conclusion

* The UCB algorithm successfully optimized ad selection.
* It effectively balanced exploration and exploitation.
* Compared to random selection, UCB achieved much higher rewards.
* This demonstrates the power of reinforcement learning in real-world decision-making problems like online advertising.

---

## 📚 References

* Machine Learning A-Z Course
* Reinforcement Learning Concepts
* Python Documentation

---

## 📦 requirements.txt

```id="8f1d2k"
numpy
matplotlib
pandas
```
