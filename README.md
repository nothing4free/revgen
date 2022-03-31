# revgen
revgen is a simple php reverse shell payload generator written in Python. It customizes the revshell provided by [pentestmonkey.net](https://pentestmonkey.net/tools/web-shells/php-reverse-shell), automatically setting the given IP and port.

## Usage
revgen does not require additional pip packages. To generate a reverse shell payload, use the following arguments:

```sh
python3 revgen -i <ip> -p <port> -o <file to be generated>
```
If you want to use this tool system-wide, you can move this script to /bin or a custom directory as long as it's properly included in the PATH variable:
```sh
revgen -i <ip> -p <port> -o <file to be generated>
```
Don't forget to set up a listener on the port you're using to establish the connection before launching the payload!
```sh
nc -lvvp <port>
```
