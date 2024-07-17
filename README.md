# Ryan-s_Repair_PS4
This is an Instructional tutorial for Ryan. PS5/PS4 Jailbreak info's Facebook group. Documented for use by anyone who may deal with similar issues. Turorial post will be updated with more information until the issue is resolved. 

-Issue: PS4 needs to be updated to 2.55 or later. Initializing new SSD with USB update Fails, black screen, powers off.
-Status: Unresolved

-Last firmware: 11.52
-Last moddable firmware: 11.00
-Suggested moddable firmware: 9.00
-Requested firmware: 5.05
-Current firmware: 2.55
-PS4 Model: TBD
-SSD: WD Blue 1TB

(WARNING)
- Please carefully read, do not skip through this tutorial as I will not be held accountable or reliable for anyone's inability to follow instructions if so any damages occure to your drives, usb's or PS4 console.

Note: 
- DOWNLAOD PREPACKED FROM RELEASES ((((OPTIONAL)))), USE LINKS IF NOT WORKING OR UNTRUSTED
- If any of this is already done, do it anyways. We're running a clean install.
- Keep in mind that the firmware being installed needs to be equivilent or greater to the previous firmware installed. 
- You will need to repeat step (3) until you locate a functional firmware without the use of mobo diognostics
- If this tutorial doesn't work first with 5.05 then redo tutorial with 2.55 system software, at the end you will select (Reinstall system software instead of update system software) then try again with 5.05 after the console boots up


Start(Attempt #1) - 1
- Eject SSD from its casing & USB from port
- We're going to focus on the SSD first, plug your SSD into your pc with your SATA to USB hub
- Navigate to disk management using the search bar on your pc and check to see if It's initialized or showing up
- If It's uninitialized, choose MBR and initialize your SSD. If It's initialized and GPT, we'll change it to MBR after we reformat
- Next, navigate to your file explorer and right click on your drive
- Select properties and check your file system
- Your file system needs to be set as exFAT
- If you have multiple drives inserted at this time you need to eject them. It's not required but will make it easier to wipe the proper drive without risking losing data on the wrong one. Only your pc os drive and ps4 SSD should be inserted at this time

(Reflashing SSD for setup) - 2
- Open your command prompt as administrator using the search bar
- ----------------------------------------
- Type in diskpart
- Type in list disk
- Select your SSD, example: select disk 1
- Type clean
- ----------------------------------------
- Close command prompt window
- Navigate to disk management again
- Initialize disk as MBR and select exFAT
- Check file manager --> SSD --> properties // to ensure you sucessfully formated
- Safely eject your SSD from the computer

(Preparing you're USB) - 3
- Use this link to open in your browser https://darthsternie.net/ps4-firmwares/
- Select next at the bottom right under the OFFICIAL FIRMWARES until you get to firmware 5.05 and click on download. The download should start immediatly
- Open your command prompt as administrator using the search bar
- ----------------------------------------
- Type in diskpart
- Type in list disk
- Select your USB, example: select disk 1
- Type clean
- ----------------------------------------
- Close command prompt window
- Navigate to disk management again
- Initialize disk as MBR and select NTFS or exFAT
- Check file manager --> USB --> properties // to ensure you sucessfully formated


// In this section you can use prepacked or links

- -OR DRAG AND DROP--
- Click https://fat32format-gui.en.lo4d.com/windows and download tool
- Open gui fat32 format tool
- Select your usb from the drop down
- If prompted device is currently in use make sure to close out all other tabs
- Name anything and format
- Check file manager --> USB --> properties // to ensure you sucessfully formated
- In file manager navigate to your freshly formatted USB root
  
- -OR DRAG AND DROP--
- Create a new folder named PS4
- Open PS4 folder
- Create a new folder named UPDATE
- Open UPDATE folder and place 5.05 PS4UPDATE.PUP file inside
- Safely eject your USB from your pc

(Updating your PS4 Firmware with USB)
- Start the PS4 console in Safe Mode: press and hold the power button, releasing after the second beep.
- Select Update System Software PS4
- Let the PS4 run It's update.

- If this tutorial doesn't work first with 5.05 then redo tutorial with 2.55 system software, at the end you will select (Reinstall system software instead of update system software) then try again with 5.05 after the console boots up
