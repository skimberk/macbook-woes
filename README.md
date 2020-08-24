# Macbook Woes
## Solving problems with my Macbrook Pro Retina 15 inch (mid-2012)

1. Downloaded release of https://github.com/timpalpant/NVDAGPUWakeHandler
2. Ran `NativeDisplayBrightness` (and gave it accessibility permissions)
3. Disabled SIP
4. Moved `NVDAGPUWakeHandler.kext` to `/Library/Extensions`
5. Ran `sudo chown -R root:wheel /Library/Extensions/NVDAGPUWakeHandler.kext`
6. Ran `sudo touch /Library/Extensions`
7. Ran `sudo kextcache -i /` and made sure it loaded ok
