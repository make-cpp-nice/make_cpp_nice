# Library utilities, methodologies and guidelines to make C++ nice to work with. 

Some thoughts:

+ Safe is nice. That doesn't have to be the bullet proof provable safety of Rust. A more humble aim that with reasonable care safety hazards can easily be avoided would be a big improvement on the status quo. So hazards of pointer, memory or data corruption should be well controlled and easy to avoid.
+ Identifiers should be named so that someone uninitiated has a good chance of guessing what they mean.
+ What you think in one sentence, you should be able to write in one line and it should look like what you thought. If you read it out load it should sound like a description of what your code does.
+ Coding should not be laborious. You should not have to code much more than what you are thinking.
+ Learning curves should be short and provide early rewards.

Library utilities:

+ ptr_to_unique - A smart pointer to an object already owned by a unique_ptr. It doesn't own the object but it self zeroes when the object is deleted so that it can never dangle. 
+ numerical conversions - A set of dedicated numerical conversions that are a better choice than the canonical application static_cast. 
+ literal integral constants - Converts literal constants into std::integral_constant using a double underscore suffix, e.g. 4__ 


<!---
inglesflamenco/inglesflamenco is a ✨ special ✨ repository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take a look at your changes.
--->
