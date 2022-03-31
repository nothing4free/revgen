# revgen
revgen is a simple php reverse shell payload generator written in Python. It customizes the revshell provided by [pentestmonkey.net](https://pentestmonkey.net/tools/web-shells/php-reverse-shell), automatically setting the given IP and port.

## Usage
revgen does not require additional pip packages. To generate a reverse shell payload, use the following arguments:

```py
python3 revgen -i <ip> -p <port> -o <file to be generated>
```
Don't forget to set up a listener on the port you're using to establish the connection before launching the payload!
```sh
nc -lvvp <port>
```
