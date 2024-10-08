# MERN_interviewQuestions
Here i describe. what kind of question company's asked to me. interview in tricity



NODE

1 - What is nodejs 
A - Node.js is an open-source server environment. Node.js is cross-platform and runs on Windows, Linux, Unix, Mac OS, etc. Node.js is a back-end JavaScript runtime environment. Node.js runs on a JavaScript Engine and executes JavaScript code outside a web browser.

link  - https://www.netguru.com/glossary/node-js

2 - Nodejs is multithread or singlethread ? 
A - Node. js runs JavaScript code in a single thread, which means that your code can only do one task at a time. However, Node. js itself is multithreaded and provides hidden threads through the libuv library, which handles I/O operations like reading files from a disk or network requests.

3. If the nodejs single thread how its handle multiple request of user in one time ? 
A - Single Threaded: Node JS works using a single thread. This means that there isn't a pool of threads, which is assigned to handle client requests, but only a single thread to accept the incoming requests. So, even if there are 100 clients, we have a single thread to handle them, in one server.

4. what is stub in nodejs
A - A small program routine that substitutes for a longer program which is possible to be loaded later or that is remotely located.

Features of stub:

Stubs can be either anonymous.
Stubs can be wrapped into existing functions. When we wrap a stub into the existing function the original function is not called.
Stubs are functions or programs that affect the behavior of components or modules.
Stubs are dummy objects for testing.
Stubs implement a pre-programmed response.

5. Nodejs pros and cons
A - https://javascript.plainenglish.io/the-pros-and-cons-of-node-js-web-app-development-a-detailed-look-c91a22f013c.

6. what is event loop in nodejs ?
A -Node.js is a single-threaded event-driven platform that is capable of running non-blocking, asynchronously programming. These functionalities of Node.js make it memory efficient. The event loop allows Node.js to perform non-blocking I/O operations despite the fact that JavaScript is single-threaded. It is done by assigning operations to the operating system whenever and wherever possible.

Features of Event Loop:

1. Event loop is an endless loop, which waits for tasks, executes them and then sleeps until it receives more tasks.
2. The event loop executes tasks from the event queue only when the call stack is empty i.e. there is no ongoing task.
3. The event loop allows us to use callbacks and promises.
4. The event loop executes the tasks starting from the oldest first.

7. what is buffer in node js ?
A - In Node Js, buffers are used to store raw binary data. A buffer represents a chunk of memory that is allocated on our computer. The size of the buffer, once set, cannot be changed. A buffer is used to store bytes.

8 . What is nodejs Stream ?
A - A stream is an abstract interface for working with streaming data in Node.js. The node:stream module provides an API for implementing the stream interface.
There are many stream objects provided by Node.js. For instance, a request to an HTTP server and process.stdout are both stream instances.
Streams can be readable, writable, or both. All streams are instances of EventEmitter. 

Types of streams#
There are four fundamental stream types within Node.js:

Writable: streams to which data can be written (for example, fs.createWriteStream()).
Readable: streams from which data can be read (for example, fs.createReadStream()).
Duplex: streams that are both Readable and Writable (for example, net.Socket).
Transform: Duplex streams that can modify or transform the data as it is written and read (for example, zlib.createDeflate()).
Additionally, this module includes the utility functions stream.pipeline(), stream.finished(), stream.Readable.from() and stream.addAbortSignal().

link - https://nodejs.org/api/stream.html#organization-of-this-document

9. what is socket in node js ? 
A - Socket.IO is a library that enables real-time, bidirectional and event-based communication between the browser and the server. It consists of: a Node. js server: Source | API. a Javascript client library for the browser (which can be also run from Node.

10. What Is Express JS? 
A - Express is a node js web application framework that provides broad features for building web and mobile applications. It is used to build a single page, multipage, and hybrid web application. It's a layer built on the top of the Node js that helps manage servers and routes.

11 . Why do we use module exports?
A - The main purpose of module. exports is to achieve modular programming. Modular programming refers to separating the functionality of a program into independent, interchangeable modules, such that each contains everything necessary to execute only one aspect of the desired functionality.

12. Can a module have more than one export?
A - Every module can have two different types of export, named export and default export. You can have multiple named exports per module but only one default export.

13. what is synchronous and asynchronous ? 
A - Asynchronous is a non-blocking architecture, so the execution of one task isn't dependent on another. Tasks can run simultaneously. Synchronous is a blocking architecture, so the execution of each operation is dependent on the completion of the one before it.

14 . Diffrence between let an var ? 
A - var and let are both used for variable declaration in javascript but the difference between them is that var is function scoped and let is block scoped.

15. What is npm and why use it?
A- npm is the world's largest Software Registry. The registry contains over 800,000 code packages. Open-source developers use npm to share software. Many organizations also use npm to manage private development.

16. Is npm and Node.js the same?
A - Node. js or Node is an open-source, cross-platform, JavaScript runtime environment(JSRE) that executes JavaScript code outside of a web browser. npm is a package manager(like Nuget package manager in . NET -Microsoft ) for the JavaScript programming language.

17. What is Mongoose ?
A - Mongoose acts as a front end to MongoDB, an open source NoSQL database that uses a document-oriented data model. A "collection" of "documents" in a MongoDB database is analogous to a "table" of "rows" in a relational database.

18 . Why Mongoose is used in backend?
A - Mongoose allows us to: map the model attributes and requirements to the database, create new collections and documents in our database, and make queries to retrieve info from the database.

19. Is ExpressJS frontend or backend?
A - Express. js is used as a backend in certain popular stacks, such as MERN (a Node. js framework). Between the frontend and the backend, multiple components can be reused.

```javascript 
console.log(a+b+c)
```


20 Oprators that are used in us
A - 
Operator	Type	Description	Example
+	Arithmetic	Addition	5 + 3 → 8
-	Arithmetic	Subtraction	5 - 3 → 2
*	Arithmetic	Multiplication	5 * 3 → 15
/	Arithmetic	Division	6 / 3 → 2
%	Arithmetic	Modulus (Remainder)	5 % 2 → 1
++	Arithmetic	Increment (Adds 1 to operand)	let a = 5; a++ → 6
--	Arithmetic	Decrement (Subtracts 1 from operand)	let a = 5; a-- → 4
=	Assignment	Assigns value	x = 10
+=	Assignment	Adds right operand to left operand and assigns	x += 5 → x = x + 5
-=	Assignment	Subtracts right operand from left operand and assigns	x -= 5 → x = x - 5
*=	Assignment	Multiplies right operand with left operand and assigns	x *= 5 → x = x * 5
/=	Assignment	Divides left operand by right operand and assigns	x /= 5 → x = x / 5
==	Comparison	Equal to (loose comparison)	5 == '5' → true
===	Comparison	Strict equal to (value and type)	5 === '5' → false
!=	Comparison	Not equal to (loose comparison)	5 != '5' → false
!==	Comparison	Strict not equal to (value and type)	5 !== '5' → true
>	Comparison	Greater than	5 > 3 → true
<	Comparison	Less than	5 < 3 → false
>=	Comparison	Greater than or equal to	5 >= 5 → true
<=	Comparison	Less than or equal to	5 <= 5 → true
?	Ternary	Conditional (ternary) operator	x > 5 ? 'yes' : 'no'
??	Nullish Coalescing	Returns right-hand operand if left-hand operand is null or undefined	null ?? 'default' → 'default'
`		`	Logical
&&	Logical	Logical AND	true && false → false
!	Logical	Logical NOT	!true → false
&	Bitwise	AND (performs AND on each bit)	5 & 1 → 1
`	`	Bitwise	OR (performs OR on each bit)
^	Bitwise	XOR (exclusive OR on each bit)	5 ^ 1 → 4
~	Bitwise	NOT (inverts all bits)	~5 → -6
<<	Bitwise	Left shift (shifts bits to the left)	5 << 1 → 10
>>	Bitwise	Right shift (shifts bits to the right)	5 >> 1 → 2
>>>	Bitwise	Zero-fill right shift (shifts bits to the right, filling with zeros)	5 >>> 1 → 2
?.	Optional Chaining	Accesses an object’s property, returns undefined if nullish	obj?.prop
**	Exponentiation	Raises the first operand to the power of the second	2 ** 3 → 8
<>	JSX	React fragment syntax (not an operator in regular JS)	<></>
