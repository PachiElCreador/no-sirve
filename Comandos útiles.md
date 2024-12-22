# Registro de Recursos y Comandos Útiles

Este documento contiene comandos, configuraciones y notas relevantes organizadas por temas.

---

## 📁 Accesos y Configuración

### Abrir archivos de instalación del TurtleBot3
sudo nautilus /home/oscar/turtlebot3_ws/install

---

## 🚀 Simulación

### Comandos para abrir simulación
cd robot_ws/
colcon build --symlink-install
source ./install/setup.bash
ros2 launch turtlebot3_multi_robot gazebo_multi_robot_house.launch.py enable_drive:=True

---

## 🛠️ Configuraciones Adicionales
### [Título del Tema]
(Especifica cualquier detalle adicional que sea útil aquí)

---

## 🔗 Referencias y Notas
- Enlace a documentación relacionada: [Enlace aquí](https://example.com)
- Notas importantes: [Escribe cualquier aclaración importante]
