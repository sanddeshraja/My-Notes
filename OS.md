An operating system is an interface between computer user and computer hardware. It is a software which performs the basic tasks like

File management 
Memory Management
Process Management
Controlling peripheral devices such as disk drives and printers


![[OS 2022-10-26 18.24.36.excalidraw]]

## Memory Management

Memory Management refers to management of Primary Memory or Main Memory

Tracking -> Keeps track of primary memory, what parts are in use by whom, part not in use
Allocation -> Allocate memory to requesting process
Deallocation -> Deallocates memory to requesting process

## Processor Management

In multiprogramming environment, the os decides which process gets the processor when and for how much time. this function is called process scheduling

TRACKING using traffic controller, ALLOCATION, DEALLOCATION, PRIORITIZATION and QUEUE TRACK-> Keeps track of all the processes in different queues and stages

## Device management

Each device has a driver some are system supported, some are installed. Device Management manages the communication between devices and os.

TRACKING using i/o controller , ALLOCATION , DEALLOCATION, PRIORITIZATION

## File Management

file management is basically to keep the data in the most optimised format possible and also to support quick updates, access and modifications. Files are generally normally organized into directories for easy navigation and usage

TRACKING ->  keeps tracks of status, location(address), permissions,naming, etc. All of these Function together known as file System.
ALLOCATION -> Allocates file to requesting process
DEALLOCATION
PRIORITIZATION

Application is nothing but an non os packaged code, performing various i/o routines, via simultaneous processes that are ran and managed by os


## TYPES OF OS

- Batch System
- Distributed OS
- Realtime OS
- Desktop System


why many os?
-> 1. A personal computer needs os that focuses more on ui rendering, ease of use
2. A supercomputer like a server needs to focus on speed of execution and faster processing and thus have different requirements

## Batch OS

In Batch OS , the communication does not happen with the computing power or the computer directly the OS uses its intelligence to sort different types of jobs coming and group them together based on jobs which may have similiar characterstics like requirement of a similiar input or similiar resource 

## Distributed Operating System

Distributed systems use multiple central processors communicating over a network to serve multiple real-time applications and multiple user(ma be communicate through telephone lines or high speed bus)
Primary, most important task is resource sharing.

## Time Sharing Operating System

n processes from one user or multiple users now, get a fixed amout of computing time in the system known as quantum

## Network OS

School computers and cyber 
Tightly coupled systems

## Real Time Operating System

A real-time operating system is an operating system  intended to serve real-time applications that should process data as it comes in, typically without buffer delays. Processing time requirements(including OS delay) 
two types
Hard - strict - time constraint
Soft - not so strict - ex micro oven

## Hand Held OS

Unix is a general purpose, interactive time sharing os