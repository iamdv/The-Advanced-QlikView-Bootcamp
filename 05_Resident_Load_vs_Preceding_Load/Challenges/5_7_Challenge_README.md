## Challenge:
### 5.7: You have been provided with five QVD files (Orders_YYYYMMDD), QVW file and the script. After reloading the script we see Synthetic Table with Synthetic Keys instead we wanted to perform auto concatenation of all the Order Tables. Please go ahead and correct the script which generates one Order table after reloading. Also, add a new field which shows the file name for each of the QVD files loaded.


### **Rules:** ###
1. You MUST use the wildcard load as shown in the script [Orders_2017*]
2. You can’t use forced concatenation on individual table
3. You MUST create the %Key_RequireDate either in Preceding Load or Resident Load ONLY

This is how the final data model should be:

![Image of output](https://github.com/iamdv/QlikView-Advanced-Developer-Part1/blob/master/05_Resident_Load_vs_Preceding_Load/Challenges/5_7_Challenge.png)


Note: Please download QVW file if you have licensed QlikView desktop edition. If you are using QlikView personal edition then please use copy the script from QVS and the QVD files.
