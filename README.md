# F1-strategy-recommendation-engine

This project analyzes Formula 1 race telemetry data and builds a strategy recommendation system to identify optimal pit stop strategies.

The project uses FastF1 race data to analyze tire degradation, simulate race scenarios, and compare different strategy combinations.

---

## Project Objectives

• Analyze tire degradation patterns across compounds  
• Identify optimal pit stop windows  
• Simulate race strategies using Monte Carlo simulation  
• Compare strategies based on total race time  

---

## Technologies Used

Python  
Pandas  
NumPy  
Matplotlib  
Seaborn  
FastF1 API  

---

## Key Analysis

### Tire Degradation Analysis

The project evaluates how lap time changes as tire life increases for different tire compounds.

Soft tires provide early race pace but degrade quickly, while medium and hard tires provide longer stint stability.

### Pit Stop Timing

Historical pit stop laps are analyzed to identify common pit windows during the race.

### Monte Carlo Race Simulation

A Monte Carlo simulation is used to model race outcomes under different strategies by incorporating:

• Tire degradation  
• Lap time variability  
• Pit stop time loss  

---

## Strategy Optimization

The simulation evaluates multiple strategies such as:

Soft → Medium  
Medium → Hard  
Soft → Hard  

The strategy with the lowest simulated race time is recommended as the optimal strategy.

## Tire Degradation Analysis

![Tire Degradation](plt.savefig(\"visuals:tire_degradation.png\", dpi=300).png)
 

## Strategy Performance Heatmap

![Strategy Heatmap] (plt.savefig(\"visuals:strategy_heatmap.png\", dpi=300).png)
---

## Key Insight

The simulation results suggest that starting on **Soft tires** and switching to **Medium tires around lap 30** provides the best balance between early race pace and long-run tire durability.

---

## Future Improvements

• Include weather and track temperature variables  
• Extend strategy search to multi-pit strategies  
• Build an interactive dashboard using Tableau or Power BI
