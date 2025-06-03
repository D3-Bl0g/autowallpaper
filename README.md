
📲 How to Install Your Repository on Termux (with cronie)

📦 1. Update and Install Dependencies

In Termux, run:

pkg update && pkg upgrade
pkg install git cronie

 ⚠️ Don’t forget cronie — it's essential for scheduling tasks.




---

📁 2. Clone and Enter Your Repository

git clone https://github.com/D3-Bl0g/autowallpaper


---
   3. Set create a folder named 'wallpapers'

 mkdir wallpapers
 
   4. create folder named 'wallpaper' in internal storage

   5. Move your desired pics to wallpaper folder
  
   6. Copy wallpaper folder to home in wallpapers
directory 
      cd /sdcard
      cp wallpaper /data/data/com.termux/files/home/wallpapers


     
🏗️ 7. Run or Install the Project

     chmod +x autowallpaper

   8. make it scheduled
      
      crontab -e
inside copy this to make wallpapers change in every
 one minute


        * * * * * bash ./autowallpaper

then hit CTRL + x, then y for yes

     9. To run script write crond


