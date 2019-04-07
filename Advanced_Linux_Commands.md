# Advanced Linux Commands

## curl

cURL is a computer command-line tool for transferring data using various protocols.

* Get info about your IP address :
  ```bash
  curl https://ipapi.co/json
  ```

* Get info about numbers ! :
  ```bash
  curl http://numbersapi.com/54
  ```
  Replace 54 with some other number you like

## wget

GNU Wget is a computer program that retrieves content from web servers. Its name derives from World Wide Web and get. It supports downloading via HTTP, HTTPS, and FTP.

```bash
wget http://example.com
```

## ssh

Secure Shell (ssh) is a cryptographic network protocol for operating network services securely over an unsecured network. Typical applications include remote command-line login and remote command execution, but any network service can be secured with SSH.

Install SSH Server & SSH Client

```bash
sudo apt install openssh-server ssh
```

Find the IP address of the remote system you want to access. You can do this by going to the remote system and doing this in terminal :

```bash
ifconfig | grep "inet addr"
```

You'll see the IP address in the output :

```
inet addr:10.1.3.19
```

In the above output, `10.1.3.19` is the IP address of the system.
