Baton
===

An open source tool that help to manage unique service instances over Docker or 
Kubernetes.

Abstract
---

Let say you try to build system where one or several components are based on 
the same container image but operates in a different modes, and you want to 
allocate them dynamically. Or event, what if one of your services act as a API 
Gateway and can be asked to give an access to previously unknown resource.

That's, where Baton came along.

It will help to spawn new instance or set of instances by command, with all 
given runtime arguments, after successful start it will inform about that or 
inform about failure.

Baton also will track container statues along their lifetime and in case of 
same service with same runtime arguments will be demanded it will return one 
that already been started or start stopped one.

Baton will provide you API with two basic methods: Attach and Detach.



