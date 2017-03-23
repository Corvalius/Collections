# Sparrow.Collections

Implementation of fast alternative data structures we implemented for use by [RavenDB](https://ravendb.net) released under permission as a standalone library.

```FastDictionary<T,K>``` uses techniques we learned from different Dictionary implementations out there but the base mechanics are more similar to the Google's Dense Hash Map than to the CoreCLR Dictionary. You should expect similar behaviors and tradeoffs. 

```FastStack<T>``` and ```FastList<T>``` are stripped down to the core implementations of their respective versions on CoreCLR. We expect them to go obsolete when CoreCLR 2.0 because of improvements in the code generation of the JIT, but meanwhile if your code is performance capped by those data structures, they can help. 


