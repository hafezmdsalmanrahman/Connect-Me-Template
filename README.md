

---
### **ConnectMe - Blogger Link in Bio Theme Documentation**

**Version:** 1.0
**Developer:** Hafez Md Salman Rahman
**Website:** https://salmanrahman.netlify.app/

---

### **Table of Contents**

1.  [Introduction](#introduction)
2.  [Theme Installation](#theme-installation)
3.  [Easy Customization (Recommended Method)](#easy-customization)
    *   [Editing Site Title, Profile & Links](#editing-site-title-profile-links)
4.  [What You Can Customize](#what-you-can-customize)
    *   [Site Title](#site-title)
    *   [Profile Information (Image, Name, Bio)](#profile-information)
    *   [Main Links & Categories](#main-links-categories)
    *   [Footer Credits (For Buyers)](#footer-credits)
5.  [Advanced Features](#advanced-features)
    *   [Search & Filtering](#search-filtering)
    *   [Click Counter](#click-counter)
    *   [Share & QR Code Buttons](#share-qr-code-buttons)
    *   [Dark/Light Mode](#darklight-mode)
6.  [Support](#support)

---

### **1. Introduction** <a name="introduction"></a>

Thank you for choosing **ConnectMe**, a premium "Link in Bio" theme for Blogger. This theme is designed with a modern **Soft UI (Neumorphism)** aesthetic and is packed with powerful features to create a stunning and professional links page. The best part is, you can customize everything easily without touching the Blogger Layout section!

**Key Features:**
*   **Easy HTML-based Customization:** Edit all your content from one central place in the theme code.
*   **Soft UI / Neumorphism Design:** A beautiful and modern design that stands out.
*   **Dynamic Search & Filtering:** Help your visitors find the links they need instantly.
*   **Click Counter:** Track how many times each link is clicked.
*   **Share & QR Code:** Make it easy for others to share and visit your page.
*   **Dark/Light Mode:** A beautiful theme for both day and night.

---

### **2. Theme Installation** <a name="theme-installation"></a>

Follow these simple steps to install the ConnectMe theme on your Blogger blog.

1.  **Download and Unzip:**
    *   First, download the `ConnectMe.xml` file.

2.  **Go to Blogger Theme Section:**
    *   Log in to your Blogger Dashboard.
    *   In the left sidebar, navigate to **Theme**.

3.  **Backup Your Current Theme (Recommended):**
    *   Click the dropdown arrow next to the **"Customize"** button.
    *   Select **Backup** and download your current theme file. This is important in case you want to revert to your old theme.

4.  **Install the New Theme:**
    *   Click the dropdown arrow again and select **Restore**.
    *   Click **Upload** and select the `ConnectMe.xml` file you downloaded.
    *   The theme will be installed, and your blog will be updated instantly.

---

### **3. Easy Customization (Recommended Method)** <a name="easy-customization"></a>

This theme is designed for super-easy customization. You don't need to use the Blogger Layout. All changes can be made from one place in the HTML editor.

#### **Editing Site Title, Profile & Links** <a name="editing-site-title-profile-links"></a>

1.  In your Blogger Dashboard, go to **Theme**.
2.  Click the dropdown arrow next to **"Customize"** and select **Edit HTML**.
3.  Scroll to the top of the code editor. You will find a section clearly marked as:
    ```javascript
    /******************************************************************
     * Easy Customization Zone: Edit all your content from here.
     ******************************************************************/
    ```
4.  Inside the `<script id="theme-data">` tag, you will see the `const themeData = { ... };` object. This is where you will make all your changes.

---

### **4. What You Can Customize** <a name="what-you-can-customize"></a>

Here is a detailed guide on what you can change inside the `themeData` object. **Remember to only edit the text inside the quotes `""`.**

#### **Site Title** <a name="site-title"></a>
This is the title that appears in the rounded header.

```javascript
siteTitle: "Your Page Title",
```

#### **Profile Information (Image, Name, Bio)** <a name="profile-information"></a>
Update this with your personal details.

```javascript
profile: {
    name: "Your Name",
    image: "https://example.com/your-photo.jpg", // Use a direct image link (e.g., from Imgur)
    bio: "Your short and catchy bio goes here."
},
```

#### **Main Links & Categories** <a name="main-links-categories"></a>
This is the most important section. You can add, edit, or remove your links here.

*   To **add a new link**, copy a whole line (from `{` to `}` including the comma) and paste it.
*   To **assign a category**, simply write the category name inside the `category: "..."` part. Links with the same category will be grouped together under the filter buttons.

```javascript
mainLinks: [
    { name: "My Website", url: "https://example.com", category: "Work" },
    { name: "Follow me on Twitter", url: "https://twitter.com/username", category: "Social Media" },
    { name: "My Latest Video", url: "https://youtube.com/video-link", category: "Content" },
    // Add more links here following the same format
],
```

#### **Footer Credits (For Buyers)** <a name="footer-credits"></a>
You can add your own credit line in the footer. This is optional.

*   To display your credit, fill in the `ownerName` and `ownerUrl`.
*   To hide it, leave `ownerName` blank (e.g., `ownerName: ""`).

```javascript
footer: {
    ownerName: "Your Brand Name", // e.g., "Page owned by Alex Doe"
    ownerUrl: "https://your-website.com" // Your website link
}
```
The "Developed By" credit is a permanent part of the theme to honor the original developer.

---

### **5. Advanced Features** <a name="advanced-features"></a>

#### **Search & Filtering** <a name="search-filtering"></a>
The search bar allows visitors to instantly find links by typing a name. The filter buttons are automatically generated from the `category` you assign to each link in the `themeData` object.

#### **Click Counter** <a name="click-counter"></a>
Each link automatically tracks how many times it has been clicked. This data is stored in the user's browser (Local Storage) and is a great way to see which of your links are most popular.

#### **Share & QR Code Buttons** <a name="share-qr-code-buttons"></a>
*   **Share Button:** Allows visitors to easily share your page on social media or copy the link.
*   **QR Code Button:** Instantly generates a QR code for your page, which is perfect for sharing in person or on printed materials.

#### **Dark/Light Mode** <a name="darklight-mode"></a>
The theme includes a beautiful dark mode. The toggle button in the header allows visitors to switch between light and dark themes. The theme will remember their choice for their next visit.

---

### **6. Support** <a name="support"></a>

If you have any questions or need help with the theme, please contact the developer:

*   **Developer:** Hafez Md Salman Rahman
*   **Website:** https://salmanrahman.netlify.app/

Thank you for using ConnectMe! We hope you love it.
