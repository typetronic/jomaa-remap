# Troubleshooting

## TCC deny IOHIDDeviceOpen
No Input Monitoring permission.
1. System Settings → Privacy & Security → Input Monitoring
2. Remove JomaaRemap if present
3. Launch app, enable toggle

## macOS cannot verify developer
Self-signed app.
- Right-click → Open → Open
- Or: xattr -dr com.apple.quarantine /Applications/JomaaRemap.app

## Reset permissions
tccutil reset ListenEvent com.local.JomaaRemap
tccutil reset Accessibility com.local.JomaaRemap
