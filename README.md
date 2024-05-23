# Digital Storage Oscilloscope (Linux Release)

Public release of Digital Storage Oscilloscope for Acute's Digital Storage 
Oscilloscope products.

## Supported Models

| Types                        | Product                                       | 
| ---------------------------- | --------------------------------------------- |
| Digital Storage Oscilloscope | Acute TravelScope 3000 series                 |
| Mixed Signal Oscilloscope    | Acute MSO3000 series                          |

## Supported Operating System
    
Ubuntu 18.04+ (Bionic Beaver)

## Usage

Download the latest software from the **Releases** page.

All our software are provided in an **AppImage** format. It requires making the 
file into executable before using it. 

Check the box that says “Allow executing file as program” as shown in the image.

![Demo Image](https://github.com/acute-technology-inc/dso-release/blob/main/res/image.png?raw=true)

Or, you can type

```
    chmod 777 DSO-x86_64.AppImage
```

Simply double-click the file to launch the software after the file is changed into an executable file.

Next, the software requires udev rules to allow non-root access to Acute’s 
devices. Thus, you may need to install the udev rule file that you can obtain from
`LinuxSoftwareResources.zip`.

1.	Download the udev file.
2.	Type the following command in the terminal

    ```
    sudo cp 99-AcuteUSB.rules /etc/udev/rules.d
    ```

3.	Restart PC.
4.	Launch the software.
