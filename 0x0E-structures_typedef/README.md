Task 0: Define a Dog Structure
Define a new data type called struct dog with the following components:

name, type: char *
age, type: float
owner, type: char *
Task 1: Initialize a Dog
Write a function named init_dog that initializes a variable of type struct dog. The function should have the following prototype:

c
Copy code
void init_dog(struct dog *d, char *name, float age, char *owner);
Task 2: Print Dog Information
Write a function called print_dog that prints the information of a struct dog. The function should have the following prototype:

c
Copy code
void print_dog(struct dog *d);
The printing format should match the example below. You may use the standard library.

If any element of d is NULL, print (nil) for that element. For instance, if name is NULL, print Name: (nil).
If d itself is NULL, do not print anything.
Example Format:

makefile
Copy code
Name: Buddy
Age: 3.5
Owner: John
Task 3: Define a Typedef
Define a new type dog_t as an alias for the struct dog data type.

Task 4: Create a New Dog
Write a function named new_dog that creates a new dog_t and stores a copy of the provided name and owner. The function should have the following prototype:

c
Copy code
dog_t *new_dog(char *name, float age, char *owner);
If the function fails to create a new dog, it should return NULL.

Task 5: Free Memory for Dogs
Write a function named free_dog that frees the memory allocated for a dog_t. The function should have the following prototype:

c
Copy code
void free_dog(dog_t *d);
