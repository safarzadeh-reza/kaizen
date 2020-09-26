# Kaizen
![Licence](https://img.shields.io/github/license/fuzailpalnak/kaizen)
![Python](https://img.shields.io/badge/python-v3.6+-blue.svg)
![Contributions welcome](https://img.shields.io/badge/contributions-welcome-orange.svg)

A Library build with two propose, to *map match* road elements either with *probe trace or road elements from different
source* and help, tackle the problem of *roads and building intersecting or overlapping*, which are results of
inaccurate digitizing, snapping, or resource mismatch.

This Library, presents, my view on tackling the aforementioned problem, caused during map making, addressed 
using obstacle avoidance and map matching

MapMatch            |  Conflict Resolver
:-------------------------:|:-------------------------:
![mapmatch](https://user-images.githubusercontent.com/24665570/94099696-2f6d9580-fe49-11ea-95f4-c5b53443f4a6.gif)   |  ![complex_conflict](https://user-images.githubusercontent.com/24665570/94338794-a86c1900-0012-11eb-9fad-434a1d6e6749.gif)

 

## Installation
    
    pip install git+https://github.com/fuzailpalnak/kaizen.git#egg=kaizen
    
## Additional Requirements

The library uses [Rtree](https://rtree.readthedocs.io/en/latest/) which has a dependency on 
[libspatialindex](https://libspatialindex.org/), 
It is recommend to resolve the dependency through [conda](https://anaconda.org/conda-forge/libspatialindex)

*_LibSpatialIndex For Linux:_*

    $ sudo apt-get update -y
    $ sudo apt-get install -y libspatialindex-dev
        
*_LibSpatialIndex For Windows:_*

Experience is pretty slim, for Windows Installation, I recommend using conda, for trouble free installation. 

## Examples

1. [Map Matching Road Element with Line String](https://github.com/fuzailpalnak/kaizen/blob/master/examples/MapMatchingWithLineString.ipynb)
2. [Map Matching Road Element with List of Point](https://github.com/fuzailpalnak/kaizen/blob/master/examples/MapMatchingWithPoint.ipynb)
3. [Solving Conflict Between Building and Road without additional Reference](https://github.com/fuzailpalnak/kaizen/blob/master/examples/ConflictResolver.ipynb)
4. [Complex Solving Conflict Between Building and Road without additional Reference](https://github.com/fuzailpalnak/kaizen/blob/master/examples/ConflictResolverComplex.ipynb)
5. [Solving Conflict Between Building and Road with matching the conflict with neighbouring data and finding 
associated reference points](https://github.com/fuzailpalnak/kaizen/blob/master/examples/ConflictResolverWithMapMatching.ipynb)


## References

1. [Fast Map Matching](https://people.kth.se/~cyang/bib/fmm.pdf)
2. [ST-Map Matching](https://www.microsoft.com/en-us/research/wp-content/uploads/2016/02/Map-Matching20for20Low-Sampling-Rate20GPS20Trajectories-cameraReady.pdf)
3. [Game Programming](http://theory.stanford.edu/~amitp/GameProgramming/)
4. [Robot Navigation](https://github.com/AtsushiSakai/PythonRobotics)




