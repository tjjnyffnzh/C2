<h1 align="center">Krypton Botnet</h1>

<p align="center">
    <img src="https://github.com/CirqueiraDev/KryptonC2/assets/118860604/25572868-0674-4963-afc4-16a8291473e7">
</p>

<br>

 **KryptonC2** is a basic open source [denial of service](https://en.wikipedia.org/wiki/Denial-of-service_attack) [botnet](https://en.wikipedia.org/wiki/Botnet) system written in Python 3, consists of a connect and control server and a bot malware script.

<img src="https://user-images.githubusercontent.com/73097560/115834477-dbab4500-a447-11eb-908a-139a6edaec5c.gif"><br>

# Installation
1. Install Git and Python 3 on your server.
2. Clone the KryptonC2 Github repository to your server via Git: `$ git clone https://github.com/CirqueiraDev/KryptonC2`.
3. Change the host address and C&C port in the configuration section in [bot.py](src/Payload/bot.py) to your server address and C&C port.
4. Install the requirements.txt
5. Start the C2 server by executing the command: `$ python main.py`.
6. Add accounts in [logins.txt](/src/logins.txt) using the format: `username:password:yyyy-mm-dd`.
7. Configure the port on the [config.json](/src/config.json) `{
"cnc_host": "0.0.0.0",
  "reg_host": "0.0.0.0",
  "cnc_port": 5511,
  "reg_port": 5512
}`.

8. Connect to the server through [PuTTY](https://www.putty.org/) on a raw socket connection.
