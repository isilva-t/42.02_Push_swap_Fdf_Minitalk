# Minitalk

A simple client-server program using UNIX signals for communication.

## What it does

- Server starts and displays its PID
- Client sends text to server using only SIGUSR1 and SIGUSR2 signals
- Server receives and displays the message

## How to use

```
make        # Compile both programs
./server    # Start the server, note the PID
./client [server_pid] "message"  # Send a message
```

## Implementation Details

- Uses binary encoding (SIGUSR1 = 0, SIGUSR2 = 1)
- 8 bits per character
- Server acknowledges each bit (inpired in TCP protocol on networks)
- Null byte signals end of message
