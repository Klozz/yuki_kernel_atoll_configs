# Yuki kernel
## some ramdisk "configurations"

To add this you can copy/paste the text from bash ```init.hardware.rc under init.device.rc or init.qcom.rc```

if you don't want to add another file.
On the other hand, if you want to add the file, you must edit init.qcom.rc to call this file. 
As follows:

bash ```import /vendor/etc/init/hw/init.hardware.rc ```

edit device makefile 

PRODUCT_COPY_FILES += devicepath/rootdir/etc/init.hardware.rc:$(TARGET_COPY_OUT_VENDOR)/etc/init/hw/init.hardware.rc


In the future and as I have more time I will add more changes

# Credits
 The Android Open Source Project
 
