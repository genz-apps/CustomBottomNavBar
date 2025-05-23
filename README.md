# 📱 CustomBottomNavBar

A sleek and customizable Bottom Navigation Bar for Android built in Java. It features an animated moving circle and a stylish curved background — perfect for modern and dynamic mobile UIs.

![preview](https://your-image-url.com/preview.gif)

---

## 📜 License

This library is **free to use for personal and individual development purposes**.  
Redistribution, modification for re-publishing, or commercial usage is **strictly prohibited** without prior written permission.

See the [LICENSE](LICENSE) file for full terms.

---

## ✨ Features

- 🔵 Smooth animated circle that moves along selected items
- 🎨 Fully customizable drawables (circle and curved background)
- 🧩 Built on top of `BottomNavigationView` (Material Design)
- 💡 Easy to use in both XML and Java
- ⚙️ Compatible with custom icons and menus
- ✅ 100% Java — no Kotlin dependency

---

## 🛠️ Installation

To use this library via **JitPack**, follow these steps:

In your **root `build.gradle`** file:

```gradle```
```
allprojects {
    repositories {
        google()
        mavenCentral()
        maven { url 'https://jitpack.io' }
    }
}


In your app-level build.gradle file:

gradle
Copy
Edit
dependencies {
    implementation 'com.github.genz-apps:CustomBottomNavBar:1.0.0'
}
```






#⚙️ Usage
📍 XML Integration

Add the custom navigation bar directly in your layout:
```xml```
```
<com.genzapps.custombottomnavbar.CustomNavBar
    android:id="@+id/customNavBar"
    android:layout_width="match_parent"
    android:layout_height="wrap_content"
    app:circleDrawable="@drawable/my_circle"
    app:curveDrawable="@drawable/my_curve"
    app:menu="@menu/my_bottom_nav_menu" />
```
    
# 💻 Java Integration
Access and control the navigation programmatically:

```java```
```
CustomNavBar customNavBar = findViewById(R.id.customNavBar);
BottomNavigationView bottomNav = customNavBar.getBottomNav();

bottomNav.setOnNavigationItemSelectedListener(item -> {
    // Handle item selection
    return true;
});
```


**#🧩 Customization**
✅ Use your own drawables for the animated circle via app:circleDrawable.

✅ Customize the curved background with app:curveDrawable.

✅ Replace the menu using app:menu="@menu/your_menu".

**📬 Contact**
For support or commercial licensing inquiries, please email:

📧 hello.genzapps@gmail.com

**🤝 Contributing**
This project is not open for public contributions or redistribution forks.

🔹 You may report bugs or suggest features by email only.
**
🔖 License Summary**
✅ Allowed: Personal use and integration in your apps (including commercial apps).

❌ Not Allowed: Reselling, redistribution, or publishing modified versions.

❌ Not Allowed: Releasing the library publicly under a different name.

See the [License](https://github.com/user-attachments/files/20415708/README.md) file for full terms.





