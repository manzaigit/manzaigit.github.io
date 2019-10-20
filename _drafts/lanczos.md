
In fMRI, a common approach is to use a correlation matrix to find salient connections between different brain regions. 
Brain parcellations are getting finer (TODO: insert history here, e.g. AAL (90) Power (264), newer ones) and that will increase with more detailed parcellations schemes proposed.

264 x 264 gives 34716 features

but there are times where a 34716 x 34716 matrix needs to be computed. 

https://stackoverflow.com/questions/17468054/the-fastest-way-to-calculate-eigenvalues-of-large-matrices
https://stackoverflow.com/questions/6684238/whats-the-fastest-way-to-find-eigenvalues-vectors-in-python

scipy.sparse.linalg.eigs(h)
only faster for bigger matrices >500

code examples
https://github.com/spartan-array/spartan/blob/master/spartan/examples/lanczos.py
https://scicomp.stackexchange.com/questions/23536/quality-of-eigenvalue-approximation-in-lanczos-method
it does a good job of simultaneously converging eigenvalues at both ends of the spectrum.
power iteration, so largest might converge before smallest

https://www.numbercrunch.de/blog/2014/08/the-lanczos-algorithm/