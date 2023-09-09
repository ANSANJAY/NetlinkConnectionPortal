# Use Case of Netlink Sockets 🌐

Greetings! Today, we're diving deep into understanding the practical applications and significance of **Netlink Sockets** in a computer's layered architecture.

## 🏢 Layered Architecture and Netlink Sockets

- **Layers Focused**: In our discussion, we're focusing on the **Application layer** and the **Kernel layer**. The hardware layer isn't in our scope for this topic.

## 🛰 Socket Interface in Linux

- **Definition** 📚: A collection of system calls provided by the Linux kernel, aiding in socket-based communication.
  
- **Key APIs**: `socket`, `accept`, `bind`, `send`, `receive`, `close` and so on.

- **Usage**: 
    - **Applications** in the Application layer utilize this socket interface for establishing various types of socket-based communications.

## 🌌 Types of Communications through Socket Interface

1. **Network Socket-Based Communication**: For applications communicating with remote machines on a network.
2. **Unix Domain Sockets**: To establish communication between two applications running on the same system.
3. **Netlink Sockets**: Facilitates communication with kernel subsystems residing in the kernel space.

## 💡 Netlink Sockets: A Deeper Look

- **Functionality**: It serves as a unified interface allowing applications to communicate with various kernel subsystems.

- **Kernel Subsystems**: The kernel, being a vast piece of code, is logically segregated into multiple subsystems. Some examples:
    1. **Routing Infrastructure**: Includes the entire TCP/IP stack.
    2. **Firewall or iptables**: Applications can program these via Netlink Sockets.
    3. **ARP Table**: Netlink Sockets can be employed to program it.
    4. **Network Interface Properties**: Refers to the properties of network interface cards used for transmitting and receiving network packets.

## ❓ Interview Questions on Netlink Sockets

**1. How does the layered architecture of a computer system relate to Netlink Sockets?**  
🔍 *Answer:* In the computer's layered architecture, Netlink Sockets enable the Application layer to communicate directly with kernel subsystems in the Kernel layer using a unified interface.

**2. Can you explain the main functionalities provided by the socket interface in Linux?**  
🔍 *Answer:* The socket interface in Linux offers a set of system calls that assist applications in setting up socket-based communications. These system calls include APIs like `socket`, `accept`, `bind`, `send`, `receive`, and `close`.

**3. How do Netlink Sockets differ from Unix Domain Sockets?**  
🔍 *Answer:* While Unix Domain Sockets facilitate communication between two applications on the same system, Netlink Sockets are designed for applications to communicate with kernel subsystems residing in the kernel space.

**4. Name some of the kernel subsystems an application can interact with using Netlink Sockets.**  
🔍 *Answer:* Applications can interact with several kernel subsystems using Netlink Sockets, including the routing infrastructure, the entire TCP/IP stack, firewall or iptables, ARP table, and various network interface properties.

---

All the best with your interviews! Feel free to refer back to these notes anytime. 🌟
