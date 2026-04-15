📦 Last-Mile Delivery Route Optimization
📌 Project Overview

This project focuses on optimizing last-mile delivery routes using real-world location data. The objective is to minimize total travel distance while ensuring operational feasibility under vehicle capacity constraints.

🧠 Business Problem

Last-mile delivery is one of the most expensive and complex parts of logistics. Inefficient routing leads to increased delivery time, higher fuel costs, and poor resource utilization.

This project addresses the challenge of selecting optimal delivery routes when multiple customers, limited vehicle capacity, and a central depot must be considered simultaneously.

⚙️ Approach
Extracted real-world location data from NYC taxi dataset and adapted it as delivery points
Simulated a delivery environment with:
50 customer locations
1 central depot
demand per customer
Computed pairwise distances using the Haversine formula
Formulated the problem as a Capacitated Vehicle Routing Problem (CVRP)
Solved using Google OR-Tools
📊 Results
Metric	Value
Customers	50
Vehicles	3
Total Demand	121
Baseline Distance	348.95 km
Optimized Distance	80.7 km
Distance Reduction	~76.9%

The optimized solution significantly reduces travel distance compared to a naive routing baseline, while respecting vehicle capacity constraints.

🛠️ Tools & Technologies
Python (Pandas, NumPy)
Google OR-Tools
Jupyter Notebook
📈 Key Insights
Naive routing leads to highly inefficient travel patterns
Optimization under constraints drastically improves operational efficiency
Feasibility depends on aligning demand with vehicle capacity
Structured optimization provides measurable business impact
🚀 Future Improvements
Add delivery time windows
Incorporate traffic and real-time constraints
Scale to larger fleets and dynamic routing
Integrate demand forecasting for end-to-end optimization
📁 Project Structure
delivery-route-optimization/
│
├── data/
│   └── delivery_project_data.csv
├── notebook/
│   └── route_optimization.ipynb
├── README.md
💡 How to Run
Clone the repository

Install dependencies:

pip install pandas numpy scipy ortools
Run the Jupyter notebook
👤 Author

Manprit Kaur
