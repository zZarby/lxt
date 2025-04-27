
---

# 👻 LxT - Lua Encryption Tool 👻
<p align="center">
<b>The best Roblox Lua encryption tool!</b><br>
<a href="https://github.com/zZarby/lxt">➡️ Check it on GitHub ⬅️</a>
</p>

---

## 🫧 How to Use 🫧

First, load the LxT encryption module:

```lua
loadstring(game:HttpGet("https://raw.githubusercontent.com/zZarby/lxt/refs/heads/main/__main__.lua", true))()
```

---

### 🔹 File Encryption (`Mypt`)

> Used for encrypting text intended for files, simple prints, or authentication keys.  
> **Note**: `Mypt` encryption is compatible with all basic Lua string manipulations, but less secure compared to `Crypt`.

Example:

```lua
local text = "Hello World"
local key = 10

-- Encrypt the text
local encrypted = LXT:Mypt(true, key, text)

-- Decrypt the text
local decrypted = LXT:Mypt(false, key, encrypted)

print("🔒 Encrypted (File): " .. encrypted)
print("🔓 Decrypted (File): " .. decrypted)
```

---

### 🔹 Normal Encryption (`Crypt`)

> Used for **stronger encryption** of strings.  
> **Note**: `Crypt` offers better security, but the result may not be compatible with all types of Lua string operations (due to special characters).

Example:

```lua
local text = "Hello World"
local key = 10

-- Encrypt the text
local encrypted = LXT:Crypt(true, key, text)

-- Decrypt the text
local decrypted = LXT:Crypt(false, key, encrypted)

print("🔒 Encrypted (Strong): " .. encrypted.Value)
print("🔓 Decrypted (Strong): " .. decrypted.Value)
```

---

## 📖 About the Methods

Both `Mypt` and `Crypt` use the same arguments:

| Argument      | Description                                                                 |
| -------------- | --------------------------------------------------------------------------- |
| `true/false`   | `true` to encrypt, `false` to decrypt                                        |
| `key`          | The encryption/decryption key (number)                                      |
| `text`         | The text to encrypt or the encrypted text to decrypt                        |

---

## 📌 Disclaimer

⚠️ **This tool is for educational purposes only.**  
⚠️ **The creator is not responsible for any misuse of this script.**

---

<p align="center"><b>Made with ❤️ by ZΛRBY</b></p>

---
