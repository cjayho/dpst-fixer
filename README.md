![screenshot](/screenshot.png?raw=true)

# dpst-fixer
Simple systray icon app to suppress intel videocard DPST screen dimming

Modern (2018...2021 years) linuxes and freeBSD (since 13.0) have annoying bug in i915 videocard drivers - screen dims after 1 second after last redraw. This is an intel power saving feature named DPST, and this feature is enabled and cannot be disabled in recent drivers.

This app is a simple workaround for this annoying behavior.

Working principle: we have two barely identical systray icons, and change them every 0.25 seconds to forse screen redraw. For human eye it is a simple and static asterisk in systray, but screen redraws, what wee need.
