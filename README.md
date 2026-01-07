# FRC 2025 Offseason Reefscape Bot

**Status: ARCHIVED** - This was our 2025 offseason development project for the FIRST Reefscape game.

## Overview

This repository contains the complete codebase for our FRC Reefscape 2025 offseason robot. Built during the offseason to prepare for competition, this robot features advanced autonomous navigation, coral/algae manipulation, and integrated vision systems.

## Robot Capabilities

### Drivetrain
- **Swerve Drive** - Phoenix 6 based holonomic swerve drivetrain
- **PathPlanner Integration** - Autonomous path following with smooth trajectory generation
- **Advanced odometry** - Real-time robot positioning and tracking

### Subsystems
- **Coral Detection** - Limelight-based vision system for automatic coral identification and alignment
- **Elevator** - Precision vertical movement for scoring at multiple reef heights
- **Pivot Intake** - Articulated intake mechanism with coral detection
- **Dump Roller** - Actuation system for coral/algae release
- **Superstructure** - Coordinated control of multiple subsystems

### Key Features
- **State Machine Architecture** - RobotStateMachine for coordinated, sequential actions
- **Vision-Guided Alignment** - AutoAlign features for coral and reef positioning
- **Telemetry System** - Real-time robot diagnostics and performance monitoring
- **Advanced Auto Autos** - 8+ autonomous routines with dynamic path selection

## Project Structure

```
src/main/
├── java/frc/robot/
│   ├── Robot.java                    # Main robot class
│   ├── RobotContainer.java          # Input/output bindings & command config
│   ├── RobotStateMachine.java       # Master state machine
│   ├── Constants.java               # Robot hardware configuration
│   ├── Telemetry.java              # Real-time logging
│   ├── commands/                    # Command implementations
│   │   ├── AlignReef.java
│   │   ├── AlignToCoral.java
│   │   ├── IntakeCoral.java
│   │   └── ...
│   └── subsystems/                  # Subsystem implementations
│       ├── CommandSwerveDrivetrain.java
│       ├── CoralDetectionSubsystem.java
│       ├── ElevatorSubsystem.java
│       ├── PivotIntakeSubsystem.java
│       └── ...
└── deploy/
    └── pathplanner/                 # Autonomous path definitions
```

## Technologies Used

- **WPILib** - Robot framework (2025 Edition)
- **Phoenix 6** - CTRE motor controllers & swerve drive
- **REVLib** - REV motor control
- **PathPlanner** - Autonomous path generation & following
- **AdvantageKit** - Advanced telemetry & logging
- **Limelight** - Computer vision system

## Legacy Notes

This codebase was developed during the 2025 FRC offseason and served as a testbed for developing robotics concepts. The architecture and implementations documented here provide valuable reference material for future projects.

## Team Acknowledgments

Built with passion and dedication by our robotics team during the offseason. Special thanks to all members who contributed hardware, software, and testing expertise.
