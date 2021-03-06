# Note

## 目录

- [学习](#学习)
	- [HTTP协议详解](#HTTP协议详解)
  	- [请求报头](#请求报头)
  	- [php中获取请求信息](#php中获取请求信息)
  	- [http请求的几种方式](#http请求的几种方式)
  		- [http响应返回](#http响应返回)
  	- [下载文件处理](#下载文件处理)
  		- [普通下载](#普通下载)
  		- [断点续传](#断点续传)
- [PHP5](#php5)
	- [1. 新增特性](#1-新增特性 "新增特性")
		- [1.1 类的高级用法](#11-类的高级用法)
			- [1.1.1 instanceof 操作符](#111-instanceof-操作符)
			- [1.1.2 final 关键字](#112-final-关键字)
			- [1.1.3 clone 关键字](#113-clone-关键字)
			- [1.1.4 const 关键字](#114-const-关键字)
			- [1.1.5 静态成员和静态方法](#115-静态成员和静态方法)
			- [1.1.6 抽象类](#116-抽象类)
			- [1.1.7 抽象方法](#117-抽象方法)
			- [1.1.8 对象类型提示](#118-对象类型提示)
			- [1.1.9 函数调用](#119-函数调用)
			- [1.1.10 继承类实现Iterator接口](#1110-继承类实现Iterator接口)
			- [1.1.11 __autoload()方法](#1111-__autoload方法)
			- [1.1.12 foreach 函数支持引用](#1112-foreach-函数支持引用)
			- [1.1.13 Tidy扩展](#1113-tidy扩展 "Tidy扩展")
	- [2. 基础用法](#2-基础用法 "基础用法")
		- [2.1 变量](#21-变量) 
			- [2.1.1 变量的间接引用](#211-变量的间接引用 "变量的间接引用")
			- [2.1.2 管理变量](#212-管理变量 "管理变量")
			- [2.1.3 超全局变量](#213-超全局变量 "超全局变量")
		- [2.2 基础数据类型](#22-基础数据类型 "超全局变量")
			- [2.2.1 int 整型](#221-int-整型 "int 整型")
			- [2.2.2 float 浮点型](#222-float-浮点型)
			- [2.2.3 string 字符串](#223-string-字符串)
			- [2.2.4 bool 布尔型](#224-bool-布尔型)
			- [2.2.5 null](#225-null)
			- [2.2.6 resources](#226-resources)
			- [2.2.7 arrays](#227-arrays)
			- [2.2.8 常量](#228-常量)
		- [2.3 运算符](#23-运算符)
			- [2.3.1 二元运算符](#231-二元运算符)
			- [2.3.2 赋值运算符](#232-赋值运算符)
			- [2.3.3 引用赋值运算符](#233-引用赋值运算符)
			- [2.3.4比较运算符](#234-比较运算符)
			- [2.3.5 逻辑运算符](#235-逻辑运算符)
			- [2.3.6 位运算符](#236-位运算符)
			- [2.3.7 否定运算符](#237-否定运算符)
			- [2.3.8 递减/递增运算符](#238-递减递增运算符)
			- [2.3.9 错误抑制运算符](#239-错误抑制运算符)
			- [2.3.10 三元运算符](#2310-三元运算符)
		- [2.4 控制结构](#24-控制结构)
			- [2.4.1 条件控制结构](#241-条件控制结构)
			- [2.4.2 循环控制结构](#242-循环控制结构)
			- [2.4.3 代码包含控制结构](#2.4.3-代码控制结构)
		- [2.5 函数](#25-函数)
			- [2.5.1 变量作用域](#251-变量作用域)
			- [2.5.2 函数返回值](#252-函数返回值)
			- [2.5.3 声明函数的参数](#253-声明函数的参数)
	- [3. 面向对象](#3-面向对象)
		- [3.1 new关键字和构造函数](#31-new关键字和构造函数)
		- [3.2 析构函数](#32-析构函数)
		- [3.3 属性和方法](#33-属性和方法)
			- [3.3.1 public、protected、private属性](#331-public、protected、private属性)
			- [3.3.2 public、protected、private方法](#332-public、protected、private方法)
			- [3.3.3 静态属性](#333-静态属性)
			- [3.3.4 静态方法](#334-静态方法)
		- [3.4 类的常量](#34-类的常量)
		- [3.5 克隆对象](#35-克隆对象)
		- [3.6 多态](#36-多态)
		- [3.7 parent::和self::](#37-parent和self)
		- [3.8 instanceof 运算符](#38-instanceof-运算符)
		- [3.9 abstract方法和类](#39-abstract方法和类)
		- [3.10 接口](#310-接口)
		- [3.11 接口的继承](#311-接口的继承)
		- [3.12 final 方法](#312-final-方法)
		- [3.13 final 类](#313-final-类)
		- [3.14 __toString() 方法](#314-__toString()-方法)
		- [3.15 异常处理](#315-异常处理)
		- [3.16 __autoload()](#316-__autoload())
	- [4. 面向对象编程和设计模式](#4-面向对象编程和设计模式)
		- [4.1 重载性能](#41-重载性能)
			- [4.1.1 属性和方法的重载](#411-属性和方法的重载)
			- [4.1.2 使用数组语法访问的重载](#412-使用数组语法访问的重载)
		- [4.2 迭代器](#42-迭代器)
		- [4.3 设计模式](#43-设计模式)
			- [4.3.1 策略模式](#431-策略模式)
			- [4.3.2 单件模式](#432-单件模式)
			- [4.3.3 工厂模式](#433-工厂模式)
			- [4.3.4 观察者模式](#434-观察者模式)
		- [4.4 映射](#44-映射)
			- [4.4.1 映射api](#441-映射api)
			- [4.4.2 映射举例](#442-映射举例)
			- [4.4.3 使用映射执行授权模式](#443-使用映射执行授权模式)
	- [性能监控](#性能监控)
----------



# 学习

## HTTP协议详解

超文本传输协议（httpwatch工具进行抓取），是建立在 tcp/ip 协议基础上

超文本传输协议之所以叫超文本，是因为它不只可以传输文本，还可以传输音频视频等其他格式数据

所有的web开发的数据传输都是依赖于 http 协议

协议版本

     1、http 1.0 （短链接：已经放弃该协议，建立链接后数据发送之后直接断开）
     2、http 1.1 （长链接:长链接是会保持链接状态，跟服务器建立链接，如果服务器没有响应是有超时反馈的）
     
一个web页面的请求会发起多次请求，首先请求的是页面文本，之后会请求图片等一系列资源    

常识：图片的返回值是以二进制的形式返回的

## 请求报头

常用请求报头

    GET /a.html HTTP/1.1            请求类型以及请求协议版本
    Accept:*/*                      数据类型（标识发送的数据类型）
    Referer:http://www.a.com        来源地址（用处很大，经常用来做防盗链功能，服务器可以判断来源地址进行访问限制）
    Accept-Language:zh-cn           页面语言
    User-Agent:Mozilla/4.0****      浏览器内核，操作系统信息（服务器可以获取这些信息并做相应的处理）
    Accept-Enocding:gzip,deflate    数据压缩格式（就是浏览器会对发送的数据进行压缩，web服务器要有相应的格式的解压功能）
    Host:localhost:80               主机名：端口，端口是可以忽略php默认80端口，传输该数据用于 tcp/ip 解析用来做域名解析使用
    Connnection:Keep-Alive          链接状态：默认就是长链接，不会与服务器立即断开
    
    消息体（通常用来存放post数据） 
                 
## php中获取请求信息
    
```php

<?php

    $_SERVER;                			//超全局变量用来存储所有http协议发送的信息
    $_SERVER['PHP_SELF']; 				//当前正在执行脚本的文件名，与 document root相关。 
    $_SERVER['argv']; 					//传递给该脚本的参数。 
    $_SERVER['argc']; 					//包含传递给程序的命令行参数的个数（如果运行在命令行模式）。 
    $_SERVER['GATEWAY_INTERFACE']; 		//服务器使用的 CGI 规范的版本。例如，“CGI/1.1”。 
    $_SERVER['SERVER_NAME']; 			//当前运行脚本所在服务器主机的名称。 
    $_SERVER['SERVER_SOFTWARE']; 		//服务器标识的字串，在响应请求时的头部中给出。 
    $_SERVER['SERVER_PROTOCOL']; 		//请求页面时通信协议的名称和版本。例如，“HTTP/1.0”。 
    $_SERVER['REQUEST_METHOD']; 		//访问页面时的请求方法。例如：“GET”、“HEAD”，“POST”，“PUT”。 
    $_SERVER['QUERY_STRING']; 			//查询(query)的字符串。 
    $_SERVER['DOCUMENT_ROOT']; 			//当前运行脚本所在的文档根目录。在服务器配置文件中定义。 
    $_SERVER['HTTP_ACCEPT']; 			//当前请求的 Accept: 头部的内容。 
	$_SERVER['HTTP_ACCEPT_CHARSET']; 	//当前请求的 Accept-Charset: 头部的内容。例如：“iso-8859-1,*,utf-8”。 
    $_SERVER['HTTP_ACCEPT_ENCODING'];	//当前请求的 Accept-Encoding: 头部的内容。例如：“gzip”。 
    $_SERVER['HTTP_ACCEPT_LANGUAGE'];	//当前请求的 Accept-Language: 头部的内容。例如：“en”。 
    $_SERVER['HTTP_CONNECTION'];		//当前请求的 Connection: 头部的内容。例如：“Keep-Alive”。 
    $_SERVER['HTTP_HOST'];				//当前请求的 Host: 头部的内容。 
    $_SERVER['HTTP_REFERER'];			//链接到当前页面的前一页面的 URL 地址。 
    $_SERVER['HTTP_USER_AGENT'];		//当前请求的 User_Agent: 头部的内容。 
    $_SERVER['HTTPS'];					//如果通过https访问,则被设为一个非空的值(on)，否则返回off 
    $_SERVER['REMOTE_ADDR'];			//正在浏览当前页面用户的 IP 地址。 
    $_SERVER['REMOTE_HOST'];			//正在浏览当前页面用户的主机名。 
    $_SERVER['REMOTE_PORT'];			//用户连接到服务器时所使用的端口。 
    $_SERVER['SCRIPT_FILENAME'];		//当前执行脚本的绝对路径名。 
    $_SERVER['SERVER_ADMIN'];			//管理员信息 
    $_SERVER['SERVER_PORT'];			//服务器所使用的端口 
    $_SERVER['SERVER_SIGNATURE'];		//包含服务器版本和虚拟主机名的字符串。 
    $_SERVER['PATH_TRANSLATED'];		//当前脚本所在文件系统（不是文档根目录）的基本路径。 
    $_SERVER['SCRIPT_NAME'];			//包含当前脚本的路径。这在页面需要指向自己时非常有用。 
    $_SERVER['REQUEST_URI'];			//访问此页面所需的 URI。例如，“/index.html”。 
    $_SERVER['PHP_AUTH_USER']; 			//当 PHP 运行在 Apache 模块方式下，并且正在使用 HTTP 认证功能，这个变量便是用户输入的用户名。 
    $_SERVER['PHP_AUTH_PW']; 			//当 PHP 运行在 Apache 模块方式下，并且正在使用 HTTP 认证功能，这个变量便是用户输入的密码。 
    $_SERVER['AUTH_TYPE']; 				//当 PHP 运行在 Apache 模块方式下，并且正在使用 HTTP 认证功能，这个变量便是认证的类型

?>

```

## http请求的几种方式
    
PSOT、GET、HEAD、OPTIONS、DELETE、TRACE、PUT

常用有：PSOT、GET

POST和GET的区别：

    1、post的请求数据是放在http协议的消息体里边的

    2、HTTP协议本身是没有对传输数据进行限制，主要是浏览器在对get和post请求做限制

    3、get请求最多只能传输 2k+35 数据，post请求没有进行数据限制


### http响应返回

状态码：例如：200    也就是请求状态，这个参考网上的解释，其他的不再解释


图片状态304是怎么产生的呢？

浏览器发送图片请求时会检测本地是否缓存该文件如果存在该文件会请求时发送 If-Modified-Since 参数用来标识缓存时间，
web服务器端会校验浏览器发送过来的 If-Modified-Since参数，判断该文件是否和服务器上的图片时间是否一致，如果一致则不再进行图片返回直接返回 304 状态码，否则会把图片传输给浏览器，并返回 200 状态码

常见响应返回值解释

	Location:http://......
	Server:nginx    web服务器类型
	Content-Encoding:gzip    web服务器返回数据压缩使用的算法，供浏览器解码使用
	Content-Length:20121     返回的数据大小，除了数据本身的大小，还包括响应头的大小
	Content-Language:zh-cn    返回的数据语言
	Content-Type:text/html,charset=GB2312 返回的html，以及文件的编码格式。当然也可以返会的是image/jpeg 
	Content-Type:image/jpeg   当然也可以返回 image/jpeg 图片 （全部以文件mime类型来代表）
	Last-Modified:Thu, 04 May 2017 09:09:32 GMT    表示浏览器请求资源的最新时间
	Refresh:1;url=http://www.baidu.com    如果有这个返回值代表：页面响应之后会在1秒之后重定向到新的网址
	Expires:-1                下边这三个选项是一组用来控制浏览器 禁止 缓存该页面，为什么有三个？
	Cache-Control:no_cache    是因为不同的浏览器 禁止 缓存不一样，这是为了兼容不同的浏览器设置禁用页面缓存
	Pragma:no_cache            这三个选项可以兼容目前常见的浏览器
    

## 下载文件处理

### 普通下载


```php

<?php
	
	//正常服务器在接收到客户端请求时会做出如下处理
    $file_name = "测试.jpg";
        
    //php读取文件名时不支持中文，所以需要对中文名称进行转码（文件名默认需要使用 gb2312 的编码）
    $file_name = iconv('utf-8', 'gb2312', $file_name);        

    if (!file_exists($file_name)) {
        echo "文件不存在";
        exit;
    }
        
    //获取文件大小，以字节为单位
    $file_size = filesize($file_name);
        
    //打开文件,可读方式打开
    $file = fopen($file_name, 'r');
        
    //返回数据给浏览器
    //下载文件需要的头
    header("Content-type: application/octet-stream"); //告知浏览器返回的是流文件的形式
    header("Accept-Ranges: bytes");    //按字节返回文件内容
    header("Accept-Length: $file_size"); //返回文件大小
    //这里可以设置浏览器端下载窗口所显示的文件名称
    header("Content-Disposition: attachment; filename=". $file_name);
        
    //定义缓冲区大小,字节为单位
    $buffer_size = 1024; 
        
    //为了保证 feof($file) 的可用性，可以考虑做一个文件字节读取计数器
    $file_count = 0;
        
    //向客户端循环发送数据，这样可以避免瞬间压力， feof用来判断文件指针是否到结尾
    while( !feof($file) && (($file_size - $file_count) > 0)){
        $buffer_data = fread($file, $buffer);
        $file_count += $buffer;
        //把部分数据回送给浏览器
        echo $buffer_data;
    }
        
    fclose($file);
?>

```

### 断点续传
    
```php

<?php

/** php下载类,支持断点续传
 *  Date:  2013-06-30
 *  Author: test
 *  Ver:  1.0  *
 *  Func:
 *  download: 下载文件
 *  setSpeed: 设置下载速度
 *  getRange: 获取header中Range
 */
class FileDownload
{
    // class start
    private $_speed = 512;  // 下载速度

    /** 下载
     * @param String $file 要下载的文件路径
     * @param String $name 文件名称,为空则与下载的文件名称一样
     * @param boolean $reload 是否开启断点续传
     */
    public function download($file, $name = '', $reload = false)
    {
        if (file_exists($file)) {
            if ($name == '') {
                $name = basename($file);
            }
            $fp = fopen($file, 'rb');
            $file_size = filesize($file);
            $ranges = $this->getRange($file_size);
            header('cache-control:public');
            header('content-type:application/octet-stream');
            header('content-disposition:attachment; filename=' . $name);
            if ($reload && $ranges != null) {
                // 使用续传
                header('HTTP/1.1 206 Partial Content');
                header('Accept-Ranges:bytes');
                // 剩余长度
                header(sprintf('content-length:%u', $ranges['end'] - $ranges['start']));
                // range信息
                header(sprintf('content-range:bytes %s-%s/%s', $ranges['start'], $ranges['end'], $file_size));
                // fp指针跳到断点位置
                fseek($fp, sprintf('%u', $ranges['start']));
            } else {
                header('HTTP/1.1 200 OK');
                header('content-length:' . $file_size);
            }
            while (!feof($fp)) {
                echo fread($fp, round($this->_speed * 1024, 0));
                ob_flush();
                //sleep(1); // 用于测试,减慢下载速度
            }
            ($fp != null) && fclose($fp);
        } else {
            return '';
        }
    }

    /** 设置下载速度
     * @param int $speed
     */
    public function setSpeed($speed)
    {
        if (is_numeric($speed) && $speed > 16 && $speed < 4096) {
            $this->_speed = $speed;
        }
    }

    /** 获取header range信息    
     * @param int $file_size 文件大小    
     * @return Array 
     */
    private function getRange($file_size)
    {
        if (isset($_SERVER['HTTP_RANGE']) && !empty($_SERVER['HTTP_RANGE'])) {
            $range = $_SERVER['HTTP_RANGE'];
            $range = preg_replace('/[\s|,].*/', '', $range);
            $range = explode('-', substr($range, 6));
            if (count($range) < 2) {
                $range[1] = $file_size;
            }
            $range = array_combine(array('start', 'end'), $range);
            if (empty($range['start'])) {
                $range['start'] = 0;
            }
            if (empty($range['end'])) {
                $range['end'] = $file_size;
            }
            return $range;
        }
        return null;
    }
}

?>

```
    


# PHP5

## **1. 新增特性**

## 1.1 类的高级用法

### 1.1.1 instanceof 操作符

    instanceof 用于确定一个 PHP 变量是否属于某一类 class 的实例

### 1.1.2 final 关键字

```php

//用来标识方法，使其不能被子类重载
class MyClass {
    final function method() {}
}

//用来标识类，使其不能被继承
final class MyClass {
}
class ExtendClass extends MyClass {
    //这个地方不能继承一个被final修饰的类
}

```

### 1.1.3 clone 关键字

```php

//你可以再类中声明一个__clone()方法，它将在克隆过程中被调用（调用的过程，在属性和方法从源对象复制过来以后进行）

class MyClass {
    function __clone() {
        echo "对象正在被克隆";
    }
}
$obj = new MyClass();

$obj_copy = colne $obj; //克隆一个对象


```

### 1.1.4 const 关键字

```php

//用来定义在类中使用的常量(注意：在类中使用常量的时候都要使用这个)
class MyClass {
    const SUCESS = "Sucess";
}
print MyClass::SUCESS

```

### 1.1.5 静态成员和静态方法

```php

//类的定义现在包含静态成员（属性），可以通过类自身来访问。通常用的最多的是单例模式
class Singleton {
    //静态成员
    static private $instance = NULL;
    //单例模式通常也定义 __clone方法,防止通过外部克隆当前类
    private function __clone(){
    }
    //私有的构造类，保证外部无法访问
    private function __construct() {
    }
    //静态方法
    static public function getInstance() {
        if (self::$instance == NULL) {
            self::$instance = new Singleton();
        }
        return self::$instance;
    }
}

```

### 1.1.6 抽象类

```php

//把类声明为抽象类可以防止它被实例化。但是你可以继承一个抽象类：
abstract class MyBaseClass{
    function display(){
        print "测试";
    }
}

	
```

### 1.1.7 抽象方法


```php

//把方法声明为抽象，以便在继承的子类中再去定义。包含抽象方法的类本身必须是一个抽象类：
abstract class MyClass{
    abstract function display();
}

```


### 1.1.8 对象类型提示
    
    
```php

//函数声明中可以对参数进行对象类型提示。如果函数调用的时候没有传递正确的对象类型，系统会报错
class MyClass() {
}
function expectsMyClass(MyClass $obj) {
    //也就是这个对象必须是指定的MyClass对象的实例
}

```

### 1.1.9 函数调用

```php

//PHP4
$dummy = $obj->method();
$dummy->method2();

//PHP5开始支持链式函数调用
$obj->method()->method2();

```
### 1.1.10 继承类实现Iterator接口

```php

//PHP5允许PHP类和PHP继承类实现Iterator接口。在实现迭代接口后，你可以用foreach语言结构遍历一个类的实例：

$obj = new MyTteratorImplementation();
foreach($obj as $value) {
    print "$value";
}

```


### 1.1.11 __autoload方法

在PHP5中，你可以定义一个__autoload()函数，它在你需要使用一个未定义类的时候自动调用。通过调用这个函数，脚本引擎在PHP抛出类未定义的错误之前提供最后一次加载类的机会：

```php

function __autoload($class_name) {
    include_once($class_name."php");
}
$obj = new MyClass1();
$obj2 = new MyClass2();

//PHP5同样新增了try/throw/catch 架构的异常处理规范。使用时，你只能抛出从Exception 类继承的对象：
class SQLException extends Exception {
    public $problem;
    function __contruct($problem) {
        $this->problem = $problem;
    }
}

try {
    throw new SQLException("Couldn't connect to database");
} catch (SQLException $e) {
    print "";
} catch (Exception $e) {

}

```


### 1.1.12 foreach 函数支持引用

```php

foreach ($arr as $key => $value) {
    $new_value = array('name' => 3);
    $arr[$key] = $new_value;
}
//在循环中使用引用改变value的值更简洁
foreach ($arr as $key => &$value) {
    $value = array('name' => 3);
}

//给引用参数设置默认值

//你可能认为只有 传递值的参数可以设置默认值，现在PHP5中也可以给引用参数设置默认值
function my_func(&$arg = null) {
    if ($arg == null) {
        print '$arg is empty';
    }
}
my_func();

```

### 1.1.13 新增SOAP支持

SOAP 是一种简单的基于 XML 的协议，它使应用程序通过 HTTP 来交换信息。在我们的 SOAP 教程中，你将了解到什么是 SOAP，以及它如何在应用程序之间交换信息。


### 1.1.14 Tidy扩展

用于修复和美化html

----------


## **2. 基础用法**
----------
## 2.1 变量


### 变量的间接引用

```php

//变量的间接引用使用两个 $ 符号
$name = "John";
$$name = "user";
print $John;  //这个变量被定义是因为上一行的间接引用 使得这个变量生效
//通过在变量的前面增加附加的 $ 标记，你可以任意增加引用次数
$$$name = 'user1';
print $user; //这个变量也会被定义

```

### 管理变量

#### *isset()*
    
isset()用来判断某个变量是否已经声明。它返回一个布尔值。

如果变量已经被设置就返回true,反之返回false，或者当变量的值被设定为NULL的时候，它也返回false.
    
isset($var1, $var2, $var3); //isset可以一次判断多个变量是否设置

`注意：检查多个变量时，它只有在所有变量都定义了的情况下才返回 true,否则将返回false。`


#### *unset()*
    
unset()可以 取消之前定义的变量，而且如果没有其他变量在引用它的话，就会释放这个变量使用的所有内存空间。调用isset()来检查一个被 

unset()处理过的变量的话，会返回false.
    
例如：

```php

$name = "test";
unset($name);
if (isset($name)) {
    print 'test';
}
//这个例子不会生成任何输出。
//unset还可以用来检查数组的元素和对象的属性，就跟isset()一样。

```
    
    
#### *empty()*
    
empty()可以用来检查一个变量是否没被声明或者值是false。这个语言结构通常被用来检查一个表单变量是否未被发送或者包含数据。当检查一个变量的值是否为真的时候，它的值会首先被转变一个布尔型的值，再检查是否为真。



### 超全局变量
    
作为一般的规律，php不支持全局变量，但是，一些PHP的特定内部变量可以像其他语言的全局数组一样运行。这些变量称为超全局变量，而且PHP预定了这些变量让你使用。这些超全局变量的一些列子：

`$_GET`、`$_POST`、`$_COOKIE`、`$_ENV`、`$_SERVER`


## 2.2 基础数据类型

PHP中使用了 `8种` 数据类型，其中有5种是数量型的。同时剩下的三种数据类型有着自己的独特性。

### int 整型
 
32位带符号数字    范围 -2147483648 到 +2147483647

### float 浮点型
    
8个字节     范围 2.2E-308 到1.8E+308    浮点型数字包含一个小数点，而且可以包含一个 +/- 号，并且可以是一个指数值

### string 字符串
    
指一序列的字符并且自动地用null做结束的组合。
`注意：字符串在使用过程中的单双引号问题`
    
#### *双引号*
字符串可以包含非常多的字符。特殊字符的话不用它原来的样子来表示，要用特殊符号表示。注意字符串也可以作为数组的结构来处理

例如：

|语法|效果|
|----|-----|
|`\n`|换行|
|`\t`|制表符|
|`\"`|双引号|
|`\\`|反斜线|
|`\0`|ASCII0(null)|
|`\r`|回到行的开始处|
|`\$`|对$符号进行转义，就不会当成变量处理，而只是一个字符|
|`\{Octal #}`|用八进制写的字符，例如 \70表示字母 8|
|`\x{Hexadecimal #}`|用十六进制写的字符，例如 \0x32表示字母 2|
    
双引号字符串的一个附加特性是一些特定的符号，如变量或表达式，可以直接嵌入使用。

例如：

"The result is $result \n"    这里 \n 用来处理换行

"The array offset $is contains $arr[$i]" 注意这里可以直接解析 $arr 数组

#### *单引号*

除了双引号，单引号也可以用来划定字符串。但是，与双引号不一样的是，单引号不支持双引号所有转义和变量替换的功能。

单引号所支持的仅有两个字符转义：单引号（\'）和反斜杠（\\）,当你需要在一个单引号前面输入反斜杠的时候就必须使用双斜杠
    
#### *定界符*

用来在脚本中嵌入大篇幅的文本，其中还可能包含许多双引号和单引号，使用定界符的时候就不需要再去转义。

这个字符串以 <<< 符号开始，紧跟着的字符串（THE_END）在你的文本中不能出现。

他使用开始的字符串标记结束整个文档，（结束字符串）这个字符串必须定格写，或者加上分号，同时你需要加上换行符（\n）.

定界符对于字符转义和变量替换的支持与双引号基本相同。不同的是，你在定界符中不需要去转义双引号。
   	
例如：
	    
```php

$str = <<<THE_END
    ASDFASDFASDF
    ASDFSDAFDASFFASFADSFDDASFASDFASF
THE_END;

```
#### *访问字符串中的字符*

字符串中的单个字符可以通过使用$str{offset}或者$str[offset] 符号访问。

你可以用它读取和写字符串该位置的字符。

当读取操作的时候，这个字符串只能用已经存在的索引来读取。

如果是修改字符串，~~你可以访问还未存在的索引~~（$i = '012'; $i[3] = '3';）这是不会报错的。

PHP会自动为修改的字符设置偏移量索引，而且如果你设置的索引与字符串中最后一个索引有差距，

PHP会自动用空格字符（''）把这中间的缺口不上。
    
`注意[]访问方式是在PHP4中的用法，在PHP5中最好使用{}，防止无法区分是字符操作还是数组操作`

例如：

```php

$a = '11111';
$i = 10;
$a[$i] = 2;
echo $a;
//会输出  '11111 2'   注意中间补白的空格；

```
 
`提示：在许多情况下，PHP中使用字符串处理函数实现有效的运算。你在直接使用偏移量访问字符串之前最好了解一些这些函数。通常使用 str_ 开头。如果是复杂的字符串操作，那就要用到正则表达式了尤其是pcre_函数族`



### bool 布尔型

范围: true 和 false    经常用来判断真假运算

### null

范围：只能有一个值的数据类型（NULL值）它表示变量的值是空的，而且他在区分空字符串和数据库的null值的时候非常有用。

### resources
    
范围：一种特殊的数据类型（资源），用来表示一种PHP的外部资源，例如：数据库访问、文件、数据库连接等
    
`注意：你永远无法直接操作这种类型的变量，但是可以把它们传递给相对应的函数，那些函数知道如何与这些特殊类型的数据进行交互。`
    
### arrays

数组：一种 键值对 的集合，可以关键字或者索引映射到值。数组索引可以是整形数或者字符串，但是它的值可以是任何一种类型

数组可以用 array() 语言结构来声明，通常使用如下形式(方括号中的元素 key 是可选的，可以没有key)：

array([key=>] value, [key=>] value) 

关键字是可选的，而且如果没有指定它的值的话，关键字会自动赋值。赋值的方法是按照自增的数字来命名（从0开始），你也可以部分使用关键字而其他部分不用关键字这样混合声明一个数组。

`注意：PHP中的数组是使用哈希表构建的，这意味着访问每一个值都是O(1)复杂度`

	    
array("1", 3=>'2', '3', '4')    	//输出  Array ( [0] => 1 [3] => 2 [4] => 3 [5] => 4 )
	
array("1", 'name'=>'2', '3', '4') 	//输出 Array ( [0] => 1 [name] => 2 [1] => 3 [2] => 4 )
	

混合使用时自增的 key 会根据手工设置 key 的地方判断从哪个值自增，上边两个案例已经说明问题
    
#### *数组的访问和修改*
```php
$arr1 = array(1, 2, 3);

$arr2[0] = 1;

echo $arr2[0];

//当然有更多用法不再解释，请参考文档
```
#### *追加数组的特殊用法*

$arr2[] = 2;

它的key根据之前的key进行自增

#### *访问嵌套数组*

$arr[key][key].... 根据层数选择使用多少个方括号来访问


#### *使用 foreach 遍历数组*

循环的大概语法如下：

```php
foreach($array as [$key =>] [&] $value){
    //....
}
```

$key是可选的，而且如果设置的话，它将包含当前所有遍历的值的关键字，它的类型依据数组内的关键字的数据类型而定。
设置 & 符在值的前面也是可选的，你在想更改 $value 的值，并在 $array 中也生效的时候，你需要使用它。
大多数情况下，你不需要在遍历数组的时候修改 $value 的值，所以就不需要设置。

#### *使用 list() 和 each() 遍历数组*

foreach()是一个遍历数组的很好的方法，同时还有一种遍历数组的方式就是用list()结构和each的函数组合：  

```php
$players = array('1', '2', '3');
reset($players); //将数组内部的指针指向第一个单元，使用each之前一定要使用reset使指针指向第一个单元
while( list($key, $val) = each($players) ){
    echo $key.'='.$val;
}
```

each 函数返回当前的键值对并且把内部指针向下一个元素。当它到达数组尾部的时，会返回一个 flase 的布尔值。

键值对是以一个数组返回的返回的结构 Array ( [1] => 28 [value] => 28 [0] => john [key] => john )。

之所以要返回一个副本是因为你要单独访问他们，可以使用 $elem['key']和$elem['value']来访问.

例如：

```php

$ages = array('john' => 28, 'bar' => 67);
reset($ages);
$person = each($ages);  //返回 Array ( [1] => 28 [value] => 28 [0] => john [key] => john )
//可以有两种访问方式
$name = $person['key'];
$name = $person[0];

```

#### *reset()*

php中的遍历是通过使用一个内置的数组指针来跟踪遍历到当前位置实现的。与 foreach() 不同的是，在你使用 each() 来遍历一个数组之前，

必须先使用 reset() 函数来处理数组。所以最好是使用 foreach 来遍历数组，尽量避免使用敏感的涉及到指针操作的 each 遍历

#### *each()*

each() 函数返回当前的键值对并且把内部指针指向下一个元素。当它到达数组的尾部的时，会返回一个false的布尔值。键值对是以一个数组返回

的，数组包含4个元素：元素 0 和 “key” ，存放的是关键字；元素 1 和 “value”, 存放的是该值的具体数值。之所以要创建一个副本是因为如

果你要单独访问他们，可以使用 $elem["key"] 和 $elem["value"] 来访问

Array ( [1] => 28 [value] => 28 [0] => john [key] => john )
       
`注意：这里我也觉得奇怪，为啥不返回一份节省空间还要再返回 0 和 1 两个key，在看完 list() 结构如何工作之后，才明白`

#### *list()*

list()结构用来把多个数组偏移量赋值给多个变量，而且通过一个语句实现

list($var1, $var2,....) = $array;

列表中的第一个变量赋值的数组中偏移量为 0 的值，第二个变量赋值的是偏移量为 1 的值，以此类推。因此，list() 结构的功能可以转化为下

面的PHP语句序列：

$var1 = $array[0];
$var2 = $array[1];

就像先前提到的， each() 返回的索引 0 和 1 是让 list() 结构使用的。你可能已经猜到 list() 和 each() 是如何协同工作的。

分析先前的 $players 遍历的例子中 while 循环：

`while( list($key, $val) = each($players) )`

while 在每一次循环遍历的时候， each 函数返回当前位置的键值对的数组，如果用print_r检测的话，数组的值如下：

Array ( [1] => 28 [value] => 28 [0] => john [key] => john )

然后 list() 函数把该数组中偏移量是 0 的值赋给 $key, 把偏移量是 1 的值赋给 $val

### 常量

常量顾名思义就是一旦定义就不能修改。常量命名的规则和变量一样，只是不用加 $符号。在许多编程语言中，大写字母来命名常量是普遍的做法

`提示：只有使用大小写敏感的常用才能与公认的代码标准相一致，特别注意PHP目前是不区分大小写的`

常量一旦定义是可以全局访问的，你不可以在其他新的函数或者PHP文件中再次声明他们

使用 define() 函数定义常量：

define("CONSTANT_NAME", value [, case_sensitivity]);

CONSTANT_NAME 是常量名称

value 可以是任何合法的PHP表达式，包括数组和对象。

case_sensitivity 是一个布尔值，可选，默认是 FLASE（区分大小写）,如果设置为 TRUE（不区分大小写）

例如：

```php
//这样使用是会报错的
define("Cont", 'test');
echo cont;

//这样使用是可以的
define("Name", 'test', TRUE);
echo name;

```
PHP内置的布尔值常量是一个很好的列子，它被定义为不区分大小写，这样我们在写的时候可以随意选择 TRUE 或者 true, FALSE 或者 false


## 2.3 运算符

php包含了三种类型的运算符：`一元运算符`、`二元运算符`、`三元运算符`

php仅能执行运算符来计算数据类型一致的两个操作数。但是，如果两个操作数的数据类型不同，php会自动把其中一个操作数的数据类型转变为另

一种数据类型，转变规则如下


| 其中一个操作数 | 另一个操作数 | 执行转换 |
|----|-----|-----|
| `整型` | 浮点型 | 整型操作数将被转变为浮点型数字 |
| `整型` | 字符串 | 字符串将被转换成数组。如果字符串转换过来的是 real 数据类型，整型数字也会被转换为 real 数据类型 |
|`Real型（例如：3.40E + 38）`| 字符串 | 字符串会被转变为 real 数据类型 |

布尔型、null和资源执行起来类似整型，所以他们按照下面的方式转变

Boolean: False = 0, True = 1
Null = 0
Resource = The rescource's #(id) //也就是资源ID号

### 2.3.1 二元运算符

#### *算术运算符*

所有的二元运算符（除了串联运算符）只计算数字操作数。如果两个操作数中有一个或全部是字符串、布尔值、null、资源，他们将被自动转变为

相应的数字（根据前面的表格），然后运算再被执行。


| 运算符 | 名字 | 值 |
|-----|-----|-----|
| `+` |  加 | 两个操作数的和 |
| `-` |  减 | 两个操作数的差 |
| `*` |  乘 | 两个操作数的乘积|
| `/` |  除 | 两个操作数的商 |
| `%` |  模 | 两个操作数都被转变成整型，结果是第一个操作数除第二个操作数的余数 |

#### *串联运算符*

串联运算符（.）把两个字符串串联起来。这个运算符只处理字符串； 因此，任何非字符串的操作数将会被首先转变为字符串。

下面的例子将打印出 "The year is 2000"
$year = 2000;
echo "The year is " . $year;

### 2.3.2 赋值运算符

赋值运算符让你把一个值写入一个变量。第一个操作数（赋值运算符值左边的操作数或者叫左值）必须是一个变量。

赋值表达式的值是赋给变量的最后的值；

例如，表达式 $var = 5 的值 5 （把 5 赋给 $var）

除了正常的赋值运算符，还有其他一些把运算符加上等于号组成的复合运算符。这些复合运算符的作用是把运算符左边的变量作为第一个操作数和右

边的操作数（右值）进行运算然后把运算结果赋值给左边的变量。

例如：

$counter += 2; //这与 $counter = $counter + 2 是同样的
$offset *= $counter; //这与 $offset = $offset * $counter 是同样的

下面的列表显示了正确的组合赋值运算符

|  运算符 | 等价 |
|  ----- | -----|
|  `+=`  |  $a = $a + 2 |
|  `-=`  |  $a = $a - 2 |
|  `*=`  |  $a = $a * 2 |
|  `/=`  |  $a = $a / 2 |
|  `%=`  |  $a = $a % 2 |
|  `.=`  |（拼接字符串）$a = $a . 'name' |
|  `^=`  |（按位异或）$a = 12 ^ 9 |
|  `&=`  | （按位与）$a = 12 & 9 |
|  `|=`  | （按位或）$a = 12 | 9 |
|  `<<=` |（左移） |
|  `>>=` |（右移） |

### 2.3.3 引用赋值运算符

使用 & 来操作

例如：

$name = "Judy";
$name_alias =& $name;

### 2.3.4 比较运算符

|  运算符 | 名字 | 值 |
|  ----- | ----- | ----- |
|  `==`  |  等于   | 检查两个操作数是否相等，由于php是类型自动转换的，所以 1 == "1" 和 1 == 1 等价 |
|  `!=`  |  不等于 | 与 == 相反 |
|  `>`  | 大于 ||
|  `>=`  | 大于等于 ||
|  `<`  | 小于 ||
|  `<=`  | 小于等于 ||

比较特殊的两个运算符

=== 全等于	与等于相似，但是不会进行变量类型转换，会在比较值的同时比较变量的类型是否相同

!== 全不等	与 === 相反

### 2.3.5 逻辑运算符

逻辑运算符首先把它们的操作数转变为布尔型的值，然后进行相应的比较操作

|  运算符 | 名字 | 值 |
|  ----- | ----- | ----- |
|  `&&,and`  |  逻辑与   |  |
|  `||,or`  |  不等于 | 与 == 相反 |
|  `xor`  | 逻辑异或 ||


短评估时间

php在处理逻辑运算的时候，会从左向右一次判断，例如， 0 && 1 的时候，它只需要检查左边就能得到结果。

所以可以在写程序逻辑的时候，把优先判断的条件放到最左边，这样可以节省逻辑判断时间

### 2.3.6 位运算符

想到位运算就头疼，官方的垃圾文档总是理解起来太扯淡，所以自己研究了一下

`特此说明：以下运算都是在转换成二进制的状态下进行的`

#### *按位异或*

12 ^  9 按位异或的结果为 5

12 的二进制：1100

9 的二进制： 1001

5 的二进制 ： 101

从上面可以明显看出你只需要按照两个数字每一位进行（切记从右往左依次判断）按位异或

按位异或又是什么意思？ 异或也叫半加运算，其运算法则相当于不带进位的二进制加法：二进制下用1表示真，0表示假，则异或的运算法则为：

0⊕0=0，1⊕0=1，0⊕1=1，1⊕1=0（同为0，异为1），这些法则与加法是相同的，只是不带进位（也就是 1 + 1 不再等于 2）

所以按位异或的计算方式的要点就是：按照两个数字的二进制位进行对照相加，同一个位置的，两个数相同结果为0，两个数不同结果为1，得到的

数字转换成十进制就是计算结果

12 ^ 9 = 5 运算过程就是

|  十进制 | 二进制 |
|  ----- | -----|
|  `12 的二进制`  |  1 1 0 0 |
|  `相同的相加为0，不同的相加为1`  |  ++++ |
|  `9 的二进制`  |  1 0 0 1 |
|  `5 的二进制`  |  0 1 0 1 |

#### *按位与*

12 & 9 按位与 的结果为 8

12 的二进制：1100

9 的二进制： 1001

5 的二进制 ：1000

从上面可以明显看出你只需要按照两个数字每一位进行（切记从右往左依次判断）按位与

按位与又是什么意思？ 参与运算的两数各对应的二进制位相与。只要对应的二个二进制位都为1时，结果位就为1。参与运算的两个数均以补码出现。

12 & 9 = 8 运算过程就是

|  十进制 | 二进制 |
|  ----- | -----|
|  `12 的二进制`  |  1 1 0 0 |
|  `相同的相加为1，不同的相加为0`  |  ++++ |
|  `9 的二进制`  |  1 0 0 1 |
|  `8 的二进制`  |  1 0 0 0 |


#### *按位或*

12 | 9 按位或  的结果为 13

12 的二进制：1100

9 的二进制： 1001

13 的二进制：1101

从上面可以明显看出你只需要按照两个数字每一位进行（切记从右往左依次判断）按位与

按位与又是什么意思？参与运算的两数各对应的二进位相或。只要对应的二个二进位有一个为1时，结果位就为1。当参与运算的是负数时，参与两个

数均以补码出现。

12 & 9 = 13 运算过程就是

|  十进制 | 二进制 |
|  ----- | -----|
|  `12 的二进制`  |  1 1 0 0 |
|  `相同的相加为1，不同的相加为0`  |  ++++ |
|  `9 的二进制`  |  1 0 0 1 |
|  `13 的二进制`  |  1 1 0 1 |


12 & -9 = -1 运算过程就是


|  十进制 | 二进制 |
|  ----- | -----:|
|  `12 的二进制`  |  1 1 0 0 |
|  `相同的相加为1，不同的相加为0`  |  ++++ |
|  `-9 的二进制`  |  11111111 11111111 11111111 11110111 |
|  `-1 的二进制`  |  11111111 11111111 11111111 11111111 |



这里会涉及到补码的问题。关于补码的计算简单解释一下

二进制原码 ---> 取反码 ---> 加1 -> 得到补码

所以求 -9 的二进制的步骤为：

求 9 的二进制表示  00001001

原码取反（所有二进制位取反） 11110110

加1得到补码   11110111

因为是32位 所以前边补 24个1

得到 11111111 11111111 11111111 11110111

#### *按位取反*

这里刚好使用到上边的补码原理

~ $a

12 按位或  的结果为 -13

12 的二进制：00000000 00000000 00000000 00001100

按位取反：   11111111 11111111 11111111 11110011

-13的二进制：11111111 11111111 11111111 11110011


-3 按位或  的结果为 2

上面是-3按位取反后得到2，我们用上面的理论来分析一下：

因为负数的二进制要使用补码进行表示所以要先进行如下处理：

源码：1000 0000 0000 0000 0000 0000 0000 0011

反码：1111 1111 1111 1111 1111 1111 1111 1100

补码：1111 1111 1111 1111 1111 1111 1111 1101 （反码加1得到补码）

现在执行按位取反操作后：

由 -3 的补码进行取反操作得到

补码：0000 0000 0000 0000 0000 0000 0000 0010
反码：0000 0000 0000 0000 0000 0000 0000 0010
源码：0000 0000 0000 0000 0000 0000 0000 0010

#### *位移运算符*

移位运算符就是在二进制的基础上对数字进行平移。

按照平移的方向和填充数字的规则分为三种：`<<`（左移）、`>>`（带符号右移）和 `>>>`（无符号右移）。

在移位运算时，byte、short和char类型移位后的结果会变成int类型，对于byte、short、char和int进行移位时，规定实际移 动的次数是移动

次数和32的余数，也就是移位33次和移位1次得到的结果相同。

移动long型的数值时，规定实际移动的次数是移动次数和64的余数，也就 是移动66次和移动2次得到的结果相同。

#### *左移*

按二进制形式把所有的数字向左移动对应的位数，高位移出（舍弃），低位的空位补零

6144 = 12 << 9

所有位置整体向左移动 9 位

00000000 00000000 00000000 00000000 00001100

移动 9 次之后得到下边的结果

00000000 00000000 00000000 00011000 00000000

将 12 中的二进制位向左移动 9 次（每一次移动都表示“乘以 2”）


3072 = 12 << 40

所以位移 40 次的真实位移次数是 40 % 32 进行取余，得到真实的移动次数为 8 次

00000000 00000000 00000000 00000000 00001100

移动 8 次之后得到下边的结果

00000000 00000000 00000000 00001100 00000000

#### *右移*

右移的原理跟左移类似，可以参考官方文档


### 2.3.7 否定运算符

PHP否定运算有两个 ! （逻辑非） 和 ~ 按位非

### 2.3.8 递减/递增运算符

#### *数字递增*

$var++ 后加

++$var 前加

$var-- 后减

--$var 前减

#### *字符串递增*

```php

$a = 'a';
$a++;
//输出 b
echo $a;
$a = 'z';
$a++;
//输出 aa
echo $a;

$name = 'name1';
$name++;
//输出 name2
echo $name;

$name = 'name9';
$name++;
//输出 name2
echo $name;

```

#### *类型转换字符串*

PHP提供了类似C的方法类型转换字符串，强制一个数值进行数据类型转换。操作数写在该运算符的右边

$str = "5"; $num = (int)$str;

### 2.3.9 错误抑制运算符

@file_get_contents() 加上@符之后可以抑制错误报出

### 2.3.10 三元运算符

$a = 99;

$message = isset($a) ? 1 : 0;

会根据是否设置 $a 变量来选择输出 1 还是 0； 

## 2.4 控制结构

### 2.4.1 条件控制结构

#### *if语句*

```php

if () {
....
} else {

}

if () {

} elseif () {

} 

//在html中混合输出
<?php if(): ?>

<?php elseif():?>

<?php elseif():?>

<?php endif;?>

```

#### *switch语句*

switch用来替换某些条件分支特别多的 if 语句，语法不再叙述

### 2.4.2 循环控制结构

#### *while循环*

最简单的循环，跟其他语言的循环一样不再叙述

#### *do while循环*

最简单的循环，跟其他语言的循环一样不再叙述

#### *for 循环*

最简单的循环，跟其他语言的循环一样不再叙述

### 2.4.3 代码包含控制结构

#### *include语句和类似语句*

PHP使用 include语句可以把代码切割到多个文件中。分离代码到多个文件是为了优化结构

被包含的文件与包含文件的变量作用域一致（除了被包含文件中函数里的变量作用域）

用法：

include "/file.php";

尽量保持相对路径，这样可以保证项目移植的时候不会有影响

incluede $_SERVER["DOCUMENT_ROOT"] . "/file.php";

包含文件另外一种方式 require，它和 include 的区别在于 require 在遇到错误代码的时候会停止代码执行，而 include 在遇到代码

错误的时候不会停止执行

include_once 和 require_once 顾名思义是只加载一次文件，后边再加载会报错
 
#### *eval()*

eval 和 include 类似，但是与编译并执行包含进来的代码不同的是，它把代码当作字符串包含进来再执行。这个功能对于运行动态生成的

代码或者从外部数据源手动获取代码然后执行是非常有用的。由于效率低下，不建议使用

`提示：由用户的输入赋值的变量永远不要直接传递给 eval(),因为这样会让用户执行任意的代码`

## 2.5 函数

```php

function function_name(arg1, agr2, ...)
{
	$arg1	
}

```

### 2.5.1 变量作用域

函数中的变量作用域只限于本函数内，但是可以使用 $GLOBALS[]数组来访问脚本全局作用域中的变量

```php

function function_name()
{
	$GLOBALS["var"] = 2;
}

$var = 1;

function_name();
//将会输出 2
echo $var;

```

或者使用 `global` 关键字也可以声明哪些外边变量在函数内是可以使用的，但是，不推荐这样用因为会出现混乱而且`不支持 unset()`

```php

function function_name()
{
	global $var;
	$var = 2;	
$GLOBALS["var"] = 2;
}

$var = 1;

function_name();

//将会输出 2
echo $var;

```

### 2.5.2 函数返回值

#### *通过引用返回值*

```php

function &get_global_variable($name)
{
	return $GLOBALS[$name];
}

$num = 10;
$value =& get_global_variable("num");
//输出 10
print $value."\n";
$value = 20;
//输出 20
print $num;

```

你可以看到 $num 在修改了 $value 以后被成功的修改了，这是因为 $valued 是通过引用指向全局变量 $num 但是，很少会这样用因为
出了bug很难排查

### 2.5.3 声明函数的参数

#### *传递值的参数*
```php
function pow($x, $y)
{
...
}
pow(2, 3)
```
#### *传递引用的参数*
```php
function pow(&$n)
{
	$n = $n*$n;
}
$number = 4;
pow($number);
print $number;
```
虽然没有返回值，但是使用的是传递引用的方式，所以外部的$number 的值会被修改为 16

#### *函数默认参数*

初始化声明好的参数

function pow($a = 1, $b = 2)
{
}

`注意：当你调用一个有默认值的函数的时候，如果你忽略了这个默认函数参数，你也将忽略接下来的所有参数。`

#### *可变数量的参数列表*

```php

```

## **3. 面向对象**

## 3.1 new关键字和构造函数

```php

class Person {
	private $name;
	//构造函数会在new一个类的时候最先执行这个方法
	function __construct($name)
	{
		$this->name = $name;
	}
	function getName()
	{
		return $this->name;
	}
}

//new关键字初始化一个类
$judy = new Person("Judy");

echo $judy->getName();

```
`注意：因为一个构造函数不能返回值，所以从构造函数内产生一个错误最常用的做法就是抛出一个异常`

## 3.2 析构函数

析构函数与构造函数的作用刚好相反。它是在对象被注销的时候调用的。因为php会在请求结束后确保所有资源都得到释放，所以析构函数显得并不重要。但是，在执行一些事件时还是很有用的，例如清空一个资源或者在对象注销的时候记录日志信息。有两种情况会调用析构函数：在执行你的脚本的时候，当一个对象所有的引用都被注销，或者当脚本运行完毕而php结束请求。第二种方式比较巧妙，因为第一种方法要慎用，而且不要在你的析构函数中引用其他对象。
```php
class MyClass{
	function __destruct(){
		echo '运行结束';	
	}
}
$obj = new MyClass();
$obj = NULL;
```
在这个例子中，当$obj = NULL;被执行的时候，该对象的唯一一个句柄会被注销，而且调用析构函数后对象本身就被注销了。但是就算没有最后一行代码，当请求结束，执行引擎关闭的时候析构函数也会被调用。这样的话会出现两次调用，所以不建议第一种调用。
`注意：PHP并不保证析构函数被调用的准确时间点，所以它可能在最后一个引用的对象被释放后几行语句时才调用。因此，你需要注意这个问题以免出现意外`

## 3.3 属性和方法

在对象创建实例的时候会自动定义一个 $this 变量，它表示一个对对象本身的引用。通过这个变量和 -> 符号，你可以引用该对象的其他方法和属性 $this->name 或者 $this->getName()

### 3.3.1 public、protected、private属性

#### *public*

公共成员既可以通过外部对象使用，也可以用特殊变量$this 从内部访问。如果另外一个类继承了这个公共变，这个规则同样适用，而且从这个类的对象的外部和内部的方法都可以访问。

#### *protected*

保护成员只能从对象内部的方法访问，如果另外一个类继承一个保护成员，同样的规则也适用，而且它可以从继承类实例化的对象的方法中通过特殊的 $this 变量访问到。

#### *private*

与私有成员与保护成员类似，因为他们都只能从对象内部的方法访问。但是，私有成员不能从继承类实例化的对象的方法访问。因为私有属性在继承类中是看不到的，而且两个相关的类可以分别声明一个名字相同的私有变量。也就是两个类都只能看到自己的私有属性，私有成员之间没有关系

`注意：定义类的属性时必须指定属性的访问权限`


### 3.3.2 public、protected、private方法

#### *public*

方法可以在任何作用域访问到，作用域和属性一样

#### *protected*


方法只能从类或者继承类的一个成员中访问到，作用域和属性一样

#### *private*

只能从类的一个成员中访问到，而且无法从继承类的成员中访问到，作用域和属性一样

`注意：如果没有给一个方法或者属性设置访问修饰符，会被默认为public修饰符。`

### 3.3.3 静态属性

类的静态属性：存储在类当中的全局变量，可以在任何地方通过类访问他们

```php
class MyClass{
	static $mysql;
	static $redis = 1;
}
MyClass::$mysql;
MyClass::$redis;

```

#### *self*

如果你想在类里的方法中访问静态成员，你可以通过self来访问它，self是一个方法所属的类的缩写；

```php
class MyClass{
	static $mysql;
	static $redis = 1;
	function myMethod() {
		echo self::$redis;	
	}
}
$obj = new MyClass();
$obj->myMethod();

```

你可能觉得这样没什么用，因为类属性也能解决这种问题，但是静态成员的功能不止如此，比如把一个唯一的ID传递到类的所有实例中：
```php
class MyClass{
    static $id= 0;
    public $uniqueID;
    function __construct()
    {
        self::$id++;
        $this->uniqueID = self::$id;
    }
}
$obj = new MyClass();
echo $obj->uniqueID . '<br>';

$obj = new MyClass();
echo $obj->uniqueID . '<br>';
```
### 3.3.4 静态方法

与静态属性类似，静态方法是类的一部分而且不能被限制到任何一个特定的对象实例和类的属性。因此，$this 在这些方法中将不能使用，但是类本身可以通过self访问。因为静态方法不被限制到任何特定的对象，所以你可以不创建对象实例就通过 class_name::method() 语法调用它。你还可以在一个对象实例中通过$this->method()访问，但是在这些方法中 $this 是没有定义的。为了更加清楚，应该使用self:method()而不是$this->method()

```php
class My{
static function printHelloWorld(){
	self::printNew();
}
static function printNew()
}
My::printNew()

```

## 3.4 类的常量

使用 const关键字来定义类的常量。全局常量可以用 define()函数定义，但是无法在类中使用。与静态成员类似，它们属于类本身而不是类的实例。类的常量总是对大小写敏感的。定义它们的语法很直观，而且访问类中的常量跟访问静态成员是类似的

```php
class My{
	const RED = "RED";
	const BLUE = "BLUE";
	function printRed(){
		//可以使用 self 来访问
		echo self::RED;
	}
}
print My::RED;
$obj = new My();
$obj->printRed();

```
两种方式访问类中的常量。常量的值是不变的，一旦定义后不能被改变也不能被注销。常量最常用的地方是定义枚举元素，例如前边的例子。

`注意：对于全局的常量来说，你最好用大写字母来编写常量的名字`

## 3.5 克隆对象
```php
class MyClass{
	public $val = 1;
}
$obj1 = new MyClass();
$obj2 = $obj1;
$obj2->var = 2;
echo $obj1->var;
```
这一段代码会输出2，因为$obj1是一个对象句柄（它的id号），所以复制到$obj2 的是一个句柄。因此，当改变 $obj2 的值的时候，其实已经改变了 $obj1 指向的那个对象句柄。

有些时候你确实需要复制一个对象的拷贝。可以通过 clone 来实现，这个内置的操作符会自动创建一个新的对象实例，并且附带原对象的所有属性。对象的属性值也会被原样复制。另外你可以重写内置的 __clone()方法来执行任何复制时的操作，它会影响新创建的对象。

```php
class MyClass{
    public $val = 1;
}
$obj1 = new MyClass();
$obj2 = $obj1;
$obj2->var = 2;
$obj3 = clone $obj2;
//克隆过之后，你再去改变$obj2并不会影响obj3
$obj2->var = 3;
echo $obj3->var;
```

`注意：引用时可以作为引用复制的，而且不会执行更加深入的复制。这意味着如果类中一个属性是通过引用指向另一个变量的话，在自动克隆执行后，克隆出来的对象的该属性也会指向相同的变量`

## 3.6 多态

多态使用继承来描述现实世界的关系
`php不能多继承，只能通过接口来实现`

## 3.7 parent::和self::

self:: 指向当前的类（注意不是类的实例），而且它通常用来访问静态成员、方法和常量。
parent::指向父类，而且它经常被用来调用父类的构造函数和方法，它也可以用来访问父类的成员和常量。你应该用parent::而不是父类的某个具体名字，这是为了让你可以方便地更改你的类的层次，因为你不用固定写入某个父类的名字。

## 3.8 instanceof 运算符

用来判断变量是否是某一个类（也包括父类）的实例
```php
if ($shape instanceof Rectangle) {
	//判断$shape是否是 Rectangle 类的一个实例
}
```
`注意：instanceof还检查一个对象是否执行了一个接口`

## 3.9 abstract方法和类

在设计类的层次时，你可能会想部分地保留一些方法给继承类执行。抽象类和抽象方法不做具体实现，交给子类来实现

## 3.10 接口

类的继承让你可以描述几个类之间的父与子的关系。但是，你可能会经常需要增加额外的接口到类中，基本上来说是类需要附带额外的约定。PHP选择了接口而不是多重继承，接口可以让你指定类需要附带的额外的约定。声明一个接口与生命一个类是类似的，但是他只包含函数原形（没有执行体）和常量。任何一个实现这个接口的类将自动获得这个接口定义的常量并且，作为实现的类需要给接口的函数原型提供函数定义，接口的函数都是抽象的。

实现了一个接口的类都将与该接口拥有一个唯一关系，例如类A执行接口myInterface,下面的代码将打印出‘$obj is-A myInterface’
class A implements B,C,..{
}
$obj = new A();
if ($obj instanceof myInterface) {
echo ‘$obj is-A myInterface’;
}

```php
interface Log {
    //日志类
    function write();
}
class FileLog implements Log {
    function write()
    {
        //这里必须要实现接口的方法
        // TODO: Implement write() method.
        echo 'is filelog';
    }
}
class MemcacheLog implements Log {
    function write()
    {
        //这里必须要实现接口的方法
        // TODO: Implement write() method.
        echo 'is memcachelog';
    }
}
```
`注意：接口总是被认为是public的；因此，你不能在定义接口时，给接口的函数原型设置访问修饰符`
`注意：你不能实现互相冲突的多重接口（例如，接口如果定义相同的常量和方法）`

## 3.11 接口的继承

接口是可以从别的接口继承来的，继承接口的语法与继承类的语法类似，但是接口可以允许多重继承

```php

interface Log {
    //日志类
    function write();
}
interface FileLog extends Log {
    function fileOpen();
}

```

与类实现接口类似，一个接口只能继承与自己互相不冲突的接口（方法或者常量不冲突）

## 3.12 final 方法

确保类的方法不能被继承类改写，通过 final 访问控制符来声明一个方法是不可重写的。

```php
class Log {
    final function write() {
        echo 'write_log';
    }
}
class FileLog extends Log {
    function write() {
        echo 'filelog_write';
    }
}
//Fatal error: Cannot override final method Log::write() 
```

```php
class Log {
    final function write() {
        echo 'write_log';
    }
}
class FileLog extends Log {
    
}
$filelog = new FileLog();
$filelog->write();

//final 修饰过之后方法的继承是正常的，但是不能重写，否则会报上边的错误
```
## 3.13 final 类

与 final 方法类似，你还可以定义一个类为 final。这么做将不允许其他类继承此类

final class My {
}
class MyChild extends My {
}

My类被声明为final，子类不能继承它。

## 3.14 __toString() 方法

__toString 方法用于一个类被当成字符串时应怎样回应。例如 echo $obj; 应该显示些什么。此方法必须返回一个字符串，否则将发出一条 E_RECOVERABLE_ERROR 级别的致命错误。
```php
class Person {
    function __toString()
    {
        // TODO: Implement __toString() method.
        return '只有定义了这个方法才能以字符串的形式打印一个类，返回内容自定义';
    }
}
$obj = new Person();
echo $obj;
```

## 3.15 异常处理

大部分语言都是使用 try/catch 语法

try {
//会抛出一个异常代码
} catch (Exception $e) {
//会处理这个异常
}
Exception是顶级异常类

try{}结构装入的代码可以抛出一个异常，后面可以加上一系列的 catch 语句，每一个 catch 声明哪个异常类应该调用并且在 catch 块中异常的对象应该用什么变量名来访问

当一个异常被抛出后，首先到达第一个catch() 并且执行 instanceof 进行异常类比较，判断抛出的异常是否是 catch() 中包好的异常类实例。如果结果是true，PHP进入catch快并且通过声明的变量名可以访问该异常。如果结果是false，将检查下一个catch。一旦进入一个catch，后面的catch语句将不再进入，就算 instanceof 判断也是true。如果找不到任何一个相关的catch语句，php引擎检查同一个函数里外部加上的 try/cathc 语句。如果没有一个存在，PHP通过展开调用堆栈到调用的函数继续搜索。

throw语句 只能抛出对象，你不能让它抛出任何其他基础数据类型，例如字符串或者整型值。PHP中存在一个预定义的异常类名叫Exception,你自己所有的异常处理类都必须从它继承。如果你尝试抛出一个不是由Exception类继承的类，最后将得到一个运行错误

`注意:永远不要使用异常类控制流程（除非不得以），因为这样会让你的代码很难理解，而且会让你的代码运行缓慢。异常应该只包含特定的错误信息，而且不应该包含会影响获取处理器中流程控制和逻辑的参数`

## 3.16 __autoload()

以往做法是将你需要的文件引入，这样做的缺陷在于你不得不经常包含大量的源文件，而且经常导致包含太多的文件和一个头疼的代码维护问题。__autoload()可以解决这个问题，它不需要你包含将要使用的类。如果你定义一个__autoload函数（每一个应用只能有一个这样的函数），而且当你访问一个还未存在的类时，它将被调用并且把类名作为它的参数。这样做给你一个实时包含类的可能性。如果你成功地包含了该类，你的源代码会继续执行，就像这个类已经定义了一样。如果你没有成功地包含该类，脚本会报一个类不存在的严重错误

__autoload() 例子

```php
//index.php
require_once "main.php";
$obj = new MyClass();
$obj->printHello();

//main.php
function __autoload($class_name) {
    require_once $_SERVER["DOCUMENT_ROOT"] . "/classes/" . $class_name . '.php';
}

//myclass.php
class MyClass
{
    function printHello() {
        echo "Hello, World";
    }
}
```

`注意：MyClass.php存在于项目根目录的classes目录下`

上边可以看到myclass.php并没有真正的包含在 main.php 文件中而是暗中通过调用 __autoload() 函数包含进来的。你通常可以将 __autoload() 函数定义在一个文件中，并在你所有的主脚本文件包含它，从而当你需要增加调用的类的数量时，可节省大量的代码而且可以减少维护代码的工作量。

`特别注意：虽然PHP中类名大小写不敏感，但是类的名字发送给 __autoload() 函数时是区分大小写的。如果你更喜欢让你的类的文件名对大小写敏感，请确保在你的代码中保持一致性，而且你的类中也要使用正确大小写的名字。而如果你不希望这么uo，你可以使用 strtolower() 函数把类的名字转变为小写再尝试包含它，同时保存类的文件名都用小写`

## **4. 面向对象编程和设计模式**

## 4.1 重载性能

PHP除了可以用C编写扩展重载对象的语法外，它还允许PHP代码重载一下经常需要的有限子集内容。

### 4.1.1 属性和方法的重载

php允许通过实现特殊的代理方法对属性的访问和方法的调用进行重载，这些代理方法将在相关属性或者方法不存在时调用。这种特性让你在中端这些动作并定义你自己的功能时获得巨大的灵活性。

你可以实现下面的方法原型：
function __get($property)
function __get($property, $value)
function __call($method, $args)

__get 传递属性的名字，并且返回属性的值
__set 传递属性的名字和新的值
__call 传递方法的名字和一个数字索引的数组，数组包含传递的参数，第一个参数的索引是 0

__get 和 __set 用法：

```php
class My {
    private $arr = array('x' => NULL, 'y' => NULL);
    function __get($property)
    {
        // TODO: Implement __get() method.
        if (array_key_exists($property, $this->arr)) {
            return $this->arr[$property];
        } else {
            print "Error:Can't read a property other than x & y\n";
        }
    }
    function __set($property, $value)
    {
        if (array_key_exists($property, $this->arr)) {
            $this->arr[$property] = $value;
        } else {
            print "Error: Can't wirte ap property other than x & y\n";
        }
    }
}
$obj = new My();
$obj->x = 1;
print $obj->x;

print "\n";

$obj->n = 2;
print $obj->n;
```

__call 有很多用途，下面的例子显示如何创建一个授权模型，通过该模型一个 HelloWorldDelegator类的实例可以授权所有的方法去调用一个 HelloWorld类的实例：

```php

class HelloWord {
    function display($count){
        for ($i = 0; $i < $count; $i++) {
            print "Hello,Word";
        }
        return $count;
    }
}
class HelloWorldDelegator {
    private $obj;
    function __construct()
    {
        $this->obj = new HelloWord();
    }
    function __call($name, $arguments)
    {
        // TODO: Implement __call() method.
        return call_user_func_array(array($this->obj, $name, $arguments));
    }
}
$obj = new HelloWorldDelegator();
print $obj->display(3);

```

以上例子会输出
Hello,world
Hello,world
Hello,world
3

call_user_func_array() 函数允许 __call() 把它的参数通过 call_user_func_array() 调用传递给 HelloWorld::display(),后者打印三次 "Hello,World",然后 __call() 返回 $count 的值。你不但可以通过 __call() 方法调用一个不同的对象，而且你还可以从 __call() 函数返回一个值，就像正常的方法一样

### 4.1.2 使用数组语法访问的重载

你需要实现 ArrayAccess 接口

ArrayAccess接口 像数组一样来访问你的PHP对象，其实就是自己实现php数组的方法

例子：

```php

<?php
class UserArray implements ArrayAccess {
    private $elements;
    /**
     * 标识一个元素是否定义
     * @param offset
     */
    function offsetExists($offset)
    {
        // TODO: Implement offsetExists() method.
        return isset($this->elements[$offset]);
    }

    /**
     * 返回一个元素的值
     * @param offset
     */
    function offsetGet($offset)
    {
        // TODO: Implement offsetGet() method.
        return $this->elements[$offset];
    }
    /**
     * 为一个元素的赋值
     * @param offset
     * @param value
     */
    function offsetSet($offset, $value)
    {
        // TODO: Implement offsetSet() method.
        $this->elements[$offset] = $value;
    }

    /**
     * 删除一个元素
     * @param offset
     */
    function offsetUnset($offset)
    {
        // TODO: Implement offsetUnset() method.
        unset($this->elements[$offset]);
    }
}
$userMap = new UserArray();
$userMap['test'] = 'test';//自动调用offsetSet
if(isset($userMap['test']))//自动调用offsetExists
{
    echo $userMap['test'];//自动调用offsetGet
    unset($userMap['test']);//自动调用offsetUnset
    var_dump($userMap['test']);
}

```

关于 ArrayAccess 接口主要抽象了几个方法用来访问数组

## 4.2 迭代器

使用 Iterators 接口可以实现自己的迭代器

例如：一个对象的属性使用 foreach() 循环进行迭代遍历

```php

class MyClass {
    public $name = 'John';
    public $sex = 'male';
}
$obj = new MyClass();
foreach ($obj as $key => $value) {
    echo $key . '=' . $value . '<br />';
}

```
但是你的类不只是表现为前面例子中一个简单的关键字/值的数组，而会表现为更加复杂的数据，例如一个数据库查询或者配置文件。
php可以让你用 foreach() 循环再你的代码中重载迭代行为，使得它按照你的类的设计执行有实际意义的遍历。

`注意：PHP不仅可以让你重载这种行为，而且它还可以让编写扩展的作者重写类似的行为，这已经让迭代器支持多种PHP扩展，例如 SimpleXML 和 SQLite`

为了在你的类中重载迭代器，你需要实现一些PHP预先定义的接口

例如： Traversable 接口的类都可以用 foreach 结构遍历。但是，Traversable 是一个空的接口而且不能被直接执行，反之你可以执行 Iteraror 或者 IteratorAggregate,它们都是从 Traversable 继承而来

主要的接口是 Iterator，它定义了你需要执行的方法以便给你类提供 foreach 迭代的功能。这些方法应该是公共的

| 接口 | Interator|
|------|------|
| void rewind() | 重写吧迭代器指向列表的开始处（这个在执行时并不总是可用的） |
| mixed current() | 返回当前位置的值 |
| mixed key() | 返回当前位置的关键字 |
| void next() | 把迭代器移动到下一个关键字/值对 |
| bool valid() | 返回 true/false值，判断是否还有更多的值（在调用 current() 和 key() 之前使用） |

例子：
```php
class MyForeach implements Iterator {
    private $start, $end;
    private $cur;
    public function __construct($start, $end)
    {
        $this->start = $start;
        $this->end = $end;
    }

    //重写把迭代器指向列表开始处
    public function rewind()
    {
        // TODO: Implement rewind() method.
        $this->cur = $this->start;
    }
    //返回当前位置的关键字
    public function key()
    {
        // TODO: Implement key() method.
        return $this->cur;
    }
    //返回当前位置的值
    public function current()
    {
        // TODO: Implement current() method.
        return pow($this->cur, 2);
    }
    //把迭代器移动到下一个 键值对
    public function next()
    {
        // TODO: Implement next() method.
        $this->cur++;
    }
    //返回true/false值，判断是否还有更多的值
    public function valid()
    {
        // TODO: Implement valid() method.
        return $this->cur <= $this->end;
    }
}
$obj = new MyForeach(3, 7);
foreach ($obj as $key => $value) {
    print "The square of $key is $value\n";
}
```

这个例子示范了如何用你自己的方法进行一个类的遍历。在这里，类表现的是整数的平方，而且在给予一个最小值和一个最大值后，迭代遍历这些值将给你数字本身和它的平方值。

许多情况下，你的类本身将表述数据和拥有与这些数据的交互的方法。事实上，需要一个迭代器可能不是它的主要目的。另外，当迭代遍历一个对象时，迭代的状态通常会存储在对象本身，因此不允许迭代的嵌套。因为这两个原因，你可以让你的类实现 IteratorAggreagate 接口从而把类的执行和它的迭代器分离开来。与先前必须定义所有方法不同，你只需要定义个返回不同类的方法，该对象就为你实现了迭代遍历的接口。

你需要实现的方法是 Iterator getIterator()，因为它将返回一个处理这个类的迭代的迭代对象。

通过使用这个把类与其迭代器分离的方法，我们改写先前的例子：

```php

<?php
class MyForeach implements IteratorAggregate {
    private $start, $end;
    private $cur;
    public function __construct($start, $end)
    {
        $this->start = $start;
        $this->end = $end;
    }
    public function getIterator()
    {
        // TODO: Implement getIterator() method.
        return new MyForachIterator($this);
    }
    public function getStart(){
        return $this->start;
    }
    public function getEnd(){
        return $this->end;
    }
}
class MyForachIterator implements Iterator {
    private $cur;
    private $obj;
    public function __construct($obj)
    {
        $this->obj = $obj;
    }
    public function rewind()
    {
        // TODO: Implement rewind() method.
        $this->cur = $this->obj->getStart();
    }
    public function key()
    {
        // TODO: Implement key() method.
        return $this->cur;
    }
    public function current()
    {
        // TODO: Implement current() method.
        return pow($this->cur, 2);
    }
    public function next()
    {
        // TODO: Implement next() method.
        $this->cur++;
    }
    public function valid()
    {
        // TODO: Implement valid() method.
        return $this->cur <= $this->obj->getEnd();
    }
}
$obj = new MyForeach(3, 7);
foreach ($obj as $key => $value) {
    print "The square of $key is $value\n";
}

```

这个代码的输出与之前一样，你可以清除地看到 IteratorAggregate 接口可以让你把你的类的主要功能与迭代遍历它需要的方法分离到两个独立的实体中。

## 4.3 设计模式

常规的解决方案包含了一些不断重复的问题，解决这些问题的方案叫做设计模式

### 4.3.1 策略模式

策略模式的一个典型应用是处理程序算法与其他算法之间的互换。例如，如果你编写了创建一副图片的代码，在一些情况下，你可以需要创建JPEG的图片，而在另外一个情况下，你可能需要创建 GIF 文件。

策略模式的实现方法通常是通过声明一个抽象的拥有一个算法方法的基类来实现的，而且通过继承这个基类的具体的类来实现。在代码中的一些关键点，设计模式将决定俺哥具体的策略是相关的，然后实例化并使用任何相关的类。

下边列子显示了一个下载服务如何根据访问它的web客户端选择不同的文件策略。在它创建一个包含链接的HTML时，它将根据浏览器的操作系统的标识创建指向 .tar.gz 或者 zip 文件的下载链接。当然，这意味着两个文件都要求通过服务器上统一的格式访问。简单来说，假设词语 “Win” 存在于 $_SERVER["HTTP_USER_AGENT"]中，说明我们正在处理一个来自 windows 系统的请求，因此需要创建 .zip 的链接，反之我们就在处理需要 .tar.gz 格式的系统。

在这个例子中，我们将使用两种策略 .tar.gz 策略和 zip策略，通过下面的代码段将让你了解如何使用这样一个策略模式：

```php
//顶层的抽象文件链接创建类
abstract class FileNaming {
    abstract function createLinkName($filename);
}
//zip策略
class ZipFileNaming extends FileNaming {
    //这里必须实现继承的抽象类的方法
    public function createLinkName($filename)
    {
        // TODO: Implement createLinkName() method.
        return "http://downloads.foo.bar/$filename.zip";
    }
}
//Tar.gz 文件策略
class TarGzFileNaming extends FileNaming {
    //这里必须实现继承的抽象类的抽象方法
    public function createLinkName($filename)
    {
        // TODO: Implement createLinkName() method.
        return "http://downloads.foo.bar/$filename.tar.gz";
    }
}

//判断浏览器类型，通过 HTTP_USER_AGENT
//判断是否是windows系统
if (strstr($_SERVER["HTTP_USER_AGENT"], "Win")) {
    //生成zip策略类
    $fileNamingObj = new ZipFileNaming();
} else {
    //创建 tar策略类
    $fileNamingObj = new TarGzFileNaming();
}
$filename = 'test';
//获取文件链接
$file_link = $fileNamingObj->createLinkName($filename);
//输出链接到页面
print <<<EOF
<h1>根据系统环境自动识别的文件下载地址(windows系统访问到的是zip文件格式)</h1>
<br>
<a href="$file_link">$filename</a>
EOF;
```
`提示：策略模式经常跟工厂模式一起使用，工厂模式将在本节的后续部分描述，工厂模式用来选择一个合适的策略`

### 4.3.2 单件模式

单件模式又叫单例模式。例如下边的情形，你需要一个对象类处理你的应用中的一些集中的操作，例如一个日志记录对象。这种情况下，人们通常希望只有一个这样的覆盖整个应用范围的对象实例存在，并让整个应用代码都可以访问它。具体地说，在一个日志记录对象中，你将需要应用中的每一个地方的代码都可以访问它来吧信息记录到日志中，而且让集中的日志机制根据日志级别设置处理日志信息的过滤。为了解决这种问题，你就需要使用单例模式。

让你的类变成一个单例类通常是通过实现一个静态的类方法 getInstance() 实现的，这个方法只返回该类的唯一实例。在你第一次调用这个方法的时候，它创建一个实例，把它存在一个私有的静态的变量中，并且给你返回实例。下一次，它将仅仅给你返回那个已经创建的实例的句柄。

例子：

```php
class Logger {
    //定义静态的实例变量
    static private $instance = NULL;
    //自定义获取类的实例的方法，名字通常都写 getInstance
    static function getInstance() {
        //调用自身的获取实例的方法
        if (self::$instance == NULL) {
            self::$instance = new Logger();
        }
        return self::$instance;
    }
    //构造函数
    private function __construct()
    {
    }
    //克隆
    private function __clone()
    {

    }

    /**
     * 日志写入方法
     * @param $str  日志内容
     * @return bool 写日志是否成功
     */
    public function write($str)
    {
        //写日志的逻辑
        return true;
    }
}
Logger::getInstance()->write('测试日志写入');

```
这个模式的本质是 Logger::getInstance(), 它让你可以在应用的任何地方访问日志对象，无论是从一个函数，一个方法，还是全局作用域中。

这个例子中，构造函数和克隆方法都被定义 private。这么做的原因是为了防止开发者用 new 或者 clone 运算符错误的创建第二个 Logger类的实例；因此，getInstance() 是唯一可以访问单件类实例的方法


### 4.3.3 工厂模式

多态和基类的使用确实是OOP的核心。但是，在一些阶段你必须创建基类的子类的一个具体实例。这个通常是用工厂模式实现的。一个工厂类拥有一个静态的方法，用来接收一些输入，并根据输入决定该创建那个类的实例（通常是一个子类）

场景：假设在你的 Web 站点上，有着不同类型的用户登录。其中一些人是游客，一些是正常的会员，还有其他一些人是管理员。一个普通的思路是，你会需要一个基类 User 和 三个子类：

GuestUser、CustomerUser与AdminUser。与 User 一样的是，它的子类将包含用户的获取信息的方法（例如，他们访问 Web 站点的权限和个人的首选项）

对你来说，编写你的 Web 应用最好的方法就是尽可能多地使用基类 User，这样代码将会比较规范而且很容易在需求增加时加上附加的用户类型。

下面的例子显示一种关于四个 User 类的实现方式，而且使用 UserFactory 类来根据用户名创建合适的用户对象：

```php
/**
 * 用户基类
 * Class User
 * ${DS}
 */
abstract class User {
    //初始化用户名
    protected  $name = NULL;
    //抽象类的方法不需要使用权限修饰符
    function __construct($name)
    {
        $this->name = $name;
    }
    function getName() {
        return $this->name;
    }
    //鉴权
    function hasReadPermission() {
        return true;
    }
    //修改权限
    function hasModifyPermission() {
        return false;
    }
    //删除权限
    function hasDeletePermission() {
        return false;
    }
    //定制的方法
    function wantsFlashInterface() {
        return true;
    }
}

/**
 * 访客类，继承 User 基类
 * Class GuestUser
 * ${DS}
 */
class GuestUser extends User {

}

/**
 * 会员类
 * Class CustomerUser
 * ${DS}
 */
class CustomerUser extends User {
    //重写父类的 修改权限方法
    function hasModifyPermission()
    {
        return true;
    }
}

/**
 * 管理员类
 * Class AdminUser
 * ${DS}
 */
class AdminUser extends User {
    function hasModifyPermission()
    {
        return true;
    }
    function hasDeletePermission()
    {
        return true;
    }
    function wantsFlashInterface()
    {
        return false;
    }
}

/**
 * 用户工厂类
 * Class UserFactory
 * ${DS}
 */
class UserFactory {
    private static $users = array("Andi" => "admin", "Stig" => "guesst", "Derick" => "customer");
    //创建用户
    static function Create($name)
    {
        if (isset(self::$users[$name])) {
            //报错，用户不存在
            //echo "用户不存在";
        }
        switch (self::$users[$name]) {
            case "guesst" :
                return new GuestUser($name);
            case "customer" :
                return new CustomerUser($name);
            case "admin" :
                return new AdminUser($name);
            default:
                //报错，用户类型不存在
                //echo "用户类型不存在";
        }
    }
}
//辅助函数
function boolToStar($bool) {
    if ($bool == true) {
        return "Yes\n";
    } else {
        return "No\n";
    }
}

/**
 * 读取用户权限
 * @param User $obj 对象必须是User类或其子类
 */
function displayPermissions(User $obj)
{
    print $obj->getName() . "是存在的用户<br>";
    print "是否有读权限：" . boolToStar($obj->hasReadPermission()).'<br>';
    print "是否有改权限：" . boolToStar($obj->hasModifyPermission()).'<br>';
    print "是否有删权限：" . boolToStar($obj->hasDeletePermission()).'<br>';
}

function displayRequirements(User $obj)
{
    if ($obj->wantsFlashInterface()) {
        print $obj->getName() . " require Flash<br>";
    }
}
$logins = array("Andi", "Stig", "Derick");
foreach ($logins as $login) {
    displayPermissions(UserFactory::Create($login));
    displayRequirements(UserFactory::Create($login));
}

```

这个例子是一个经典的工厂模式的例子。你拥有一个类分层但是你的代码例如 displayPermission() 采用同样的方法处理。唯一一个不同方法处理类的就是工厂本身，`他负责构造这些实例`。在这个例子中，工厂检查用户名属于哪种类型的用户并且创建与它相对应的实例。在实际开发中，与把用户存在用户名映射的一个静态数组中不同的是，你可能会把用户信息存储在数据库或者配置文件中。

`提示：除了 Create()，你将经常能发现其他用于工厂的方法名，例如 factory()、factoryMethod()，或者 createInstance()`

### 4.3.4 观察者模式

场景：一个电子商务站点显示的每一个产品的单价如果显示为用户当地的货币就需要使用当前的汇率进行转换。现在假设每一个产品项目都是由一个PHP对象从数据库获取并呈现出来的，而货币转换的汇率本身大部分可能是由一个另外的资源获得而并不是产品数据库条目的一部分。让我们在假定这样一个对象有一个 display() 方法来输出和这个产品相关的html页面。

观察者模式允许对象注册到一个特定的时间或者数据，并且当这个事件发生或者数据改变时，它会自动通报。通过这个方法，你可以把产品项目开发成一个给予货币汇率的观察者，而且在打印出项目的条目时，你可以驱动一个事件来用正确的汇率更新注册的对象。这么做是为了让对象有机会自我更新并且在 display 方法中使用新的数据

通常，观察者模式通过使用一个叫 Observer 的接口实现的，对作为观察者感兴趣的类需要实现这个接口

一个对象想要 “可观察”，通常需要一个注册方法，这让观察者对象可以注册它自己。例如，下面的例子可能是我们需要的汇率类：

没有理解，将去看另外一本书户

## 4.4 映射

$className = 'MyClass';
$myclass = new $className();

### 4.4.1 映射api

映射 API 包含了大量的类，你可以用他们内观你的应用。

### 4.4.2 映射举例

简单的例子

下面的代码显示了一个使用 RrefectionClass::export() 静态方法的简单的例子，目的是从 ReflectionParameter 获取信息。ReflectionCalss::export()可以用来获取一个PHP类的信息

### 4.4.3 使用映射执行授权模式

开发中会遇到，一个类需要去执行另一个类或者更多其他类的方法的次数越来越多。最开始的临时解决办法是让类1去继承类2，并因此继承所有该类的功能。但是许多时候这种方法是错误的，不但因为他们之间不是一个明确的父子关系，而且因为类1有可能已经继承另外一个类，所以不能再继承了。在这种情况下，使用授权模块（通过`授权设计模式`）就变的有用了，如果调用一个类1不具备的方法时，会转向调用类2。一些情况下，你甚至需要连接起大量的对象，其中列表中的第一个对象拥有最高的优先级。

下面的例子创建了名叫 ClassOneDelegator 的授权模型，它首先检查方法是否存在并可以从 ClassOne 访问到；如果不行，它将尝试从注册到该对象的其他对象去寻找方法。这个应用可以通过 addObject($obj) 方法注册附加的对象来提供授权。增加对象的顺序就是 ClassOne 寻找一个可以满足请求的对象的优先级顺序：

```php

class ClassOne {
    function callClassOne() {
        print "这是类1<br/>";
    }
}
class ClassTwo {
    function callClassTwo() {
        print "这是类2<br/>";
    }
}

/**
 * 授权模型
 * Class ClassOneDelegator
 * ${DS}
 */
class ClassOneDelegator {
    private $targets;
    function __construct()
    {
        //追加类1到数组中
        $this->targets[] = new ClassOne();
    }

    /**
     * 添加对象到授权数组中
     * @param $obj
     */
    function addObject($obj) {
        $this->targets[] = $obj;
    }
    function __call($name, $arguments)
    {
        // TODO: Implement __call() method.
        foreach ($this->targets as $obj) {
            //获取类的报告信息
            $r = new ReflectionClass($obj);
            try {
                $method = $r->getMethod($name);
            } catch (ReflectionException $e) {
                continue;
            }

            //判断你调用的方法是否存于授权模型中
            //确保要授权的方法是公有的而且不是抽象方法
            if ($method && $method->isPublic() && !$method->isAbstract()) {
                //执行一个反射方法
                return $method->invoke($obj, $arguments);
            }
        }
    }
}
$obj = new ClassOneDelegator();
$obj->addObject(new ClassTwo());
$obj->callClassOne();
$obj->callClassTwo();

```

## **性能监控**

使用 php-fpm.conf 配置文件下边的 slowlog 来监控运行较慢的脚本代码

