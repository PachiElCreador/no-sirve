# Registro de Recursos y Comandos Útiles

Este documento contiene comandos, configuraciones y notas relevantes organizadas por temas.

---

## 📁 Accesos y Configuración

### Abrir archivos de instalación del TurtleBot3
```bash
sudo nautilus /home/oscar/turtlebot3_ws/install
```

### Editar bringup_launch.py
```bash
gedit /home/oscar/robot_ws/src/turtlebot3_multi_robot/launch/nav2_bringup/bringup_launch.py
```

---

## 🚀 Simulación

### Comandos para abrir simulación multi robot house
```bash
cd robot_ws/
colcon build --symlink-install
source ./install/setup.bash
ros2 launch turtlebot3_multi_robot gazebo_multi_robot_house.launch.py enable_drive:=True
```

### Comandos para abrir simulación ejemplo Robotis 
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

## 🔗 Referencias y Notas
- Enlace a documentación relacionada: [Enlace aquí](https://example.com)
- Notas importantes: [Escribe cualquier aclaración importante]


