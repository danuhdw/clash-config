# OpenClash Configuration Repository

This repository contains OpenClash configurations for both **dual modem** and **single modem** setups. It includes proxy providers, rule providers, and example configurations to help you get started with OpenClash.

---

## **Features**
- **Dual Modem Configuration**: Supports failover and load balancing between two modems (WAN-1 and WAN-2).
- **Single Modem Configuration**: A general-purpose configuration for single modem setups.
- **Proxy Providers**: Pre-configured proxy providers for easy integration.
- **Rule Providers**: Custom rule sets for blocking, directing, and tunneling traffic.
- **Customizable**: Easily adapt the configurations to your specific needs.

---

## **File Structure**
```
openclash-config/
├── config-dual-modem.yaml        # Configuration for dual modem setups
├── config.yaml                   # Configuration for single modem setups
├── proxy_provider/               # Proxy provider files
│   ├── wan1.yaml                 # Proxy list for WAN-1
│   ├── wan2.yaml                 # Proxy list for WAN-2
│   └── proxies.yaml              # Proxy list for single modem
├── rule_provider/                # Rule provider files
│   ├── direct.yaml               # Rules for direct traffic
│   ├── reject.yaml               # Rules for blocking traffic
│   ├── adult.yaml                # Rules for adult content
│   ├── facebook.yaml             # Rules for Facebook
│   ├── games.yaml                # Rules for gaming traffic
│   ├── instagram.yaml            # Rules for Instagram
│   ├── tiktok.yaml               # Rules for TikTok
│   ├── twitter.yaml              # Rules for Twitter
│   ├── whatsapp.yaml             # Rules for WhatsApp
│   └── youtube.yaml              # Rules for YouTube
└── README.md                     # This file
```

---

## **Getting Started**

### **1. Clone the Repository**
Clone this repository to your local machine:
```bash
git clone https://github.com/danuhdw/openclash-config.git
cd openclash-config
```

### **2. Choose Your Configuration**
- For **dual modem** setups, use `config-dual-modem.yaml`.
- For **single modem** setups, use `config.yaml`.

### **3. Customize Proxy and Rule Providers**
- Edit the files in the `proxy_provider/` and `rule_provider/` directories to match your proxy lists and rules.

### **4. Deploy the Configuration**
- Copy the desired configuration file to your OpenClash configuration directory (usually `/etc/openclash/config/`).
- Restart OpenClash to apply the new configuration.

---

## **Configuration Details**

### **Dual Modem Setup**
- **Failover**: Automatically switches to the secondary modem if the primary fails.
- **Load Balancing**: Distributes traffic between both modems for optimal performance.
- **Health Checks**: Regularly tests the availability of proxies.

### **Single Modem Setup**
- **General Use**: Suitable for most single modem setups.
- **Custom Rules**: Includes rules for direct traffic, blocking, and tunneling.

---

## **Contributing**
Contributions are welcome! If you have suggestions or improvements, please:
1. Fork the repository.
2. Create a new branch (`git checkout -b feature/your-feature`).
3. Commit your changes (`git commit -m 'Add some feature'`).
4. Push to the branch (`git push origin feature/your-feature`).
5. Open a pull request.

---

## **License**
This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

---

## **Support**
If you encounter any issues or have questions, please open an issue on GitHub or contact the maintainers.

---

**Happy Clashing!** 🚀
