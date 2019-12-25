# ObjectC_set
資料集合結構(可變與不可變)

NSset 提供了一個無序的資料集合儲存資料型態，分為可變與不可變的兩種集合。

此處示範不可變的實作

       #import <Foundation/NSSet.h>
         
       NSSet * setQ = [NSSet setWithObjects: @"fool", @"bar", nil];
       //建立物件與初始化之，結尾特別要加上 nil
       
       [setQ count];
       // 存取物件中的元素個數
       
       [setQ isEqualToSet: setK];
       // 兩集合相同，則相等，bool val 回傳 “TRUE”
       
       //不可變集合中的元素無法被修改和刪除

此處示範可變的實作

       #import <Foundation/NSSet.h>

       NSMutableSet *setM = [NSMutableSet set];
       // 沒有參數時，建立物件的方式如上
       
       NSMutableSet *setM = [NSMutableSet setWithCapacity: size];
       // 有參數時，建立物件的方式如上，以設定集合大小，也就是元素個數為其參數
       
       [setM addObject: 元素物件]
       //新增元素至物件中
       
       [setM removeObject: 元素物件];
       //刪除物件中存在的元素
       
       [setM unionSet: setPQ];
       // 將 setPQ 的元素添加到 setM
       
       

       
