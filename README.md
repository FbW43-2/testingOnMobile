# Viewing and Debugging your Project from an Android Phone

## Setting up your Android phone

### [Android: Set up Developer Options](https://developer.android.com/studio/debug/dev-options)

1. Find the Build Number of your phone:
   Settings > (System >) About Phone > Build Number
2. Tap on the Build Number 7 times
3. In the System section of Settings, you should now see Developer Options

### Enable USB debugging

1. Settings > (System > (Advanced >)) Developer Options > USB debugging

## Setting up Chrome on your laptop

1. Connect your phone to your laptop via USB
2. Open Chrome on your phone, and [visit a site](https://xkcd.com/2212/)
3. Open Chrome on your laptop
4. Go to [chrome://inspect#devices](chrome://inspect#devices).
5. Make sure that the Discover USB devices checkbox is enabled.
6. You should see an **Offline** notice: check your phone
7. Check the "Always allow from this computer" checkbox
8. Accept the Allow USB Debugging permission prompt on your phone
9. The pages that are open in Chrome on your phone should now appear in the [chrome://inspect#devices](chrome://inspect#devices) on your laptop
10. Click on the **inspect** link for one of the pages
11. You can now use the Elements Inspector to view the HTML and CSS of the page on your phone

### Connecting your phone to your frontend server

1. In [chrome://inspect#devices](chrome://inspect#devices) on your laptop, click on the Port Forwarding button
2. Enter 3000 | 127.0.0.1:3000
3. Select the "Enable Port Forwarding" checkbox
4. Click Done

4. In VS Code, open your frontend project folder
5. Start the frontend server by running `npm start`
6. A new tab should open in Chrome
7. Copy the URL from the address bar*
8. In [chrome://inspect#devices](chrome://inspect#devices), paste the address into the Open Tab With URL field
9. Press Open
10. A new tab will open on your phone
11. In [chrome://inspect#devices](chrome://inspect#devices), click on the Inspect link.

* If the address uses a port other than :3000, repeat steps 1-3, to enable forwarding from the new port.
