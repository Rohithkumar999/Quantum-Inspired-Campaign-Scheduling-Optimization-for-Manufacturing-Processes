# Quantum-Inspired-Campaign-Scheduling-Optimization-for-Manufacturing-Processes

# Quantum-Inspired Campaign Scheduling Optimization for Manufacturing

## Project Overview
Manufacturing campaign scheduling is a complex combinatorial optimization problem faced by companies like Bayer Crop Science. Efficient scheduling of jobs on machines minimizes production time, reduces costs, and improves overall resource utilization. This project models such scheduling challenges using real-world manufacturing data and applies advanced optimization techniques to produce high-quality schedules.

In this project, a Genetic Algorithm (GA) metaheuristic is developed to optimize job sequences on manufacturing machines, aiming to **minimize makespan** — the total time required to complete all jobs — surpassing baseline heuristics like First-Come-First-Served (FCFS). The work also lays the foundation for exploring quantum-inspired optimization methods, aligning with cutting-edge research in industrial scheduling.

---

## Dataset
The dataset consists of 1000 manufacturing jobs detailing:

- **Job_ID:** Unique identifier for each manufacturing job  
- **Machine_ID:** Machine where the job is to be processed  
- **Operation_Type:** Type of operation (e.g., Grinding, Lathe, Milling)  
- **Material_Used:** Quantity of raw material used  
- **Processing_Time:** Time required by the machine to complete the job (in minutes)  
- **Machine_Availability:** Percentage availability of machine for scheduling  
- Other metadata like energy consumption, scheduled vs. actual times, and job status.

For scheduling optimization, the focus is on `Job_ID`, `Machine_ID`, `Processing_Time`, and `Machine_Availability`.



---


![Alt text](https://user-gen-media-assets.s3.amazonaws.com/gemini_images/43def2ec-ec1a-4383-b972-cb349db26f27.png)


## Methodology

### 1. Data Preprocessing
- Load and clean the dataset by handling missing values.  
- Extract relevant columns and convert data types for efficient scheduling.

### 2. Baseline Scheduling
- Implement First-Come-First-Served (FCFS), assigning jobs on machines in arrival order.  
- Calculate makespan as the baseline metric.

### 3. Genetic Algorithm Optimization
- Represent schedules as sequences (chromosomes) of job IDs.  
- Define a fitness function based on schedule makespan.  
- Apply genetic operators: selection, crossover (order crossover), and mutation (swap mutation).  
- Iterate to evolve better schedules over generations.

### 4. Visualization
- Generate Gantt charts to visualize machine-wise job scheduling and completion times.

---

## Installation and Usage

### Prerequisites
- Python 3.x  
- Libraries: `pandas`, `numpy`, `matplotlib`

Install required packages with:
pip install pandas numpy matplotlib

text

### Usage Steps
1. Clone this repository:
git clone

text
2. Download and place the CSV dataset `hybrid_manufacturing_categorical.csv` in the project root.  
3. Run the preprocessing script to clean and prepare data.  
4. Execute the genetic algorithm to optimize the schedule:
python genetic_scheduler.py

text
5. View console outputs for makespan results and Gantt chart visualizations.

---

## Results
- The Genetic Algorithm reduces makespan compared to FCFS baseline significantly.  
- Visualizations provide clear insights into job sequencing and machine utilization efficiency.  
- Demonstrates the power of metaheuristic optimization in real-world manufacturing scheduling.

---

## Relevance to Bayer Crop Science
Campaign scheduling is critical to Bayer’s operational effectiveness in seed and material production. This project models real scheduling challenges inside a manufacturing setup similar to Bayer's. By optimizing scheduling, the project contributes to reducing production delays, enhancing resource utilization, and aligning with Bayer’s innovation and sustainability objectives. The project showcases skillsets valuable to Bayer’s digital transformation and Industrial AI initiatives.

---

## Future Work and Extensions
- Integrate quantum-inspired optimization frameworks such as Fujitsu's Digital Annealer or D-Wave Ocean SDK.  
- Add multi-objective optimization to balance costs, energy consumption, and priority constraints.  
- Develop an interactive web dashboard for live schedule visualization and management.

---

## Author
[Rohith Kumar Reddipogula]  
MSc Data Science Student, Berlin, Germany  
Email: [rohith.reddipogula@outlook.com]  
LinkedIn: [(https://www.linkedin.com/in/rohith-kumar-reddipogula-a6692030b/)]  
GitHub: [https://github.com/Rohithkumar999]
