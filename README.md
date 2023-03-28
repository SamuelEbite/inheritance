# inheritance
 This program simulates the genetic inheritance of blood type across three generations using a data structure of a person who has two parents and two alleles.

The main function initializes the random number generator, creates a new family using create_family() function, prints out the family tree using print_family() function, and frees the memory using free_family() function.

The create_family() function takes an integer generations as a parameter and returns a pointer to a person struct. The function allocates memory for a new person using malloc() and recursively creates parents for the current person until the number of generations is greater than one. Then, it randomly assigns alleles based on the alleles of their parents and returns the newly created person.

The print_family() function takes a pointer to a person p and an integer generation as parameters. The function prints out each family member's blood type and their generation using indentation based on the generation number.

The free_family() function takes a pointer to a person p as a parameter and frees memory for the person and all of their ancestors recursively.

The random_allele() function generates a random number between 0 and 2 and assigns an A, B, or O blood type allele based on the random number.

To run the program, simply compile and execute the code in your preferred C compiler. The output will display the family tree of blood types for three generations.
