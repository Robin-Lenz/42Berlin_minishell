# minishell

This project focuses on developing a basic shell, much alike a personalized version of bash. It made me learn a lot about processes and file descriptors.


# usage

Compile the project

	make

Run the programm

	./mupfel

# Features
<ul>
	<li> 
	    Displays a prompt when waiting for a new command.
	</li>
	<li>
	    Supports command history.
	</li>
	<li>
	    Searches and launches the right executable based on the PATH variable or using a relative or absolute path.
     	</li>
	<li>
	    Uses a single global variable to set the right errorcode for ctrl-C.
     	</li>
	<li> 
	    Does not interpret unclosed quotes or unnecessary special characters such as \ or ;.
     	</li>
	<li> 
	    Handles single quotes (') to prevent interpreting meta-characters in the quoted sequence.
     	</li>
	<li> 
	    Handles double quotes (") to prevent interpreting meta-characters in the quoted sequence except for '$'.
     	</li>
	<li> 
	    Implements redirections (<, >, <<, >>).
	</li>
	<li>
	    Implements pipes (|) to connect the output of one command to the input of the next.
	</li>
	<li>
	    Handles environment variables ('$') to expand to their values.
	</li>
	<li> 
	    Handles $? to expand to the exit status of the most recently executed foreground pipeline.
	</li>
	<li> 
	    Handles ctrl-C, ctrl-D, and ctrl-\ as in bash.
	</li>
	<li> 
	    These built-in commands are handeled by the shell itself: echo, cd, pwd, export, unset, env, exit.
	</li>
</ul>

