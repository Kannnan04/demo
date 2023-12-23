
# Day-1 Task

    1.**Write a blog on Difference between HTTP1.1 vs HTTP2**
        HTTP 1.0
HTTP/1.0 supports both non-persistent (connection-close after each request-response) and persistent (keep-alive) connections.

HTTP/1.0 does not require the “Host” header and lacks explicit support for virtual hosting.

HTTP/1.0 includes basic caching mechanisms using headers like “Expires” and “Last-Modified.”

HTTP/1.0 primarily focuses on the transmission of ASCII characters and does not explicitly handle internationalization or multilingual content. Support for non-ASCII characters and language-specific features is limited.

HTTP/1.0 is a stateless protocol, meaning that each request-response cycle is independent and does not retain any information about previous interactions.

HTTP/1.0 defines several request methods, including GET, POST, HEAD, PUT, DELETE, and OPTIONS.

HTTP 1.1
Through the HTTP protocol, resources are exchanged between client devices and servers over the internet. Client devices send requests to servers for the resources needed to load a web page; the servers send responses back to the client to fulfill the requests.

Requests and responses share sub-documents — such as data on images, text, text layouts, etc. — which are pieced together by a client web browser to display the full web page file.


In addition to the web page files it can serve, a web server contains an HTTP daemon, a program that waits for HTTP requests and handles them when they arrive.

A web browser is an HTTP client that sends requests to servers. When the browser user enters file requests by either “opening” a web file by typing in a URL or clicking on a hypertext link, the browser builds an HTTP request and sends it to the Internet Protocol address (IP address) indicated by the URL.

The HTTP daemon in the destination server receives the request and sends back the requested file or files associated with the request.

    2.**Write a blog about objects and its internal representation in Javascript**

        Objects, in JavaScript, is it’s most important data-type and forms the building blocks for modern JavaScript. These objects are quite different from JavaScript’s primitive data-types(Number, String, Boolean, null, undefined and symbol) in the sense that while these primitive data-types all store a single value each (depending on their types).

Objects are more complex and each object may contain any combination of these primitive data-types as well as reference data-types.
An object, is a reference data type. Variables that are assigned a reference value are given a reference or a pointer to that value. That reference or pointer points to the location in memory where the object is stored. The variables don’t actually store the value.

Loosely speaking, objects in JavaScript may be defined as an unordered collection of related data, of primitive or reference types, in the form of “key: value” pairs. These keys can be variables or functions and are called properties and methods, respectively, in the context of an object.

For Eg. If your object is a student, it will have properties like name, age, address, id, etc and methods like updateAddress, updateNam, etc.

Objects and properties
A JavaScript object has properties associated with it. A property of an object can be explained as a variable that is attached to the object. Object properties are basically the same as ordinary JavaScript variables, except for the attachment to objects. The properties of an object define the characteristics of the object. You access the properties of an object with a simple dot-notation:

objectName.propertyName
Like all JavaScript variables, both the object name (which could be a normal variable) and property name are case sensitive. You can define a property by assigning it a value. For example, let’s create an object named myCar and give it properties named make, model, and year as follows:

var myCar = new Object();
myCar.make = 'Ford';
myCar.model = 'Mustang';
myCar.year = 1969;
Unassigned properties of an object are undefined (and not null).

myCar.color; // undefined
Properties of JavaScript objects can also be accessed or set using a bracket notation (for more details see property accessors). Objects are sometimes called associative arrays, since each property is associated with a string value that can be used to access it. So, for example, you could access the properties of the myCar object as follows:

myCar['make'] = 'Ford';
myCar['model'] = 'Mustang';
myCar['year'] = 1969;
An object property name can be any valid JavaScript string, or anything that can be converted to a string, including the empty string. However, any property name that is not a valid JavaScript identifier (for example, a property name that has a space or a hyphen, or that starts with a number) can only be accessed using the square bracket notation. This notation is also very useful when property names are to be dynamically determined (when the property name is not determined until runtime). Examples are as follows:

// four variables are created and assigned in a single go, 
// separated by commas
var myObj = new Object(),
    str = 'myString',
    rand = Math.random(),
    obj = new Object();
myObj.type              = 'Dot syntax';
myObj['date created']   = 'String with space';
myObj[str]              = 'String value';
myObj[rand]             = 'Random Number';
myObj[obj]              = 'Object';
myObj['']               = 'Even an empty string';console.log(myObj);git