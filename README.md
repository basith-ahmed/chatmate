# ChatMate

ChatMate is a local network-based chat application where users can create and join chat groups with a passkey. The program allows multiple users to connect within the same local network, chat in real-time, and assigns each user a unique color for their messages.

## Features

- **Group Creation**: Create a chat group with a name and passkey.
- **Join Group**: Join an existing group using the group name and passkey.
- **User Identification**: Each user enters a username when joining, which is displayed with their messages.
- **Colored Messages**: Each user gets a unique color in the chat for easy identification.
- **Local Network Chat**: Communicate with users on the same local network.

## How It Works

- **Server Mode**: The user who creates the group acts as the server, and others connect to them.
- **Client Mode**: Other users on the network join the chat by providing the group name, passkey, and server IP.

## Installation

### Prerequisites

- Python 3.x
- Required libraries:
  - `termcolor`
  - `pyfiglet`
  
Install the required packages using:

```bash
pip install -r requirements.txt
```

## Usage

1. **Clone the Repository**:

```bash
git clone https://github.com/MuhammadRamzy/ChatMate.git
cd ChatMate
```

2. **Run the Program**:

```bash
python chatmate.py
```

### Creating a Group

- Select option `1` when prompted.
- Provide a **group name** and **passkey**.
- Share your **IP address**, **group name**, and **passkey** with other users on the local network.

### Joining a Group

- Select option `2` when prompted.
- Enter the **group creator’s IP address**, the **group name**, and the **passkey**.
- Provide your **username**, which will be displayed in the chat.

## Example

### Creating a Group

```bash
[*] Your local IP address is 192.168.1.100
Do you want to (1) create a group or (2) join a group? [1/2]: 1
Enter a group name: devchat
Set a passkey for the group: secret123
[*] Group 'devchat' created. Waiting for members to join...
Enter your name to join the chat: Alice
```

### Joining a Group

```bash
[*] Your local IP address is 192.168.1.105
Do you want to (1) create a group or (2) join a group? [1/2]: 2
Enter the group creator's IP address: 192.168.1.100
Enter the group name: devchat
Enter the passkey: secret123
Enter your name to join the chat: Bob
[+] Joined group 'devchat' on 192.168.1.100
```

### Chat Example

```
Alice: Hello, everyone!
Bob: Hi Alice! How’s it going?
```

## Exiting the Chat

Type `exit` to leave the chat and disconnect from the group.

## Platform Compatibility

ChatMate is cross-platform and works on:

- **Windows**
- **Linux**
- **macOS**

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for more details.

## Contributing

Feel free to submit issues or pull requests. Contributions are welcome!

## Author

- **Muhammad Ramzy** - [GitHub](https://github.com/MuhammadRamzy)
