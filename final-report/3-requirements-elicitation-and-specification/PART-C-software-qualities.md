Correctness: Correctness is partly enforced by pushing updates from the Arduinos using a reliable protocol. Furthermore, the web interface holds no state by default and relies upon up-to-date information provided by the control system.
 
Time-efficiency: Time efficiency is an important quality, but we are not aiming for a hard realtime system. This is due to the nature of plants. However, the user interface should not exceed two seconds to provide an up-to-date view when required by the user.
  
Robustness: Due to the straightforward nature of communication between machines in this project, white-list validation can be performed against all incoming requests. This simplicity affords a certain amount of stability for our application. Otherwise, we have alerts for the user in case the situation demands it.

User friendliness: Implemented for both the end user in the form of a pleasant web-interface and for the developer by separating responsibilities across modules that only discuss with their peered systems. Documentation will be provided at all levels. This is not only as part of our work hand-in, but as a means of attracting and retaining valuable early-stage users.
