# :wave: C / C ++ CSCE 489 Operating Systems Project 1: Simple Linux Shell

# This project implements a simple Unix shell that executes a limited subset of commands.

Commands available to the user are case senstive, and are the following:

"dir" - lists the files in the current directory (this shell only has one directory, the one in which it is located)

"create" - the user may create a new file.  If the file exists, the program will give an error.

"update" - format is: "update" "filename" "onewordoftext" to add to the fle"

"list" - lists the file and single word(s) of text that have been appended using the update command

"halt" - exits the shell

Additionally, there is a wait function, that should be implemented if an amperstand (&) is the last character in a string of input.  In its current form, the program appears to wait regardless of the command input.  Any construtive feedback would be welcomed.

# Note: Commands are entered without quotations.
Use of quotations may cause errors and unpredictable outcomes with the update command based on user command input parsing limitations

_________________________________________________________________________________________________
# Under the hood: 🚙☁️☁️☁️

This shell operates using an infinite while loop, with nested "if" , "else", and "else if" statements.

A simple breakdown of the program architecture is below:

While

  1. If Command 1\
      a. Then execute
      
  2. If Command 2\
      a. Then execute
     
  3. If Command 3\
      a. Then execute
     
  4. If not a command\
     a. Then print "Invalid Command"

Process IDs are printed with each command to assist with troubleshooting, and commands are limited to "create", "update", "list", "dir", and "halt" for simplicity.
 
Error handling was not implemented in a meaningful fashion, but the shell relies upon the basic logic that if a valid command is not entered, no action will result.  This simplicity in and of itself can be conssidered a form of error handling.

There are some limitations and potential bugs in this shell, largely due to the author's inexperience with programming in C (or any language really.) Processes seem to spawn without a logical order, and exit conditions may or may not be intact.  Finally, as discussed above, a "wait" function is present where the program looks an amperstand, but it is unclear if that function has been implemented correctly.

See comments in the program for additional information.

The author utilized various templates, guides, youtube videos, and coding assistant platforms to produce this shell.  Comments are used extensively in the file to acknowledge sources and references, but is by no means all inclusive.

If you have any questions, comments, or concerns, please feel free to reach out at anytime to reidlearnstocode@github.com
