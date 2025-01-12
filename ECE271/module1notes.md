# Abstraction

Hiding details when they are not important.

#### Levels of Abstraction

| ##### Level          | #### Example           |
| :------              | :--------:             |
| Application          | Programs               |
| OS                   | Device drivers         |
| Architecture         | Instruction Registers  | 
| Micro Architecture   | Datapaths; controllers |
| Logic                | Adders; Memories       |
| Digital Circuits     | AND gates; NOT gates   |
| Analog circuits      | Amplifiers; filters    |
| Devices              | Transistors; diodes    |
| Physics              | Electrons              |

Microarchitecture links the logic and architecture levels of abstraction. The architecture level of abstraction describes a computer from the programmer’s perspective.

A particular architecture can be implemented by one of many different microarchitectures. For example, the Intel Core i7, the Intel 80486, and the AMD Athlon all implement the x86 architecture with different microarchitectures.

The operating system handles low level details such as accessing a hard drive or managing memory.

The application software uses these facilities provided by the operating system to solve a problem for the user.

---

# Discipline

Intentionally restricting your design choices so that you can work more productively at a higher level of abstraction.

By limiting ourselves to digital circuits, we can easily combine components into sophisticated systems that ultimately outperform those built from analog components in many applications.

---

# Heirarchy

Organizing a complex system into manageable modules or components.

Each module encapsulates specific functionalities or operations, contributing to the overall system's functionality. 

By breaking down the system into these modular and hierarchical structures, designers can easily understand and manage each component independently. This hierarchical approach facilitates efficient design, debugging, and maintenance of complex digital systems.

---

# Modularity

 Modules communicate via well-defined interfaces, enabling accurate data transmission without interference.

Modular design facilitates easy integration, testing, maintenance, and upgrades, enhancing system reliability and flexibility.

---

# Regularity

Achieving uniformity among modules, often by reusing common modules multiple times.

---

