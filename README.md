# serial3_robot
# Brazo Serial 3 GDL -- Version 1.0

Repositorio de control y manejo de un Manipulador Serial de 3 GDL
Incluye sus definiciones del modelo en archivos URDF

Compatible con **ROS Noetic en Ubuntu 20.04**

## Controladores
Se puede controlar mediante el uso de **JointTrajectoryController** y **JointPositionController**
Tambien contiene un controlador para uso con otros programas, llamado **arm_controller**

Para la correcta ejecución de estos controladores, es necesario tener instalados los siguientes paquetes:

```
sudo apt-get install ros-noetic-ros-control ros-noetic-ros-controllers
```

## Archivos de Iniciacion (.launch)
Contiene archivos base de lanzamiento mediante RViz y/o Gazebo. En el caso de RViz, se adjunta una preconfiguracion dentro del archivo config.rviz

Para la ejecución del controlador **arm_controller** se puede hacer mediante el siguiente comando:

```
roslaunch serial3_robot serial_controller.launch
```

Para la visualización en **RViz** del robot, puedes ejecutar el siguiente comando:

```
roslaunch serial3_robot mostrar.launch model:=serial3_robot.urdf gui:=true
```

## Archivos de Configuracion (.yaml)
Contiene las definiciones para controladores de posicion y de trajectoria. 

## Archivos de Definicion del Robot (.urdf)
Contiene las exportaciones del modelo CAD del robot, asi como su representacion visual y de colision de cada elemento del Manipulador.

## Enlaces
- Instalación de ROS Noetic http://wiki.ros.org/noetic/Installation/Ubuntu
