# Virtual Collaborative Environment
This project creates a collaborative virtual environment using Unity 3D and Photon 2 Networking API. It allows multiple users to interact in a 3D space in real time, enabling remote collaboration on shared tasks such as building a maze. This environment supports interaction awareness, shared object manipulation, and integrated communication tools.

## Project Overview
The Virtual Collaborative Environment enables users to connect to a shared virtual space where they can interact with objects collaboratively. This project is designed to simulate real-time, remote teamwork by allowing users to observe each other’s actions and communicate within the environment.

## Features
- Multi-User Support:

    * Supports multiple users interacting within the same environment.
    * Real-time object manipulation and synchronization across clients.
- Physical Interaction with Objects:

    * Users can interact with shared objects such as cubes and cuboids to build structures.
    * Implemented mechanisms to ensure real-time synchronization of object states between all clients.
- WYSIWIS Interaction (What You See Is What I See):

    * Ensures consistent views of the environment for all participants.
    * Custom cursors to visually distinguish between users, supporting interaction awareness.

- Enhanced Collaboration Levels:

    * Level 0: Users observe actions of others.
    * Level 1: Multiple users manipulate individual objects simultaneously.
    * Level 2: Users collaborate on a single object by reducing its weight to move it together.

- User-Defined Starting Points:

    * Customizable initial spawn position for each user to prevent overlap on start.

- Join/Leave Notifications:

    * Real-time notifications for users when others join or leave the environment.

- Connected User List:

    * A dynamically updated list of currently connected users.

- Integrated Communication Tools:

    * Users can request help from others for collaborative tasks, displayed with an urgency indicator.
## Installation and Setup

- Unity and Photon Setup:

    * Install Unity and set up a new 3D project.
    * Import the required packages:
    * XR Interaction Toolkit
    * XR Plugin Management
    * Photon Unity Networking (PUN 2) for real-time network communication.
- Photon Configuration:

    * Create a Photon account at Photon Engine.
    * Obtain an Application ID and configure Photon within Unity:
        * Set up the server to enable multi-user connections.
        * Use the custom Application ID for this environment.

- Running the Project:

    * Open the Unity project and run the scene to start the collaborative environment.
    * Users can join the environment and begin interacting with objects and each other.

## Usage
- Object Manipulation:

    * Use the space key to spawn a cube, and the left shift key to spawn a cuboid.
Heavy objects require two users to manipulate, achieved by one user pressing the 'P' key to assist.
- Communication:

    * Use in-environment tools to request help or view connected users.
    * User actions, like joining and leaving, are notified in real time to all users.

## Additional Information
- Development Notes
    * Synchronization Challenges:

        * To prevent desynchronization, each object is managed with Photon components to update its position, scale, and rotation consistently across all clients.
Ownership transfer mechanisms are implemented to allow multiple users to interact with the same object.
    * Interaction Awareness:

        * Interactive elements like color changes and custom cursors are added to show when users interact with objects or each other.
        Users are visually differentiated by their cursor colors chosen on the launch screen.

## Contributing

Contributions are welcome. Please follow the established coding standards, add detailed comments, and test all changes thoroughly.

## Acknowledgments
Supervisor: Thierry Duval
Developer: Mohamed Mellouky && Nihal Dakkoune.

This project was developed as part of the 2023-2024 academic year.