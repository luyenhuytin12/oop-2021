# So sánh với mẫu chuẩn

Thành viên:

- Trần Minh Trí
- Cấn Quang Thịnh
- Luyện Huy Tín


1. Nhóm Creational (nhóm khởi tạo)

Singleton Class được khởi tạo ngay khi được gọi đến. Đây là cách dễ nhất nhưng nó có một nhược điểm mặc dù instance đã được khởi tạo mà có thể sẽ không dùng tới.
package com.gpcoder.patterns.creational.singleton;
 
public class EagerInitializedSingleton {
 
    private static final EagerInitializedSingleton INSTANCE = new EagerInitializedSingleton();
 
    // Private constructor to avoid client applications to use constructor
    private EagerInitializedSingleton() {
         
    }
 
    public static EagerInitializedSingleton getInstance() {
        return INSTANCE;
    }
}
