# Dell Latitude 7390 EFI - Ventura
This Hackintosh EFI for Dell Latitude 7390 has been tested with BigSur & Ventura macOS. OpenCore v0.8.8 has been used to build the EFI.

# <h2>Specification</h2>
<ul>
  <li>CPU: Intel Core i5-8350U</li>
  <li>RAM: Micron 16GB</li>
  <li>SSD: Micron 1300 M.2 2280 500GB SATA III</li>
  <li>GPU: Intel UHD 620</li>
  <li>Audio: Realtek ID 0256</li>
  <li>WiFi & Bluetooth: Intel AC 8265</li>
  <li>Ethernet: Intel I219-LM</li>
  <li>Microphone: Builtin</li>
  <li>Webcam: Builtin</li>
</ul>

# <h2>What Works?</h2>
Pretty much everything holding the fact that you have the same specification on your laptop. Following item were tested in working order.
<ul>
  <li>GPU Support</li>
  <li>Sound Card</li>
  <li>Microphone</li>
  <li>Webcam</li>
  <li>USB Ports</li>
  <li>Trackpad</li>
  <li>Ethernet</li>
  <li>WiFi</li>
  <li>Keyboard Backlight</li>
</ul>
Please bare in mind that I didn't get the chance to test out the HDMI and SD Card Reader. Natively Mac OS supported WiFi modules should work out of the box but if you are using Intel based Card with different model number, please feel free to check out the <a href="https://github.com/OpenIntelWireless/itlwm/">OpenIntelWireless</a> repository for appropriate KEXT. You must use the <a href="https://openintelwireless.github.io/HeliPort/">HeliPort</a> app to connect to your network. Ethernet works without any issue.

# <h2>Important Note</h2>
<ul>
  <li>You must update your SMBIOS info and generate your own MLB, SystemSerialNumber and SystemUUID. Please DO NOT use mine.</li>
  <li>I made lots of changes on Boot options section. So, please use <a href="https://github.com/ic005k/OCAuxiliaryTools">OC Auxiliary Tools</a> to re-adjust those changes as per Dortania's instruction mentioned <a href="https://dortania.github.io/OpenCore-Install-Guide/config-laptop.plist/kaby-lake.html#misc">here</a>.</li>
  <li>I won't be providing any support with this EFI at this point as this was a hobby project and I am done with it for the most of the part.</li>
</ul>

Thank you for stopping by.
