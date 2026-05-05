# Mini Project 1 : Installation and Deployment of Web Server using Apache HTTP Server

---

## 🎯 Objective

To install and configure Apache web server and host a basic website.

---

## 🔧 Step 1: Install Apache httpd

```bash
sudo dnf install httpd
```

![Install Apache](screenshots/screenshot_page1_1.png)

---

## ▶️ Step 2: Start and Enable Apache

```bash
sudo systemctl start httpd
sudo systemctl enable httpd
```

![Start Apache](screenshots/screenshot_page1_2.png)

---

## 🔍 Step 3: Check Apache Status

```bash
sudo systemctl status httpd
```

![Apache Status](screenshots/screenshot_page1_3.png)

---

## 🔥 Step 4: Allow Firewall

```bash
sudo firewall-cmd --permanent --add-service=http
sudo firewall-cmd --reload
```

![Firewall](screenshots/screenshot_page1_4.png)

---

## 🌐 Step 5: Test Apache in Browser

Open browser and enter your server IP:

```
http://your-ip-address
```

![Apache Test Page](screenshots/screenshot_page2_1.png)

---

## 📝 Step 6: Create Website

```bash
cd /var/www/html
sudo nano index.html
```

![Create Website](screenshots/screenshot_page2_2.png)

---

## 🔄 Step 7: Restart Apache

```bash
sudo systemctl restart httpd
```

![Restart Apache](screenshots/screenshot_page2_3.png)

---

## 👀 Step 8: View Website

Open browser:

```
http://localhost/index.html
```

![Website Output](screenshots/screenshot_page2_4.png)

---

## 📘 Step 9: Short Explanation of Apache Working

* Apache is a web server software.
* It receives requests from clients (web browsers).
* User enters URL in browser.
* Browser sends request to Apache server.
* Apache processes the request.
* It searches for requested file (e.g., `index.html`) in `/var/www/html`.
* If file is found → Apache sends it to browser.
* Browser displays the webpage to user.
* If file is not found → Apache shows error or default page.

---

## 📂 Folder Structure

```
.
├── README.md
└── screenshots/
    ├── screenshot_page1_1.png
    ├── screenshot_page1_2.png
    ├── screenshot_page1_3.png
    ├── screenshot_page1_4.png
    ├── screenshot_page2_1.png
    ├── screenshot_page2_2.png
    ├── screenshot_page2_3.png
    └── screenshot_page2_4.png
```

---

## ✅ Conclusion

Successfully installed and configured Apache HTTP Server and deployed a basic website.

---

✨ **Note:** This README follows the same step-by-step structure and screenshot placement as your original PDF.
