---

# SUBFTP - TOOL

SUBFTP - TOOL is a command-line utility for performing FTP brute force attacks on a list of IP addresses. It supports multi-threaded execution and allows you to specify a custom wordlist for username and password combinations. This tool is intended for ethical hacking purposes and should only be used with explicit permission.

## Features

- **Multi-threaded execution:** Speed up the process by running multiple threads.
- **Custom wordlist support:** Specify your own list of username and password combinations.
- **Single IP or list of IPs:** Test a single IP address or a list of IP addresses.
- **Output to file:** Save results to an output file for later review.

## Banner
![Screenshot 2024-08-27 203653](https://github.com/user-attachments/assets/bcafb233-610d-46ee-9872-fc73fafd010f)



## Installation

Clone the repository:

```
git clone https://github.com/subchat/SUBFTP.git
cd SUBFTP
```

Make sure you have Python 3 installed, then install any required packages (if necessary):

```
pip install -r requirements.txt
```

## Usage

### Basic Usage

```
python subftp.py -l ip_list.txt -w wordlist.txt -o output.txt -t 10
```

### Parameters

- `-l, --list`: File containing a list of IP addresses to scan.
- `-ip, --single-ip`: Single IP address to scan.
- `-w, --wordlist`: File containing username:password combinations for brute force attempts.
- `-o, --output`: Output file to save the results.
- `-t, --threads`: Number of concurrent threads (default: 10).
![Screenshot 2024-08-27 203754](https://github.com/user-attachments/assets/7de9b8ba-a5b4-4e7e-ba7d-2206994cf9bb)

  

### Example
![Screenshot 2024-08-27 205231](https://github.com/user-attachments/assets/00e9b383-d98a-4c1f-bbec-b5511bab0d13)

Brute force a single IP with a custom wordlist:

```
python subftp.py -ip 192.168.1.1 -w wordlist.txt -o output.txt -t 5
```

Brute force a list of IPs with the default anonymous login:

```
python subftp.py -l ip_list.txt -o output.txt -t 10
```

## Output

Results will be printed to the console and optionally saved to the output file specified with the `-o` parameter.

## Disclaimer

This tool is intended for educational purposes and should only be used on networks you own or have explicit permission to test. Unauthorized use of this tool is illegal and unethical. The author is not responsible for any misuse or damage caused by this tool.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for more details.

---
