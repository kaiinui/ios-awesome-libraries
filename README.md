ios-awesome-libraries
=====================

Also in iOS, there are many awesome libraries!

[JGActionSheet](https://github.com/JonasGessner/JGActionSheet)

<p align="center">
<img src="https://github.com/JonasGessner/JGActionSheet/raw/master/JGActionSheet%20Tests/Screenshots/1.png" width="36.2%"/>&nbsp;
<img src="https://github.com/JonasGessner/JGActionSheet/raw/master/JGActionSheet%20Tests/Screenshots/2.png" width="48%"/></p>

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
