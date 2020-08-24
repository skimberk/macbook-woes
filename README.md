# Macbook Woes
## Solving problems with my Macbrook Pro Retina 15 inch (mid-2012)

### Getting display brightness (and hopefully waking from sleep) to work again

1. Downloaded release of https://github.com/timpalpant/NVDAGPUWakeHandler
2. Ran `NativeDisplayBrightness` (and gave it accessibility permissions)
3. Disabled SIP
4. Moved `NVDAGPUWakeHandler.kext` to `/Library/Extensions`
5. Ran `sudo chown -R root:wheel /Library/Extensions/NVDAGPUWakeHandler.kext`
6. Ran `sudo touch /Library/Extensions`
7. Ran `sudo kextcache -i /` and made sure it loaded ok


### Related links

- https://dhavaldalal.wordpress.com/2018/05/29/how-to-disable-failed-discrete-gpu-nvidia-geforce-gt-650m-for-macbook-pro-101-mid-2012-on-high-sierra-10-13-4/
- https://dhavaldalal.wordpress.com/2018/05/29/how-to-disable-failed-discrete-gpu-nvidia-geforce-gt-650m-for-macbook-pro-101-mid-2012-on-high-sierra-10-13-4/comment-page-1/#comment-975
- https://github.com/TankTheFrank/NativeDisplayBrightness
- https://tim.palpant.us/sysadmin/macos/2018/09/09/nvda-gpu-wake-handler/#disable-nvidia-gpu-after-waking-from-sleep
