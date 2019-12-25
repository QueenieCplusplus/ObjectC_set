# ObjectC_set
資料集合結構(可變與不可變)

NSset 提供了一個無序的資料集合儲存資料型態，分為可變與不可變的兩種集合。

此處示範不可變的實作

       #import <Foundation/NSSet.h>
         
       NSSet * set = [NSSet setWithObjects: @"fool", @"bar", nil];
       //建立物件與初始化之，結尾特別要加上 nil
       
       [集合物件 count];
       // 存取物件中的元素個數
       
       [集合物件Q isEqualToSet: 集合物件K];
       // 兩集合相同，則相等，bool val 回傳 “TRUE”

