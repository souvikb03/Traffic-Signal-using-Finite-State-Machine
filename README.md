# Traffic-Signal-using-Finite-State-Machine
Design & Implementation of Two way Traffic Signal using Finite State Machine

#### pdf- 
[Mini Project Report .pdf](https://github.com/user-attachments/files/19934923/Mini.Project.Report.pdf)

 ### Objective The main objective of this and implement practical two way traffic signal using the concept of of finite State machine and design it on prointed Circuit board.
#
#

![{C8C328C9-D58E-4518-85D5-F266694D7AF4}](https://github.com/user-attachments/assets/5388064f-7b64-4529-9db5-59e9472a82c8)

#
#

<div style="display: flex; justify-content: space-around;">
  <img src="https://github.com/user-attachments/assets/669b526f-53cd-4f01-85b7-cd10b1ef6f0d" width="360" />
  <img src="https://github.com/user-attachments/assets/139a9f5d-b3dc-482a-9bc4-4f6c2b5b4c7e" width="360" />
</div>

<div style="display: flex; justify-content: space-around;">
  <img src="https://github.com/user-attachments/assets/ad77fe03-3a65-457f-8873-7ba5290bba13" width="360" />
  <img src="https://github.com/user-attachments/assets/ad77fe03-3a65-457f-8873-7ba5290bba13" width="360" />
</div>

#
#

<div style="display: flex; justify-content: space-around;">
  <img src="https://github.com/user-attachments/assets/22612810-3b28-45b4-9a27-5ec2544843c9" width="360" />
  <img src="https://github.com/user-attachments/assets/3f375c15-394d-43b5-89c5-368f4bc2e42b" width="360" />
</div>

<div style="display: flex; justify-content: space-around;">
  <img src="https://github.com/user-attachments/assets/41824637-48cd-46c4-b088-f17adaa428c1" width="360" />
  <img src="https://github.com/user-attachments/assets/13a4469f-65c7-42c9-8e72-c79d67419594" width="360" />
</div>


#
#
<div style="display: flex; justify-content: space-around;">
  <img src="https://github.com/user-attachments/assets/bc5546b1-92ad-4833-80c8-c526d7dc1246" width="360" />
  <img src="https://github.com/user-attachments/assets/c7865a31-b358-4e16-9065-12b4cc0ed987" width="360" />
</div>




#
 
### Literature Survey

Traffic control systems have evolved significantly over the years, transitioning from simple mechanical timers to intelligent, automated systems based on microcontrollers and digital logic design. In particular, the application of Finite State Machines (FSM) in traffic control has gained prominence due to their ability to model sequential operations efficiently.

FSMs are mathematical models of computation that transition between a finite number of states based on input conditions and predefined logic. In traffic signal control, FSMs allow for systematic switching between various traffic light states (such as Green, Yellow, and Red) based on timing sequences or sensor inputs.

Several research works have demonstrated the effectiveness of FSMs in traffic management. For example, traditional timer-based circuits were found to be less adaptive and harder to maintain compared to FSM-based designs, which offer modularity, scalability, and ease of implementation. Furthermore, FSMs can be efficiently implemented using hardware description languages (HDL) on FPGAs, or directly with digital logic circuits for simpler models like two-way intersections.

Regarding the hardware realization, Printed Circuit Boards (PCBs) provide an organized and durable platform for embedding traffic control circuitry. PCBs not only improve the reliability of the system but also make the design compact and manufacturable at scale.

Prior studies have highlighted the importance of integrating simple traffic control logic with PCB design for educational purposes, urban planning models, and cost-effective traffic management solutions in less congested areas. Many designs incorporate microcontrollers (like Arduino or PIC), but this project focuses on discrete digital logic using FSM principles to deepen understanding of fundamental electronic and logic circuit concepts.


#
### Traffic Light System

A Traffic Light System is an essential part of modern transportation infrastructure, designed to manage vehicle and pedestrian flow at road intersections, pedestrian crossings, and other locations. By using a sequence of colored lights — typically Red, Yellow (Amber), and Green — the system ensures the safe and orderly movement of traffic, reducing accidents and congestion.

The standard meaning of the lights is:

Red Light: Stop

Yellow Light: Caution; prepare to stop

Green Light: Go

Basic Operation:
The traffic light operates based on a fixed or dynamic timing mechanism, switching between different states (Green, Yellow, Red) in a specific sequence. For a simple two-way intersection, the system must ensure that while one direction has a green light, the perpendicular direction has a red light, preventing collisions.

Control Techniques:

Timer-Based Systems: Use a fixed time for each light regardless of actual traffic conditions.

Sensor-Based Systems: Use road sensors (like pressure pads or cameras) to adapt the signal timings based on traffic flow.

Finite State Machine (FSM) Systems: Use a set of defined states and transitions to control the light sequence logically.

Components of a Basic Traffic Light System:

Timers or Clock Circuits

Logic Circuits or Microcontrollers

LEDs or Bulbs for Lights

Power Supply

Printed Circuit Board (PCB) for assembly

Modern traffic systems can also integrate smart technologies like vehicle-to-infrastructure communication, adaptive signal control, and emergency vehicle preemption to improve efficiency.
#
### Finite State Machine 

A Finite State Machine (FSM) is a computational model used to design systems that can be in exactly one of a finite number of states at any given time. FSMs are widely used in engineering and computer science for modeling sequential logic, control systems, and decision-making processes.

Key Concepts:

State: A condition or situation during the life of an object when it satisfies some condition, performs some activity, or waits for an event.

Transition: The movement from one state to another, triggered by an event or condition.

Input: External factors or events that cause state transitions.

Output: The system's behavior or action resulting from a specific state or transition.

An FSM can be formally defined by:

A finite set of states

A finite set of inputs

A finite set of outputs (for Mealy and Moore machines)

A transition function that maps state-input pairs to next states

(For some types) an output function

Types of FSMs:

Moore Machine: Outputs depend only on the current state.

Mealy Machine: Outputs depend on both the current state and the current inputs.

FSM in Traffic Light Systems:
In a traffic light controller, each light phase (e.g., North-South Green, East-West Red, etc.) can be considered a "state." The system transitions between these states based on a timer or sensor input, following a logical sequence to manage traffic safely.

Advantages of using FSM:

Easy to design and understand for sequential operations

Provides clear visualization and management of system behavior

Suitable for both hardware (digital circuits) and software (programming logic)
#
![{99C03F57-9389-4800-8422-C05D420C3F17}](https://github.com/user-attachments/assets/74690a47-2e19-43ef-9dc1-ca35acbadb7a)

#
### FSMs ca be classified into 2 main types- I) Moore state machine, II) Mealy state machine
### Moore state machine- 
A Moore State Machine is a type of Finite State Machine (FSM) where the outputs depend only on the current state, not on the inputs.
This means that whenever the system is in a particular state, the output is fixed and determined solely by that state.

Key Characteristics:

Output changes only when the state changes.

Output is not directly influenced by the input — only the transitions between states are.

Generally simpler and more stable outputs compared to Mealy machines, especially in hardware design.

Formal Components:

States (S): A finite set of states.

Inputs (I): A set of possible external inputs.

Outputs (O): A set of outputs, each linked to a state.

State Transition Function (δ): Defines the next state based on current state and input.

Output Function (λ): Defines the output based only on the current state.

Moore Machine Diagram:
In diagrams, each state is usually drawn as a circle with the output labeled inside. Arrows between states show transitions based on input conditions.

Application in Traffic Lights:
In a two-way traffic light system:

Each state can represent a specific traffic signal combination (e.g., "North-South Green, East-West Red").

The output (light color) is determined only by the current state.

A timer or sensor triggers transitions between states.

Advantages in Traffic Light Control:

Predictable Outputs: Light changes are smooth and based only on stable state transitions.

Simpler Design: Easier to implement on a PCB using basic logic circuits.

No Glitching: Outputs do not change unexpectedly due to input noise or glitches.

<img src="https://github.com/user-attachments/assets/608127f9-e5b7-4179-87dc-2122490a7245" width="400"/>


  #
  ### Mealy state machine
  A Mealy State Machine is a type of Finite State Machine (FSM) where the outputs depend on both the current state and the current inputs.
This means that the output can change immediately in response to an input, even without changing the state.

Key Characteristics:

Output is a function of state and input.

Outputs can change between states if the input changes.

Generally faster in response to input changes compared to Moore machines.

Formal Components:

States (S): A finite set of states.

Inputs (I): A set of possible external inputs.

Outputs (O): A set of outputs.

State Transition Function (δ): Defines the next state based on current state and input.

Output Function (λ): Defines the output based on current state and current input.

Mealy Machine Diagram:
In diagrams, transitions (arrows) are labeled with both the input and the output (often in the format "input/output").

Application in Traffic Lights:
While less common for simple fixed-time traffic signals, Mealy machines are useful when:

Sensors are used (like vehicle detectors at intersections).

Immediate responses are needed (e.g., extending the green light if traffic is still flowing).

Example: If no vehicles are detected on one side, the machine can immediately change to another state without waiting for a full timer cycle.

Advantages in Traffic Light Control:

Faster reaction to changes in traffic conditions.

More flexible logic design.

Efficient when handling sensor-based or dynamic traffic control.



<img src="https://github.com/user-attachments/assets/d02a224b-004f-4f03-86b0-1a5f93ac5465" width="400"/>

  #
  ### Methodology
  The design and implementation of the two-way traffic signal system using a Finite State Machine (FSM) were carried out through the following steps:
  ##### 01 State-level design 
  ##### 02 State Diagram Design
  ##### 03 Truth Table Implementation
  ##### 04 State Table Implementation 
  ##### 05 Logic Design Using Kmap
  ##### 06 Timer Calculations 
  ##### 07 Circuit Diagram 
  #
  #
  # 01 State-level design



The state-level design defines how the traffic signal system transitions between different operational phases based on a finite set of states and conditions. A **Moore model** was used, where outputs (traffic lights) depend only on the current state.

###  Definition of States
Each state represents a specific configuration of traffic lights for the two directions (North-South and East-West).  
The system consists of **four main states**:

| State | North-South Lights | East-West Lights | Description |
|:---|:---|:---|:---|
| S0 | Green | Red | North-South vehicles move, East-West stop |
| S1 | Yellow | Red | North-South prepare to stop, East-West still stop |
| S2 | Red | Green | East-West vehicles move, North-South stop |
| S3 | Red | Yellow | East-West prepare to stop, North-South still stop |



For implementation, each state is assigned a unique binary code:

| State | Encoding (Q1 Q0) |
|:---|:---|
| S0 | 00 |
| S1 | 01 |
| S2 | 10 |
| S3 | 11 |
  
  

  <img src="https://github.com/user-attachments/assets/6ecd8317-3850-4392-9602-fb0c8de61cf1" width="400"/>

  #

  # 02 State Diagram Design



The **State Diagram Design** represents the logical flow of the traffic signal system and shows how the system transitions from one state to another. Using the **Moore state machine** model, each state corresponds to a specific configuration of the traffic lights, and the transitions between the states are driven by time-based conditions.

## State Diagram

The system is designed to cycle through four states that represent different traffic light phases:

1. **State 0 (S0)**: North-South Green, East-West Red
2. **State 1 (S1)**: North-South Yellow, East-West Red
3. **State 2 (S2)**: North-South Red, East-West Green
4. **State 3 (S3)**: North-South Red, East-West Yellow

### Diagram:

   +-------+     Timer     +-------+     Timer     +-------+     Timer     +-------+
   |   S0  | ------------> |   S1  | ------------> |   S2  | ------------> |   S3  |
   +-------+               +-------+               +-------+               +-------+
      ^                                                                                  |
      |                                                                                  |
      +----------------------------------------------------------------------------------+
                              (Timer Expired)



- **S0**: North-South is Green, East-West is Red.
- **S1**: North-South is Yellow, East-West is Red.
- **S2**: North-South is Red, East-West is Green.
- **S3**: North-South is Red, East-West is Yellow.

### Explanation:
- The system transitions from one state to the next after a fixed time interval (timer-based control).
- The sequence repeats indefinitely in the order: **S0 -> S1 -> S2 -> S3 -> S0**.
- Each state corresponds to a specific light configuration, and transitions happen on a timer, meaning the system doesn’t depend on external inputs like vehicle sensors.

### Advantages of this Design:
- **Simplicity**: The state diagram is simple and easy to implement using a timer.
- **Predictability**: The system behavior is deterministic and consistent, making it reliable for real-world traffic control.
- **Scalability**: This design can be adapted for more complex intersections or systems with additional sensors or logic if needed.




  <img src="https://github.com/user-attachments/assets/9adf16d1-3075-41d4-81b7-9bb7e652f480" width="400"/>

#
# 

# 03 Truth Table Implementation



The **Truth Table** describes the logic of the traffic light system based on the current state (encoded as binary) and the next state after a timer expires. The system operates as a **Moore State Machine**, where the output depends only on the current state.

### 1. State Encoding

Each state is assigned a unique binary code for easier representation in the truth table:

| State | Binary Encoding (Q1 Q0) |
|:-----|:------------------------|
| S0   | 00                       |
| S1   | 01                       |
| S2   | 10                       |
| S3   | 11                       |

### 2. State Transition Table

The **State Transition Table** outlines the current state, the next state after the timer expires, and the output for each state. The **outputs** represent the traffic lights for the North-South (NS) and East-West (EW) directions.

| Present State (Q1 Q0) | Next State (Q1+ Q0+) | NS Light | EW Light |
|:---------------------|:---------------------|:--------|:--------|
| 00 (S0)              | 01 (S1)              | Green   | Red     |
| 01 (S1)              | 10 (S2)              | Yellow  | Red     |
| 10 (S2)              | 11 (S3)              | Red     | Green   |
| 11 (S3)              | 00 (S0)              | Red     | Yellow  |

### Explanation:
- **Present State**: The current state of the system represented by two binary digits (Q1 and Q0).
- **Next State**: The state the system transitions to after the timer expires. This is determined by the present state.
- **NS Light**: The state of the North-South traffic light (Green, Yellow, Red).
- **EW Light**: The state of the East-West traffic light (Green, Yellow, Red).

### Output Logic

The output logic is directly related to the current state:
- **S0 (00)**: North-South is Green, East-West is Red.
- **S1 (01)**: North-South is Yellow, East-West is Red.
- **S2 (10)**: North-South is Red, East-West is Green.
- **S3 (11)**: North-South is Red, East-West is Yellow.

This design ensures that traffic flows in one direction at a time and prevents collisions at the intersection.

### Boolean Equations for State Transitions

From the truth table, we can derive the **Boolean equations** for the state transitions:

- **Next State Logic**:
    - Q1+ = (Q1 AND NOT Q0) OR (NOT Q1 AND Q0)
    - Q0+ = NOT Q0
    
These equations determine the next state based on the current state.

### Output Logic

The output logic for the traffic lights is directly derived from the present state:
- NS Light = (NOT Q1 AND NOT Q0) OR (Q1 AND Q0)
- EW Light = (Q1 AND NOT Q0) OR (Q0 AND Q1)
### Explanation:
State Encoding: This section maps each state to a binary code for easy representation.

State Transition Table: This summarizes the transitions and outputs for each state.

Output Logic: Defines the logic for how each output (traffic light) behaves based on the current state.

Boolean Equations: Derives the Boolean logic required for the state transitions and outputs.




  <img src="https://github.com/user-attachments/assets/ea2789f0-dbe0-4f27-b893-cd4c2e20d04c" width="400"/>

#
#
# 04 State Table Implementation 



  <img src="https://github.com/user-attachments/assets/45a8f5d1-3615-49d3-bdc4-dfdf1ac32786" width="400"/>

#
# 05 Logic Design Using K-map



In the **Logic Design Using K-map** section, the Boolean equations for the next state logic and the output logic are simplified using **Karnaugh Maps (K-map)**. This helps in minimizing the logic required for the state machine implementation, ensuring the design is efficient and practical for hardware implementation.

## 1. K-map for Next State Logic

### Given Boolean Equations for Next State:
- **Q1+** = (Q1 AND NOT Q0) OR (NOT Q1 AND Q0)
- **Q0+** = NOT Q0

### K-map for Q1+ (Next state for Q1):
We create a K-map to simplify the Boolean expression for **Q1+**:

| Q1 Q0 | 00 | 01 | 11 | 10 |
|:-----:|:--:|:--:|:--:|:--:|
| **Q1+** | 0  | 1  | 1  | 0  |

- Group the ones in pairs or a single block: We have a pair of 1s at (01) and (11), which simplifies to: **Q1+ = Q0**
- The simplified Boolean equation for Q1+ is:  
  **Q1+ = Q0**

### K-map for Q0+ (Next state for Q0):
For **Q0+**, the Boolean expression is simply:  
- **Q0+ = NOT Q0**

Thus, the simplified Boolean equations for the next state logic are:
- **Q1+ = Q0**
- **Q0+ = NOT Q0**

## 2. K-map for Output Logic

### Given Output Equations:
The output for the traffic lights is determined based on the current state (Q1, Q0). Since the outputs are a function of the state, we will create K-maps for the **NS Light** and **EW Light**.

### K-map for NS Light (North-South Light):
The NS Light is set to:
- **Green** (1) when state = S0 (00)
- **Yellow** (1) when state = S1 (01)
- **Red** (0) when state = S2 (10) and S3 (11)

| Q1 Q0 | 00 | 01 | 11 | 10 |
|:-----:|:--:|:--:|:--:|:--:|
| **NS Light** | 1  | 1  | 0  | 0  |

- The simplified Boolean expression for NS Light is:  
  **NS Light = NOT Q1**

### K-map for EW Light (East-West Light):
The EW Light is set to:
- **Green** (1) when state = S2 (10)
- **Yellow** (1) when state = S3 (11)
- **Red** (0) when state = S0 (00) and S1 (01)

| Q1 Q0 | 00 | 01 | 11 | 10 |
|:-----:|:--:|:--:|:--:|:--:|
| **EW Light** | 0  | 0  | 1  | 1  |

- The simplified Boolean expression for EW Light is:  
  **EW Light = Q1**

## 3. Final Simplified Logic Equations

After simplifying the Boolean expressions using the K-map, we arrive at the following equations for the state transitions and outputs:

### Next State Logic:
- **Q1+ = Q0**
- **Q0+ = NOT Q0**

### Output Logic:
- **NS Light = NOT Q1**
- **EW Light = Q1**

These simplified logic equations will be used in the hardware implementation of the FSM for the traffic light system.
### Explanation:
K-map for Next State Logic:

We use K-maps to simplify the Boolean equations for the next state logic.

The K-map for Q1+ simplifies to Q1+ = Q0, and the K-map for Q0+ simplifies to Q0+ = NOT Q0.

K-map for Output Logic:

The K-maps for the NS Light and EW Light outputs are used to derive simplified Boolean equations.

The simplified output equations are:

NS Light = NOT Q1

EW Light = Q1

### Simplified Logic:

The simplified logic equations make the hardware implementation of the traffic signal FSM more efficient and easier to design.




  <img src="https://github.com/user-attachments/assets/21d32e03-b8cc-4dd3-b838-09e051c672e4" width="400"/>

#
#
# 06 Timer Calculations



<div style="display: flex; justify-content: space-around;">
  <img src="https://github.com/user-attachments/assets/2a779fbb-e40d-4a10-9c31-a3ec16a1c02a" width="365" />
  <img src="https://github.com/user-attachments/assets/d26be3b7-2cf4-4489-aba8-23c61f964cd4" width="400" />
</div>


<img src="https://github.com/user-attachments/assets/1f1daceb-6ad1-45c8-9e5d-f5555a2a481f" width="400"/>


# 07 Circuit Diagram 


<img src="https://github.com/user-attachments/assets/b38be5b8-1d27-465e-a5bb-e9d69d95b79d" width="400"/>









  
