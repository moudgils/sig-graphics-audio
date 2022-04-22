
## OpenXR 



**Summary**
OpenXR is an open royalty-free API standard from Khronos, providing engines with native access to a range of devices. It provides access to following API and we will need to add support for it in a modular fashion within O3DE. The api to add support for is as follows

XrSpace	A representation of 3D space
XrInstance	A representation of the OpenXR Runtime
XrSystemId	A representation of the devices
XrActions	A representation of user inputs
XrSession	A representation of the session between the app an the user
XrSwapChain	A representation of XR swapchain 

*Goals*
This document aims to provide framework around setting up XR related functionality that will need to work with Atom (O3de renderer) in an abstract modular manner. As part of setting up this framework we want to adhere to following goals. 


* Clean XR api accessible to all gems that require XR functionality.  
* Iterative development
* Modularity across multiple XR backends
* Debugging support
* Profiling tools
* Supported device - Quest 2. Eventually any device that supports OpenXr with Vk and Dx12 should work. 

