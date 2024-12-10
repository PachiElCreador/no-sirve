# An Adaptable Approach to Multi-Robot Navigation in ROS2

Sistema de navegación y mapeo colaborativo para múltiples TurtleBots en un entorno ROS2 y Gazebo.

## Descripción
Este proyecto implementa un sistema multi-SLAM para coordinar varios robots TurtleBot3 en un entorno simulado. Utiliza algoritmos de SLAM (Simultaneous Localization and Mapping) para fusionar mapas generados por cada robot y crear una representación global del entorno. 

Está desarrollado en ROS2 y simulado en Gazebo.

## Documentación basada en
Parte de este proyecto utiliza como referencia el artículo 
["A Guide to Multi-Robot Navigation Utilizing TurtleBot3 and Nav2"](https://medium.com/@arshad.mehmood/a-guide-to-multi-robot-navigation-utilizing-turtlebot3-and-nav2-cd24f96d19c6) 
escrito por Arshad Mehmood.

Se han adaptado algunos pasos y configuraciones para satisfacer los requisitos de este proyecto, incluyendo:
- Instalación de dependencias específicas.
- Configuración de los nodos de Nav2.
- Uso de `tf` y mapas compartidos para la navegación multi-robot.

Se recomienda revisar el artículo original para más detalles o enfoques alternativos.


## Instalación
1. Instala 
```bash
mkdir -p robot_ws/src
cd robot_ws/src

git clone https://github.com/arshadlab/turtlebot3_multi_robot.git -b master

cd robot_ws
source /opt/ros/humble/setup.bash
rosdep install --from-paths src -r -y
```

## Ejecución
1. Ejecuta comandos para abrir simulación
```bash
cd robot_ws/
colcon build --symlink-install
source ./install/setup.bash
ros2 launch turtlebot3_multi_robot gazebo_multi_robot_house.launch.py
```
## Referencias
1. ["A Guide to Multi-Robot Navigation Utilizing TurtleBot3 and Nav2"](https://medium.com/@arshad.mehmood/a-guide-to-multi-robot-navigation-utilizing-turtlebot3-and-nav2-cd24f96d19c6) por Arshad Mehmood.


