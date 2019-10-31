# msserialization序列化框架

参考Boost的archive编写的序列化框架：
能够较为容易的序列化/反序列化复杂的数据结构（不限于扁平数据）。

特点：
1. 小巧、纯头文件、C++模板实现，无需编译。
2. 用非侵入式设计，原有数据结构无需修改。
3. 序列化、反序列化只需要一套代码。
4. 数据结构成员发生添加或删除时，不影响其其他数据成员。
5. 可序列化常用数据类型（如字符串、bool等）、数组、容器、嵌套自定义类型。
6. 可序列化指针、智能指针。
7. 可序列化指向子类的基类指针、智能指针（需要额外编写基类到子类的适配器）。
8. 可序列化枚举类型（转为可视的字符串，需要提供枚举值和字符串对应关系）。

