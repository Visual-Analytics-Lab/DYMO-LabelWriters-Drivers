# DYMO-LabelWriters-Drivers
Contains Drivers for runing DYMO LabelWriter 450 and DYMO LabelWriter 550

## DYMO LabelWriter 450 or Below

### Step1:
Run the following command to install cups libararies:

`sudo apt-get install libcups2-dev libcupsimage2-dev gcc g++`
### Step 2:

Do either of the methods to install the drivers for DYMO Label Writer 450 or below.

### Method 1:
Run the following command for installing all the drivers:

`sudo apt install printer-driver-dymo `

### Method 2:
Clone the Driver from github and cd into DYMO-LabelWriter-450 Folder, and run the following commands to install the drivers:

```
git clone https://github.com/Visual-Analytics-Lab/DYMO-LabelWriters-Drivers
cd DYMO-LabelWriter-450-Drivers
aclocal
autoconf
automake
./configure
make
sudo make install
```

### Final Step:

After doing either of the methods run the following command to open cups interface:

 `cupsctl WebInterface=Yes`

Next, head to the web browser and go to navigate to https://localhost:631 or https://your-ip-address:631(most times:  https://127.0.0.1:631 should work)
Navigate to Administration Tab and add DYMO LabelWriter 450 from the devices mentioned(make sure that the device is connected).
Also, changes can be made in the default settings page to configure the printer according to the need.

Now you should be able to Print anything to DYMO LabelWriter 450 from anywhere.

## DYMO LabelWriters 550

### Step1:
Run the following command to install cups libararies:

`sudo apt-get install libcups2-dev libcupsimage2-dev gcc g++`
### Step 2:

Clone the Driver from github and cd into DYMO-LabelWriter-550 Folder, and run the following commands to install the drivers:

```
git clone https://github.com/Visual-Analytics-Lab/DYMO-LabelWriters-Drivers
cd DYMO-LabelWriter-550-Driver
aclocal
autoconf
automake
./configure
make
sudo make install
```

### Final Step:

After doing either of the methods run the following command to open cups interface:

 `cupsctl WebInterface=Yes`

 Next, head to the web browser and go to navigate to https://localhost:631 or https://<your-ip-address>:631(most times:  https://127.0.0.1:631 should work)
Navigate to Administration Tab and add DYMO LabelWriter 550 from the devices mentioned(make sure that the device is connected).
Also, changes can be made in the default settings page to configure the printer according to the need.

Now you should be able to Print anything to DYMO LabelWriter 550 from anywhere.
