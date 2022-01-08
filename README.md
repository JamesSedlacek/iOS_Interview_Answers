# iOS Interview Questions and Answers

<details>
  <summary><strong>Classes vs. Structs</strong></summary>
  <br>
  
  ## YouTube
  
  [![IMAGE ALT TEXT HERE](https://img.youtube.com/vi/im4FKxqrj5c/0.jpg)](https://www.youtube.com/watch?v=im4FKxqrj5c)
  
  ## Script
  
  ### Q: What is the difference between a class and a struct in Swift?

  A: The main difference is that classes are reference types and structs are value types.

  When you pass a class through a function or assign it to a variable, it will increase its reference count.

  When you pass a struct through a function or assign it to a variable, its value is copied instead of increasing its reference count.

  A good analogy is comparing a google doc to a word doc. When you send someone a word doc they’re able to edit a copy of the document, this is like a struct. And when you send someone a google doc then you’re both able to edit the same document, just like a class.

  Other differences are: classes have inheritance, type casting, & de-initializers .
  <hr>
</details>

<details>
  <summary><strong>ARC, Retain Cycles, & Memory Leaks</strong></summary>
  <br>
  
  ## YouTube
  
  [![IMAGE ALT TEXT HERE](https://img.youtube.com/vi/kkJu0EbIvYg/0.jpg)](https://www.youtube.com/watch?v=kkJu0EbIvYg)
  
  ## Script
  
  ### Q: How is memory management handled in iOS?

  A: Swift uses Automatic Reference Counting to handle memory management.

  ### Q: What is ARC and how does it work?

  A: Automatic Reference Counting keeps track of strong references to instances of classes. 
  It increases or decreases their reference count whenever you assign or unassign them to constants, properties, or variables. 
  Memory only gets deallocated whenever the reference count reaches zero.

  ### Q: What is a memory leak?

  A: A memory leak is when an amount of allocated space in memory cannot be deallocated due to a retain cycle.

  ### Q: What is a retain cycle?

  A: A retain cycle occurs when two or more objects hold strong references to each other. 
  As a result these objects retain each other in memory because their retain count never reaches zero.

  ### Q: How do you prevent retain cycles?

  A: You can prevent a retain cycle by using ‘weak’ or ‘unowned’ references. 
  A good example of this would be using [weak self] in a closure. 

  ### Q: What’s the difference between ‘weak’ and ‘unowned’?

  A: Weak references are allowed to be nil. Unowned references are never nil. 

  ### Q: How do you detect memory leaks?

  A: The easiest way to detect a memory leak is by using the debug memory graph. 
  If the memory usage keeps increasing and never decreases then that’s an indicator that you might have a retain cycle.

  <hr>
</details>

<details>
  <summary><strong>Observer & Delegation</strong></summary>
  <br>
  Work in-progress<br>
  
  ## Script
  
  ### Q: What is the Delegation Design Pattern?

  A: The delegation design pattern enables an object to delegate some of its responsibilities to another object. The delegating object typically keeps a reference to the other object.

  ### Q: How do you avoid memory leaks when using the delegation pattern?

  A: The delegate variable has to be declared as ‘weak’ to avoid a retain cycle.

  ### Q: What are some examples of when we use the delegation pattern in iOS development?

  A: The most common place where we use the delegation pattern in iOS development would be with TableViews & CollectionViews.

  ### Q: What is the Observer Design Pattern?

  A: The Observer Design Pattern allows an object to notify other objects about changes in its state.

  ### Q: What are some examples of when we use the Observer Design Pattern in iOS development?

  A: TODO://

  ### Q: What is the main difference between the Delegation and Observer pattern?

  A: The delegation design pattern is a one-to-one relationship, meaning one object communicates with one other object & the observer pattern is a one-to-many relationship, meaning one object can communicate with multiple other objects.

  <hr>
</details>

<details>
  <summary><strong>MVC & MVVM</strong></summary>
  <br>
  Work in-progress
  
  <hr>
</details>

<details>
  <summary><strong>Static & Singletons</strong></summary>
  <br>
  Work in-progress
  
  <hr>
</details>


<details>
  <summary><strong>Access Controls</strong></summary>
  <br>
  Work in-progress
  
  <hr>
</details>

<details>
  <summary><strong>3rd Party Libraries</strong></summary>
  <br>
  Work in-progress
  
  <hr>
</details>


<details>
  <summary><strong>Data Persistence</strong></summary>
  <br>
  Work in-progress
  
  <hr>
</details>

<details>
  <summary><strong>App & VC Lifecycle</strong></summary>
  <br>
  Work in-progress
  
  <hr>
</details>


<details>
  <summary><strong>Frames vs. Bounds</strong></summary>
  <br>
  Work in-progress
  
  <hr>
</details>

<details>
  <summary><strong>Networking</strong></summary>
  <br>
  Work in-progress
  
  <hr>
</details>


<details>
  <summary><strong>Swift Fundamentals</strong></summary>
  <br>
  Work in-progress
  
  <hr>
</details>

<details>
  <summary><strong>Testing</strong></summary>
  <br>
  Work in-progress
  
  <hr>
</details>


<details>
  <summary><strong>Recruiter Phone Screen</strong></summary>
  <br>
  Work in-progress
  
</details>

<hr>

# Other Resources

## Videos
- <a href="https://www.youtube.com/watch?v=HgC57v69AEs&list=PL8seg1JPkqgF5wazzCKSq3EEfqt3t8mvA">Sean Allen's YouTube Playlist </a>
- <a href="https://www.youtube.com/playlist?list=PL5PR3UyfTWvdra1XrLZTWW9SNttriKR8E">iOS Academy's YouTube Playlist </a>

## Reading
- <a href="https://www.hackingwithswift.com/interview-questions">Hacking with Swift, Over 150 iOS interview questions</a>
- <a href="https://iosinterviewguide.com">The iOS Interview Guide, Alex Bush</a>

<hr>

# Contributing

Feel free to create issues for questions you want answered. <br>
If you already have a good answer then you can submit a pull request.

<hr>

# Author

James Sedlacek created this to help minimize the amount of time it takes to study for iOS interviews.
