---
layout:     post
title:      Distributed Infrastructure
summary:    I
categories: 
---

### Use Case
Higher than normal level or redundancy required. 

An increase in performance is required, in certain circumstances. ( Don't you want to be [web scale](http://www.mongodb-is-web-scale.com/)? :) ).


### Terminology
Distributed infrastructure can mean many things. The term is vague and can be over used in some circles. In most cases context can be inferred based on usage, but to be perfectly clear this is the definition that I'm going with.

> Distributed infrastructure refers to geographically separate servers that work together to fulfil a particular requirement or purpose.

Some projects are referenced by name; You can find their respective websites below:

* [salt](http://saltstack.org)
* [bind](https://www.isc.org/downloads/bind/)

### Problems
Shared state.
Management.

### Solutions
Don't share state.
Lazy replication.

### Conclusion

