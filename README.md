MPMessagePack
===========

Objective-C implementation for [MessagePack](http://msgpack.org/). 

# Install

[CocoaPods](http://cocoapods.org) is a dependency manager for Objective-C, which automates and simplifies the process of using 3rd-party libraries in your projects.

## Podfile

```ruby
platform :ios, "7.0"
pod "MPMessagePack"
```

# MPMessagePack

```objc
#import <MPMessagePack/MPMessagePack.h>

NSDictionary *dict =
  @{
    @"n": @(32134123),
    @"bool": @(YES),
    @"array": @[@(1.1f), @(2.1)],
    @"body": [NSData data],
  };

NSData *data = [dict mp_messagePack];
```
