# Sendbird UIKit Android Architecture
- [Application](#application)
- [UIKit](#uikit--application)
- [Chat SDK](#chat-sdk)
- [Android](#android)

## Android
- Android platform.

## Chat SDK
- Sendbird server <- Chat SDK: Chat features -> UIKit 


## UIKit & Application
- UIKit provides UI components to customer applications using features of Chat SDK.
Using UIKit, a customer can easily implement UIs for Chat features.

#### Migration
- UIKit 2.0: Activity - Fragment - Style - Res
- UIKit 3.0: Activity - Fragment - Style - Res - Module - Components - ViewModel

#### UIKit Architecture
- View: Activity - Fragment - Module - Components - Style/Res
- Data + API: ViewModel

#### Fragment
- Fragments are the central UI component of UlKit.
- It serves to bind the View provided by the Module and the Data or API provided by the ViewModel.

#### Module
- A module provides a view of the entire screen of the Fragment.
- There is one Module per fragment. A module has several components.

#### Components
- A component creates the smallest unit of view that can be customized in UIKit.
- The screen, which used to be a fragment unit, is now divided into a component unit.

#### ViewModel
- The ViewModel actually communicates with the Chat SDK and provides data and APIs related to Chat. 
- A fragment uses data by using APIs provided by ViewModel or by observing data changes.

#### BaseModuleFragment Lifecycle

## Application


## Conclusion



## Source
[Sendbird UIKit Android](https://www.youtube.com/watch?v=oH41o2iKhgs)
\
[Sample app](https://github.com/sendbird/sendbird-uikit-android)
\
[Architecture](https://sendbird.com/docs/chat/uikit/v3/android/introduction/migration-guide)
\
[BaseModuleFragment lifecycle](https://sendbird.com/docs/chat/uikit/v3/android/screens/overview#2-basemodulefragment-lifecycle)







