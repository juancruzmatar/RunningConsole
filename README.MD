# DemoQA Text Box Automation

## Overview
This script automatically:
1. Fills the form at [https://demoqa.com/text-box](https://demoqa.com/text-box)  
2. Submits it and checks the output  
3. Calls a public API (`https://jsonplaceholder.typicode.com/posts/1`)  
4. Prints `✅ All tests passed` if everything works

---

## What changed and why
- **Form filling fixed**: now values are set with proper `input` and `change` events so the site accepts them.  
- **Submit fixed**: uses the real **Submit** button click, which is more reliable than `requestSubmit()`.  
- **Validation improved**: waits for the output box, normalizes values, and compares them with the expected text.  
- **Clear feedback**: shows a single success message or a descriptive error.

---

## How to run
1. Open [https://demoqa.com/text-box](https://demoqa.com/text-box) in Chrome (or any modern browser).  
2. Open **DevTools → Console** (`F12` or `Ctrl+Shift+I` / `Cmd+Opt+I`).  
3. If Chrome shows a yellow warning about pasting, type `allow pasting` and press **Enter** once.  
4. Copy the entire script (`script.js`) and paste it into the **Console**.  
5. Press **Enter** to run.  

You should see:
✅ All tests passed