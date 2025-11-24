## Day1
**1.下面关于C++命名空间描述错误的是( )**
A.命名空间定义了一个新的作用域。
B.std是C++标准库的命名空间。
C.在C++程序中，命名空间必须写成using namespace std;
D.我们可以自己定义命名空间

**2.下面关于C++缺省参数描述错误的是( ) 【不定项缺省】**
A.缺省参数是声明或定义函数时为函数的参数指定一个默认值.
B.在调用有缺省参数的函数时，如果没有指定实参则采用该默认值，否则使用指定的实参
C.C和C++都支持缺省参数
D.全缺省就是参数全部给缺省值，半缺省就是缺省一半的值

**3.以下不是double compare(int,int)的重载函数的是( )**
A.int compare(double,double)
B.double compare(double,double)
C.double compare(double,int)
D.int compare(int,int)

**4.下面关于函数重载描述错误的是( )【多选择】**
A.构成函数重载的条件是函数名相同就可以
B.重载的函数参数可以相同
C.重载的函数返回值可以相同
D.C和C++都支持函数重载

## Day2
1. **在（ ）情况下适宜采用 inline 定义内联函数**
   A .函数体含有循环语句
   B .函数体含有递归语句
   C .函数代码少、频繁调用
   D .函数代码多，不常调用
   
2. **关于c++的inline关键字,以下说法正确的是( )**
   A .使用inline关键字的函数会被编译器在调用处展开
   B .头文件中可以包含inline函数的声明
   C .可以在同一个项目的不同源文件内定义函数名相同但实现不同的inline函数
   D .递归函数也都可以成为inline函数
   
3. **有一个如下的结构体：**
   ``` C++
   struct A
   {
	   long a1;
	   short a2;
	   int a3;
	   int* a4;
   };
   ```
   **请问在64位编译器下用sizeof(struct A)计算出的大小是多少？( )**
   A .24
   B .28
   C .16
   D .18
   
4. **在C++中的结构体是否可以有成员函数？( )**
   A .不可以，结构类型不支持成员函数
   B .可以有
   C .不可以，只有类允许有成员函数
   
5. **下列有关this指针使用方法的叙述正确的是（ ）**
   A .保证基类保护成员在子类中可以被访问
   B .保证基类私有成员在子类中可以被访问
   C .保证基类公有成员在子类中可以被访问
   D .保证每个对象拥有自己的数据成员，但共享处理这些数据的代码
   
6. **下面描述错误的是( )**
   A .this指针是非静态成员函数的隐含形参.
   B .每个非静态的成员函数都有一个this指针.
   C .this指针是存在对象里面的.
   D .this指针可以为空
   
7. **下列关于构造函数的描述正确的是( )**
   A .构造函数可以声明返回类型
   B .构造函数不可以用private修饰
   C .构造函数必须与类名相同
   D .构造函数不能带参数
   
8. **假定MyClass为一个类，则该类的拷贝构造函数的声明语句是( )**
   A .MyClass(MyClass x)
   B .MyClass &(MyClass x)
   C .MyClass(MyClass &x)
   D .MyClass(MyClass *x)
   
9. **在函数F中，本地变量a和b的构造函数(constructor)和析构函数(destructor)的调用顺序是: ( )**
   ``` C++
   class A;
   class B;
   void F()
   {
	   A a;
	   B b;   
   }
   ```
   A .b构造 a构造 a析构 b析构
   B .a构造 a析构 b构造 b析构
   C .b构造 a构造 b析构 a析构
   D .a构造 b构造 b析构 a析构

10. **设已经有A,B,C,D 4个类的定义，程序中A,B,C,D析构函数调用顺序为？()**
    ``` C++
    C c;
    int main()
    {
	    A a;
	    B b;
	    static D d;
	    return 0;
    }
    
    ```
    A .D B A C
    B .B A D C
    C .C D B A
    D .A B D C