The logical architecture of the main control system is as follows:


- The Arduinos are considered actors within our management framework. They pass information to the control system via a push strategy, over a reliable protocol.

- The control system maintains a database of all records in addition to a proxy object representing the state of our Arduinos.

- The each system is separated by a facade pattern implementing the service.

- When individual Arduino systems need detailing to the user, a memento object can simply be created and sent over a network socket to the web interface system.

- When requesting attributes over a set of devices, we trigger an iterator that uses a visitor to collect state information.


Note: We would like to emphasize that the web interface is one of many potential interfaces that an operator can use. If required, the system can be trivially updated to allow information to be sent to any alternative consumer. For example, we can easily envision a command-line control applications, inline report-making, backup systems, other layers of a management system, or even AI: The genericity allows to scale!
