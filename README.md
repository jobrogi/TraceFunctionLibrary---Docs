# Trace Function Library

A streamlined plugin offering a complete set of Blueprint-callable trace and sweep functions tailored for FPS, third-person, and RTS games in Unreal Engine 5.4+. This library removes boilerplate tracing logic and adds debug-friendly, flexible alternatives to standard line, sweep, and visibility checks.

---

## 🔧 Installation

1. Purchase or download the plugin from the Fab Marketplace.
2. Open your Unreal project and go to `Edit > Plugins`.
3. Locate the **Trace Function Library** and enable it.
4. Restart the editor to finalize activation.


---

## 🚀 How To Use

Using the Trace Function Library is simple and modular. All functions are **Blueprint-callable** and grouped under the category:

> **Trace Function Library**

### ✅ Quick Start (Blueprint)

1. Open any Blueprint (e.g., a character, controller, or utility BP).
2. Right-click in the graph and search for any trace function.
3. Look under the **Trace Function Library** category in the context menu.

![image](https://github.com/user-attachments/assets/99a18482-0987-4541-aa11-61e54e878f8e)

5. Connect your desired input parameters (e.g., controller, trace distance, shape, etc.).
6. Toggle `bDrawDebug` to visualize the trace results during gameplay.

## 📚 Function Overview

| **Function**                    | **Description**                                                                 |
|--------------------------------|---------------------------------------------------------------------------------|
| `TraceFromCameraByType`        | Performs a line trace from the player’s perspective (FPS, third-person, or RTS).|
| `SphereTraceFromCameraByType`  | Same as above, but uses a sphere shape for broader hit detection.              |
| `LineTraceMultiFromCamera`     | Multi-hit trace from the camera’s perspective.                                 |
| `SweepFromActorShape`          | Sweeps a shape (sphere, box, or capsule) from an actor’s location.             |
| `TraceGroundBelowActor`        | Traces downward from an actor to detect ground surfaces.                        |
| `TraceCeilingAboveActor`       | Traces upward from an actor to detect ceilings or overheads.                   |
| `GetCameraTraceStartEnd`       | Calculates trace start/end points based on camera type.                         |
| `DrawDebugTraceShape`          | Visualizes shape traces at impact for debugging (sphere, box, capsule).         |
| `GetRandomGroundPointNearby`   | Finds a random surface below a point — useful for spawning or AI logic.         |
| `ConeTraceMulti`               | Performs a cone-shaped multi-trace, ideal for vision cones or area scanning.    |
| `TraceFromSocket`              | Traces from a specific socket on a skeletal mesh. Ideal for weapons or effects. |


---

## 🎮 Camera Trace Modes (Enum: `ECameraTraceType`)

* `FPS`: Trace from camera viewpoint direction.
* `ThirdPerson`: Trace from the pawn's location + rotation.
* `RTS`: Trace from deprojected mouse cursor.

---

## 🧪 Debugging

Most functions support the following debug options:

* `bDrawDebug`: Enables visual debug.
* `TraceColor` / `HitColor`: Sets line and impact point colors.
* `DebugDuration`: How long visuals persist.

---

## 📞 Support

* **Email:** [Jobrogi@gmail.com](mailto:Jobrogi@gmail.com)
* **Discord:** [Ghillie Studios Community](https://discord.gg/6xmYHNKk)

---

## 📄 License

This plugin is licensed for commercial and non-commercial use in Unreal Engine projects. Redistribution of source or compiled binaries outside the Fab Marketplace is prohibited.

---

## ✅ Version Compatibility

Tested and verified in:

* Unreal Engine 5.3
* Unreal Engine 5.4
* Unreal Engine 5.5
* Unreal Engine 5.6
