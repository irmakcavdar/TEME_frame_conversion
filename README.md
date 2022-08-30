# TEME_frame_conversion

Often the SGP4 propagator is used for analytically propagating a set of satellite data, called Two Line Element (TLE). The propagator inputs the string of TLE and outputs the velocity and position for a desired time in the cartesian frame. However, the reference frame used by the propagator is an unconventional reference frame, which is a True Equator Mean Equinox frame (TEME). Although it is an ECI reference frame, how the frame is defined is not that trivial. Therefore, for post-processing, it is often required to convert the cartesian position and velocity elements to another reference frame. 

GCRS/J2000 is a commonly used ECI frame, often frame of choice for numerical propagators. It is defined with respect to the Earth's mean quator and mean equniox at 12:00 (TT) on 1 January 2000. The short code provided in this repository is an example for converting an SGP4 propagated state from the TEME reference frame to the J2000 reference frame. 
