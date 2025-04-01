# HTML-CSS-JS-projects
HTML,CSS,JS projects
# Navbar Scroll Effect 🚀

```This is a simple **fixed navbar** that changes background color when the user scrolls down. It is useful for websites where you want a transparent navbar initially but need a solid background after scrolling.```

```## 📌 How to Use?```
```
### 1️⃣ Add this HTML structure
<nav class="navbar">
    <div class="logo">My Website</div>
    <ul class="nav-links">
        <li><a href="#">Home</a></li>
        <li><a href="#">About</a></li>
        <li><a href="#">Contact</a></li>
    </ul>
</nav>


### 2️⃣ Add this CSS for styling
.navbar {
    position: fixed;
    width: 100%;
    top: 0;
    z-index: 1000;
    padding: 20px 50px;
    display: flex;
    justify-content: space-between;
    align-items: center;
    box-shadow: 0 4px 20px rgba(0, 0, 0, 0.1);
    transition: background 0.3s ease-in-out;
    background: transparent;
}

.navbar.scrolled {
    background: black !important;
}


## 3️⃣ Add this JavaScript
window.addEventListener("scroll", function () {
    let navbar = document.querySelector(".navbar");
    if (window.scrollY > 50) {
        navbar.classList.add("scrolled");
    } else {
        navbar.classList.remove("scrolled");
    }
});
```
