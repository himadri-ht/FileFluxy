# FileFluxy

File sharing and messaging platform.

## About the project

FileFluxy is a peer-to-peer platform for file sharing and messaging. Designed for simplicity and ease of use, it enables users to share files directly, browse directories, download files, and chat seamlessly. With its streamlined interface and minimal setup requirements, FileFluxy is ideal for use on local networks, offering a seamless experience for connecting and collaborating with peers.

## Features

- **P2P Messaging**: Communicate with other users in real-time, ensuring direct and secure messaging.
- **P2P File Sharing**: Share files directly with other users in the network.
- **User Visibility**: View all users on the network, check their online status, and see when they were last active.
- **Download Files and Folders**: Download individual files or entire folders to your local system, with support for downloading complete directories.
- **Browsing**: Easily browse through the available files and directories shared over the network without needing to remember which user has the file, making it easy to find the resources you need.
- **Pause and Resume Downloads**: For convenience, you can pause and resume downloads, making large file transfers more manageable.
- **Folder Sharing**: A designated section contains the files and folders you choose to share publicly on the network. Any files stored outside this folder stay private and are inaccessible to other users.
- **Notifications**: Get notified when a file is downloaded or when you receive a new message.
  
## Technologies and Libraries used

- Python
- Qt Framework
- Sockets
- tinydb
- fuzzysearch
- msgpack
- notify-py
  
## Installation

- Clone this repository
  
```sh
git clone https://github.com/himadri-ht/FileFluxy.git
cd FileFluxy
```

- **Start the Server**: Navigate to the src directory and start the server. 
The server should be executed on a single computer within the network.

```sh
cd src
python -m server.server
```

- **Obtain the Server IP**: Once the server starts, it will display the IP address assigned to it. You’ll need this IP address when connecting new clients to the network.
- **Create Required Directories**: Set up the necessary folders for the client.
  
```sh
mkdir ~/.Fluxy/db ~/.Fluxy/logs ~/.Fluxy/tmp ~/.Fluxy/share
```

- **Start the Client**: Navigate to the src directory and run the application.
  
```sh
cd src
python -m client.app
```
