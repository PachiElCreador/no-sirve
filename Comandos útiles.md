# Registro de Recursos y Comandos Útiles

Este documento contiene comandos, configuraciones y notas relevantes organizadas por temas.

---

## 📁 Accesos y Configuración

### Abrir archivo donde se guarda el perro mapa
```bash
sudo nautilus /opt/ros/humble/share/turtlebot3_navigation2/map
```

### Editar bringup_launch.py
```bash
gedit /home/oscar/robot_ws/src/turtlebot3_multi_robot/launch/nav2_bringup/bringup_launch.py
```

---

## 🚀 Simulación

## Comandos para abrir simulación multi robot house
```bash
cd robot_ws/
colcon build --symlink-install
source ./install/setup.bash
ros2 launch turtlebot3_multi_robot gazebo_multi_robot_house.launch.py #enable_drive:=True enable_rviz:=False

```
#### Teleoperation mode
```bash
ros2 run turtlebot3_teleop teleop_keyboard --ros-args -r /cmd_vel:=/tb1/cmd_vel
```
```bash
ros2 run turtlebot3_teleop teleop_keyboard --ros-args -r /cmd_vel:=/tb2/cmd_vel
```

#### Start slam for tb1 and tb2
```bash
ros2 launch slam_toolbox online_sync_launch.py namespace:=/tb1 use_sim_time:=true
```
```bash
ros2 launch slam_toolbox online_sync_launch.py namespace:=/tb1 use_sim_time:=true
```
## Comandos para abrir simulación ejemplo Robotis 
```bash
cd ~/turtlebot3_ws
colcon build --symlink-install
```
```bash
ros2 launch turtlebot3_gazebo turtlebot3_house.launch.py
```
```bash
ros2 launch turtlebot3_cartographer cartographer.launch.py use_sim_time:=True
```

Run teleoperation mode:
```bash
ros2 run turtlebot3_teleop teleop_keyboard
```

Save map
```bash
ros2 run nav2_map_server map_saver_cli -f ~/map
```

---

### Cerrar procesos residuales
```bash
pkill -f gazebo
pkill -f rviz
pkill -f ros2
```
### Cerrar procesos residuales
```bash
ps aux | grep gazebo
ps aux | grep ros2
ps aux | grep rviz
```

Lista los nodos activos:
```bash
ros2 node list
```
Verifica los temas disponibles:
```bash
ros2 topic list
```


## 🛠️ Configuraciones Adicionales
### Chat GPT
Answer in chat instead

---

## Comandos útiles:

ctrl c: Terminar procesos

ctrl shift c: copiar

ctrl shift v: pegar

## 🔗 Referencias y Notas
- Enlace a documentación relacionada: [Enlace aquí](https://example.com)
- Notas importantes: [Escribe cualquier aclaración importante]


### 
```bash

```


