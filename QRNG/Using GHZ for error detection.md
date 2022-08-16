# Using GHZ states for error detection

![[ghz_error_detection.pdf]]

The above article details research which has previously been conducting with regards to using the GHZ states for basic error detection and correction. The idea is simply to throw away illegal states that result. They detail an improvement in the fidelity of the system as a result. This paper in particular describes how such a procedure could improve existing protocols such as teleportation and superdense coding which use EPR pairs traditionally. 
- This is known as destructive error-correction; information is destroyed in the process of enhancing fidelity of the overall system
- Their approach is noteworthy. They prove its performance enhancement to a good degree of mathematical rigor, and their argument is abstract and theoretical in nature. 
- Would we be able to add something here by showing it in practical use as opposed to making a theoretical argument? I wonder if our argument would be as rigorous...

![[ghz_non_destructive.pdf]]

Another approach using a non-destructive discrimination algorithm is investigated in this paper. The researchers detail how their automated error correction algorithm works to remove not only bit-flip, but also phase-flip errors. The previous paper's approach would only defend against bit-flip errors as erroneous states that have bit-flips are discarded. GHZ/Bell states come into play when they would like to prove that their algorithm is effective in protecting against both types of errors. 
- The proof is again mathematical in nature, and they even mention "We hope this qubit entangled state discrimination and error correction finds experimental verification in near future. We aim that the present experiment will soon be extended to the experimental discrimination and automated error correction of more complex entangled states."
	- One avenue we can take is experimental verification of previously shown theoretical results in error-correction
- One thing I didn't understand: they mention that experimental and theoretical density matrices were constructed using quantum state tomography. Wouldn't this mean their results are experimentally verified already as they've gathered data to construct the experimental density matrix?

