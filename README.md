# CS50_volume

This is my implememtation of an assignment to open, change the volume, and close a file provided by cs50.

This program modifies the volume of an audio file in the WAV format. It takes three command-line arguments: the input file name, the output file name, and a factor by which to scale the volume. It first checks if the correct number of arguments are provided, printing a usage message if not. Then it opens the input and output files and reads the scaling factor from the command line arguments.

The program then copies the header of the input file to the output file, which is 44 bytes in size for WAV files. It does this by reading the header from the input file into a buffer and then writing it to the output file.

Next, it reads the audio samples from the input file, updates their volume according to the scaling factor, and writes the updated samples to the output file. Finally, it closes both files before terminating.

The program performs two main tasks:

Copying the header from the input file to the output file.
Reading audio samples from the input file, adjusting their volume, and writing the modified samples to the output file.
