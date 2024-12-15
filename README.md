# rafi_sim
RAFI simulation package

## Paquetes

### rafi_gazebo

Este paquete incluye los archivos de descripción, inicializacón y entornos para lanzar la simulación de la base de RAFI y del modelo completo de RAFI.

### rafi_plugin

Este paquete incluye una versión modificada del plugin `ros_force_based_move`.

## Instalación

### 1) Instalar las dependencias

Es importante instalar los paquetes y librerías de franka, disponibles en https://github.com/frankaemika/franka_ros y https://github.com/frankaemika/libfranka.

### 2) Clonar el paquete

```
git clone https://github.com/TaISLab/rafi_sim.git
```

### 3) Compilar el paquete

```
catkin build
source devel/setup.bash
```

## Uso del paquete

```
roslaunch rafi_gazebo display_base.launch
```

Este comando lanza la simulación de la base de RAFI. Se recomienda el uso del nodo de ROS `teleop_twist_keyboard` para el control de la base, disponible en https://github.com/ros-teleop/teleop_twist_keyboard.git

```
roslaunch rafi_gazebo display_v2.launch
```

Este comando lanza la simulación del modelo de cuerpo completo de RAFI.
