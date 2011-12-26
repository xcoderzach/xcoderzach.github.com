---
layout: post
title: Why use Node.js?
published: false
---

## Why Node.js?

  For me, it's not the speed, and it's not the scalability. 
it's not even the event-driven non-blocking i/o.  It's code isomorphism.

### Isomorphic Code.

  With node.js we have the opportunity to abstract away all interactions
between client and server.  Descisions about what goes on the client and what
goes on the server will be a non-issue.  We can build a system where you have
one code base. All written one language.  

  Validating data?  Run it on the client, then run it on the server.  

  Persisting data?  Persist your data to localStorage on the client, or to a
database on the server, or to both.  

  You won't have to worry about writing a backbone app to manage it on the
client, and then punt it off to rails on the server.  The same code that
handles models on the client, can do it on the server.

### Real-time user interaction
  
  Another advantage of breaking the barrier between the client and the server,
is that we can push real-time notifications to users.  And with node.js it's so
easy that we'll soon reach the point where it'll be easier to build your apps
_with_ real-time interaction than without.  

  Notifications that you care about will be routed to the browser in real-time,
all you have to do is tell the view what to do with them.

### No JavaScript? No problem!

  Your users are using IE 3?  No problem!  Run it for them and send them the result!
It's just javascript after all.
