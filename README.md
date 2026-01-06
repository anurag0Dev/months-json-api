<div align="center">

# 📅 Months JSON Data

✨ A simple, reusable JSON file for all 12 months ✨

![JSON](https://img.shields.io/badge/format-JSON-blue)
![Status](https://img.shields.io/badge/status-ready-success)
![License](https://img.shields.io/badge/license-free-green)

</div>

---

## 📦 What’s Inside

A lightweight JSON file that contains:
- 🔢 Month number (1–12)
- 📝 Full month name
- ✂️ Short month name

Perfect for **frontend projects**, **APIs**, and **UI components**.

---

## 📁 Project Structure

```txt
📦 months-json-data
 ┣ 📄 months.json
 ┗ 📄 README.md
```
## 🧩 Data Example

```
months.json
{
  "month": 1,
  "full": "January",
  "short": "Jan"
}
```
## 🚀 Use Cases
- ✅ Dropdown menus
- ✅ Date pickers
- ✅ Calendar UI
- ✅ Forms & filters
- ✅ React / JavaScript apps
- ✅ Chrome extensions

## API URL 
```
https://cdn.jsdelivr.net/gh/anurag0Dev/months-json-api@main/months.json
```

## ⚡ How to Use
Just import or fetch months.json and use it in your project.

```
fetch("months.json")
  .then(res => res.json())
  .then(data => console.log(data));
```
## OR 
JS
```
fetch("https://cdn.jsdelivr.net/gh/anurag0Dev/months-json-api@main/months.json")
  .then(response => response.json())
  .then(data => {
    console.log(data.months); // all months
  })
  .catch(error => {
    console.error("Error fetching months:", error);
  });
```
## Example: Use in Dropdown (JavaScript)

```
const select = document.getElementById("monthSelect");

fetch("https://cdn.jsdelivr.net/gh/anurag0Dev/months-json-api@main/months.json")
  .then(res => res.json())
  .then(data => {
    data.months.forEach(item => {
      const option = document.createElement("option");
      option.value = item.month;
      option.textContent = item.full;
      select.appendChild(option);
    });
  });
```
## Example: React Usage

```
useEffect(() => {
  fetch("https://cdn.jsdelivr.net/gh/anurag0Dev/months-json-api@main/months.json")
    .then(res => res.json())
    .then(data => setMonths(data.months));
}, []);

```
## 📜 License

🟢 Free to use for personal and commercial projects.

<div align="center">

⭐ If you find this useful, don’t forget to star the repo ⭐

</div> 
