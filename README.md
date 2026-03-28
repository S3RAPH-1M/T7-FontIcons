# T7-FontIcons

T7-FontIcons allows you to add images directly into text strings in **Call of Duty: Black Ops III**. This is useful for creating custom icons, logos, or other graphics within in-game text.

---

## Installation Instructions

Follow these steps to set up T7-FontIcons in your project:

### Step 1: Open Asset List
- Navigate to your game's asset list:  
  ```
  Call of Duty Black Ops III\zone_source\all\assetlist
  ```
- Open the `core_post_gfx.csv` file using a text editor. **Visual Studio Code** (VSC) is recommended.

### Step 2: Comment Out Default Font Icon
- In `core_post_gfx.csv`, comment out the following line:  
  ```
  fonticon,fonticon/defaultfonticon.csv
  ```

### Step 3: Copy Example FontIcon Folder
- Go to the example map folder:  
  ```
  { zm_hashiba_test }
  ```
- Copy the `fonticon` folder from `zone_source` and add it to your project.

### Step 4: Update Material Name
- Inside the copied `fonticon` folder, open the `.csv` file.  
- Change the **material name** in the **third column** to your 2D blend material.

### Step 5: Assign a Name to Your Font Icon
- Assign a name to your font icon.  
- Default name: `DEVRAW_LOGO`  
- You can choose any name you like.

### Step 6: Insert Image into Text String
- Go to the string where you want the image to appear.  
- Create a billboard by typing:
  ```
  ^B^
  ```
- Directly after the `B`, add your font icon name.  
- Example:
  ```
  ^BDEVRAW_LOGO^
  ```

---

## Notes
- Make sure your material is Marked down as 2D Blend.  
- Each font icon must have a unique name to prevent conflicts.  

---

Enjoy adding custom images to your text strings with T7-FontIcons!
