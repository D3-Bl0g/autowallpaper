
📲 How to Install Your Repository on Termux (with cronie)

📦 1. Update and Install Dependencies

In Termux, run:
```bash
pkg update && pkg upgrade
```
```bash
pkg install git cronie
```

 ⚠️ Don’t forget cronie — it's essential for scheduling tasks.




---

📁 2. Clone and Enter Your Repository
```bash
git clone https://github.com/D3-Bl0g/autowallpaper
```

---
   3. Set create a folder named 'wallpapers'
```bash
mkdir wallpapers
```
   4. create folder named 'wallpaper' in internal storage

   5. Move your desired pics to wallpaper folder
  
   6. Copy wallpaper folder to home in wallpapers
directory
```bash
cd /sdcard
```
```bash
cp -r wallpaper /data/data/com.termux/files/home/wallpapers
```

     
🏗️ 7. Run or Install the Project
```bash
cd
```
```bash
cd autowallpaper
```
```bash
chmod +x autowallpaper
```
8. Test it
```bash
./autowallpaper
```
 9. make it scheduled
 ```bash    
 crontab -e
 ```
inside copy this to make wallpapers change in every
 one minute

```bash
* * * * * bash /data/data/com.termux/files/home/autowallpaper/autowallpaper
```
then hit CTRL + x, then y for yes

To run script write 
```bash
crond
```
⚠️☢️9. Install termux-Api for better functioning 
