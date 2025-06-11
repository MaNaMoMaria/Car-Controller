# Car-Controller
A foundational C# script for realistic 3D car movement in Unity, covering acceleration, braking, and steering. Perfect for beginners and quick prototyping.
# 3D Car Movement Script (Unity)

---

This repository features a robust and easy-to-use C# script (`CarController.cs`) for implementing **realistic 3D car movement** within your Unity projects. Whether you're building a racing game, a driving simulator, or just need a solid base for vehicle physics, this script provides foundational controls for **acceleration, braking, and steering** in a 3D environment.

## Features

* **Smooth Acceleration & Braking:** Utilizes `Mathf.Lerp` for gradual speed changes, mimicking real-world vehicle behavior.
* **Intuitive Steering:** Responsive steering controls with an optional check to prevent turning when the car is stationary.
* **Physics-Based Movement:** Leverages Unity's `Rigidbody` for accurate and stable physics interactions.
* **Configurable Parameters:** Easily adjust `forwardSpeed`, `backwardSpeed`, `turnSpeed`, `brakeForce`, `acceleration`, and `deceleration` directly from the Unity Inspector to fine-tune your car's performance.

## How to Use

To integrate this script into your Unity project, follow these simple steps:

1.  **Download the Script:** Grab the `CarController.cs` file from this repository.
2.  **Add to Your Unity Project:**
    * Open your Unity project.
    * Drag and drop the `CarController.cs` file into your `Assets/Scripts` folder (or any other preferred location).
3.  **Prepare Your Car GameObject:**
    * Ensure your 3D car model has a **Rigidbody** component attached. This script heavily relies on Unity's physics engine.
    * It's generally recommended to set the `Rigidbody`'s **"Collision Detection"** to `Continuous` or `Continuous Dynamic` for better collision stability, especially at higher speeds.
    * Consider adding appropriate **colliders** (e.g., Box Colliders for the body, Wheel Colliders if you need more advanced wheel physics) to your car model.
4.  **Attach the Script:**
    * Select your car's main GameObject in the Unity Hierarchy.
    * In the Inspector panel, click "Add Component" and search for "Car Controller" (or simply drag the `CarController.cs` script onto the GameObject).
5.  **Configure Parameters (Optional but Recommended):**
    * Adjust the public variables (like `forwardSpeed`, `turnSpeed`, etc.) in the Inspector to match your car's desired feel and performance.

## Requirements

* **Unity 3D:** Developed and tested with Unity 6, but highly compatible with Unity 2019.4 LTS and newer versions due to the use of core Unity APIs.
* **Rigidbody Component:** Your car GameObject **must** have a `Rigidbody` component.
* **Input Setup:** Relies on the default "Vertical" (W/S or Up/Down arrows) and "Horizontal" (A/D or Left/Right arrows) input axes, and `KeyCode.Space` for braking.

## Contributing

Feel free to fork this repository, suggest improvements, or submit pull requests. Your contributions are welcome!

## License

This project is open-source and available under the [MIT License](LICENSE.md).
