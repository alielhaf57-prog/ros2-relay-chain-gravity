  Autonomous Relay-Chain Architecture for Communication in Strong Gravitational Fields
 
This project simulates an autonomous relay-probe chain for missions in extreme gravitational fields – concretely oriented toward Gaia BH1, the nearest known black hole to Earth (approx. 1,560 light-years away).
 
Problem	Approach
Extreme time dilation near black holes	Schwarzschild metric as Gazebo plugin
Signal loss & gravitational redshift	Attenuation model on ROS 2 topics
Autonomous decisions without Earth contact	Behaviour Trees + RL agent
Relay communication beyond ISCO	Multi-agent ROS 2 architecture
 
 
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
 
# Create ROS 2 workspace mkdir -p ~/ros2_ws/src cd ~/ros2_ws/src git clone https://github.com/alielhaf57-prog/ros2-relay-chain-gravity.git
# Build cd ~/ros2_ws colcon build
# Run source install/setup.bash ros2 run relay_chain probe_node
 
Conference / Journal	Field
IEEE ICRA – Int. Conference on Robotics and Automation	Robotics · A*
iROS – Intelligent Robots and Systems	Autonomy · A
IEEE Aerospace Conference	Space Systems · A
Acta Astronautica	Journal · Q1
 
This framework addresses real challenges in the space industry – particularly for autonomous communication systems in deep-space missions:
Organization	Relevance
DLR – German Aerospace
Center	Space robotics, autonomous systems – ideal for internship / thesis
ESA – European Space
Agency	Space Robotics Team, deep space communication
Airbus Defence & Space	Autonomous satellite communication, Germany/Europe
OHB System AG	German space company, Munich & Bremen
NASA JPL	Autonomous Systems Group, deep space relay
SpaceX	Deep space communication architecture
  Author
Ali El-Haf
 AI & Software Engineering Student Interests: Space Robotics, ROS 2,
Planetary Exploration & Deep Space Communication
 
MIT License – free to use, attribution appreciated.
