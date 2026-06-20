# Shell, processes and signals

This project covers process management and Unix signals in Bash: finding PIDs, listing processes, sending and trapping signals, and managing background daemons with PID files.

## Tasks

- 0-what-is-my-pid: Displays the script's own PID using the special variable $$
- 1-list_your_processes: Displays all running processes for all users, with hierarchy, using ps auxf
- 2-show_your_bash_pid: Displays lines containing "bash" from the process list using ps and grep
- 3-show_your_bash_pid_made_easy: Displays the PID and name of processes containing "bash", reading from /proc instead of using ps
- 4-to_infinity_and_beyond: Displays "To infinity and beyond" indefinitely, using a while loop with a sleep 2 between iterations
- 5-dont_stop_me_now: Stops the 4-to_infinity_and_beyond process using kill
- 6-stop_me_if_you_can: Stops the 4-to_infinity_and_beyond process without using kill or killall, using pkill
- 7-highlander: Displays "To infinity and beyond" indefinitely and survives SIGTERM by printing "I am invincible!!!" using trap
- 67-stop_me_if_you_can: Stops the 7-highlander process by sending SIGTERM instead of SIGKILL, without using kill or killall
- 8-beheaded_process: Kills the 7-highlander process for good using pkill with SIGKILL
- 10-process_and_pid_file: Creates a PID file and runs indefinitely, handling SIGTERM, SIGINT, and SIGQUIT differently, using trap
- 11-manage_my_process / manage_my_process: An init-style script that starts, stops, and restarts a background process while  managing its PID file, using case and kill
