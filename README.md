ios-awesome-libraries
=====================

Also in iOS, there are many awesome libraries!

[JTSImageViewController](https://github.com/jaredsinclair/JTSImageViewController)

Lightbox for iOS

[RS3DSegmentedControl](https://github.com/rsoffer/RS3DSegmentedControl)

![](https://camo.githubusercontent.com/3400bb08b831f99c1c34e340ab934be567be4ecf/68747470733a2f2f7261772e6769746875622e636f6d2f72736f666665722f525333445365676d656e746564436f6e74726f6c2f6d61737465722f73616d706c652e676966)

[pop](https://github.com/facebook/pop)

```objc
POPSpringAnimation *anim = [POPSpringAnimation animation];
...
[layer pop_addAnimation:anim forKey:@"myKey"];
```

[JGActionSheet](https://github.com/JonasGessner/JGActionSheet)

<p align="center">
<img src="https://github.com/JonasGessner/JGActionSheet/raw/master/JGActionSheet%20Tests/Screenshots/1.png" width="36.2%"/>&nbsp;
<img src="https://github.com/JonasGessner/JGActionSheet/raw/master/JGActionSheet%20Tests/Screenshots/2.png" width="48%"/></p>

[THCalendarDatePicker](https://github.com/hons82/THCalendarDatePicker)

![](https://github.com/hons82/THCalendarDatePicker/raw/master/Screenshots/Screenshot1.png?raw=true)

[SSAppURLs](https://github.com/splinesoft/SSAppURLs)

```objc
if (deviceSupportsSkype) {
    [[UIApplication sharedApplication] openAppType:SSAppURLTypeSkype 
                                         withValue:@"415-555-1212"];
}

if (deviceHasChrome) {
    [[UIApplication sharedApplication] openAppType:SSAppURLTypeChromeHTTP 
                                         withValue:@"http://www.splinesoft.net"];
}
```

[IntentKit](https://github.com/intentkit/IntentKit) - An easier way to handle third-party URL schemes in iOS apps.

![](https://raw.github.com/intentkit/IntentKit/master/example.gif)

[oxen](https://github.com/jacksonh/oxen) - Observable collection in iOS.

```objc
self.array.onCollectionChanged = ^(id<OXNChangeInfo> change) {
    self.itemsArray = change.currentArray;
    if ([change isKindOfClass:[OXNItemAddedChangeInfo class]]) {
        [self.collectionView inserItemAtIndex:[NSIndexPath indexPathForItem:change.index inSection:1]];
    }
};
```

[KeepLayout](https://github.com/iMartinKiss/KeepLayout) - Easy programmable AutoLayout.

```objc
[view keepSize:CGSizeMake(100, 200)];
[view keepInsets:UIEdgeInsetsMake(10, 20, 30, 40)];
[view keepCentered];
```

[KVOController](https://github.com/facebook/KVOController) - Super handy KVO.

```objc
FBKVOController *KVOController = [FBKVOController controllerWithObserver:self];
[KVOController observe:clock keyPath:@"date" options:NSKeyValueObservingOptionInitial|NSKeyValueObservingOptionNew block:^(ClockView *clockView, Clock *clock, NSDictionary *change) {
  // update clock view with new value
  clockView.date = change[NSKeyValueChangeNewKey];
}];
```

[ClusterPrePermissions](https://github.com/clusterinc/ClusterPrePermissions)

![](https://camo.githubusercontent.com/7eef0b117818b9da198cfc850ce21171e4b9d204/687474703a2f2f662e636c2e6c792f6974656d732f32493156315233623371334133483379337531382f6e65772d312e6a7067)

Asset
---

[LKAssetsLibrary](https://github.com/lakesoft/LKAssetsLibrary)

![](https://github.com/lakesoft/LKAssetsLibrary/raw/master/Docs/LKAssetsLibrary-Pic2.png)

Support
---

[rdotm](https://github.com/ksoichiro/rdotm) - R.java in iOS!

![](https://github.com/ksoichiro/rdotm/raw/master/testdata/images/demo.gif)

[Chameleon](https://github.com/VAlexander/Chameleon) - A Lightweight x Powerful Flat Color Framework

![](https://camo.githubusercontent.com/2a1ed77e3950ac3908283d0a23970a6e1407e463/687474703a2f2f692e696d6775722e636f6d2f4873384943744a2e706e67)

Testing
===

- [Specta](https://github.com/specta/specta) & [Expecta](https://github.com/specta/expecta)

```objc
describe(@"Foo", ^{
  beforeAll(^{
    // All asynchronous matching using `will` and `willNot`
    // will have a timeout of 2.0 seconds
    [Expecta setAsynchronousTestTimeout:2];
  });
  
  if(@"foo should be foo", ^{
    expect(@"foo").to.equal(@"foo");
  });

  it(@"will not be nil", ^{
    // Test case where default timeout is used
    expect(foo).willNot.beNil();
  });
});
```

- [OCMockito](https://github.com/jonreid/OCMockito)

```objc
NSMutableArray *mockArray = mock([NSMutableArray class]);
[mockArray addObject:@"one"];
[verify(mockArray) addObject:@"one"];

NSArray *mockArray = mock([NSArray class]);
[given([mockArray objectAtIndex:0]) willReturn:@"first"];
```

- [UI Auto Monkey](https://github.com/jonathanpenn/ui-auto-monkey)

[Screencast](http://vimeo.com/channels/trianglecocoa/54727965)
