# PowerIK
This is PowerIK for Unreal 5.8
This tool is not maintained by anyone, so I fixed it and compiled it for Unreal 5.8. It might be useful for some people.

PowerIK is a full-body **Inverse Kinematics (IK)** plugin for Unreal Engine. Unlike traditional IK solvers that only affect a single limb, PowerIK solves the **entire skeleton simultaneously**, allowing characters to naturally adapt their pose when one or more body parts are constrained.

This makes it ideal for creating realistic procedural animation and dynamic interactions with the environment.

## Features

- **Full Body IK Solver**
  - Solves the entire character skeleton in real time.
  - Produces natural body movement and weight shifting.

- **Automatic Foot Placement**
  - Adapts feet to uneven terrain.
  - Automatically adjusts pelvis height.
  - Supports stairs, slopes, rocks, and rough landscapes.

- **Multiple IK Effectors**
  - Control multiple body parts at the same time.
  - Supports:
    - Hands
    - Feet
    - Head
    - Pelvis
    - Weapon grips
    - Tails and other appendages

- **Procedural Animation**
  - Runtime pose adjustment without pre-authored animations.
  - Perfect for dynamic gameplay interactions.

- **Blueprint Friendly**
  - Fully exposed Animation Blueprint nodes.
  - Easy integration into existing animation systems.

## Typical Use Cases

- Foot placement on uneven terrain
- Climbing systems
- Hand placement on walls and objects
- Two-handed weapon gripping
- VR full-body avatars
- Large creatures adapting to terrain
- Dynamic character interactions

## Why PowerIK?

Traditional Unreal IK nodes (Two Bone IK, FABRIK, CCDIK, etc.) solve **individual bone chains**. For example:

```
Shoulder → Elbow → Hand
```

PowerIK instead solves the **entire skeleton** as a single system, allowing all body parts to react naturally to the movement of any IK target.

This results in:

- More realistic body balance
- Natural weight shifting
- Better interaction with the environment
- Reduced need for handcrafted animations

## PowerIK vs Unreal Full Body IK (PBIK)

Since Unreal Engine 5, Epic provides **PBIK (Position-Based IK)** as a built-in Full Body IK solution.

| PowerIK | Unreal PBIK |
|----------|-------------|
| External plugin | Built into Unreal Engine |
| Excellent terrain adaptation | More manual setup required |
| Simple Blueprint workflow | More configurable |
| Mature gameplay-oriented features | Deep Control Rig integration |
| Great for procedural gameplay | Great for animation pipelines |
