# 📡 Real-Time Data Pipeline (Local-Only Setup)

This project builds a complete **real-time data engineering pipeline** locally using **Docker, Kafka, Spark, and MongoDB**. It's designed for beginners to learn how data flows through modern streaming systems — without using any cloud services or incurring costs.

---

## 🔧 Tools Used

- **Docker & Docker Compose** – to containerize and manage services
- **Apache Kafka** – to simulate real-time data streams
- **Apache Spark (Structured Streaming)** – to process data in real time
- **MongoDB** – to store processed data
- **Python** – for producing test data

---

## 🎯 Project Objective

- Simulate real-time sensor or event data (via Kafka Producer)
- Stream that data into Kafka topics
- Use Spark to consume Kafka data, transform it, and store results in MongoDB
- All services run locally using Docker Compose

---

## 📁 Folder Structure

real-time-data-pipeline/
├── .env # Environment variables (hostnames, ports, etc.)
├── docker-compose.yml # Orchestrates all services
├── README.md # Project documentation
└── src/
├── producer/
│ └── producer.py # Sends fake data to Kafka topic
├── spark/
│ └── spark_job.py # Spark reads from Kafka & writes to MongoDB
└── consumer/
└── consumer.py # (Optional) Reads data from Kafka for testing


---

## 🚀 How to Run (Step-by-Step)

1. **Install Prerequisites**  
   - Docker Desktop  
   - Git  
   - Python 3.x (for local scripts)

2. **Clone the Repository**

   ```bash
   git clone https://github.com/your-username/real-time-data-pipeline.git
   cd real-time-data-pipeline

3. **Start All Services**

    This sets up:

        Kafka broker & Zookeeper

        MongoDB

        Spark app

        Python producer (manual or scripted)

📌 Notes
This project runs 100% locally. No cloud credentials needed.

Good for portfolio projects and interview preparation.

You can extend it with dashboards (e.g., using Flask + Chart.js or Superset).


