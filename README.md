# Video Streaming Pipeline for NVIDIA Jetson AGX Orin
This code repository is a video streaming pipeline using NVIDIA Jetson AGX Orin as the client. The client sends all images from a given directory to the server, which can be a laptop. The pipeline records latency, network bandwidth, and energy consumption while for each image sent.

## client_agx.py
- run by the NVIDIA Jetson AGX Orin
- HOST: hostname where it sends images to
- PORT: port number where it sends images to
- SEND_DIRECTORY: path to the image folder from which it sends images
- LOG_FILE: path to the log file which it records sending timestamps, network bandwidth, and energy consumption

## server_laptop.py
- run by any machine, e.g., a laptop
- HOST: IP address of the server
- PORT: port number from where it receives images
- RECEIVE_DIRECTORY: path to the image folder to which it saves images
- LOG_FILE: path to the log file which it records receiving timestamps