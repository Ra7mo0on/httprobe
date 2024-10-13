# httprobe

**Effortlessly probe a list of domains for active HTTP and HTTPS servers!**

---

## 📥 Installation

To get started with `httprobe`, you can install it quickly using Go. Follow these simple steps:

### Requirements

- [Go](https://golang.org/dl/) (version 1.17 or later)

### Installation Command

Open your terminal and run the following command to install `httprobe`:

```bash
go install github.com/tomnomnom/httprobe@latest
```
## 🛠 Usage
Using httprobe is straightforward. After installation, you can pipe in a list of domains or URLs, and it will check for active HTTP/HTTPS servers.
### Basic Usage Example
```
cat domains.txt | httprobe
```
This command checks which domains from the domains.txt file respond on HTTP or HTTPS.
### Advanced Usage
You can customize the behavior of httprobe with additional flags. Here are some useful options:
- -p: Add additional ports to probe, e.g., 8080 or 8443.
- -c: Set a concurrency limit for probing.
Example:
```
cat domains.txt | httprobe -p http:8080 -c 50
```
This command probes both port 8080 and the default HTTP/HTTPS ports for the domains listed in domains.txt and uses 50 concurrent requests.
## ⚙️ Features
- Efficient: Quickly probes large domain lists.
- Flexible: Supports custom ports and concurrency levels.
- Simple: Easy to integrate into pipelines and other tools.
## 🤝 Contributing
Contributions are welcome! To contribute:
<br>
1. Fork this repository.
2. Create a new branch (git checkout -b feature/newFeature).
3. Make your changes and commit (git commit -m 'Add newFeature').
4. Push to the branch (git push origin feature/newFeature).
5. Open a Pull Request.
## 📝 License
This project is licensed under the MIT License - see the LICENSE file for details.
## 🙌 Acknowledgements
Special thanks to TomNomNom for the original project.
