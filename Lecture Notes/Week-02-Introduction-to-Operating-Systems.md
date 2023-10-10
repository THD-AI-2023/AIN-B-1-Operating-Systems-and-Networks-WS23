# Introduction to Operating Systems.

## What is an operating system?

- An operating system (OS) is a software that controls the execution of programs and provides services such as resource allocation, scheduling, input-output control, and data management.
- The OS's job is to provide user programs with a better, simpler, and cleaner interface to the computer's hardware.
- The OS also manages the hardware components, such as CPU, memory, disk, and network devices.

## How does a computer work?

- A computer is based on the Von Neuman architecture, which consists of a central processing unit (CPU), a memory unit, and input/output (I/O) devices.
- The CPU contains the arithmetic and logic unit (ALU), the control unit (CU), and various registers that store data and instructions.
- The memory unit holds the programs and data that are being executed by the CPU. It is divided into memory locations, each with a unique address and a byte of data.
- The I/O devices allow the computer to communicate with the external world, such as keyboard, mouse, display, printer, etc.

## How are programs executed?

- A program is a sequence of instructions that tell the computer what to do. Programs can be written in different languages, such as assembler or high-level languages like C or Java.
- Programs written in high-level languages need to be translated into machine language by a compiler before they can be executed by the CPU.
- The CPU executes programs by following the machine instruction cycle: fetch, decode, execute, and store. In each cycle, the CPU fetches an instruction from memory, decodes it in the CU, executes it in the ALU, and stores the result in memory or registers.

## How have operating systems evolved?

- Operating systems have evolved along with the hardware and software technologies over several generations.
- The first generation (1945 - 1955) used relays or vacuum tubes and had no operating system. Programs were wired up manually using plugboards or punch cards.
- The second generation (1955 - 1965) used transistors and introduced programming languages like assembler and FORTRAN. Programs were still submitted using punch cards or tapes. Batch processing was used to group similar programs together and reduce setup time.
- The third generation (1965 - 1980) used integrated circuits and introduced operating systems like OS/360. Programs were read from cards or tapes to a hard disk using spooling. Multiprogramming was used to run multiple programs concurrently by switching between them when one was waiting for I/O. Timesharing was used to allow multiple users to access the computer via online terminals by allocating time slices to each user.
- The fourth generation (1980 - present) used large scale integration and introduced personal computers with operating systems like DOS, Windows, Linux, and MacOS. Programs were loaded from floppy disks, CD-ROMs, or USB drives. Graphical user interfaces were developed to make the interaction more user-friendly.
- The fifth generation (1990 - present) used system on chips and introduced mobile computers with operating systems like Android and iOS. Programs were downloaded from wireless networks or app stores. Touchscreens were used as input and output devices.

## What are system calls?

- System calls are the programmatic way in which a program requests a service from the operating system's API (application programming interface).
- System calls allow programs to perform operations that require privileged access to system resources, such as starting a process, creating a file, getting the current time, reading from USB, or transferring data over a network.
- System calls are executed by switching from user mode to kernel mode using a trap instruction. The kernel decodes the system call code in a register and invokes the corresponding implementation. After the implementation finishes, the result values are stored in memory and control is returned to the user process.

## What is virtualization?

- Virtualization is the process of creating a software-based simulation of something, such as a virtual version of computer hardware, network, or an operating system.
- A software-representation of a computer is called a virtual machine (VM). The program managing and executing virtual machines is called a hypervisor. The computer running the hypervisor is called the host machine. The computer that is virtualized is called the guest machine.
- There are two types of hypervisors: type-1 and type-2. Type-1 hypervisors run directly on the hardware and manage multiple VMs. Type-2 hypervisors run on top of an existing operating system and leverage its services to manage VMs.
- Virtualization has many benefits, such as improving resource utilization, enhancing security and reliability, enabling portability and compatibility, and facilitating testing and development.