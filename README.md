# Setting Up Arduino IDE for LGT8F328P

## 1. Install Driver CH340

1. Download the CH340 Driver:  
   [https://sparks.gogo.co.nz/ch340.html](https://sparks.gogo.co.nz/ch340.html?srsltid=AfmBOoqLAOmrfzoob7wI9eAc2ZUFVEBzvEZ-2m6V1wNqpFqhSOaVu-Jy)

2. Extract the downloaded ZIP file.

3. Run the installer that you extracted.

4. Once CH340 is connected, you will see a COM port in **Tools > Port** in Arduino IDE.  
   The COM number may vary depending on your system.
   ![CH340 Driver Screenshot](img/comport.png)

   **Example:**
   `Driver connected on COM3`

---

## 2. Setting Up LGT8F328P Board in Arduino IDE

1. Open **Arduino IDE** (make sure it's installed).

2. Go to: **File > Preferences**

   ![CH340 Driver Screenshot](img/preference.png)

3. In the "Additional Board Manager URLs" field, add this URL:
   ```
   https://raw.githubusercontent.com/dbuezas/lgt8fx/master/package_lgt8fx_index.json
   ```
   ![CH340 Driver Screenshot](img/pref.png)
4. Click **OK**.

   For more info about this board manager, visit:  
   [https://github.com/dbuezas/lgt8fx](https://github.com/dbuezas/lgt8fx)

---

## 3. Install the Board via Boards Manager

1. Go to menu: **Tools > Board > Boards Manager**

   ![CH340 Driver Screenshot](img/tools.png)

2. Search for `LGT8F328`

   ![CH340 Driver Screenshot](img/ins.png)

3. Click **Install**

---

## 4. Upload the Blink Sketch

1. Go to:  **File > Examples > 01.Basics > Blink**
   ![CH340 Driver Screenshot](img/basic.png)

2. Then select the Select other Board and Port menu, if the installation is correct, the board and port will be read or appear as in the image below :   
   **Select other board and port**

   ![CH340 Driver Screenshot](img/port.png)

   If the installation is successful, the board and port will appear.

3. Click **OK**, then click **Upload** (right arrow icon)

   ![CH340 Driver Screenshot](img/blink.png)

4. Wait for the compile and upload process to complete.

   ![CH340 Driver Screenshot](img/comp.png)

---

## 5. Result

If the onboard LED blinks, the board is working correctly ✅

   ![CH340 Driver Screenshot](img/result.png)

---

## Author

**Name:** Hafidh Najib  
**Email:** hafidhnajib.2022@student.uny.ac.id
