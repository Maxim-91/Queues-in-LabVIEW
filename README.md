# Queues in LabVIEW

This project demonstrates the use of **Queues** in LabVIEW for managing multiple states and operations in a structured and efficient way. The program includes several different queue operations, such as creating a queue, reading, writing, clearing, and deleting elements in the queue.

## States Implemented

The program uses an **enum** (enumerated type) to manage different states of the queue operations. The following states are included:

1. **Create Queue ("Створ чи")**  
   This state initializes and creates a new queue, storing a reference to it for further use.

2. **Delete Queue ("Видал")**  
   Deletes the queue that was created, freeing up any memory or resources associated with it.

3. **Clear Queue ("Очист")**  
   Empties all the elements currently in the queue.

4. **Read from Queue ("Зчит")**  
   Reads and removes an element from the queue.

5. **Write to Queue (End of Queue) ("Зап на кін")**  
   Writes an element to the end of the queue.

6. **Write to Queue (Front of Queue) ("Зап на поч")**  
   Writes an element to the front of the queue.

## Inputs and Outputs

- **Name**: The identifier for the queue being processed. It is used to manage the correct queue for different operations.
  
- **Queue In / Queue Out**: The references passed into the various queue operations. A queue is created in the initial state and passed through the system to be used in other states.
  
- **Element In / Element Out**: The data being added to or read from the queue.
  
- **Error In / Error Out**: Handles any errors that occur during queue operations, ensuring smooth and safe execution.

## Error Handling

The program uses a consistent error handling approach, with `error in` and `error out` clusters ensuring that any issues with queue management are properly managed and reported. This allows the program to terminate safely or provide meaningful feedback to the user.

## Usage

To use the program:

1. Start with the **Create Queue** state to initialize a new queue.
2. Use **Write to Queue** (either "End" or "Front") to add elements.
3. Use **Read from Queue** to retrieve elements from the queue.
4. Use **Clear Queue** if needed to empty all elements.
5. When the queue is no longer needed, use **Delete Queue** to free resources.

## Code
![image](https://github.com/user-attachments/assets/60fe502d-bf6a-4b57-8805-211c2469ae9d)
![image](https://github.com/user-attachments/assets/0d29b57b-003a-4430-a35d-d3020379489e)
![image](https://github.com/user-attachments/assets/0aeb4686-7f7b-4b2e-91e2-99cb05d7e0ab)
![image](https://github.com/user-attachments/assets/5ac32cc5-6a97-4661-95e4-d7bdbe787f86)
![image](https://github.com/user-attachments/assets/ab4b7934-9049-4e43-9137-fd21d1932255)
![image](https://github.com/user-attachments/assets/5898f855-88d5-4871-b622-88c2ff039644)

## The appearance of the running program
