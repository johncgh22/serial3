# serial3_robot
# Brazo Serial 3 GDL -- Version 1.0

Repositorio de control y manejo de un Manipulador Serial de 3 GDL
Incluye sus definiciones del modelo en archivos URDF

## Controladores
Se puede controlar mediante el uso de **JointTrajectoryController** y **JointPositionController**

## Archivos de Iniciacion (.launch)
Contiene archivos base de lanzamiento mediante RViz y/o Gazebo. En el caso de RViz, se adjunta una preconfiguracion dentro del archivo config.rviz

## Archivos de Configuracion (.yaml)
Contiene las definiciones para controladores de posicion y de trajectoria. 

## Archivos de Definicion del Robot (.urdf)
Contiene las exportaciones del modelo CAD del robot, asi como su representacion visual y de colision de cada elemento del Manipulador.
