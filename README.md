# reels_viewer

This flutter package designed to replicate the Instagram Reels viewer experience within your
application. It provides a seamless and intuitive way to display and view videos in a manner similar
to the Instagram Reels interface.

## Usage

In the `pubspec.yaml` of your flutter project, add the following dependency:

```yaml
dependencies:
  ...
  insta_reels_viewer: ^1.0.0
```

In your library add the following import:

```dart
import 'package:insta_reels_viewer/insta_reels_viewer.dart';
```

For help getting started with Flutter, view the online [documentation](https://flutter.io/).

## Example

Initializing a List

```dart

List<ReelsModel> reelsList = [
  ReelsModel(
      url: "https://commondatastorage.googleapis.com/gtv-videos-bucket/sample/BigBuckBunny.mp4",
      likeCount: 578,
      commentCount: 200,
      sendCount: 70,
      isLiked: true,
      musicName: "my music name 1",
      musicImageUrl: "",
      description: "this is demo descriptioin, adkf alkd adkjhfladhlfkja ajkldhfkahfkj  alkjfhaldjfh  akjdhfa jhkfhadhjfkjhfkjdhfd dfd",
      createdAt: DateTime.now().toString(),
      updatedAt: DateTime.now().toString(),
      user: User(
          userName: "Raman Thakur",
          profileUrl: "https://img.freepik.com/free-photo/young-indian-man-dressed-trendy-outfit-monitoring-information-from-social-networks_231208-2766.jpg",
          createdAt: DateTime.now().toString(),
          updatedAt: DateTime.now().toString(),
          isFollow: true
      ),
      reelComments: [
        ReelComments(
            cmment: "akkdfhkaljhflkajdf",
            createdAt: DateTime.now().toString(),
            updatedAt: DateTime.now().toString(),
            user: User(
              userName: "Vanit Dev",
              profileUrl: "https://img.freepik.com/free-photo/young-indian-man-dressed-trendy-outfit-monitoring-information-from-social-networks_231208-2766.jpg",
              createdAt: DateTime.now().toString(),
              updatedAt: DateTime.now().toString(),
            )
        )
      ]

  ),
  ReelsModel(
    url: "https://assets.mixkit.co/videos/preview/mixkit-tree-with-yellow-flowers-1173-large.mp4",
    likeCount: 578,
    commentCount: 43,
    sendCount: 80,
    isLiked: false,
    musicName: "my music name 1",
    musicImageUrl: "",
    description: "this is demo descriptioin, adkf alkd adkjhfladhlfkja ajkldhfkahfkj  alkjfhaldjfh  akjdhfa jhkfhadhjfkjhfkjdhfd dfd",
    createdAt: DateTime.now().toString(),
    updatedAt: DateTime.now().toString(),
    user: User(
        userName: "Pankaj Thakur",
        profileUrl: "https://img.freepik.com/free-photo/young-indian-man-dressed-trendy-outfit-monitoring-information-from-social-networks_231208-2766.jpg",
        createdAt: DateTime.now().toString(),
        updatedAt: DateTime.now().toString(),
        isFollow: false
    ),


  ),
  ReelsModel(
      url: "https://assets.mixkit.co/videos/preview/mixkit-portrait-of-a-woman-in-a-pool-1259-small.mp4",
      likeCount: 578,
      commentCount: 30,
      sendCount: 7,
      isLiked: true,
      musicName: "",
      musicImageUrl: "",
      description: "",
      createdAt: DateTime.now().toString(),
      updatedAt: DateTime.now().toString(),
      reelComments: []
  ),
];

```

Simple implementation

```dart
InstaReelsViewer
(
reelList: reelsList,
onClickCommentIcon:(reelData){},
onClickShareIcon: (reelData){},
onLike: (reelData){},
onUnLike: (reelData){},
onClickName: (reelData){},
onFollow: (reelData){},
onUnFollow: (reelData){},
);
```

## Options

|        Name        |                        Description                         |   Default    |                    Return                    |
|:------------------:|:----------------------------------------------------------:| :----------: |:--------------------------------------------:|
|      reelList      |                   For assign reels list                    |     `[]`     |                      -                       |
|  onClickShareIcon  |              Trigger when click on Share btn               |      -       |                 `ReelsModel`                 |
|       onLike       |    Trigger when click on Like btn or double tap to like    |      -       |                 `ReelsModel`                 |
|      onUnLike      |  Trigger when click on Like btn when it is already liked   |      -       |                 `ReelsModel`                 |
|      onFollow      |              Trigger when click on Follow btn              |      -       |                 `ReelsModel`                 |
|     onUnFollow     | Trigger when click on Follow btn when it already following |      -       |                 `ReelsModel`                 |
| onClickCommentIcon |             Trigger when click on Comment Icon             |      -       |                 `ReelsModel`                 |
|   onClickName      |              Trigger when click on User Name               |      -       |                 `ReelsModel`                 |


## Demo APK

[Click here](https://gogle.com) for
download demo app.

## ScreenShots

initial view

Screenshot 1
<p float="left"> 
<img src="https://drive.google.com/file/d/1uy0mUvgVvD4dCrNEr6RlbhJt7CQH83I0/view?usp=sharing" width="150" height="250">
</p>  

Screenshot 2
<p float="left"> 
<img src="https://drive.google.com/file/d/12x6Riwovq27eKd3impNX5URVmXQ70FQy/view?usp=sharing" width="150" height="250">
</p>  

Screenshot 3
<p float="left"> 
<img src="https://drive.google.com/file/d/1e4XqHv2Ew0CjIq3WvmJzCmBkpOQTSdyi/view?usp=drive_link" width="150" height="250">
</p>

Screenshot 4
<p float="left"> 
<img src="https://drive.google.com/file/d/15IUfsIFO5vFiCyHHxCxpqLtvv-FzWQMW/view?usp=sharing" width="150" height="250">
</p>

## Demo video

[Click here](https://drive.google.com/file/d/1x2uqiQvCm9L5NwFySi4kTJ3-Iz8p9PmJ/view?usp=sharing)
for watch demo video.
