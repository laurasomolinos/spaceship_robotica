# Práctica Spaceship ROS2

1. Copiar todas las carpetas dentro de una carpeta `spaceship` dentro de `~/ros_ws/src`.
2. Compilar desde la raíz del workspace:
   `cd ~/ros_ws && source /opt/ros/jazzy/setup.bash && colcon build && source install/setup.bash`
3. Ejecutar sin viento:
   `ros2 launch spaceship_student_laha student.launch.py target_x:=10.0 target_y:=8.0 wind_strength:=0.0 wind_frequency:=0.0 full_sim:=true`
4. Ejecutar con viento:
   `ros2 launch spaceship_student_laha student.launch.py target_x:=10.0 target_y:=8.0 wind_strength:=1.0 wind_frequency:=0.15 wind_seed:=42 full_sim:=true`
5. Ver depuración:
   `ros2 topic echo /control_debug`
