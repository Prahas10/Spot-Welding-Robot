# Mipie: 6 DOF Manipulator for Robot Welding

Mipie is a 6 Degrees of Freedom (DOF) manipulator designed for robot welding tasks. This project utilizes the SerialLink() function to control Mipie and perform various welding operations such as drawing lines, squares, circles, rectangles, and spot welding.

## Algorithm

1. **Main Class:** The main class contains a switch case based on user input for choosing the desired shape or operation.
2. **Function Calls:** User inputs for coordinates are passed to their respective functions.
3. **Boundary Definition:** Boundaries for the drawing space are defined to ensure that the manipulator stays within the specified area.
4. **Translation Matrices:** Translation matrices are created for the sets of points using transl() function.
5. **Inverse Kinematics:** The inverse kinematics process is implemented using the ikine() function to determine the joint configurations needed to reach the desired end-effector position.
6. **Spot Welding Operation:** The mathematical formula (1-λ)A + λB is utilized to represent all the points between points A and B. A for loop is used to iterate through different values of λ, generating points between A and B for spot welding.
7. **Drawing/Welding Operation:** A for loop iterates through translation matrices, plotting points for the desired shape or performing spot welding.

## Conclusion

The Mipie project demonstrates the implementation of a 6 DOF manipulator for robot welding tasks. By utilizing the SerialLink() function and various mathematical operations, Mipie can accurately perform drawing and spot welding operations. This project provides a practical illustration of robotics and automation in industrial applications.

For further insights and understanding, explore the code and experiment with different shapes and welding scenarios. Happy exploring with Mipie!
