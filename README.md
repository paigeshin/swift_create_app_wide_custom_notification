# swift_create_app_wide_custom_notification

```swift

extension Notification.Name {
    static let watchToPhoneTransferInfo: Notification.Name = Notification.Name("WatchToPhoneTransferInfo")
}

NotificationCenter.default.post(name: Notification.Name.taskAddedNotification, object: "Do launtry")


.onReceive(NotificationCenter.default.publisher(for: Notification.Name.taskAddedNotification)) { object in
     newTask = object as? String
 }
 



```
