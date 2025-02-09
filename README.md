## Library utilities, methodologies and guidelines to make C++ nice to work with. 

Single header Library utilities:

+ [ptr_to_unique](https://github.com/make-cpp-nice/ptr_to_unique) - A smart pointer to an object already owned by a unique_ptr. It doesn't own the object but it self zeroes when the object is deleted so that it can never dangle. 
+ [numerical conversions](https://github.com/make-cpp-nice/numerical-conversions) - A set of dedicated numerical conversions that are a better choice than the canonical application of static_cast. 
+ [literal integral constants](https://github.com/make-cpp-nice/literal-integral-constants) - Converts literal 
constants into std::integral_constant using a double underscore suffix, e.g. 4__ 

Some thoughts:

+ Safe is nice. That doesn't have to be the bullet proof provable safety of Rust. A more humble aim that with reasonable care safety hazards can easily be avoided would be a big improvement on the status quo. So hazards of pointer, memory or data corruption should be well controlled and easy to avoid. The problem that needs addressing with C++ is not that you can shoot yourself in the foot, it is that it can be difficult not to shoot yourself in the foot. 
+ Identifiers should be named so that someone uninitiated has a good chance of guessing what they mean.
+ What you think in one sentence, you should be able to write in one line and it should look like what you thought. If you read it out load it should sound like a description of what your code does.
+ Coding should not be laborious. You should not have to code much more than what you are thinking. But don't try to cram more onto one line than the mind can comfortably grasp.
+ Learning curves should be short and provide early rewards.
+ Some clever and useful C++ constructs are difficult to decipher. Use them if they serve your purpose but encapsulate it so others don't have to go there.
+ Always prefer existing standard solutions but if they don't meet your needs then find or create something that does.

Please post any feedback or comments on [Comment and discussion](https://github.com/make-cpp-nice/make_cpp_nice/discussions/1)


<!---
inglesflamenco/inglesflamenco is a ✨ special ✨ repository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take a look at your changes.
--->
