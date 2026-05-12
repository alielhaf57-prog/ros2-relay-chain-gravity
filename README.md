# 📡 Autonomous Relay-Chain Architecture for Communication in Strong Gravitational Fields

> **A ROS 2 Simulation Framework**
>
> Inspired by Gaia BH1 – nearest known black hole to Earth (1,560 ly)

![Status](https://img.shields.io/badge/Status-Phase%201%20%E2%80%93%20In%20Progress-00D4FF?style=flat-square)
![ROS2](https://img.shields.io/badge/ROS%202-Jazzy%20%2F%20Humble-7C3AED?style=flat-square)
![License](https://img.shields.io/badge/License-MIT-10B981?style=flat-square)

---

## 🔭 What is this?

This project simulates an **autonomous relay-probe chain** for missions in extreme gravitational fields – concretely oriented toward **Gaia BH1**, the nearest known black hole to Earth (approx. 1,560 light-years away).

**Core research question:**

> How can a relay chain with time-dilation compensation transmit signals from the ISCO zone (just outside the event horizon) to Earth in a measurable way?

---

## 🚀 Scientific Motivation

| Problem | Approach |
|---|---|
| Extreme time dilation near black holes | Schwarzschild metric as Gazebo plugin |
| Signal loss & gravitational redshift | Attenuation model on ROS 2 topics |
| Autonomous decisions without Earth contact | Behaviour Trees + RL agent |
| Relay communication beyond ISCO | Multi-agent ROS 2 architecture |

---

## 🛠️ Tech Stack

- **ROS 2** Jazzy / Humble – Multi-agent node architecture
- **Gazebo Harmonic** – 3D physics simulation
- **RViz2** – Visualization of the relay communication chain
- **Python / C++** – Node implementation & plugins
- **Stable Baselines 3** – RL agent (Phase 3)

---

## 📁 Project Structure

```
ros2-relay-chain-gravity/
├── README.md
├── docs/
│   ├── projektplan.md             # Full project plan
│   ├── paper_draft.md             # Paper draft
│   └── SETUP_DE.md                # Setup guide (German)
├── src/
│   └── relay_chain/
│       ├── probe_node.py          # Probe node (Phase 1)
│       ├── relay_node.py          # Relay communication logic
│       └── latency_model.py       # Signal propagation delay model
├── simulation/
│   └── gazebo/
│       └── schwarzschild_plugin.cpp  # Gravitational field plugin (Phase 2)
└── paper/
    └── draft.md
```

---

## ▶️ Quickstart (Phase 1)

```bash
# Create ROS 2 workspace
mkdir -p ~/ros2_ws/src
cd ~/ros2_ws/src
git clone https://github.com/alielhaf57-prog/ros2-relay-chain-gravity.git

# Build
cd ~/ros2_ws
colcon build

# Run
source install/setup.bash
ros2 run relay_chain probe_node
```

---

## 📅 Project Phases

- [x] **Phase 1** – ROS 2 foundation, 3 probe nodes, latency model *(current)*
- [ ] **Phase 2** – Schwarzschild physics in Gazebo, time dilation, thruster model
- [ ] **Phase 3** – Behaviour Trees, RL agent, paper submission (ICRA / iROS)

---

## 🎯 Target Publications

| Conference / Journal | Field |
|---|---|
| IEEE ICRA – Int. Conference on Robotics and Automation | Robotics · A* |
| iROS – Intelligent Robots and Systems | Autonomy · A |
| IEEE Aerospace Conference | Space Systems · A |
| Acta Astronautica | Journal · Q1 |

---

## 🏭 Industry Relevance

This framework addresses real challenges in the space industry – particularly for autonomous communication systems in deep-space missions:

| Organization | Relevance |
|---|---|
| **DLR** – German Aerospace Center | Space robotics, autonomous systems – ideal for internship / thesis |
| **ESA** – European Space Agency | Space Robotics Team, deep space communication |
| **Airbus Defence & Space** | Autonomous satellite communication, Germany/Europe |
| **OHB System AG** | German space company, Munich & Bremen |
| **NASA JPL** | Autonomous Systems Group, deep space relay |
| **SpaceX** | Deep space communication architecture |

---

## 👤 Author

**[Ali El-Haf]**
AI & Software Engineering Student
Interests: Space Robotics, ROS 2, Planetary Exploration & Deep Space Communication

---

## 📄 License

MIT License – free to use, attribution appreciated.
