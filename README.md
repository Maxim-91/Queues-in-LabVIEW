Queues in LabVIEW
This project demonstrates the use of Queues in LabVIEW for managing multiple states and operations in a structured and efficient way. The program includes several different queue operations, such as creating a queue, reading, writing, clearing, and deleting elements in the queue.

States Implemented
The program uses an enum (enumerated type) to manage different states of the queue operations. The following states are included:

Create Queue ("Створ чи"):
This state initializes and creates a new queue, storing a reference to it for further use.

Delete Queue ("Видал"):
Deletes the queue that was created, freeing up any memory or resources associated with it.

Clear Queue ("Очист"):
Empties all the elements currently in the queue.

Read from Queue ("Зчит"):
Reads and removes an element from the queue.

Write to Queue (End of Queue) ("Зап на кін"):
Writes an element to the end of the queue.

Write to Queue (Front of Queue) ("Зап на поч"):
Writes an element to the front of the queue.

Inputs and Outputs
Name: The identifier for the queue being processed. It is used to manage the correct queue for different operations.

Queue In / Queue Out: The references passed into the various queue operations. A queue is created in the initial state and passed through the system to be used in other states.

Element In / Element Out: The data being added to or read from the queue.

Error In / Error Out: Handles any errors that occur during queue operations, ensuring smooth and safe execution.

Error Handling
The program uses a consistent error handling approach, with error in and error out clusters ensuring that any issues with queue management are properly managed and reported. This allows the program to terminate safely or provide meaningful feedback to the user.

Usage
To use the program:

Start with the Create Queue state to initialize a new queue.
Use Write to Queue (either "End" or "Front") to add elements.
Use Read from Queue to retrieve elements from the queue.
Use Clear Queue if needed to empty all elements.
When the queue is no longer needed, use Delete Queue to free resources.
