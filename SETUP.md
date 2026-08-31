# Setup

git clone git@github.com:Khouloud-Hamrouni/PX4_Firefighter.git ~/px4_firefighter_ws/src/PX4_Firefighter
cd ~/px4_firefighter_ws
vcs import src < src/PX4_Firefighter/px4_firefighter.repos
cd src/PX4-Autopilot && bash ./Tools/setup/ubuntu.sh && cd ../..
sudo snap install micro-xrce-dds-agent --edge
colcon build --symlink-install
EOF