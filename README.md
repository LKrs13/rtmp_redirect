## How to run

1. Install Docker on your machine.
2. Build the Docker containers by running the command: docker-compose build.
3. Start the application using Docker Compose: docker-compose up.
4. Configure OBS:
    Launch OBS.
    Go to the settings and set the server to rtmp://localhost:1935/live and the stream key to {name}?/key=supersecret (modify it in server.js if needed).
5. Start the stream in OBS
6. Configure VLC:
    Open VLC media player.
    Go to "Open a Network Stream" option.
    Set the URL to rtmp://localhost:1935/live/{name}.
7. Verify that the stream is running smoothly.
8. Modify the streaming information in forward_stream.py as required.
9. Open your Twitch channel.
10. Run the forward_stream.py script.
11. Watch stream
