# 🗺️ Tour Guide Planner: Optimizing Travel Routes For Efficient Planning

## 📌 Project Overview

This project focuses on building a **Tour Guide Planner** that optimizes travel routes for users based on **time, distance, or cost**. The system accepts multiple destinations and identifies the most efficient travel path from a starting location.

The goal is to enhance travel planning by helping users **save time and money** while covering multiple destinations in a trip.

---

## ✨ Features

* 📍 **Multi-Destination Input** – Accepts multiple travel points.
* 🛣️ **Optimized Route Planning** – Finds the shortest or cheapest route.
* ⏳ **Time & Cost Efficiency** – Helps minimize travel cost, distance, or time.
* 📊 **Graph-Based Modeling** – Efficient route calculation using graph theory.
* 🚦 **Route Availability Check** – Marks unreachable locations.

---

## 🛠️ Solution Methodology

1. **Graph Construction**

   * Locations are modeled as **nodes (vertices)**.
   * Travel routes are modeled as **edges with weights**.
   * Weights represent **cost, time, or distance**.

2. **Shortest Path Algorithm (Dijkstra’s Algorithm)**

   * Uses a **priority queue (min-heap)** for efficient selection.
   * Computes shortest path from the source to all other destinations.
   * Ensures optimized performance in **O((V + E) log V)** time.

3. **Output Generation**

   * Displays optimized cost/time to reach each destination.
   * Highlights **unreachable locations**.
   * Helps travelers build an **efficient itinerary**.

---

## 📐 Approach

### Step 1: Problem Modeling

* Model locations as **nodes**.
* Model travel routes as **weighted edges**.
* Define this as a **Shortest Path Problem in a Weighted Graph**.

### Step 2: Data Structures Used

* `unordered_map<string, int>` → Maps location names to indices.
* `vector<string>` → Stores location names.
* `vector<vector<Edge>>` → Graph adjacency list.
* `priority_queue` → For Dijkstra’s shortest path calculation.
* `vector<int> dist` → Stores minimum distances from source.

### Step 3: Dijkstra’s Algorithm

* Initialize all distances as **infinity**.
* Set source distance = 0.
* Use **priority queue** to pick the next closest node.
* Update neighbors if a shorter path is found.
* Repeat until all nodes are processed.

### Step 4: Route Optimization

* Print **optimized travel costs** from source to each destination.
* Mark unreachable destinations.
* Helps users prioritize **cheaper & closer routes**.

---

## ⚡ Benefits for Users

✔️ Save **time and money** during travel.
✔️ Avoid **unreachable or costly paths**.
✔️ Create an **efficient travel plan** with multiple destinations.
✔️ Gain confidence in **planning routes smartly**.

---

## 📂 Repository Structure

```bash
TOUR_GUIDE/
├── README.md            # Project documentation
├── TOUR GUIDE.pdf       # Project Report
```

---

## 🚀 Future Enhancements

* 🌍 Integration with **real-world map APIs (Google Maps, OpenStreetMap)**.
* 📱 Mobile App version for travelers.
* ⭐ Personalized route suggestions based on user preferences.

---

## 👩‍💻 Author

**Anchal Verma**
📧 [anchalxv@gmail.com](mailto:anchalxv@gmail.com)
🔗 [GitHub Profile](https://github.com/anchalV194)

---

