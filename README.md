# Link Budget and Constellation Coverage Tool

This project is an interactive web-based mission design tool for computing LEO communication link budgets, propagating satellite orbits, and analyzing constellation coverage. 

> **Note:** This project was developed as part of the ROSPIN Summer School. 
> Find out more about the organization here: [Romanian Space Initiative](https://github.com/Romanian-Space-Initiative).

## 🚀 Features
* **Link Budget Calculator:** Computes transmit power, antenna gains, free space/atmospheric losses, system noise, and margins for specific data rates.
* **Orbit Geometry:** Propagates satellites from TLEs and computes passes, elevation, and range over a ground station.
* **Constellation Coverage:** Computes coverage and revisit statistics over Romania for small constellations.
* **Interactive UI:** Built with Streamlit for easy, browser-based mission design.

## 📂 Project Structure
* `app.py`: The main Streamlit web application.
* `link_budget.py`: Core logic for communication link computations.
* `orbit.py`: Satellite propagation and geometry calculations (using Skyfield/SGP4).
* `coverage.py`: Algorithms for constellation revisit statistics.
* `data.py`: Data handling and TLE parsing.
* `test_link_budget.py`: Unit tests and validation cases.
* `requirements.txt`: Python dependencies.

## 🛠️ Installation and Setup

1. **Clone the repository:**
   ```bash
   git clone https://github.com/Mariuca509/dsat-link-budget-app.git
   cd dsat-link-budget-app
2. **Install dependencies:**
   It is recommended to use a virtual environment.
   ```bash
   pip install -r requirements.txt
3. **Run the application:**
   ```bash
   streamlit run app.py

## 📖 Short User Guide
Launch the app using the command above.

Use the sidebar sliders to adjust key parameters (e.g., transmit power, frequencies, data rates).

Select or input the desired TLEs for the satellite/constellation.

View the generated link budget margins and coverage statistics over Romania directly in the dashboard.
