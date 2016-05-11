# FMDBsharedInstance
多线程FMDB单例类
````objc

DataBaseHelper *he = [DataBaseHelper sharedInstance];
[he DatabaseWithDBName:@"sq.db"];

[he createTable:@"ssd1a" WithKey:@{@"a":@0,@"b":@0,@"c":@0}];
[he insertInTable:@"ssd1a" WithKey:@{@"a":@"1",@"b":@"2",@"c":@"1"}];
[he deleteInTable:@"ssd1a" WithKey:@{@"a":@""}];
[he updateInTable:@"ssd1a" WithKey:@{@"a":@""}];
NSArray * arr = [he selectInTable:@"ssd1a" WithKey:@{@"a":@0,@"b":@0,@"c":@0}];
NSLog(@"%@",arr);

````
