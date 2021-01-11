# Bluetooth-Network-Status
A simple android application that shows the current network and bluetooth status. It also shows the statuses in a persistent notification in system tray even after removing the app from recent list of apps.
## Screenshots
<p align="center">
  <img width="200" height="400" src="PICTURES/1.jpeg">&nbsp;&nbsp;<img src="PICTURES/2.jpeg" width="200" height="400">&nbsp;&nbsp;
  <img src="PICTURES/3.jpeg" width="200" height="400">&nbsp;&nbsp;<img src="PICTURES/last.jpeg" width="200" height="400">
</p>

## Class Diagram
<p align="center">
  <img src="PICTURES/5.png">
</p>

* MainActivity and NotificationService classes implement both BluetoothReceiverInterface and NetworkReceiverInterface.
* Activity/Service specific implementation of abstract function handleState() in the interfaces are provided.
* BluetoothReceiver and NetworkReceiver classes are BroadcastReceivers which update UI through handleState() function in the respective interfaces mentioned above.
