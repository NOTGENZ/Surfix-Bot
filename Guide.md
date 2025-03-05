# 📖 **Surfix - Complete Guide**
🚀 **A powerful open-source Discord bot built using BDFD!**  
📲 **This guide will help you download BDFD on Android and set up Surfix easily!**  

---

## 📥 **How to Download & Install BDFD (Bot Designer for Discord) on Android**
Bot Designer for Discord (BDFD) is a powerful tool that allows you to create bots without coding.  

### 📌 **Steps to Download:**
1. 🔍 **Go to Play Store** and search for **"Bot Designer for Discord"**  
2. 📥 **Download & Install** the app  
3. 🚀 **Open the app and log in** with your Discord account  
4. 🔧 **Start creating your own bot** or modify an existing one  

🔗 **[Download BDFD from Play Store](https://play.google.com/store/apps/details?id=com.jakubtomana.discordbotdesinger)**  

---

## 🤖 **How to Use Surfix Bot**
Surfix is easy to use! Just **invite the bot** and start using commands!  

### 📌 **Basic Setup:**
1. **Invite Surfix to your server** ➝ [Click Here](https://discord.com/oauth2/authorize?client_id=1340719763562823690)  
2. **Make sure the bot has permissions** (Manage Messages, Kick/Ban Members, etc.)  
3. **Use `S!help`** to see the list of available commands  
4. **Enjoy using Surfix!** 🎉  

---

## 🌟 **BoostC Command Setup (`S!boostc`)**
The `S!boostc` command allows you to check the number of boosts in a server!  

### 📌 **How It Works:**
- The **BDFD variable used:** `$getServerVar[boost_counter]`  
- It fetches the boost count from the server  

### 📝 **BDFD Script for `S!boostc`**
```bds
$onlyIf[$hasPerms[$authorID;admin]==true;❌ You need Admin permissions to use this!]
$onlyIf[$serverBoostCount!=0;❌ This server has no boosts!]
✅ This server has **$serverBoostCount** boosts!
