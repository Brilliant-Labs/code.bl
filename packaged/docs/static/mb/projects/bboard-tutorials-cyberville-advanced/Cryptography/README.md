## ACTIVITY 13
# ⛓️ CRYPTOGRAPHY

---
##### ~avatar
Intro video about Cybersecurity Level 3 Advanced
https://youtu.be/HIquW6LqKH8
##### ~
</br>

# 📘 __*Guide Document:*__  
- Official Document in **English** [__👉 Here__](https://www.canva.com/design/DAGICy3MfKA/YIhqH8Rpvg1w_WFIQg0F_Q/view?utm_content=DAGICy3MfKA&utm_campaign=designshare&utm_medium=link2&utm_source=uniquelinks&utlId=h4dd22028ad)
- Document officiel en **French** [__👉 Ici__](https://www.canva.com/design/DAGIaIMzciU/43hKFcn0OyW_Vhndyd1I6Q/view?utm_content=DAGIaIMzciU&utm_campaign=designshare&utm_medium=link2&utm_source=uniquelinks&utlId=hd4ec95ab91)
</br>
</br>

# 🚀 __*Let's get started!*__

## ⬇️ Download Codes </br>
- It’s a great idea to prepare four separate projects, each with the correct code for its task, before getting started. This will help you stay organized and feel ready when it’s time to work on them.

    👉 Download the next two .hex files, then for each file, create a ``➕ New Project`` and drag and drop the file for each task </br>
    + __``Task #1: QR hash``__ [⬇️ Here](https://www.brilliantlabs.ca/documents/cybersec/Cryptography-QR.hex).</br>
    + __``Task #2: Hash Function``__  [⬇️ Here](https://www.brilliantlabs.ca/documents/cybersec/Cryptography-HashDJB2.hex).</br>

## __``Task #1: QR hash``__
- 1️⃣ Use the micro:bit's LED display to represent a QR code. Personalize your code by selecting multiple LEDs on the screen to create a unique pattern. Then, convert this pattern into a numeric string (letters) to obtain your digital signature. The more LEDs you select, the longer the resulting code will be, you have to select at least 6 LEDs.

- 2️⃣ Download the ``Code Example`` .hex file for this activity by clicking [⬇️ Here](https://brilliantlabs.ca/documents/cybersec/Confidentiality.hex). 
Once downloaded, you can either drag and drop it into a new project or click the **📝 Edit** icon in the programming view below to open and customize it using the 🧩 Blocks editor.

    You can also cut and paste the following code into the 📜 JavaScript code area, and then back into the 🧩 blocks code if you prefer to do so:

```blocks
input.onButtonPressed(Button.A, function () {
    CybersecAdvanced.Scan()
})
basic.showLeds(`
    # . . . #
    . . . # .
    . # . . .
    . . # . #
    # . . . .
    `)
```

## __``Task #2: Hash Function``__
- 1️⃣ Create a hash funcion to obtein the DJ-B2 Hash from your code signature letters, use it as name to be hasehed. You can downlod the .hex file example from here.
- 2️⃣ Download the ``Code Example`` .hex file for this activity by clicking [⬇️ Here](https://brilliantlabs.ca/documents/cybersec/Confidentiality.hex). 
Once downloaded, you can either drag and drop it into a new project or click the **📝 Edit** icon in the programming view below to open and customize it using the 🧩 Blocks editor.

    You can also cut and paste the following code into the 📜 JavaScript code area, and then back into the 🧩 blocks code if you prefer to do so:

```blocks
// Example usage
input.onButtonPressed(Button.A, function () {
    name = "Cyberville123"
    hash2 = djb2Hash(name)
    console.log(hash2)
basic.showString("" + (hash2.toString()))
})
// Calculation Hash
function djb2Hash (input2: string) {
    hash = 5381
    for (let i = 0; i <= input2.length - 1; i++) {
        // Get the character at index i
        char = input2.charAt(i)
        let charCode = char.charCodeAt(0);
hash = (hash << 5) + hash + charCode
    }
    // Ensure a positive 31-bit result
    return hash & 0x7FFFFFFF
}
let name = ""
let hash2 = 0
let hash = 0
let char = ""
```