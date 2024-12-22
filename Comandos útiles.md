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

### Comandos para abrir simulación
```bash
cd robot_ws/
colcon build --symlink-install
source ./install/setup.bash
ros2 launch turtlebot3_multi_robot gazebo_multi_robot_house.launch.py enable_drive:=True
```

---

## 🛠️ Configuraciones Adicionales
### Chat GPT
Answer in chat instead

---

## 🔗 Referencias y Notas
- Enlace a documentación relacionada: [Enlace aquí](https://example.com)
- Notas importantes: [Escribe cualquier aclaración importante]
