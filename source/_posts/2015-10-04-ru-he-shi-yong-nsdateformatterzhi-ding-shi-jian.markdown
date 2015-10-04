---
layout: post
title: "如何使用NSDateFormatter指定时间"
date: 2015-10-04 23:39:40 +0800
comments: true
categories: iOS

---
#如何指定NSDate的具体时间
```
NSString *setDateString = @"2015-01-19";
NSDateFormatter *parser = [[NSDateFormatter alloc] init];
    [parser setDateFormat:@"yyyy-MM-dd"];
NSDate *setDate = [parser dateFromString:setDateString];
```
