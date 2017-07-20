## Bluetooth Low Energy AutoLock

### (Used for automatically locking a linux workstation when a specially configured beacon goes out of range)

This is currently in the planning stages but will likely:

 * Use a Laird BC600 in peripheral mode (v4.0 or v4.1), powered by a single 3v lithium coin cell battery
 * Create a simple smartBASIC application to run on the BC600 that will allow pairing with the PC
 * Allow the creation of a symmetric code so that the beacon can generate a matching code for the PC (future use)
 * Allow resetting of the dongle to clear its data and be reused (and also allow remote erasing of the application to allow another application to be loaded OTA)
 * Allow removing of the dongle ID from the user's files so that it can no longer have any effect e.g. if its been lost or stolen
 * Maintain a high-latency large connection interval BLE connection with a PC
 * Lock the PC if the module goes out of range
 * (Future possibility) unlock the PC if the module comes back into range
 * (Future possibility) emergency mode: lock the PC by pressing a button on the dongle
